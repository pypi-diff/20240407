# Comparing `tmp/interrogate-1.5.0.tar.gz` & `tmp/interrogate-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/folders/g0/7rcby3gn13d06kt_3vtvz3gw0000gn/T/tmpc06kzrtr/tmpl86j3ix6/interrogate-1.5.0.tar", last modified: Fri Sep 10 23:00:14 2021, max compression
+gzip compressed data, was "interrogate-1.6.0.tar", last modified: Sat Apr  6 23:29:20 2024, max compression
```

## Comparing `interrogate-1.5.0.tar` & `interrogate-1.6.0.tar`

### file list

```diff
@@ -1,182 +1,183 @@
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.694463 interrogate-1.5.0/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.476703 interrogate-1.5.0/.github/
--rw-r--r--   0 lynn       (501) staff       (20)      110 2021-06-02 17:37:31.000000 interrogate-1.5.0/.github/FUNDING.yml
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.477886 interrogate-1.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 lynn       (501) staff       (20)      774 2020-07-13 14:28:37.000000 interrogate-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 lynn       (501) staff       (20)      801 2020-07-13 14:28:37.000000 interrogate-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 lynn       (501) staff       (20)      183 2020-10-06 21:30:36.000000 interrogate-1.5.0/.github/dependabot.yml
--rw-r--r--   0 lynn       (501) staff       (20)     2075 2020-07-13 14:28:37.000000 interrogate-1.5.0/.github/pull_request_template.md
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.482545 interrogate-1.5.0/.github/workflows/
--rw-r--r--   0 lynn       (501) staff       (20)     1298 2021-06-02 17:37:31.000000 interrogate-1.5.0/.github/workflows/autoupdate-pre-commit-config.yml
--rw-r--r--   0 lynn       (501) staff       (20)     2719 2021-09-10 19:42:40.000000 interrogate-1.5.0/.github/workflows/main.yml
--rw-r--r--   0 lynn       (501) staff       (20)     2085 2021-09-10 19:42:40.000000 interrogate-1.5.0/.github/workflows/sanity.yml
--rw-r--r--   0 lynn       (501) staff       (20)      814 2021-09-10 19:42:40.000000 interrogate-1.5.0/.github/workflows/windows.yml
--rw-r--r--   0 lynn       (501) staff       (20)      799 2021-09-10 19:42:40.000000 interrogate-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 lynn       (501) staff       (20)      214 2020-09-03 20:48:53.000000 interrogate-1.5.0/.pre-commit-hooks.yaml
--rw-r--r--   0 lynn       (501) staff       (20)     1076 2020-04-23 23:11:52.000000 interrogate-1.5.0/LICENSE
--rw-r--r--   0 lynn       (501) staff       (20)      533 2021-05-14 23:07:04.000000 interrogate-1.5.0/MANIFEST.in
--rw-r--r--   0 lynn       (501) staff       (20)    34952 2021-09-10 23:00:14.694067 interrogate-1.5.0/PKG-INFO
--rw-r--r--   0 lynn       (501) staff       (20)    32651 2021-09-10 22:54:27.000000 interrogate-1.5.0/README.rst
--rw-r--r--   0 lynn       (501) staff       (20)      173 2020-10-06 21:30:36.000000 interrogate-1.5.0/codecov.yml
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.484932 interrogate-1.5.0/docs/
--rw-r--r--   0 lynn       (501) staff       (20)     1179 2021-05-14 21:40:18.000000 interrogate-1.5.0/docs/Makefile
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.487172 interrogate-1.5.0/docs/_static/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.489836 interrogate-1.5.0/docs/_static/badge_examples/
--rw-r--r--   0 lynn       (501) staff       (20)    11389 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_f.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5733 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_fs.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_fsm.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5771 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_ftb.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11511 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_p.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_s.svg
--rw-r--r--   0 lynn       (501) staff       (20)      456 2020-04-25 00:55:09.000000 interrogate-1.5.0/docs/_static/custom.css
--rw-r--r--   0 lynn       (501) staff       (20)     4791 2020-04-24 15:39:59.000000 interrogate-1.5.0/docs/_static/favicon.png
--rw-r--r--   0 lynn       (501) staff       (20)     5733 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/_static/interrogate_badge.svg
--rw-r--r--   0 lynn       (501) staff       (20)    12422 2020-04-24 15:16:06.000000 interrogate-1.5.0/docs/_static/logo_pink.png
--rw-r--r--   0 lynn       (501) staff       (20)     1079 2020-04-24 16:27:33.000000 interrogate-1.5.0/docs/_static/logo_smol.png
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.490244 interrogate-1.5.0/docs/_templates/
--rw-r--r--   0 lynn       (501) staff       (20)      292 2020-04-24 20:51:06.000000 interrogate-1.5.0/docs/_templates/navigation.html
--rw-r--r--   0 lynn       (501) staff       (20)     5139 2021-09-10 22:54:09.000000 interrogate-1.5.0/docs/changelog.rst
--rw-r--r--   0 lynn       (501) staff       (20)     3100 2020-04-29 14:02:22.000000 interrogate-1.5.0/docs/conf.py
--rw-r--r--   0 lynn       (501) staff       (20)       53 2020-04-23 23:25:03.000000 interrogate-1.5.0/docs/docutils.conf
--rw-r--r--   0 lynn       (501) staff       (20)     4270 2021-09-10 22:52:06.000000 interrogate-1.5.0/docs/index.rst
--rw-r--r--   0 lynn       (501) staff       (20)      996 2021-09-10 19:42:40.000000 interrogate-1.5.0/pyproject.toml
--rw-r--r--   0 lynn       (501) staff       (20)       38 2021-09-10 23:00:14.694603 interrogate-1.5.0/setup.cfg
--rw-r--r--   0 lynn       (501) staff       (20)     3610 2021-09-10 19:42:40.000000 interrogate-1.5.0/setup.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.440771 interrogate-1.5.0/src/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.497861 interrogate-1.5.0/src/interrogate/
--rw-r--r--   0 lynn       (501) staff       (20)      296 2021-09-10 22:53:02.000000 interrogate-1.5.0/src/interrogate/__init__.py
--rw-r--r--   0 lynn       (501) staff       (20)      129 2020-05-12 21:37:28.000000 interrogate-1.5.0/src/interrogate/__main__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.531707 interrogate-1.5.0/src/interrogate/badge/
--rw-r--r--   0 lynn       (501) staff       (20)    11935 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/flat-square-modified-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5815 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/flat-square-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11460 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/flat-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5824 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/for-the-badge-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11648 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/plastic-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6812 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge/social-style.svg
--rw-r--r--   0 lynn       (501) staff       (20)     8136 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/badge_gen.py
--rw-r--r--   0 lynn       (501) staff       (20)    10275 2021-09-10 22:52:06.000000 interrogate-1.5.0/src/interrogate/cli.py
--rw-r--r--   0 lynn       (501) staff       (20)     7863 2021-09-10 19:42:40.000000 interrogate-1.5.0/src/interrogate/config.py
--rw-r--r--   0 lynn       (501) staff       (20)    17743 2021-09-10 19:42:40.000000 interrogate-1.5.0/src/interrogate/coverage.py
--rw-r--r--   0 lynn       (501) staff       (20)     8021 2021-09-10 19:42:40.000000 interrogate-1.5.0/src/interrogate/utils.py
--rw-r--r--   0 lynn       (501) staff       (20)     7865 2021-05-14 23:07:04.000000 interrogate-1.5.0/src/interrogate/visit.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.500633 interrogate-1.5.0/src/interrogate.egg-info/
--rw-r--r--   0 lynn       (501) staff       (20)    34952 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/PKG-INFO
--rw-r--r--   0 lynn       (501) staff       (20)     5844 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/SOURCES.txt
--rw-r--r--   0 lynn       (501) staff       (20)        1 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/dependency_links.txt
--rw-r--r--   0 lynn       (501) staff       (20)       54 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/entry_points.txt
--rw-r--r--   0 lynn       (501) staff       (20)        1 2020-04-24 23:31:30.000000 interrogate-1.5.0/src/interrogate.egg-info/not-zip-safe
--rw-r--r--   0 lynn       (501) staff       (20)      217 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/requires.txt
--rw-r--r--   0 lynn       (501) staff       (20)       12 2021-09-10 23:00:14.000000 interrogate-1.5.0/src/interrogate.egg-info/top_level.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.442506 interrogate-1.5.0/tests/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.533310 interrogate-1.5.0/tests/functional/
--rw-r--r--   0 lynn       (501) staff       (20)       87 2020-04-29 14:04:06.000000 interrogate-1.5.0/tests/functional/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.540473 interrogate-1.5.0/tests/functional/fixtures/
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/functional/fixtures/expected_badge.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5265 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_detailed.txt
--rw-r--r--   0 lynn       (501) staff       (20)     4779 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_detailed_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)     2350 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_detailed_single_file.txt
--rw-r--r--   0 lynn       (501) staff       (20)     3564 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/expected_detailed_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)       47 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_no_verbosity.txt
--rw-r--r--   0 lynn       (501) staff       (20)      810 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_summary.txt
--rw-r--r--   0 lynn       (501) staff       (20)      729 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/expected_summary_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)      810 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/expected_summary_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)      405 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/expected_summary_skip_covered_all.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.543961 interrogate-1.5.0/tests/functional/fixtures/windows/
--rw-r--r--   0 lynn       (501) staff       (20)     5200 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed.txt
--rw-r--r--   0 lynn       (501) staff       (20)     4720 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)     2321 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt
--rw-r--r--   0 lynn       (501) staff       (20)     3520 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)       47 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_no_verbosity.txt
--rw-r--r--   0 lynn       (501) staff       (20)      800 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary.txt
--rw-r--r--   0 lynn       (501) staff       (20)      720 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary_no_module.txt
--rw-r--r--   0 lynn       (501) staff       (20)      640 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt
--rw-r--r--   0 lynn       (501) staff       (20)      400 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.550645 interrogate-1.5.0/tests/functional/sample/
--rw-r--r--   0 lynn       (501) staff       (20)       55 2020-04-23 21:07:42.000000 interrogate-1.5.0/tests/functional/sample/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.551443 interrogate-1.5.0/tests/functional/sample/child_sample/
--rw-r--r--   0 lynn       (501) staff       (20)       62 2020-04-23 21:07:37.000000 interrogate-1.5.0/tests/functional/sample/child_sample/__init__.py
--rw-r--r--   0 lynn       (501) staff       (20)      528 2020-04-23 23:10:45.000000 interrogate-1.5.0/tests/functional/sample/child_sample/child_sample_module.py
--rw-r--r--   0 lynn       (501) staff       (20)       33 2020-04-28 21:22:07.000000 interrogate-1.5.0/tests/functional/sample/empty.py
--rw-r--r--   0 lynn       (501) staff       (20)     1298 2021-05-14 20:05:20.000000 interrogate-1.5.0/tests/functional/sample/full.py
--rw-r--r--   0 lynn       (501) staff       (20)       43 2020-04-28 21:22:07.000000 interrogate-1.5.0/tests/functional/sample/ignoreme.txt
--rw-r--r--   0 lynn       (501) staff       (20)     1147 2020-08-23 20:59:33.000000 interrogate-1.5.0/tests/functional/sample/partial.py
--rw-r--r--   0 lynn       (501) staff       (20)     5996 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/functional/test_cli.py
--rw-r--r--   0 lynn       (501) staff       (20)     9122 2021-09-10 19:42:40.000000 interrogate-1.5.0/tests/functional/test_coverage.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.553027 interrogate-1.5.0/tests/unit/
--rw-r--r--   0 lynn       (501) staff       (20)       81 2020-04-29 14:04:11.000000 interrogate-1.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.446998 interrogate-1.5.0/tests/unit/fixtures/
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.559356 interrogate-1.5.0/tests/unit/fixtures/default-style/
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6720 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/default.svg
--rw-r--r--   0 lynn       (501) staff       (20)     1685 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/default-style/no_logo.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.562982 interrogate-1.5.0/tests/unit/fixtures/flat/
--rw-r--r--   0 lynn       (501) staff       (20)    11392 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11389 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     7766 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11393 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11396 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.630441 interrogate-1.5.0/tests/unit/fixtures/flat-square/
--rw-r--r--   0 lynn       (501) staff       (20)     5736 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5733 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5583 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     5736 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5739 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.635429 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11873 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6720 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11876 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11879 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.683572 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/
--rw-r--r--   0 lynn       (501) staff       (20)     5774 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5771 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5779 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5803 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     5776 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     5777 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/for-the-badge/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.687438 interrogate-1.5.0/tests/unit/fixtures/plastic/
--rw-r--r--   0 lynn       (501) staff       (20)    11514 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11511 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     8002 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/99.png
--rw-r--r--   0 lynn       (501) staff       (20)    11515 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)    11518 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/plastic/default.svg
-drwxr-xr-x   0 lynn       (501) staff       (20)        0 2021-09-10 23:00:14.693522 interrogate-1.5.0/tests/unit/fixtures/social/
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/0.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6724 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/100.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/45.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/60.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/89.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/90.svg
--rw-r--r--   0 lynn       (501) staff       (20)     7102 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/99.png
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/99.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6726 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/fixtures/social/default.svg
--rw-r--r--   0 lynn       (501) staff       (20)     6431 2021-09-10 22:52:06.000000 interrogate-1.5.0/tests/unit/test_badge_gen.py
--rw-r--r--   0 lynn       (501) staff       (20)     7431 2021-06-02 19:43:28.000000 interrogate-1.5.0/tests/unit/test_config.py
--rw-r--r--   0 lynn       (501) staff       (20)    12596 2020-08-23 21:43:30.000000 interrogate-1.5.0/tests/unit/test_utils.py
--rw-r--r--   0 lynn       (501) staff       (20)     1713 2021-09-10 19:42:40.000000 interrogate-1.5.0/tox.ini
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.848620 interrogate-1.6.0/
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.806166 interrogate-1.6.0/.github/
+-rw-r--r--   0 lynn       (501) staff       (20)      110 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/FUNDING.yml
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.806492 interrogate-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 lynn       (501) staff       (20)      774 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 lynn       (501) staff       (20)      801 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 lynn       (501) staff       (20)      183 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/dependabot.yml
+-rw-r--r--   0 lynn       (501) staff       (20)     2075 2023-01-07 16:39:14.000000 interrogate-1.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.807309 interrogate-1.6.0/.github/workflows/
+-rw-r--r--   0 lynn       (501) staff       (20)     4477 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/main.yml
+-rw-r--r--   0 lynn       (501) staff       (20)        0 2024-04-06 23:26:56.000000 interrogate-1.6.0/.github/workflows/pypi.yml
+-rw-r--r--   0 lynn       (501) staff       (20)     2159 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/sanity.yml
+-rw-r--r--   0 lynn       (501) staff       (20)      779 2024-04-06 18:03:19.000000 interrogate-1.6.0/.github/workflows/windows.yml
+-rw-r--r--   0 lynn       (501) staff       (20)      947 2024-04-06 21:44:22.000000 interrogate-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 lynn       (501) staff       (20)      214 2023-01-07 16:39:14.000000 interrogate-1.6.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 lynn       (501) staff       (20)      225 2024-04-06 18:03:19.000000 interrogate-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 lynn       (501) staff       (20)     1076 2023-01-07 16:39:14.000000 interrogate-1.6.0/LICENSE
+-rw-r--r--   0 lynn       (501) staff       (20)      533 2024-04-06 18:03:07.000000 interrogate-1.6.0/MANIFEST.in
+-rw-r--r--   0 lynn       (501) staff       (20)    35835 2024-04-06 23:29:20.848387 interrogate-1.6.0/PKG-INFO
+-rw-r--r--   0 lynn       (501) staff       (20)    33051 2024-04-06 23:21:11.000000 interrogate-1.6.0/README.rst
+-rw-r--r--   0 lynn       (501) staff       (20)      173 2023-01-07 16:39:14.000000 interrogate-1.6.0/codecov.yml
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.808221 interrogate-1.6.0/docs/
+-rw-r--r--   0 lynn       (501) staff       (20)     1179 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/Makefile
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.809072 interrogate-1.6.0/docs/_static/
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.809991 interrogate-1.6.0/docs/_static/badge_examples/
+-rw-r--r--   0 lynn       (501) staff       (20)    11389 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_f.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5733 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fs.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fsm.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5771 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_ftb.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11511 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_p.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_s.svg
+-rw-r--r--   0 lynn       (501) staff       (20)      456 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/custom.css
+-rw-r--r--   0 lynn       (501) staff       (20)     4791 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/favicon.png
+-rw-r--r--   0 lynn       (501) staff       (20)    11873 2024-04-06 18:03:19.000000 interrogate-1.6.0/docs/_static/interrogate_badge.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    12422 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/logo_pink.png
+-rw-r--r--   0 lynn       (501) staff       (20)     1079 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_static/logo_smol.png
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.810146 interrogate-1.6.0/docs/_templates/
+-rw-r--r--   0 lynn       (501) staff       (20)      292 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/_templates/navigation.html
+-rw-r--r--   0 lynn       (501) staff       (20)     5630 2024-04-06 23:21:43.000000 interrogate-1.6.0/docs/changelog.rst
+-rw-r--r--   0 lynn       (501) staff       (20)     3091 2024-04-06 18:03:19.000000 interrogate-1.6.0/docs/conf.py
+-rw-r--r--   0 lynn       (501) staff       (20)       53 2023-01-07 16:39:14.000000 interrogate-1.6.0/docs/docutils.conf
+-rw-r--r--   0 lynn       (501) staff       (20)     4391 2024-04-06 21:44:22.000000 interrogate-1.6.0/docs/index.rst
+-rw-r--r--   0 lynn       (501) staff       (20)     1173 2024-04-06 23:03:15.000000 interrogate-1.6.0/pyproject.toml
+-rw-r--r--   0 lynn       (501) staff       (20)       38 2024-04-06 23:29:20.848657 interrogate-1.6.0/setup.cfg
+-rw-r--r--   0 lynn       (501) staff       (20)     3445 2024-04-06 23:23:17.000000 interrogate-1.6.0/setup.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.802338 interrogate-1.6.0/src/
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.811830 interrogate-1.6.0/src/interrogate/
+-rw-r--r--   0 lynn       (501) staff       (20)      296 2024-04-06 23:18:55.000000 interrogate-1.6.0/src/interrogate/__init__.py
+-rw-r--r--   0 lynn       (501) staff       (20)      129 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/__main__.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.813907 interrogate-1.6.0/src/interrogate/badge/
+-rw-r--r--   0 lynn       (501) staff       (20)    11935 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-square-modified-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5815 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-square-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11460 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/flat-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5824 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/for-the-badge-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11648 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/plastic-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6812 2023-01-07 16:39:14.000000 interrogate-1.6.0/src/interrogate/badge/social-style.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     8243 2024-04-06 22:07:45.000000 interrogate-1.6.0/src/interrogate/badge_gen.py
+-rw-r--r--   0 lynn       (501) staff       (20)    10587 2024-04-06 21:44:22.000000 interrogate-1.6.0/src/interrogate/cli.py
+-rw-r--r--   0 lynn       (501) staff       (20)     8003 2024-04-06 23:05:46.000000 interrogate-1.6.0/src/interrogate/config.py
+-rw-r--r--   0 lynn       (501) staff       (20)    17660 2024-04-06 23:16:35.000000 interrogate-1.6.0/src/interrogate/coverage.py
+-rw-r--r--   0 lynn       (501) staff       (20)     8013 2024-04-06 18:03:19.000000 interrogate-1.6.0/src/interrogate/utils.py
+-rw-r--r--   0 lynn       (501) staff       (20)     8276 2024-04-06 21:44:22.000000 interrogate-1.6.0/src/interrogate/visit.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.847423 interrogate-1.6.0/src/interrogate.egg-info/
+-rw-r--r--   0 lynn       (501) staff       (20)    35835 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/PKG-INFO
+-rw-r--r--   0 lynn       (501) staff       (20)     5838 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/SOURCES.txt
+-rw-r--r--   0 lynn       (501) staff       (20)        1 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/dependency_links.txt
+-rw-r--r--   0 lynn       (501) staff       (20)       53 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/entry_points.txt
+-rw-r--r--   0 lynn       (501) staff       (20)        1 2023-01-07 17:13:34.000000 interrogate-1.6.0/src/interrogate.egg-info/not-zip-safe
+-rw-r--r--   0 lynn       (501) staff       (20)      247 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/requires.txt
+-rw-r--r--   0 lynn       (501) staff       (20)       12 2024-04-06 23:29:20.000000 interrogate-1.6.0/src/interrogate.egg-info/top_level.txt
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.802814 interrogate-1.6.0/tests/
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.814436 interrogate-1.6.0/tests/functional/
+-rw-r--r--   0 lynn       (501) staff       (20)       87 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/__init__.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.816230 interrogate-1.6.0/tests/functional/fixtures/
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_badge.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6237 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     5751 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_no_module.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     2836 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_single_file.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     4050 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_detailed_skip_covered.txt
+-rw-r--r--   0 lynn       (501) staff       (20)       47 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_no_verbosity.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      810 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      729 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_no_module.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      810 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      405 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered_all.txt
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.817534 interrogate-1.6.0/tests/functional/fixtures/windows/
+-rw-r--r--   0 lynn       (501) staff       (20)     6160 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     6401 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     2801 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     4000 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt
+-rw-r--r--   0 lynn       (501) staff       (20)       47 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_no_verbosity.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      800 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      560 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_no_module.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      640 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt
+-rw-r--r--   0 lynn       (501) staff       (20)      560 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered_all.txt
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.818459 interrogate-1.6.0/tests/functional/sample/
+-rw-r--r--   0 lynn       (501) staff       (20)       55 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/__init__.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.818820 interrogate-1.6.0/tests/functional/sample/child_sample/
+-rw-r--r--   0 lynn       (501) staff       (20)       62 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/child_sample/__init__.py
+-rw-r--r--   0 lynn       (501) staff       (20)      488 2024-04-06 18:03:19.000000 interrogate-1.6.0/tests/functional/sample/child_sample/child_sample_module.py
+-rw-r--r--   0 lynn       (501) staff       (20)       33 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/empty.py
+-rw-r--r--   0 lynn       (501) staff       (20)     1893 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/sample/full.py
+-rw-r--r--   0 lynn       (501) staff       (20)       43 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/functional/sample/ignoreme.txt
+-rw-r--r--   0 lynn       (501) staff       (20)     1582 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/sample/partial.py
+-rw-r--r--   0 lynn       (501) staff       (20)     6097 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/test_cli.py
+-rw-r--r--   0 lynn       (501) staff       (20)     9467 2024-04-06 21:44:22.000000 interrogate-1.6.0/tests/functional/test_coverage.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.819533 interrogate-1.6.0/tests/unit/
+-rw-r--r--   0 lynn       (501) staff       (20)       81 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.803267 interrogate-1.6.0/tests/unit/fixtures/
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.821007 interrogate-1.6.0/tests/unit/fixtures/default-style/
+-rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6720 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/default.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     1685 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/default-style/no_logo.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.838644 interrogate-1.6.0/tests/unit/fixtures/flat/
+-rw-r--r--   0 lynn       (501) staff       (20)    11392 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11389 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     7766 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)    11393 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11396 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat/default.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.839985 interrogate-1.6.0/tests/unit/fixtures/flat-square/
+-rw-r--r--   0 lynn       (501) staff       (20)     5736 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5733 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5583 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)     5736 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5739 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square/default.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.841364 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/
+-rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11873 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6720 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)    11876 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11879 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/default.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.842687 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/
+-rw-r--r--   0 lynn       (501) staff       (20)     5774 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5771 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5779 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5803 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)     5776 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     5777 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/for-the-badge/default.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.845958 interrogate-1.6.0/tests/unit/fixtures/plastic/
+-rw-r--r--   0 lynn       (501) staff       (20)    11514 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11511 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     8002 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)    11515 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)    11518 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/plastic/default.svg
+drwxr-xr-x   0 lynn       (501) staff       (20)        0 2024-04-06 23:29:20.847209 interrogate-1.6.0/tests/unit/fixtures/social/
+-rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/0.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6724 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/100.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/45.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/60.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/89.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/90.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     7102 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/99.png
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/99.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6726 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/fixtures/social/default.svg
+-rw-r--r--   0 lynn       (501) staff       (20)     6426 2024-04-06 18:03:19.000000 interrogate-1.6.0/tests/unit/test_badge_gen.py
+-rw-r--r--   0 lynn       (501) staff       (20)     7511 2023-01-07 16:39:14.000000 interrogate-1.6.0/tests/unit/test_config.py
+-rw-r--r--   0 lynn       (501) staff       (20)    10955 2024-04-06 18:03:20.000000 interrogate-1.6.0/tests/unit/test_utils.py
+-rw-r--r--   0 lynn       (501) staff       (20)     1312 2024-04-06 21:32:01.000000 interrogate-1.6.0/tox.ini
```

### Comparing `interrogate-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `interrogate-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `interrogate-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/.github/pull_request_template.md` & `interrogate-1.6.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/.github/workflows/main.yml` & `interrogate-1.6.0/.github/workflows/sanity.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,69 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
+# Run workflow weekly to make sure interrogate can regularly build in case
+# there are new releases of dependencies. This is the same as main workflow,
+# but (1) coverage isn't uploaded, and (2) `install-dev` job runs only on
+# ubuntu, not all three OS platforms.
 
-name: CI
+name: sanity
 
+# trigger weekly on Monday at 5am UTC (no particular reason why this date/time)
 on:
-  push:
-    branches: [ master ]
-  pull_request:
-    branches: [ master ]
-  # Allow rebuilds via API.
-  repository_dispatch:
-    types: rebuild
+  schedule:
+    - cron: "0 5 * * 1"
 
-jobs:
-  pre-commit:
-    name: "Pre-commit"
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
-      - name: Locally install interrogate
-        run: python -m pip install .
-      - name: Run pre-commit
-        uses: pre-commit/action@v2.0.3
+env:
+  FORCE_COLOR: "1"
+  TOX_TESTENV_PASSENV: FORCE_COLOR
+  PYTHON_LATEST: "3.10"
 
+jobs:
   tests:
     name: "Python ${{ matrix.python-version }} on Ubuntu"
     runs-on: "ubuntu-latest"
-    env:
-      USING_COVERAGE: '3.7,3.8,3.9,3.10.0-rc.2'
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10.0-rc.2"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
-      - uses: "actions/checkout@v2"
-      - uses: "actions/setup-python@v2"
+      - uses: "actions/checkout@v3"
+      - uses: "actions/setup-python@v4"
         with:
           python-version: "${{ matrix.python-version }}"
+          allow-prereleases: true
+          cache: pip
+
       - name: "Install dependencies"
         run: |
           set -xe
           python -VV
           python -m site
           python -m pip install --upgrade pip setuptools wheel
           python -m pip install --upgrade virtualenv tox tox-gh-actions
       - name: "Run tox targets for ${{ matrix.python-version }}"
         run: "python -m tox"
-      - name: "Upload coverage to Codecov"
-        if: "contains(env.USING_COVERAGE, matrix.python-version)"
-        uses: "codecov/codecov-action@v2.0.3"
-        with:
-          file: ./coverage.xml
-          fail_ci_if_error: true
 
   package:
     name: "Build & Verify Package on Ubuntu"
     runs-on: "ubuntu-latest"
     steps:
-      - uses: "actions/checkout@v2"
-      - uses: "actions/setup-python@v2"
+      - uses: "actions/checkout@v3"
+      - uses: "actions/setup-python@v4"
         with:
-          python-version: "3.8"
-      - name: "Install pep517 and twine"
-        run: "python -m pip install pep517 twine"
-      - name: "Build package"
-        run: "python -m pep517.build --source --binary ."
-      - name: "List result"
-        run: "ls -l dist"
-      - name: "Check long_description"
-        run: "python -m twine check dist/*"
+          python-version: ${{env.PYTHON_LATEST}}
+      - run: python -m pip install build twine check-wheel-contents
+      - run: python -m build --sdist --wheel .
+      - run: ls -l dist
+      - run: check-wheel-contents dist/*.whl
+      - name: Check long_description
+        run: python -m twine check dist/*
 
   install-dev:
-    name: "Verify Dev Env on ${{ matrix.os }}"
-    strategy:
-      matrix:
-        os: ["ubuntu-latest", "windows-latest", "macos-latest"]
-    runs-on: "${{ matrix.os }}"
+    name: "Verify Dev Env on Ubuntu"
+    runs-on: "ubuntu-latest"
     steps:
-      - uses: "actions/checkout@v2"
-      - uses: "actions/setup-python@v2"
+      - uses: "actions/checkout@v3"
+      - uses: "actions/setup-python@v4"
         with:
-          python-version: "3.8"
+          python-version: ${{env.PYTHON_LATEST}}
       - name: "Install in dev mode"
         run: "python -m pip install -e .[dev]"
       - name: "Import package"
         run: "python -c 'import interrogate; print(interrogate.__version__)'"
```

### Comparing `interrogate-1.5.0/.github/workflows/windows.yml` & `interrogate-1.6.0/.github/workflows/windows.yml`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 jobs:
   windows-tests:
     name: "Python ${{ matrix.python-version }} on Windows"
     runs-on: "windows-latest"
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10.0-rc.2"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
-      - uses: "actions/checkout@v2"
-      - uses: "actions/setup-python@v2"
+      - uses: "actions/checkout@v3"
+      - uses: "actions/setup-python@v4"
         with:
           python-version: "${{ matrix.python-version }}"
-      - name: "Install dependencies"
-        run: |
-          python -m pip install --upgrade pip setuptools wheel
-          python -m pip install --upgrade virtualenv tox tox-gh-actions
-      - name: "Run tox targets for ${{ matrix.python-version }}"
-        run: "python -m tox"
+          allow-prereleases: true
+          cache: pip
+      - run: python -Im pip install --upgrade tox
+
+      - name: Run tests on ${{ matrix.python-version }} sans PNG
+        run: python -Im tox -e py$(echo ${{ matrix.python-version }} | tr -d .)
```

### Comparing `interrogate-1.5.0/.pre-commit-config.yaml` & `interrogate-1.6.0/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,43 @@
+---
+ci:
+  autoupdate_schedule: monthly
+
 repos:
-  - repo: local
+  - repo: https://github.com/econchick/interrogate
+    rev: 1.5.0
     hooks:
       - id: interrogate
-        name: interrogate
-        language: system
-        entry: interrogate
-        types: [python]
         exclude: ^(docs/conf.py|setup.py|tests/functional/sample)
         args: [--config=pyproject.toml]
 
   - repo: https://github.com/psf/black
-    rev: 21.8b0
+    rev: 24.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.15.2
     hooks:
-      - id: flake8
-        exclude: ^(tests/functional/sample)
+      - id: pyupgrade
+        args: [--py38-plus]
 
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.9.3
+  - repo: https://github.com/pycqa/isort
+    rev: 5.13.2
     hooks:
       - id: isort
         additional_dependencies: [toml]
 
+  - repo: https://github.com/pycqa/flake8
+    rev: 7.0.0
+    hooks:
+      - id: flake8
+        exclude: ^(tests/functional/sample)
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
+      - id: check-toml
+      - id: check-yaml
```

### Comparing `interrogate-1.5.0/LICENSE` & `interrogate-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/MANIFEST.in` & `interrogate-1.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/PKG-INFO` & `interrogate-1.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: interrogate
-Version: 1.5.0
-Summary: Interrogate a codebase for docstring coverage.
-Home-page: https://interrogate.readthedocs.io
-Author: Lynn Root
-Author-email: lynn@lynnroot.com
-Maintainer: Lynn Root
-Maintainer-email: lynn@lynnroot.com
-License: UNKNOWN
-Project-URL: Documentation, https://interrogate.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/econchick/interrogate/issues
-Project-URL: Source Code, https://github.com/econchick/interrogate
-Keywords: documentation,coverage,quality
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: png
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://interrogate.readthedocs.io/en/latest/_static/logo_pink.png
     :alt: Pink Sloth Logo
 
 =================================
 ``interrogate``: explain yourself
 =================================
 
@@ -80,15 +41,15 @@
 * Assess a new code base for (one aspect of) code quality and maintainability.
 
 Let's get started.
 
 Requirements
 ============
 
-``interrogate`` supports Python 3.6 and above.
+``interrogate`` supports Python 3.8 and above.
 
 
 Installation
 ============
 
 ``interrogate`` is available on `PyPI <https://pypi.org/project/interrogate/>`_ and `GitHub <https://github.com/econchick/interrogate>`_. The recommended installation method is `pip <https://pip.pypa.io/en/stable/>`_-installing into a `virtualenv <https://hynek.me/articles/virtualenv-lives/>`_:
 
@@ -353,18 +314,19 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.5.0  # or master if you're bold
+        rev: 1.6.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
+            pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
 .. code-block:: pycon
 
     >>> from interrogate import coverage
     >>> cov = coverage.InterrogateCoverage(paths=["src"])
@@ -394,14 +356,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
@@ -426,14 +389,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
@@ -483,14 +447,17 @@
 | ``plastic``                        | |plastic-example|              |
 +------------------------------------+--------------------------------+
 | ``social``                         | |social-example|               |
 +------------------------------------+--------------------------------+
 
 .. end-readme
 
+Command Line Options
+====================
+
 To view all options available, run ``interrogate --help``:
 
 .. code-block:: console
 
     interrogate -h
     Usage: interrogate [OPTIONS] [PATHS]...
 
@@ -530,14 +497,18 @@
                                       False]
 
       -n, --ignore-nested-functions   Ignore nested functions and methods.
                                       [default: False]
 
       -C, --ignore-nested-classes     Ignore nested classes.  [default: False]
 
+      -O, --ignore-overloaded-functions
+                                      Ignore `@typing.overload`-decorated functions.
+                                      [default: False]
+
       -p, --ignore-private            Ignore private classes, methods, and
                                       functions starting with two underscores.
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
@@ -637,29 +608,7 @@
 
 .. |docstr-coverage| replace:: ``docstr-coverage``
 .. _docstr-coverage: https://pypi.org/project/docstr-coverage
 .. |docstring-coverage| replace:: ``docstring-coverage``
 .. _docstring-coverage: https://bitbucket.org/DataGreed/docstring-coverage
 
 .. end-credits
-
-Release Information
-===================
-
-1.5.0 (2021-09-10)
-------------------
-
-Added
-^^^^^
-
-* Set minimum ``click`` version (thank you bildzeitung! `#81 <https://github.com/econchick/interrogate/issues/81>`_, `#82 <https://github.com/econchick/interrogate/pull/82>`_).
-* Add ``--omit-covered-files`` flag to skip reporting fully-covered files (`#85 <https://github.com/econchick/interrogate/issues/85>`_).
-* Add support for different badge styles via new ``--badge-style`` flag (`#86 <https://github.com/econchick/interrogate/issues/86>`_).
-* Add 3.10 support!
-
-Fixed
-^^^^^
-* Clarify ``verbose`` configuration (`#83 <https://github.com/econchick/interrogate/issues/83>`_).
-
-
-`Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
-
```

### Comparing `interrogate-1.5.0/README.rst` & `interrogate-1.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,63 @@
+Metadata-Version: 2.1
+Name: interrogate
+Version: 1.6.0
+Summary: Interrogate a codebase for docstring coverage.
+Home-page: https://interrogate.readthedocs.io
+Author: Lynn Root
+Author-email: lynn@lynnroot.com
+Maintainer: Lynn Root
+Maintainer-email: lynn@lynnroot.com
+Project-URL: Documentation, https://interrogate.readthedocs.io
+Project-URL: Bug Tracker, https://github.com/econchick/interrogate/issues
+Project-URL: Source Code, https://github.com/econchick/interrogate
+Keywords: documentation,coverage,quality
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: attrs
+Requires-Dist: click>=7.1
+Requires-Dist: colorama
+Requires-Dist: py
+Requires-Dist: tabulate
+Requires-Dist: toml
+Provides-Extra: png
+Requires-Dist: cairosvg; extra == "png"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-mock; extra == "tests"
+Requires-Dist: coverage[toml]; extra == "tests"
+Provides-Extra: dev
+Requires-Dist: cairosvg; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: coverage[toml]; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+
 .. image:: https://interrogate.readthedocs.io/en/latest/_static/logo_pink.png
     :alt: Pink Sloth Logo
 
 =================================
 ``interrogate``: explain yourself
 =================================
 
@@ -41,15 +97,15 @@
 * Assess a new code base for (one aspect of) code quality and maintainability.
 
 Let's get started.
 
 Requirements
 ============
 
-``interrogate`` supports Python 3.6 and above.
+``interrogate`` supports Python 3.8 and above.
 
 
 Installation
 ============
 
 ``interrogate`` is available on `PyPI <https://pypi.org/project/interrogate/>`_ and `GitHub <https://github.com/econchick/interrogate>`_. The recommended installation method is `pip <https://pip.pypa.io/en/stable/>`_-installing into a `virtualenv <https://hynek.me/articles/virtualenv-lives/>`_:
 
@@ -314,18 +370,19 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.5.0  # or master if you're bold
+        rev: 1.6.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
+            pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
 .. code-block:: pycon
 
     >>> from interrogate import coverage
     >>> cov = coverage.InterrogateCoverage(paths=["src"])
@@ -355,14 +412,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
@@ -387,14 +445,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
@@ -444,14 +503,17 @@
 | ``plastic``                        | |plastic-example|              |
 +------------------------------------+--------------------------------+
 | ``social``                         | |social-example|               |
 +------------------------------------+--------------------------------+
 
 .. end-readme
 
+Command Line Options
+====================
+
 To view all options available, run ``interrogate --help``:
 
 .. code-block:: console
 
     interrogate -h
     Usage: interrogate [OPTIONS] [PATHS]...
 
@@ -491,14 +553,18 @@
                                       False]
 
       -n, --ignore-nested-functions   Ignore nested functions and methods.
                                       [default: False]
 
       -C, --ignore-nested-classes     Ignore nested classes.  [default: False]
 
+      -O, --ignore-overloaded-functions
+                                      Ignore `@typing.overload`-decorated functions.
+                                      [default: False]
+
       -p, --ignore-private            Ignore private classes, methods, and
                                       functions starting with two underscores.
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
@@ -598,7 +664,27 @@
 
 .. |docstr-coverage| replace:: ``docstr-coverage``
 .. _docstr-coverage: https://pypi.org/project/docstr-coverage
 .. |docstring-coverage| replace:: ``docstring-coverage``
 .. _docstring-coverage: https://bitbucket.org/DataGreed/docstring-coverage
 
 .. end-credits
+
+Release Information
+===================
+
+1.6.0 (2024-04-06)
+------------------
+
+Added
+^^^^^
+
+* Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
+* Support for Python 3.11 & 3.12.
+
+Removed
+^^^^^^^
+
+* Support for Python 3.6 & 3.7.
+
+
+`Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `interrogate-1.5.0/docs/Makefile` & `interrogate-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_f.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_f.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_fs.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fs.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_fsm.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_fsm.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_ftb.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_ftb.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_p.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_p.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/badge_examples/interrogate_badge_s.svg` & `interrogate-1.6.0/docs/_static/badge_examples/interrogate_badge_s.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/favicon.png` & `interrogate-1.6.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/interrogate_badge.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/logo_pink.png` & `interrogate-1.6.0/docs/_static/logo_pink.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/_static/logo_smol.png` & `interrogate-1.6.0/docs/_static/logo_smol.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/docs/changelog.rst` & `interrogate-1.6.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 Changelog
 =========
 
 .. short-log
 
+1.6.0 (2024-04-06)
+------------------
+
+Added
+^^^^^
+
+* Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
+* Support for Python 3.11 & 3.12.
+
+Removed
+^^^^^^^
+
+* Support for Python 3.6 & 3.7.
+
+.. short-log
+
 1.5.0 (2021-09-10)
 ------------------
 
 Added
 ^^^^^
 
 * Set minimum ``click`` version (thank you bildzeitung! `#81 <https://github.com/econchick/interrogate/issues/81>`_, `#82 <https://github.com/econchick/interrogate/pull/82>`_).
@@ -14,15 +30,14 @@
 * Add support for different badge styles via new ``--badge-style`` flag (`#86 <https://github.com/econchick/interrogate/issues/86>`_).
 * Add 3.10 support!
 
 Fixed
 ^^^^^
 * Clarify ``verbose`` configuration (`#83 <https://github.com/econchick/interrogate/issues/83>`_).
 
-.. short-log
 
 1.4.0 (2021-05-14)
 ------------------
 
 Added
 ^^^^^
```

### Comparing `interrogate-1.5.0/docs/conf.py` & `interrogate-1.6.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 project = "interrogate"
 copyright = "2020, Lynn Root"
 author = "Lynn Root"
 
 # The short X.Y version.
 release = find_version("../src/interrogate/__init__.py")
-version = release.rsplit(u".", 1)[0]
+version = release.rsplit(".", 1)[0]
 
 master_doc = "index"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -85,15 +85,15 @@
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_favicon = "_static/favicon.png"
 html_css_files = [
     "custom.css",
 ]
 templates_path = ["_templates"]
-html_title = "Python docstring coverage (v{})".format(release)
+html_title = f"Python docstring coverage (v{release})"
 html_short_title = "interrogate: Python docstring coverage"
 
 # -- Other config
 
 # For when I want to turn on API documentation
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
```

### Comparing `interrogate-1.5.0/docs/index.rst` & `interrogate-1.6.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 
     Ignore nested functions and methods.  [default: ``False``]
 
 .. option:: -C, --ignore-nested-classes
 
     Ignore nested classes.  [default: ``False``]
 
+.. option:: -O, --ignore-overloaded-functions
+
+    Ignore `@typing.overload`-decorated functions.  [default: ``False``]
+
 .. option:: -p, --ignore-private
 
     Ignore private classes, methods, and functions starting with two underscores.  [default: ``False``]
 
     NOTE: This does not include magic methods; use ``--ignore-magic`` and/or ``--ignore-init-method`` instead.
 
 .. option:: -P, --ignore-property-decorators
```

### Comparing `interrogate-1.5.0/pyproject.toml` & `interrogate-1.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 [build-system]
-requires = ["setuptools>=40.6.0", "wheel"]
+requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.check-wheel-contents]
+toplevel = ["interrogate"]
+
+
+[tool.pytest.ini_options]
+addopts = ["-ra", "--strict-markers", "--strict-config"]
+testpaths = "tests"
+xfail_strict = true
+
 [tool.coverage.run]
 parallel = true
 branch = true
 source = ["interrogate"]
 omit = ["**/__main__.py"]
 
 [tool.coverage.paths]
-source = ["src", ".tox/*/site-packages"]
+source = ["src", ".tox/py*/**/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = ["pragma: no cover"]
 fail_under = 95
 
 [tool.black]
```

### Comparing `interrogate-1.5.0/setup.py` & `interrogate-1.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         with codecs.open(os.path.join(HERE, fl), "rb", encoding) as f:
             buf.append(f.read())
     return sep.join(buf)
 
 
 def find_meta(meta):
     """Extract __*meta*__ from META_FILE."""
-    re_str = r"^__{meta}__ = ['\"]([^'\"]*)['\"]".format(meta=meta)
+    re_str = rf"^__{meta}__ = ['\"]([^'\"]*)['\"]"
     meta_match = re.search(re_str, META_FILE, re.M)
     if meta_match:
         return meta_match.group(1)
-    raise RuntimeError("Unable to find __{meta}__ string.".format(meta=meta))
+    raise RuntimeError(f"Unable to find __{meta}__ string.")
 
 
 #####
 # Project-specific constants
 #####
 NAME = "interrogate"
 PACKAGE_NAME = "interrogate"
@@ -50,27 +50,24 @@
 KEYWORDS = ["documentation", "coverage", "quality"]
 PROJECT_URLS = {
     "Documentation": "https://interrogate.readthedocs.io",
     "Bug Tracker": "https://github.com/econchick/interrogate/issues",
     "Source Code": "https://github.com/econchick/interrogate",
 }
 CLASSIFIERS = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 INSTALL_REQUIRES = [
     "attrs",
     "click>=7.1",
@@ -78,15 +75,15 @@
     "py",
     "tabulate",
     "toml",
 ]
 EXTRAS_REQUIRE = {
     "png": ["cairosvg"],
     "docs": ["sphinx", "sphinx-autobuild"],
-    "tests": ["pytest", "pytest-cov", "pytest-mock"],
+    "tests": ["pytest", "pytest-cov", "pytest-mock", "coverage[toml]"],
 }
 EXTRAS_REQUIRE["dev"] = (
     EXTRAS_REQUIRE["png"]
     + EXTRAS_REQUIRE["docs"]
     + EXTRAS_REQUIRE["tests"]
     + ["wheel", "pre-commit"]
 )
@@ -94,15 +91,15 @@
 LONG = (
     read("README.rst")
     + "\n"
     + "Release Information\n"
     + "==================="
     + read("docs/changelog.rst").split(".. short-log")[1]
     + "\n`Full changelog "
-    + "<{url}/en/latest/#changelog>`_.".format(url=URL)
+    + f"<{URL}/en/latest/#changelog>`_."
 )
 
 setup(
     name=NAME,
     version=find_meta("version"),
     description=find_meta("description"),
     long_description=LONG,
@@ -114,15 +111,15 @@
     maintainer=find_meta("author"),
     maintainer_email=find_meta("email"),
     keywords=KEYWORDS,
     packages=PACKAGES,
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     entry_points={
         "console_scripts": ["interrogate = interrogate.cli:main"],
     },
     classifiers=CLASSIFIERS,
 )
```

### Comparing `interrogate-1.5.0/src/interrogate/badge/flat-square-modified-style.svg` & `interrogate-1.6.0/src/interrogate/badge/flat-square-modified-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge/flat-square-style.svg` & `interrogate-1.6.0/src/interrogate/badge/flat-square-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge/flat-style.svg` & `interrogate-1.6.0/src/interrogate/badge/flat-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge/for-the-badge-style.svg` & `interrogate-1.6.0/src/interrogate/badge/for-the-badge-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge/plastic-style.svg` & `interrogate-1.6.0/src/interrogate/badge/plastic-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge/social-style.svg` & `interrogate-1.6.0/src/interrogate/badge/social-style.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/src/interrogate/badge_gen.py` & `interrogate-1.6.0/src/interrogate/badge_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright 2020 Lynn Root
 """Module for generating an SVG badge.
 
 Inspired by `coverage-badge <https://github.com/dbrgn/coverage-badge>`_.
 """
 
 import os
+import sys
 
+from importlib import resources
 from xml.dom import minidom
 
-import pkg_resources
-
 
 try:
     import cairosvg
 except ImportError:  # pragma: no cover
     cairosvg = None
 
 
@@ -134,15 +134,15 @@
 
 
 def _format_result(result):
     """Format result into string for templating."""
     # do not include decimal if it's 100
     if result == 100:
         return "100"
-    return "{:.1f}".format(result)
+    return f"{result:.1f}"
 
 
 def get_badge(result, color, style=None):
     """Generate an SVG from template.
 
     :param float result: coverage % result.
     :param str color: color of badge.
@@ -153,17 +153,23 @@
     if style is None:
         style = "flat-square-modified"
     template_file = f"{style}-style.svg"
     badge_template_values = _get_badge_measurements(result, style)
     result = _format_result(result)
     badge_template_values["result"] = result
     badge_template_values["color"] = color
-    template_path = os.path.join("badge", template_file)
-    tmpl = pkg_resources.resource_string(__name__, template_path)
-    tmpl = tmpl.decode("utf8")
+
+    if sys.version_info >= (3, 9):
+        tmpl = (
+            resources.files("interrogate") / "badge" / template_file
+        ).read_text()
+    else:
+        with resources.path("interrogate", "badge") as p:
+            tmpl = (p / template_file).read_text()
+
     for key, value in badge_template_values.items():
         tmpl = tmpl.replace("{{ %s }}" % key, str(value))
     return tmpl
 
 
 def should_generate_badge(output, color, result):
     """Detect if existing badge needs updating.
@@ -208,25 +214,25 @@
 
     rects = badge.getElementsByTagName("rect")
     current_colors = [
         r.getAttribute("style")
         for r in rects
         if r.hasAttribute("data-interrogate")
     ]
-    fill_color = "fill:{}".format(color)
+    fill_color = f"fill:{color}"
     if fill_color not in current_colors:
         return True
 
     texts = badge.getElementsByTagName("text")
     current_results = [
         t.childNodes[0].data
         for t in texts
         if t.hasAttribute("data-interrogate")
     ]
-    result = "{:.1f}%".format(result)
+    result = f"{result:.1f}%"
     if result in current_results:
         return False
     return True
 
 
 def get_color(result):
     """Get color for current doc coverage percent.
```

### Comparing `interrogate-1.5.0/src/interrogate/cli.py` & `interrogate-1.6.0/src/interrogate/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,22 @@
     "--ignore-nested-classes",
     is_flag=True,
     default=False,
     show_default=True,
     help="Ignore nested classes.",
 )
 @click.option(
+    "-O",
+    "--ignore-overloaded-functions",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="Ignore `@typing.overload`-decorated functions.",
+)
+@click.option(
     "-p",
     "--ignore-private",
     is_flag=True,
     default=False,
     show_default=False,
     help=(
         "Ignore private classes, methods, and functions starting with two "
@@ -297,14 +305,15 @@
     .. versionadded:: 1.3.0 ``--ignore-property-decorators``
     .. versionadded:: 1.3.0 config parsing support for setup.cfg
     .. versionadded:: 1.4.0 ``--badge-format``
     .. versionadded:: 1.4.0 ``--ignore-nested-classes``
     .. versionadded:: 1.4.0 ``--ignore-setters``
     .. versionadded:: 1.5.0 ``--omit-covered-files``
     .. versionadded:: 1.5.0 ``--badge-style``
+    .. versionadded:: 1.6.0 ``--ignore-overloaded-functions``
 
     .. versionchanged:: 1.3.1 only generate badge if results change from
         an existing badge.
     """
     gen_badge = kwargs["generate_badge"]
     if kwargs["badge_format"] is not None and gen_badge is None:
         raise click.BadParameter(
@@ -335,14 +344,15 @@
         ignore_module=kwargs["ignore_module"],
         ignore_private=kwargs["ignore_private"],
         ignore_semiprivate=kwargs["ignore_semiprivate"],
         ignore_init_method=kwargs["ignore_init_method"],
         ignore_init_module=kwargs["ignore_init_module"],
         ignore_nested_classes=kwargs["ignore_nested_classes"],
         ignore_nested_functions=kwargs["ignore_nested_functions"],
+        ignore_overloaded_functions=kwargs["ignore_overloaded_functions"],
         ignore_property_setters=kwargs["ignore_setters"],
         ignore_property_decorators=kwargs["ignore_property_decorators"],
         include_regex=kwargs["whitelist_regex"],
         omit_covered_files=kwargs["omit_covered_files"],
     )
     interrogate_coverage = coverage.InterrogateCoverage(
         paths=paths,
@@ -364,10 +374,10 @@
         output_path = badge_gen.create(
             gen_badge,
             results,
             output_format=badge_format,
             output_style=badge_style,
         )
         if not is_quiet:
-            click.echo("Generated badge to {}".format(output_path))
+            click.echo(f"Generated badge to {output_path}")
 
     sys.exit(results.ret_code)
```

### Comparing `interrogate-1.5.0/src/interrogate/config.py` & `interrogate-1.6.0/src/interrogate/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     :param bool ignore_nested_functions: Ignore nested functions and
         methods.
     :param bool ignore_init_module: Ignore ``__init__.py`` modules.
     :param str include_regex: Regex identifying class, method, and
         function names to include.
     :param bool omit_covered_files: Omit reporting files that have 100%
         documentation coverage.
+    :param bool ignore_overloaded_functions: Ignore `@typing.overload`-decorated
+        functions.
     """
 
     color = attr.ib(default=False)
     fail_under = attr.ib(default=80.0)
     ignore_regex = attr.ib(default=False)
     ignore_magic = attr.ib(default=False)
     ignore_module = attr.ib(default=False)
@@ -50,24 +52,25 @@
     ignore_semiprivate = attr.ib(default=False)
     ignore_init_method = attr.ib(default=False)
     ignore_init_module = attr.ib(default=False)
     ignore_nested_classes = attr.ib(default=False)
     ignore_nested_functions = attr.ib(default=False)
     ignore_property_setters = attr.ib(default=False)
     ignore_property_decorators = attr.ib(default=False)
+    ignore_overloaded_functions = attr.ib(default=False)
     include_regex = attr.ib(default=False)
     omit_covered_files = attr.ib(default=False)
 
 
 def find_project_root(srcs):
     """Return a directory containing .git, .hg, or pyproject.toml.
     That directory can be one of the directories passed in `srcs` or their
     common parent.
     If no directory in the tree contains a marker that would specify it's the
-    project root, the root of the file system is returned.k
+    project root, the root of the file system is returned.
     """
     if not srcs:
         return pathlib.Path("/").resolve()
 
     common_base = min(pathlib.Path(src).resolve() for src in srcs)
     if common_base.is_dir():
         # Append a fake file so `parents` below returns `common_base_dir`, too.
@@ -198,24 +201,24 @@
     config = None
     if value.endswith(".toml"):
         try:
             config = parse_pyproject_toml(value)
         except (toml.TomlDecodeError, OSError) as e:
             raise click.FileError(
                 filename=value,
-                hint="Error reading configuration file: {}".format(e),
+                hint=f"Error reading configuration file: {e}",
             )
 
     elif value.endswith(".cfg"):
         try:
             config = parse_setup_cfg(value)
         except configparser.ParsingError as e:
             raise click.FileError(
                 filename=value,
-                hint="Error reading configuration file: {}".format(e),
+                hint=f"Error reading configuration file: {e}",
             )
 
     if not config:
         return None
 
     if ctx.default_map is None:
         ctx.default_map = {}
```

### Comparing `interrogate-1.5.0/src/interrogate/coverage.py` & `interrogate-1.6.0/src/interrogate/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,30 +139,30 @@
             yield f
 
     def get_filenames_from_paths(self):
         """Find all files to measure for docstring coverage."""
         filenames = []
         for path in self.paths:
             if os.path.isfile(path):
-                if not path.endswith(".py"):
+                if not path.endswith(".py") and not path.endswith(".pyi"):
                     msg = (
-                        "E: Invalid file '{}'. Unable interrogate non-Python "
-                        "files.".format(path)
+                        "E: Invalid file '{}'. Unable to interrogate non-Python"
+                        " files.".format(path)
                     )
                     click.echo(msg, err=True)
                     return sys.exit(1)
                 filenames.append(path)
                 continue
             for root, dirs, fs in os.walk(path):
                 full_paths = [os.path.join(root, f) for f in fs]
                 filenames.extend(self._filter_files(full_paths))
 
         if not filenames:
             p = ", ".join(self.paths)
-            msg = "E: No Python files found to interrogate in '{}'.".format(p)
+            msg = f"E: No Python files found to interrogate in '{p}'."
             click.echo(msg, err=True)
             return sys.exit(1)
 
         self.common_base = utils.get_common_base(filenames)
         return filenames
 
     def _filter_nodes(self, nodes):
@@ -198,15 +198,15 @@
 
         filtered_nodes = [n for n in nodes if n not in inner_nested_nodes]
         filtered_nodes = [n for n in filtered_nodes if n not in nested_cls]
         return filtered_nodes
 
     def _get_file_coverage(self, filename):
         """Get coverage results for a particular file."""
-        with open(filename, "r", encoding="utf-8") as f:
+        with open(filename, encoding="utf-8") as f:
             source_tree = f.read()
 
         parsed_tree = ast.parse(source_tree)
         visitor = visit.CoverageVisitor(filename=filename, config=self.config)
         visitor.visit(parsed_tree)
 
         filtered_nodes = self._filter_nodes(visitor.nodes)
@@ -264,21 +264,21 @@
     def _get_detailed_row(self, node, filename):
         """Generate a row of data for the detailed view."""
         filename = self._get_filename(filename)
 
         if node.node_type == "Module":
             if self.config.ignore_module:
                 return [filename, ""]
-            name = "{} (module)".format(filename)
+            name = f"{filename} (module)"
         else:
             name = node.path.split(":")[-1]
-            name = "{} (L{})".format(name, node.lineno)
+            name = f"{name} (L{node.lineno})"
 
         padding = "  " * node.level
-        name = "{}{}".format(padding, name)
+        name = f"{padding}{name}"
         status = "MISSED" if not node.covered else "COVERED"
         return [name, status]
 
     def _create_detailed_table(self, combined_results):
         """Generate table for the detailed view.
 
         The detailed view shows coverage of each module, class, and
@@ -348,30 +348,30 @@
         for file_result in combined_results.file_results:
             filename = self._get_filename(file_result.filename)
             if (
                 self.config.omit_covered_files
                 and file_result.perc_covered == 100
             ):
                 continue
-            perc_covered = "{:.0f}%".format(file_result.perc_covered)
+            perc_covered = f"{file_result.perc_covered:.0f}%"
             row = [
                 filename,
                 file_result.total,
                 file_result.missing,
                 file_result.covered,
                 perc_covered,
             ]
             table.append(row)
 
         # avoid printing an unneeded second separator if there are
         # no summary results from --omit-covered
         if len(table) > 2:
             table.append(self.output_formatter.TABLE_SEPARATOR)
 
-        total_perc_covered = "{:.1f}%".format(combined_results.perc_covered)
+        total_perc_covered = f"{combined_results.perc_covered:.1f}%"
         total_row = [
             "TOTAL",
             combined_results.total,
             combined_results.missing,
             combined_results.covered,
             total_perc_covered,
         ]
@@ -396,21 +396,19 @@
         self.output_formatter.tw.line(to_print)
 
     @staticmethod
     def _sort_results(results):
         """Sort results by filename, directories first"""
         all_filenames_map = {r.filename: r for r in results.file_results}
         all_dirs = sorted(
-            set(
-                [
-                    os.path.dirname(r.filename)
-                    for r in results.file_results
-                    if os.path.dirname(r.filename) != ""
-                ]
-            )
+            {
+                os.path.dirname(r.filename)
+                for r in results.file_results
+                if os.path.dirname(r.filename) != ""
+            }
         )
 
         sorted_results = []
         while all_dirs:
             current_dir = all_dirs.pop(0)
             files = []
             for p in os.listdir(current_dir):
@@ -481,15 +479,15 @@
                 file=f, config=self.config
             )
             results = self._sort_results(results)
             if verbosity > 0:
                 base = self._get_header_base()
                 self.output_formatter.tw.sep(
                     "=",
-                    "Coverage for {}".format(base),
+                    f"Coverage for {base}",
                     fullwidth=self.output_formatter.TERMINAL_WIDTH,
                 )
             if verbosity > 1:
                 self._print_detailed_table(results)
             if verbosity > 0:
                 self._print_summary_table(results)
```

### Comparing `interrogate-1.5.0/src/interrogate/utils.py` & `interrogate-1.6.0/src/interrogate/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
         :return: A table formatter for printing desired output.
         :rtype: tabulate.TableFormat
         """
         assert table_type in (
             "detailed",
             "summary",
-        ), "'{}' is not a supported table type".format(table_type)
+        ), f"'{table_type}' is not a supported table type"
         line_formatter = functools.partial(
             self._interrogate_line_formatter, table_type=table_type
         )
         return tabulate.TableFormat(
             lineabove=None,
             linebelowheader=None,
             linebetweenrows=None,
```

### Comparing `interrogate-1.5.0/src/interrogate/visit.py` & `interrogate-1.6.0/src/interrogate/visit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # Copyright 2020 Lynn Root
 """AST traversal for finding docstrings."""
 
 import ast
 import os
-import sys
 
 import attr
 
 
-PY_38_HIGHER = sys.version_info >= (3, 8)
-
-
 @attr.s(eq=False)
 class CovNode:
     """Coverage of an AST Node.
 
     :param str name: Name of node (module, class, method or function
         names).
     :param str path: Pseudo-import path to node (i.e. ``sample.py:
@@ -79,20 +75,14 @@
                 path = parent_path + ":" + node_name
             else:
                 path = parent_path + "." + node_name
 
         lineno = None
         if hasattr(node, "lineno"):
             lineno = node.lineno
-            # Python 3.8+ fixed the line number calc for decorated functions;
-            # previously the AST node would report the line number of the
-            # decorator, not the obj itself. We're going to try and back-port.
-            if not PY_38_HIGHER:
-                if hasattr(node, "decorator_list"):
-                    lineno += len(node.decorator_list)
 
         node_type = type(node).__name__
         cov_node = CovNode(
             name=node_name,
             path=path,
             covered=self._has_doc(node),
             level=len(self.stack),
@@ -186,35 +176,58 @@
 
         for dec in node.decorator_list:
             if hasattr(dec, "attr"):
                 if dec.attr == "setter":
                     return True
         return False
 
+    def _has_overload_decorator(self, node):
+        """Detect if node has a typing.overload decorator."""
+        if not hasattr(node, "decorator_list"):
+            return False
+
+        for dec in node.decorator_list:
+            if (
+                hasattr(dec, "attr")
+                and hasattr(dec, "value")
+                and hasattr(dec.value, "id")
+                and dec.value.id == "typing"
+                and dec.attr == "overload"
+            ):
+                # @typing.overload decorator
+                return True
+            if hasattr(dec, "id") and dec.id == "overload":
+                # @overload decorator
+                return True
+        return False
+
     def _is_func_ignored(self, node):
         """Should the AST visitor ignore this func/method node."""
         is_init = node.name == "__init__"
         is_magic = all(
             [
                 node.name.startswith("__"),
                 node.name.endswith("__"),
                 node.name != "__init__",
             ]
         )
         has_property_decorators = self._has_property_decorators(node)
         has_setters = self._has_setters(node)
+        has_overload = self._has_overload_decorator(node)
 
         if self.config.ignore_init_method and is_init:
             return True
         if self.config.ignore_magic and is_magic:
             return True
         if self.config.ignore_property_decorators and has_property_decorators:
             return True
         if self.config.ignore_property_setters and has_setters:
             return True
+        if self.config.ignore_overloaded_functions and has_overload:
+            return True
 
         return self._is_ignored_common(node)
 
     def _is_class_ignored(self, node):
         """Should the AST visitor ignore this class node."""
         return self._is_ignored_common(node)
```

### Comparing `interrogate-1.5.0/src/interrogate.egg-info/PKG-INFO` & `interrogate-1.6.0/src/interrogate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 Metadata-Version: 2.1
 Name: interrogate
-Version: 1.5.0
+Version: 1.6.0
 Summary: Interrogate a codebase for docstring coverage.
 Home-page: https://interrogate.readthedocs.io
 Author: Lynn Root
 Author-email: lynn@lynnroot.com
 Maintainer: Lynn Root
 Maintainer-email: lynn@lynnroot.com
-License: UNKNOWN
 Project-URL: Documentation, https://interrogate.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/econchick/interrogate/issues
 Project-URL: Source Code, https://github.com/econchick/interrogate
 Keywords: documentation,coverage,quality
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: attrs
+Requires-Dist: click>=7.1
+Requires-Dist: colorama
+Requires-Dist: py
+Requires-Dist: tabulate
+Requires-Dist: toml
 Provides-Extra: png
+Requires-Dist: cairosvg; extra == "png"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-mock; extra == "tests"
+Requires-Dist: coverage[toml]; extra == "tests"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: cairosvg; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: coverage[toml]; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 .. image:: https://interrogate.readthedocs.io/en/latest/_static/logo_pink.png
     :alt: Pink Sloth Logo
 
 =================================
 ``interrogate``: explain yourself
 =================================
@@ -80,15 +97,15 @@
 * Assess a new code base for (one aspect of) code quality and maintainability.
 
 Let's get started.
 
 Requirements
 ============
 
-``interrogate`` supports Python 3.6 and above.
+``interrogate`` supports Python 3.8 and above.
 
 
 Installation
 ============
 
 ``interrogate`` is available on `PyPI <https://pypi.org/project/interrogate/>`_ and `GitHub <https://github.com/econchick/interrogate>`_. The recommended installation method is `pip <https://pip.pypa.io/en/stable/>`_-installing into a `virtualenv <https://hynek.me/articles/virtualenv-lives/>`_:
 
@@ -353,18 +370,19 @@
 
 Or use it with `pre-commit <https://pre-commit.com/>`_:
 
 .. code-block:: yaml
 
     repos:
       - repo: https://github.com/econchick/interrogate
-        rev: 1.5.0  # or master if you're bold
+        rev: 1.6.0  # or master if you're bold
         hooks:
           - id: interrogate
             args: [--quiet, --fail-under=95]
+            pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 
 Use it within your code directly:
 
 .. code-block:: pycon
 
     >>> from interrogate import coverage
     >>> cov = coverage.InterrogateCoverage(paths=["src"])
@@ -394,14 +412,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = ["setup.py", "docs", "build"]
     ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
     # possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex = []
@@ -426,14 +445,15 @@
     ignore-semiprivate = false
     ignore-private = false
     ignore-property-decorators = false
     ignore-module = false
     ignore-nested-functions = false
     ignore-nested-classes = true
     ignore-setters = false
+    ignore-overloaded-functions = false
     fail-under = 95
     exclude = setup.py,docs,build
     ignore-regex = ^get$,^mock_.*,.*BaseClass.*
     ; possible values: 0 (minimal output), 1 (-v), 2 (-vv)
     verbose = 0
     quiet = false
     whitelist-regex =
@@ -483,14 +503,17 @@
 | ``plastic``                        | |plastic-example|              |
 +------------------------------------+--------------------------------+
 | ``social``                         | |social-example|               |
 +------------------------------------+--------------------------------+
 
 .. end-readme
 
+Command Line Options
+====================
+
 To view all options available, run ``interrogate --help``:
 
 .. code-block:: console
 
     interrogate -h
     Usage: interrogate [OPTIONS] [PATHS]...
 
@@ -530,14 +553,18 @@
                                       False]
 
       -n, --ignore-nested-functions   Ignore nested functions and methods.
                                       [default: False]
 
       -C, --ignore-nested-classes     Ignore nested classes.  [default: False]
 
+      -O, --ignore-overloaded-functions
+                                      Ignore `@typing.overload`-decorated functions.
+                                      [default: False]
+
       -p, --ignore-private            Ignore private classes, methods, and
                                       functions starting with two underscores.
                                       [default: False]
 
                                       NOTE: This does not include magic methods;
                                       use `--ignore-magic` and/or `--ignore-init-
                                       method` instead.
@@ -641,25 +668,23 @@
 .. _docstring-coverage: https://bitbucket.org/DataGreed/docstring-coverage
 
 .. end-credits
 
 Release Information
 ===================
 
-1.5.0 (2021-09-10)
+1.6.0 (2024-04-06)
 ------------------
 
 Added
 ^^^^^
 
-* Set minimum ``click`` version (thank you bildzeitung! `#81 <https://github.com/econchick/interrogate/issues/81>`_, `#82 <https://github.com/econchick/interrogate/pull/82>`_).
-* Add ``--omit-covered-files`` flag to skip reporting fully-covered files (`#85 <https://github.com/econchick/interrogate/issues/85>`_).
-* Add support for different badge styles via new ``--badge-style`` flag (`#86 <https://github.com/econchick/interrogate/issues/86>`_).
-* Add 3.10 support!
+* Add ``--ignore-overloaded-functions`` flag to ignore overload decorators (`#97 <https://github.com/econchick/interrogate/issues/97>`_) – thank you `ErwinJunge <https://github.com/econchick/interrogate/pull/98>`_ (via `#167 <https://github.com/econchick/interrogate/pull/167>`_) and `zackyancey <https://github.com/econchick/interrogate/pull/160>`_.
+* Support for Python 3.11 & 3.12.
 
-Fixed
-^^^^^
-* Clarify ``verbose`` configuration (`#83 <https://github.com/econchick/interrogate/issues/83>`_).
+Removed
+^^^^^^^
 
+* Support for Python 3.6 & 3.7.
 
-`Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
 
+`Full changelog <https://interrogate.readthedocs.io/en/latest/#changelog>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `interrogate-1.5.0/src/interrogate.egg-info/SOURCES.txt` & `interrogate-1.6.0/src/interrogate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 .pre-commit-config.yaml
 .pre-commit-hooks.yaml
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
 codecov.yml
 pyproject.toml
 setup.py
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/autoupdate-pre-commit-config.yml
 .github/workflows/main.yml
+.github/workflows/pypi.yml
 .github/workflows/sanity.yml
 .github/workflows/windows.yml
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/docutils.conf
 docs/index.rst
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_badge.svg` & `interrogate-1.6.0/tests/functional/fixtures/expected_badge.svg`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 2e63 6f6d 2f22 2073 7479 6c65 3d22 6669  .com/" style="fi
 000000d0: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
 000000e0: 636c 6970 2d72 756c 653a 6576 656e 6f64  clip-rule:evenod
 000000f0: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
 00000100: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
 00000110: 6974 6572 6c69 6d69 743a 323b 223e 0a20  iterlimit:2;">. 
 00000120: 2020 203c 7469 746c 653e 696e 7465 7272     <title>interr
-00000130: 6f67 6174 653a 2034 362e 3425 3c2f 7469  ogate: 46.4%</ti
+00000130: 6f67 6174 653a 2035 302e 3025 3c2f 7469  ogate: 50.0%</ti
 00000140: 746c 653e 0a20 2020 203c 6720 7472 616e  tle>.    <g tran
 00000150: 7366 6f72 6d3d 226d 6174 7269 7828 312c  sform="matrix(1,
 00000160: 302c 302c 312c 3232 2c30 2922 3e0a 2020  0,0,1,22,0)">.  
 00000170: 2020 2020 2020 3c67 2069 643d 2262 6163        <g id="bac
 00000180: 6b67 726f 756e 6473 2220 7472 616e 7366  kgrounds" transf
 00000190: 6f72 6d3d 226d 6174 7269 7828 312e 3332  orm="matrix(1.32
 000001a0: 3738 392c 302c 302c 312c 2d32 322e 3338  789,0,0,1,-22.38
@@ -72,22 +72,22 @@
 00000470: 7465 7874 2078 3d22 3131 3630 2220 793d  text x="1160" y=
 00000480: 2231 3530 2220 6669 6c6c 3d22 2330 3130  "150" fill="#010
 00000490: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
 000004a0: 793d 222e 3322 2074 7261 6e73 666f 726d  y=".3" transform
 000004b0: 3d22 7363 616c 6528 2e31 2922 2074 6578  ="scale(.1)" tex
 000004c0: 744c 656e 6774 683d 2233 3730 2220 6461  tLength="370" da
 000004d0: 7461 2d69 6e74 6572 726f 6761 7465 3d22  ta-interrogate="
-000004e0: 7265 7375 6c74 223e 3436 2e34 253c 2f74  result">46.4%</t
+000004e0: 7265 7375 6c74 223e 3530 2e30 253c 2f74  result">50.0%</t
 000004f0: 6578 743e 0a20 2020 2020 2020 203c 7465  ext>.        <te
 00000500: 7874 2078 3d22 3131 3630 2220 793d 2231  xt x="1160" y="1
 00000510: 3430 2220 7472 616e 7366 6f72 6d3d 2273  40" transform="s
 00000520: 6361 6c65 282e 3129 2220 7465 7874 4c65  cale(.1)" textLe
 00000530: 6e67 7468 3d22 3337 3022 2064 6174 612d  ngth="370" data-
 00000540: 696e 7465 7272 6f67 6174 653d 2272 6573  interrogate="res
-00000550: 756c 7422 3e34 362e 3425 3c2f 7465 7874  ult">46.4%</text
+00000550: 756c 7422 3e35 302e 3025 3c2f 7465 7874  ult">50.0%</text
 00000560: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00000570: 6720 6964 3d22 6c6f 676f 2d73 6861 646f  g id="logo-shado
 00000580: 7722 2073 6572 6966 3a69 643d 226c 6f67  w" serif:id="log
 00000590: 6f20 7368 6164 6f77 2220 7472 616e 7366  o shadow" transf
 000005a0: 6f72 6d3d 226d 6174 7269 7828 302e 3835  orm="matrix(0.85
 000005b0: 3438 3736 2c30 2c30 2c30 2e38 3534 3837  4876,0,0,0.85487
 000005c0: 362c 2d36 2e37 3335 3134 2c31 2e37 3332  6,-6.73514,1.732
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_detailed.txt` & `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,77 @@
------------------------------- Detailed Coverage -------------------------------
-| Name                                                             |    Status |
-|------------------------------------------------------------------|-----------|
-| __init__.py (module)                                             |   COVERED |
-|------------------------------------------------------------------|-----------|
-| empty.py (module)                                                |    MISSED |
-|------------------------------------------------------------------|-----------|
-| full.py (module)                                                 |   COVERED |
-|   Foo (L5)                                                       |   COVERED |
-|     Foo.__init__ (L8)                                            |   COVERED |
-|     Foo.__str__ (L12)                                            |   COVERED |
-|     Foo._semiprivate (L16)                                       |   COVERED |
-|     Foo.__private (L20)                                          |   COVERED |
-|     Foo.method_foo (L24)                                         |   COVERED |
-|     Foo.get (L28)                                                |   COVERED |
-|     Foo.get (L32)                                                |   COVERED |
-|     Foo.prop (L37)                                               |   COVERED |
-|     Foo.prop (L42)                                               |   COVERED |
-|   top_level_func (L47)                                           |   COVERED |
-|     top_level_func.inner_func (L50)                              |   COVERED |
-|   Bar (L55)                                                      |   COVERED |
-|     Bar.method_bar (L58)                                         |   COVERED |
-|       Bar.method_bar.InnerBar (L61)                              |   COVERED |
-|   _SemiprivateClass (L67)                                        |   COVERED |
-|   __PrivateClass (L73)                                           |   COVERED |
-|------------------------------------------------------------------|-----------|
-| partial.py (module)                                              |   COVERED |
-|   Foo (L5)                                                       |   COVERED |
-|     Foo.__init__ (L8)                                            |   COVERED |
-|     Foo.__str__ (L12)                                            |   COVERED |
-|     Foo.__repr__ (L16)                                           |    MISSED |
-|     Foo._semiprivate_documented (L19)                            |   COVERED |
-|     Foo._semiprivate_undocumented (L23)                          |    MISSED |
-|     Foo.__private (L26)                                          |    MISSED |
-|     Foo.method_foo (L29)                                         |    MISSED |
-|     Foo.get (L32)                                                |    MISSED |
-|     Foo.get (L35)                                                |    MISSED |
-|     Foo.a_prop (L39)                                             |    MISSED |
-|     Foo.a_prop (L43)                                             |    MISSED |
-|   documented_top_level_func (L47)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L50)        |   COVERED |
-|   undocumented_top_level_func (L55)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L56)    |    MISSED |
-|   Bar (L60)                                                      |    MISSED |
-|     Bar.method_bar (L61)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L62)                              |    MISSED |
-|   _SemiprivateClass (L66)                                        |    MISSED |
-|   __PrivateClass (L70)                                           |    MISSED |
-|------------------------------------------------------------------|-----------|
-| child_sample/__init__.py (module)                                |    MISSED |
-|------------------------------------------------------------------|-----------|
-| child_sample/child_sample_module.py (module)                     |    MISSED |
-|   ChildFoo (L5)                                                  |    MISSED |
-|     ChildFoo.__init__ (L6)                                       |    MISSED |
-|     ChildFoo.__str__ (L9)                                        |    MISSED |
-|     ChildFoo._ignore_me (L12)                                    |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
-|     ChildFoo.method_foo (L18)                                    |    MISSED |
-|   a_child_func (L22)                                             |    MISSED |
-|   ChildBar (L26)                                                 |    MISSED |
-|     ChildBar.method_bar (L27)                                    |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
-|   _ChildBaz (L34)                                                |    MISSED |
-|   __ChildBla (L38)                                               |    MISSED |
-|------------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage ------------------------------
+| Name                                                            |    Status |
+|-----------------------------------------------------------------|-----------|
+| __init__.py (module)                                            |   COVERED |
+|-----------------------------------------------------------------|-----------|
+| empty.py (module)                                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| full.py (module)                                                |   COVERED |
+|   Foo (L8)                                                      |   COVERED |
+|     Foo.__init__ (L11)                                          |   COVERED |
+|     Foo.__str__ (L15)                                           |   COVERED |
+|     Foo._semiprivate (L19)                                      |   COVERED |
+|     Foo.__private (L23)                                         |   COVERED |
+|     Foo.method_foo (L27)                                        |   COVERED |
+|     Foo.get (L31)                                               |   COVERED |
+|     Foo.get (L35)                                               |   COVERED |
+|     Foo.prop (L40)                                              |   COVERED |
+|     Foo.prop (L45)                                              |   COVERED |
+|     Foo.module_overload (L50)                                   |   COVERED |
+|     Foo.module_overload (L55)                                   |   COVERED |
+|     Foo.module_overload (L59)                                   |   COVERED |
+|     Foo.simple_overload (L64)                                   |   COVERED |
+|     Foo.simple_overload (L69)                                   |   COVERED |
+|     Foo.simple_overload (L73)                                   |   COVERED |
+|   top_level_func (L78)                                          |   COVERED |
+|     top_level_func.inner_func (L81)                             |   COVERED |
+|   Bar (L86)                                                     |   COVERED |
+|     Bar.method_bar (L89)                                        |   COVERED |
+|       Bar.method_bar.InnerBar (L92)                             |   COVERED |
+|   _SemiprivateClass (L98)                                       |   COVERED |
+|   __PrivateClass (L104)                                         |   COVERED |
+|-----------------------------------------------------------------|-----------|
+| partial.py (module)                                             |   COVERED |
+|   Foo (L8)                                                      |   COVERED |
+|     Foo.__init__ (L11)                                          |   COVERED |
+|     Foo.__str__ (L15)                                           |   COVERED |
+|     Foo.__repr__ (L19)                                          |    MISSED |
+|     Foo._semiprivate_documented (L22)                           |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                         |    MISSED |
+|     Foo.__private (L29)                                         |    MISSED |
+|     Foo.method_foo (L32)                                        |    MISSED |
+|     Foo.get (L35)                                               |    MISSED |
+|     Foo.get (L38)                                               |    MISSED |
+|     Foo.a_prop (L42)                                            |    MISSED |
+|     Foo.a_prop (L46)                                            |    MISSED |
+|     Foo.module_overload (L50)                                   |    MISSED |
+|     Foo.module_overload (L53)                                   |    MISSED |
+|     Foo.module_overload (L55)                                   |   COVERED |
+|     Foo.simple_overload (L60)                                   |    MISSED |
+|     Foo.simple_overload (L63)                                   |    MISSED |
+|     Foo.simple_overload (L65)                                   |   COVERED |
+|   documented_top_level_func (L70)                               |   COVERED |
+|     documented_top_level_func.documented_inner_func (L73)       |   COVERED |
+|   undocumented_top_level_func (L78)                             |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L79)   |    MISSED |
+|   Bar (L83)                                                     |    MISSED |
+|     Bar.method_bar (L84)                                        |    MISSED |
+|       Bar.method_bar.InnerBar (L85)                             |    MISSED |
+|   _SemiprivateClass (L89)                                       |    MISSED |
+|   __PrivateClass (L93)                                          |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\__init__.py (module)                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\child_sample_module.py (module)                    |    MISSED |
+|   ChildFoo (L5)                                                 |    MISSED |
+|     ChildFoo.__init__ (L6)                                      |    MISSED |
+|     ChildFoo.__str__ (L9)                                       |    MISSED |
+|     ChildFoo._ignore_me (L12)                                   |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
+|     ChildFoo.method_foo (L18)                                   |    MISSED |
+|   a_child_func (L22)                                            |    MISSED |
+|   ChildBar (L26)                                                |    MISSED |
+|     ChildBar.method_bar (L27)                                   |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
+|   _ChildBaz (L34)                                               |    MISSED |
+|   __ChildBla (L38)                                              |    MISSED |
+|-----------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_detailed_no_module.txt` & `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_skip_covered.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,50 @@
------------------------------- Detailed Coverage -------------------------------
-| Name                                                             |    Status |
-|------------------------------------------------------------------|-----------|
-| full.py                                                          |           |
-|   Foo (L5)                                                       |   COVERED |
-|     Foo.__init__ (L8)                                            |   COVERED |
-|     Foo.__str__ (L12)                                            |   COVERED |
-|     Foo._semiprivate (L16)                                       |   COVERED |
-|     Foo.__private (L20)                                          |   COVERED |
-|     Foo.method_foo (L24)                                         |   COVERED |
-|     Foo.get (L28)                                                |   COVERED |
-|     Foo.get (L32)                                                |   COVERED |
-|     Foo.prop (L37)                                               |   COVERED |
-|     Foo.prop (L42)                                               |   COVERED |
-|   top_level_func (L47)                                           |   COVERED |
-|     top_level_func.inner_func (L50)                              |   COVERED |
-|   Bar (L55)                                                      |   COVERED |
-|     Bar.method_bar (L58)                                         |   COVERED |
-|       Bar.method_bar.InnerBar (L61)                              |   COVERED |
-|   _SemiprivateClass (L67)                                        |   COVERED |
-|   __PrivateClass (L73)                                           |   COVERED |
-|------------------------------------------------------------------|-----------|
-| partial.py                                                       |           |
-|   Foo (L5)                                                       |   COVERED |
-|     Foo.__init__ (L8)                                            |   COVERED |
-|     Foo.__str__ (L12)                                            |   COVERED |
-|     Foo.__repr__ (L16)                                           |    MISSED |
-|     Foo._semiprivate_documented (L19)                            |   COVERED |
-|     Foo._semiprivate_undocumented (L23)                          |    MISSED |
-|     Foo.__private (L26)                                          |    MISSED |
-|     Foo.method_foo (L29)                                         |    MISSED |
-|     Foo.get (L32)                                                |    MISSED |
-|     Foo.get (L35)                                                |    MISSED |
-|     Foo.a_prop (L39)                                             |    MISSED |
-|     Foo.a_prop (L43)                                             |    MISSED |
-|   documented_top_level_func (L47)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L50)        |   COVERED |
-|   undocumented_top_level_func (L55)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L56)    |    MISSED |
-|   Bar (L60)                                                      |    MISSED |
-|     Bar.method_bar (L61)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L62)                              |    MISSED |
-|   _SemiprivateClass (L66)                                        |    MISSED |
-|   __PrivateClass (L70)                                           |    MISSED |
-|------------------------------------------------------------------|-----------|
-| child_sample/child_sample_module.py                              |           |
-|   ChildFoo (L5)                                                  |    MISSED |
-|     ChildFoo.__init__ (L6)                                       |    MISSED |
-|     ChildFoo.__str__ (L9)                                        |    MISSED |
-|     ChildFoo._ignore_me (L12)                                    |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
-|     ChildFoo.method_foo (L18)                                    |    MISSED |
-|   a_child_func (L22)                                             |    MISSED |
-|   ChildBar (L26)                                                 |    MISSED |
-|     ChildBar.method_bar (L27)                                    |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
-|   _ChildBaz (L34)                                                |    MISSED |
-|   __ChildBla (L38)                                               |    MISSED |
-|------------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage ------------------------------
+| Name                                                            |    Status |
+|-----------------------------------------------------------------|-----------|
+| empty.py (module)                                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| partial.py (module)                                             |   COVERED |
+|   Foo (L8)                                                      |   COVERED |
+|     Foo.__init__ (L11)                                          |   COVERED |
+|     Foo.__str__ (L15)                                           |   COVERED |
+|     Foo.__repr__ (L19)                                          |    MISSED |
+|     Foo._semiprivate_documented (L22)                           |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                         |    MISSED |
+|     Foo.__private (L29)                                         |    MISSED |
+|     Foo.method_foo (L32)                                        |    MISSED |
+|     Foo.get (L35)                                               |    MISSED |
+|     Foo.get (L38)                                               |    MISSED |
+|     Foo.a_prop (L42)                                            |    MISSED |
+|     Foo.a_prop (L46)                                            |    MISSED |
+|     Foo.module_overload (L50)                                   |    MISSED |
+|     Foo.module_overload (L53)                                   |    MISSED |
+|     Foo.module_overload (L55)                                   |   COVERED |
+|     Foo.simple_overload (L60)                                   |    MISSED |
+|     Foo.simple_overload (L63)                                   |    MISSED |
+|     Foo.simple_overload (L65)                                   |   COVERED |
+|   documented_top_level_func (L70)                               |   COVERED |
+|     documented_top_level_func.documented_inner_func (L73)       |   COVERED |
+|   undocumented_top_level_func (L78)                             |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L79)   |    MISSED |
+|   Bar (L83)                                                     |    MISSED |
+|     Bar.method_bar (L84)                                        |    MISSED |
+|       Bar.method_bar.InnerBar (L85)                             |    MISSED |
+|   _SemiprivateClass (L89)                                       |    MISSED |
+|   __PrivateClass (L93)                                          |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\__init__.py (module)                               |    MISSED |
+|-----------------------------------------------------------------|-----------|
+| child_sample\child_sample_module.py (module)                    |    MISSED |
+|   ChildFoo (L5)                                                 |    MISSED |
+|     ChildFoo.__init__ (L6)                                      |    MISSED |
+|     ChildFoo.__str__ (L9)                                       |    MISSED |
+|     ChildFoo._ignore_me (L12)                                   |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
+|     ChildFoo.method_foo (L18)                                   |    MISSED |
+|   a_child_func (L22)                                            |    MISSED |
+|   ChildBar (L26)                                                |    MISSED |
+|     ChildBar.method_bar (L27)                                   |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
+|   _ChildBaz (L34)                                               |    MISSED |
+|   __ChildBla (L38)                                              |    MISSED |
+|-----------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_detailed_single_file.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_single_file.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 ------------------------------ Detailed Coverage -------------------------------
 | Name                                                |                 Status |
 |-----------------------------------------------------|------------------------|
 | full.py (module)                                    |                COVERED |
-|   Foo (L5)                                          |                COVERED |
-|     Foo.__init__ (L8)                               |                COVERED |
-|     Foo.__str__ (L12)                               |                COVERED |
-|     Foo._semiprivate (L16)                          |                COVERED |
-|     Foo.__private (L20)                             |                COVERED |
-|     Foo.method_foo (L24)                            |                COVERED |
-|     Foo.get (L28)                                   |                COVERED |
-|     Foo.get (L32)                                   |                COVERED |
-|     Foo.prop (L37)                                  |                COVERED |
-|     Foo.prop (L42)                                  |                COVERED |
-|   top_level_func (L47)                              |                COVERED |
-|     top_level_func.inner_func (L50)                 |                COVERED |
-|   Bar (L55)                                         |                COVERED |
-|     Bar.method_bar (L58)                            |                COVERED |
-|       Bar.method_bar.InnerBar (L61)                 |                COVERED |
-|   _SemiprivateClass (L67)                           |                COVERED |
-|   __PrivateClass (L73)                              |                COVERED |
+|   Foo (L8)                                          |                COVERED |
+|     Foo.__init__ (L11)                              |                COVERED |
+|     Foo.__str__ (L15)                               |                COVERED |
+|     Foo._semiprivate (L19)                          |                COVERED |
+|     Foo.__private (L23)                             |                COVERED |
+|     Foo.method_foo (L27)                            |                COVERED |
+|     Foo.get (L31)                                   |                COVERED |
+|     Foo.get (L35)                                   |                COVERED |
+|     Foo.prop (L40)                                  |                COVERED |
+|     Foo.prop (L45)                                  |                COVERED |
+|     Foo.module_overload (L50)                       |                COVERED |
+|     Foo.module_overload (L55)                       |                COVERED |
+|     Foo.module_overload (L59)                       |                COVERED |
+|     Foo.simple_overload (L64)                       |                COVERED |
+|     Foo.simple_overload (L69)                       |                COVERED |
+|     Foo.simple_overload (L73)                       |                COVERED |
+|   top_level_func (L78)                              |                COVERED |
+|     top_level_func.inner_func (L81)                 |                COVERED |
+|   Bar (L86)                                         |                COVERED |
+|     Bar.method_bar (L89)                            |                COVERED |
+|       Bar.method_bar.InnerBar (L92)                 |                COVERED |
+|   _SemiprivateClass (L98)                           |                COVERED |
+|   __PrivateClass (L104)                             |                COVERED |
 |-----------------------------------------------------|------------------------|
 
 ----------------------------------- Summary ------------------------------------
 | Name             |        Total |        Miss |        Cover |        Cover% |
 |------------------|--------------|-------------|--------------|---------------|
-| full.py          |           18 |           0 |           18 |          100% |
+| full.py          |           24 |           0 |           24 |          100% |
 |------------------|--------------|-------------|--------------|---------------|
-| TOTAL            |           18 |           0 |           18 |        100.0% |
+| TOTAL            |           24 |           0 |           24 |        100.0% |
 --------------- RESULT: PASSED (minimum: 80.0%, actual: 100.0%) ----------------
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_detailed_skip_covered.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_skip_covered.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 ------------------------------ Detailed Coverage -------------------------------
 | Name                                                             |    Status |
 |------------------------------------------------------------------|-----------|
 | empty.py (module)                                                |    MISSED |
 |------------------------------------------------------------------|-----------|
 | partial.py (module)                                              |   COVERED |
-|   Foo (L5)                                                       |   COVERED |
-|     Foo.__init__ (L8)                                            |   COVERED |
-|     Foo.__str__ (L12)                                            |   COVERED |
-|     Foo.__repr__ (L16)                                           |    MISSED |
-|     Foo._semiprivate_documented (L19)                            |   COVERED |
-|     Foo._semiprivate_undocumented (L23)                          |    MISSED |
-|     Foo.__private (L26)                                          |    MISSED |
-|     Foo.method_foo (L29)                                         |    MISSED |
-|     Foo.get (L32)                                                |    MISSED |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo.__repr__ (L19)                                           |    MISSED |
+|     Foo._semiprivate_documented (L22)                            |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                          |    MISSED |
+|     Foo.__private (L29)                                          |    MISSED |
+|     Foo.method_foo (L32)                                         |    MISSED |
 |     Foo.get (L35)                                                |    MISSED |
-|     Foo.a_prop (L39)                                             |    MISSED |
-|     Foo.a_prop (L43)                                             |    MISSED |
-|   documented_top_level_func (L47)                                |   COVERED |
-|     documented_top_level_func.documented_inner_func (L50)        |   COVERED |
-|   undocumented_top_level_func (L55)                              |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L56)    |    MISSED |
-|   Bar (L60)                                                      |    MISSED |
-|     Bar.method_bar (L61)                                         |    MISSED |
-|       Bar.method_bar.InnerBar (L62)                              |    MISSED |
-|   _SemiprivateClass (L66)                                        |    MISSED |
-|   __PrivateClass (L70)                                           |    MISSED |
+|     Foo.get (L38)                                                |    MISSED |
+|     Foo.a_prop (L42)                                             |    MISSED |
+|     Foo.a_prop (L46)                                             |    MISSED |
+|     Foo.module_overload (L50)                                    |    MISSED |
+|     Foo.module_overload (L53)                                    |    MISSED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.simple_overload (L60)                                    |    MISSED |
+|     Foo.simple_overload (L63)                                    |    MISSED |
+|     Foo.simple_overload (L65)                                    |   COVERED |
+|   documented_top_level_func (L70)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
+|   undocumented_top_level_func (L78)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
+|   Bar (L83)                                                      |    MISSED |
+|     Bar.method_bar (L84)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
+|   _SemiprivateClass (L89)                                        |    MISSED |
+|   __PrivateClass (L93)                                           |    MISSED |
 |------------------------------------------------------------------|-----------|
 | child_sample/__init__.py (module)                                |    MISSED |
 |------------------------------------------------------------------|-----------|
 | child_sample/child_sample_module.py (module)                     |    MISSED |
 |   ChildFoo (L5)                                                  |    MISSED |
 |     ChildFoo.__init__ (L6)                                       |    MISSED |
 |     ChildFoo.__str__ (L9)                                        |    MISSED |
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_summary.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_summary.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | Name                                     |  Total |  Miss |  Cover |  Cover% |
 |------------------------------------------|--------|-------|--------|---------|
 | __init__.py                              |      1 |     0 |      1 |    100% |
 | empty.py                                 |      1 |     1 |      0 |      0% |
-| full.py                                  |     18 |     0 |     18 |    100% |
-| partial.py                               |     22 |    15 |      7 |     32% |
+| full.py                                  |     24 |     0 |     24 |    100% |
+| partial.py                               |     28 |    19 |      9 |     32% |
 | child_sample/__init__.py                 |      1 |     1 |      0 |      0% |
 | child_sample/child_sample_module.py      |     13 |    13 |      0 |      0% |
 |------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     56 |    30 |     26 |   46.4% |
+| TOTAL                                    |     68 |    34 |     34 |   50.0% |
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_summary_no_module.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_summary_no_module.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ----------------------------------- Summary ------------------------------------
 | Name                                     |  Total |  Miss |  Cover |  Cover% |
 |------------------------------------------|--------|-------|--------|---------|
-| full.py                                  |     17 |     0 |     17 |    100% |
-| partial.py                               |     21 |    15 |      6 |     29% |
+| full.py                                  |     23 |     0 |     23 |    100% |
+| partial.py                               |     27 |    19 |      8 |     30% |
 | child_sample/child_sample_module.py      |     12 |    12 |      0 |      0% |
 |------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     50 |    27 |     23 |   46.0% |
----------------- RESULT: FAILED (minimum: 80.0%, actual: 46.0%) ----------------
+| TOTAL                                    |     62 |    31 |     31 |   50.0% |
+---------------- RESULT: FAILED (minimum: 80.0%, actual: 50.0%) ----------------
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/expected_summary_skip_covered.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_summary_skip_covered.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | Name                                     |  Total |  Miss |  Cover |  Cover% |
 |------------------------------------------|--------|-------|--------|---------|
 | empty.py                                 |      1 |     1 |      0 |      0% |
-| partial.py                               |     22 |    15 |      7 |     32% |
+| partial.py                               |     28 |    19 |      9 |     32% |
 | child_sample/__init__.py                 |      1 |     1 |      0 |      0% |
 | child_sample/child_sample_module.py      |     13 |    13 |      0 |      0% |
 |------------------------------------------|--------|-------|--------|---------|
-| TOTAL                                    |     56 |    30 |     26 |   46.4% |
+| TOTAL                                    |     68 |    34 |     34 |   50.0% |
 |------------------------------------------------------------------------------|
 |               (2 of 6 files omitted due to complete coverage)                |
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_detailed.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,77 @@
------------------------------- Detailed Coverage ------------------------------
-| Name                                                            |    Status |
-|-----------------------------------------------------------------|-----------|
-| __init__.py (module)                                            |   COVERED |
-|-----------------------------------------------------------------|-----------|
-| empty.py (module)                                               |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| full.py (module)                                                |   COVERED |
-|   Foo (L5)                                                      |   COVERED |
-|     Foo.__init__ (L8)                                           |   COVERED |
-|     Foo.__str__ (L12)                                           |   COVERED |
-|     Foo._semiprivate (L16)                                      |   COVERED |
-|     Foo.__private (L20)                                         |   COVERED |
-|     Foo.method_foo (L24)                                        |   COVERED |
-|     Foo.get (L28)                                               |   COVERED |
-|     Foo.get (L32)                                               |   COVERED |
-|     Foo.prop (L37)                                              |   COVERED |
-|     Foo.prop (L42)                                              |   COVERED |
-|   top_level_func (L47)                                          |   COVERED |
-|     top_level_func.inner_func (L50)                             |   COVERED |
-|   Bar (L55)                                                     |   COVERED |
-|     Bar.method_bar (L58)                                        |   COVERED |
-|       Bar.method_bar.InnerBar (L61)                             |   COVERED |
-|   _SemiprivateClass (L67)                                       |   COVERED |
-|   __PrivateClass (L73)                                          |   COVERED |
-|-----------------------------------------------------------------|-----------|
-| partial.py (module)                                             |   COVERED |
-|   Foo (L5)                                                      |   COVERED |
-|     Foo.__init__ (L8)                                           |   COVERED |
-|     Foo.__str__ (L12)                                           |   COVERED |
-|     Foo.__repr__ (L16)                                          |    MISSED |
-|     Foo._semiprivate_documented (L19)                           |   COVERED |
-|     Foo._semiprivate_undocumented (L23)                         |    MISSED |
-|     Foo.__private (L26)                                         |    MISSED |
-|     Foo.method_foo (L29)                                        |    MISSED |
-|     Foo.get (L32)                                               |    MISSED |
-|     Foo.get (L35)                                               |    MISSED |
-|     Foo.a_prop (L39)                                            |    MISSED |
-|     Foo.a_prop (L43)                                            |    MISSED |
-|   documented_top_level_func (L47)                               |   COVERED |
-|     documented_top_level_func.documented_inner_func (L50)       |   COVERED |
-|   undocumented_top_level_func (L55)                             |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L56)   |    MISSED |
-|   Bar (L60)                                                     |    MISSED |
-|     Bar.method_bar (L61)                                        |    MISSED |
-|       Bar.method_bar.InnerBar (L62)                             |    MISSED |
-|   _SemiprivateClass (L66)                                       |    MISSED |
-|   __PrivateClass (L70)                                          |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| child_sample\__init__.py (module)                               |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| child_sample\child_sample_module.py (module)                    |    MISSED |
-|   ChildFoo (L5)                                                 |    MISSED |
-|     ChildFoo.__init__ (L6)                                      |    MISSED |
-|     ChildFoo.__str__ (L9)                                       |    MISSED |
-|     ChildFoo._ignore_me (L12)                                   |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
-|     ChildFoo.method_foo (L18)                                   |    MISSED |
-|   a_child_func (L22)                                            |    MISSED |
-|   ChildBar (L26)                                                |    MISSED |
-|     ChildBar.method_bar (L27)                                   |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
-|   _ChildBaz (L34)                                               |    MISSED |
-|   __ChildBla (L38)                                              |    MISSED |
-|-----------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage -------------------------------
+| Name                                                             |    Status |
+|------------------------------------------------------------------|-----------|
+| __init__.py (module)                                             |   COVERED |
+|------------------------------------------------------------------|-----------|
+| empty.py (module)                                                |    MISSED |
+|------------------------------------------------------------------|-----------|
+| full.py (module)                                                 |   COVERED |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo._semiprivate (L19)                                       |   COVERED |
+|     Foo.__private (L23)                                          |   COVERED |
+|     Foo.method_foo (L27)                                         |   COVERED |
+|     Foo.get (L31)                                                |   COVERED |
+|     Foo.get (L35)                                                |   COVERED |
+|     Foo.prop (L40)                                               |   COVERED |
+|     Foo.prop (L45)                                               |   COVERED |
+|     Foo.module_overload (L50)                                    |   COVERED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.module_overload (L59)                                    |   COVERED |
+|     Foo.simple_overload (L64)                                    |   COVERED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|     Foo.simple_overload (L73)                                    |   COVERED |
+|   top_level_func (L78)                                           |   COVERED |
+|     top_level_func.inner_func (L81)                              |   COVERED |
+|   Bar (L86)                                                      |   COVERED |
+|     Bar.method_bar (L89)                                         |   COVERED |
+|       Bar.method_bar.InnerBar (L92)                              |   COVERED |
+|   _SemiprivateClass (L98)                                        |   COVERED |
+|   __PrivateClass (L104)                                          |   COVERED |
+|------------------------------------------------------------------|-----------|
+| partial.py (module)                                              |   COVERED |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo.__repr__ (L19)                                           |    MISSED |
+|     Foo._semiprivate_documented (L22)                            |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                          |    MISSED |
+|     Foo.__private (L29)                                          |    MISSED |
+|     Foo.method_foo (L32)                                         |    MISSED |
+|     Foo.get (L35)                                                |    MISSED |
+|     Foo.get (L38)                                                |    MISSED |
+|     Foo.a_prop (L42)                                             |    MISSED |
+|     Foo.a_prop (L46)                                             |    MISSED |
+|     Foo.module_overload (L50)                                    |    MISSED |
+|     Foo.module_overload (L53)                                    |    MISSED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.simple_overload (L60)                                    |    MISSED |
+|     Foo.simple_overload (L63)                                    |    MISSED |
+|     Foo.simple_overload (L65)                                    |   COVERED |
+|   documented_top_level_func (L70)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
+|   undocumented_top_level_func (L78)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
+|   Bar (L83)                                                      |    MISSED |
+|     Bar.method_bar (L84)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
+|   _SemiprivateClass (L89)                                        |    MISSED |
+|   __PrivateClass (L93)                                           |    MISSED |
+|------------------------------------------------------------------|-----------|
+| child_sample/__init__.py (module)                                |    MISSED |
+|------------------------------------------------------------------|-----------|
+| child_sample/child_sample_module.py (module)                     |    MISSED |
+|   ChildFoo (L5)                                                  |    MISSED |
+|     ChildFoo.__init__ (L6)                                       |    MISSED |
+|     ChildFoo.__str__ (L9)                                        |    MISSED |
+|     ChildFoo._ignore_me (L12)                                    |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
+|     ChildFoo.method_foo (L18)                                    |    MISSED |
+|   a_child_func (L22)                                             |    MISSED |
+|   ChildBar (L26)                                                 |    MISSED |
+|     ChildBar.method_bar (L27)                                    |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
+|   _ChildBaz (L34)                                                |    MISSED |
+|   __ChildBla (L38)                                               |    MISSED |
+|------------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed_no_module.txt` & `interrogate-1.6.0/tests/functional/fixtures/expected_detailed_no_module.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,71 @@
------------------------------- Detailed Coverage ------------------------------
-| Name                                                            |    Status |
-|-----------------------------------------------------------------|-----------|
-| full.py                                                         |           |
-|   Foo (L5)                                                      |   COVERED |
-|     Foo.__init__ (L8)                                           |   COVERED |
-|     Foo.__str__ (L12)                                           |   COVERED |
-|     Foo._semiprivate (L16)                                      |   COVERED |
-|     Foo.__private (L20)                                         |   COVERED |
-|     Foo.method_foo (L24)                                        |   COVERED |
-|     Foo.get (L28)                                               |   COVERED |
-|     Foo.get (L32)                                               |   COVERED |
-|     Foo.prop (L37)                                              |   COVERED |
-|     Foo.prop (L42)                                              |   COVERED |
-|   top_level_func (L47)                                          |   COVERED |
-|     top_level_func.inner_func (L50)                             |   COVERED |
-|   Bar (L55)                                                     |   COVERED |
-|     Bar.method_bar (L58)                                        |   COVERED |
-|       Bar.method_bar.InnerBar (L61)                             |   COVERED |
-|   _SemiprivateClass (L67)                                       |   COVERED |
-|   __PrivateClass (L73)                                          |   COVERED |
-|-----------------------------------------------------------------|-----------|
-| partial.py                                                      |           |
-|   Foo (L5)                                                      |   COVERED |
-|     Foo.__init__ (L8)                                           |   COVERED |
-|     Foo.__str__ (L12)                                           |   COVERED |
-|     Foo.__repr__ (L16)                                          |    MISSED |
-|     Foo._semiprivate_documented (L19)                           |   COVERED |
-|     Foo._semiprivate_undocumented (L23)                         |    MISSED |
-|     Foo.__private (L26)                                         |    MISSED |
-|     Foo.method_foo (L29)                                        |    MISSED |
-|     Foo.get (L32)                                               |    MISSED |
-|     Foo.get (L35)                                               |    MISSED |
-|     Foo.a_prop (L39)                                            |    MISSED |
-|     Foo.a_prop (L43)                                            |    MISSED |
-|   documented_top_level_func (L47)                               |   COVERED |
-|     documented_top_level_func.documented_inner_func (L50)       |   COVERED |
-|   undocumented_top_level_func (L55)                             |    MISSED |
-|     undocumented_top_level_func.undocumented_inner_func (L56)   |    MISSED |
-|   Bar (L60)                                                     |    MISSED |
-|     Bar.method_bar (L61)                                        |    MISSED |
-|       Bar.method_bar.InnerBar (L62)                             |    MISSED |
-|   _SemiprivateClass (L66)                                       |    MISSED |
-|   __PrivateClass (L70)                                          |    MISSED |
-|-----------------------------------------------------------------|-----------|
-| child_sample\child_sample_module.py                             |           |
-|   ChildFoo (L5)                                                 |    MISSED |
-|     ChildFoo.__init__ (L6)                                      |    MISSED |
-|     ChildFoo.__str__ (L9)                                       |    MISSED |
-|     ChildFoo._ignore_me (L12)                                   |    MISSED |
-|     ChildFoo.__ignore_me_too (L15)                              |    MISSED |
-|     ChildFoo.method_foo (L18)                                   |    MISSED |
-|   a_child_func (L22)                                            |    MISSED |
-|   ChildBar (L26)                                                |    MISSED |
-|     ChildBar.method_bar (L27)                                   |    MISSED |
-|       ChildBar.method_bar.InnerBar (L28)                        |    MISSED |
-|   _ChildBaz (L34)                                               |    MISSED |
-|   __ChildBla (L38)                                              |    MISSED |
-|-----------------------------------------------------------------|-----------|
+------------------------------ Detailed Coverage -------------------------------
+| Name                                                             |    Status |
+|------------------------------------------------------------------|-----------|
+| full.py                                                          |           |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo._semiprivate (L19)                                       |   COVERED |
+|     Foo.__private (L23)                                          |   COVERED |
+|     Foo.method_foo (L27)                                         |   COVERED |
+|     Foo.get (L31)                                                |   COVERED |
+|     Foo.get (L35)                                                |   COVERED |
+|     Foo.prop (L40)                                               |   COVERED |
+|     Foo.prop (L45)                                               |   COVERED |
+|     Foo.module_overload (L50)                                    |   COVERED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.module_overload (L59)                                    |   COVERED |
+|     Foo.simple_overload (L64)                                    |   COVERED |
+|     Foo.simple_overload (L69)                                    |   COVERED |
+|     Foo.simple_overload (L73)                                    |   COVERED |
+|   top_level_func (L78)                                           |   COVERED |
+|     top_level_func.inner_func (L81)                              |   COVERED |
+|   Bar (L86)                                                      |   COVERED |
+|     Bar.method_bar (L89)                                         |   COVERED |
+|       Bar.method_bar.InnerBar (L92)                              |   COVERED |
+|   _SemiprivateClass (L98)                                        |   COVERED |
+|   __PrivateClass (L104)                                          |   COVERED |
+|------------------------------------------------------------------|-----------|
+| partial.py                                                       |           |
+|   Foo (L8)                                                       |   COVERED |
+|     Foo.__init__ (L11)                                           |   COVERED |
+|     Foo.__str__ (L15)                                            |   COVERED |
+|     Foo.__repr__ (L19)                                           |    MISSED |
+|     Foo._semiprivate_documented (L22)                            |   COVERED |
+|     Foo._semiprivate_undocumented (L26)                          |    MISSED |
+|     Foo.__private (L29)                                          |    MISSED |
+|     Foo.method_foo (L32)                                         |    MISSED |
+|     Foo.get (L35)                                                |    MISSED |
+|     Foo.get (L38)                                                |    MISSED |
+|     Foo.a_prop (L42)                                             |    MISSED |
+|     Foo.a_prop (L46)                                             |    MISSED |
+|     Foo.module_overload (L50)                                    |    MISSED |
+|     Foo.module_overload (L53)                                    |    MISSED |
+|     Foo.module_overload (L55)                                    |   COVERED |
+|     Foo.simple_overload (L60)                                    |    MISSED |
+|     Foo.simple_overload (L63)                                    |    MISSED |
+|     Foo.simple_overload (L65)                                    |   COVERED |
+|   documented_top_level_func (L70)                                |   COVERED |
+|     documented_top_level_func.documented_inner_func (L73)        |   COVERED |
+|   undocumented_top_level_func (L78)                              |    MISSED |
+|     undocumented_top_level_func.undocumented_inner_func (L79)    |    MISSED |
+|   Bar (L83)                                                      |    MISSED |
+|     Bar.method_bar (L84)                                         |    MISSED |
+|       Bar.method_bar.InnerBar (L85)                              |    MISSED |
+|   _SemiprivateClass (L89)                                        |    MISSED |
+|   __PrivateClass (L93)                                           |    MISSED |
+|------------------------------------------------------------------|-----------|
+| child_sample/child_sample_module.py                              |           |
+|   ChildFoo (L5)                                                  |    MISSED |
+|     ChildFoo.__init__ (L6)                                       |    MISSED |
+|     ChildFoo.__str__ (L9)                                        |    MISSED |
+|     ChildFoo._ignore_me (L12)                                    |    MISSED |
+|     ChildFoo.__ignore_me_too (L15)                               |    MISSED |
+|     ChildFoo.method_foo (L18)                                    |    MISSED |
+|   a_child_func (L22)                                             |    MISSED |
+|   ChildBar (L26)                                                 |    MISSED |
+|     ChildBar.method_bar (L27)                                    |    MISSED |
+|       ChildBar.method_bar.InnerBar (L28)                         |    MISSED |
+|   _ChildBaz (L34)                                                |    MISSED |
+|   __ChildBla (L38)                                               |    MISSED |
+|------------------------------------------------------------------|-----------|
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt` & `interrogate-1.6.0/tests/functional/fixtures/windows/expected_detailed_single_file.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 ------------------------------ Detailed Coverage ------------------------------
 | Name                                               |                 Status |
 |----------------------------------------------------|------------------------|
 | full.py (module)                                   |                COVERED |
-|   Foo (L5)                                         |                COVERED |
-|     Foo.__init__ (L8)                              |                COVERED |
-|     Foo.__str__ (L12)                              |                COVERED |
-|     Foo._semiprivate (L16)                         |                COVERED |
-|     Foo.__private (L20)                            |                COVERED |
-|     Foo.method_foo (L24)                           |                COVERED |
-|     Foo.get (L28)                                  |                COVERED |
-|     Foo.get (L32)                                  |                COVERED |
-|     Foo.prop (L37)                                 |                COVERED |
-|     Foo.prop (L42)                                 |                COVERED |
-|   top_level_func (L47)                             |                COVERED |
-|     top_level_func.inner_func (L50)                |                COVERED |
-|   Bar (L55)                                        |                COVERED |
-|     Bar.method_bar (L58)                           |                COVERED |
-|       Bar.method_bar.InnerBar (L61)                |                COVERED |
-|   _SemiprivateClass (L67)                          |                COVERED |
-|   __PrivateClass (L73)                             |                COVERED |
+|   Foo (L8)                                         |                COVERED |
+|     Foo.__init__ (L11)                             |                COVERED |
+|     Foo.__str__ (L15)                              |                COVERED |
+|     Foo._semiprivate (L19)                         |                COVERED |
+|     Foo.__private (L23)                            |                COVERED |
+|     Foo.method_foo (L27)                           |                COVERED |
+|     Foo.get (L31)                                  |                COVERED |
+|     Foo.get (L35)                                  |                COVERED |
+|     Foo.prop (L40)                                 |                COVERED |
+|     Foo.prop (L45)                                 |                COVERED |
+|     Foo.module_overload (L50)                      |                COVERED |
+|     Foo.module_overload (L55)                      |                COVERED |
+|     Foo.module_overload (L59)                      |                COVERED |
+|     Foo.simple_overload (L64)                      |                COVERED |
+|     Foo.simple_overload (L69)                      |                COVERED |
+|     Foo.simple_overload (L73)                      |                COVERED |
+|   top_level_func (L78)                             |                COVERED |
+|     top_level_func.inner_func (L81)                |                COVERED |
+|   Bar (L86)                                        |                COVERED |
+|     Bar.method_bar (L89)                           |                COVERED |
+|       Bar.method_bar.InnerBar (L92)                |                COVERED |
+|   _SemiprivateClass (L98)                          |                COVERED |
+|   __PrivateClass (L104)                            |                COVERED |
 |----------------------------------------------------|------------------------|
 
 ----------------------------------- Summary -----------------------------------
 | Name            |        Total |        Miss |        Cover |        Cover% |
 |-----------------|--------------|-------------|--------------|---------------|
-| full.py         |           18 |           0 |           18 |          100% |
+| full.py         |           24 |           0 |           24 |          100% |
 |-----------------|--------------|-------------|--------------|---------------|
-| TOTAL           |           18 |           0 |           18 |        100.0% |
+| TOTAL           |           24 |           0 |           24 |        100.0% |
 --------------- RESULT: PASSED (minimum: 80.0%, actual: 100.0%) ---------------
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary.txt` & `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | Name                                    |  Total |  Miss |  Cover |  Cover% |
 |-----------------------------------------|--------|-------|--------|---------|
 | __init__.py                             |      1 |     0 |      1 |    100% |
 | empty.py                                |      1 |     1 |      0 |      0% |
-| full.py                                 |     18 |     0 |     18 |    100% |
-| partial.py                              |     22 |    15 |      7 |     32% |
+| full.py                                 |     24 |     0 |     24 |    100% |
+| partial.py                              |     28 |    19 |      9 |     32% |
 | child_sample\__init__.py                |      1 |     1 |      0 |      0% |
 | child_sample\child_sample_module.py     |     13 |    13 |      0 |      0% |
 |-----------------------------------------|--------|-------|--------|---------|
-| TOTAL                                   |     56 |    30 |     26 |   46.4% |
+| TOTAL                                   |     68 |    34 |     34 |   50.0% |
```

### Comparing `interrogate-1.5.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt` & `interrogate-1.6.0/tests/functional/fixtures/windows/expected_summary_skip_covered.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 | Name                                    |  Total |  Miss |  Cover |  Cover% |
 |-----------------------------------------|--------|-------|--------|---------|
 | empty.py                                |      1 |     1 |      0 |      0% |
-| partial.py                              |     22 |    15 |      7 |     32% |
+| partial.py                              |     28 |    19 |      9 |     32% |
 | child_sample\__init__.py                |      1 |     1 |      0 |      0% |
 | child_sample\child_sample_module.py     |     13 |    13 |      0 |      0% |
 |-----------------------------------------|--------|-------|--------|---------|
-| TOTAL                                   |     56 |    30 |     26 |   46.4% |
+| TOTAL                                   |     68 |    34 |     34 |   50.0% |
```

### Comparing `interrogate-1.5.0/tests/functional/sample/full.py` & `interrogate-1.6.0/tests/functional/sample/partial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 # Copyright 2020 Lynn Root
 """Sample module-level docs"""
+import typing
 
+from typing import overload
 
-class Foo(object):
+
+class Foo:
     """Foo class"""
 
     def __init__(self):
         """init method of Foo class"""
         self.foo = None
 
     def __str__(self):
-        """a magic method."""
+        """a documented magic method."""
+        pass
+
+    def __repr__(self):
+        pass
+
+    def _semiprivate_documented(self):
+        """a documented semipriate method"""
         pass
 
-    def _semiprivate(self):
-        """a semipriate method"""
+    def _semiprivate_undocumented(self):
         pass
 
     def __private(self):
-        """a private method"""
         pass
 
     def method_foo(self):
-        """this method does foo"""
         pass
 
     def get(self):
-        """this method gets something"""
         pass
 
     async def get(self):
-        """this async method gets something"""
         pass
 
     @property
-    def prop(self):
-        """this method has a get property decorator"""
+    def a_prop(self):
         pass
 
-    @prop.setter
-    def prop(self):
-        """this method has a set property decorator"""
+    @a_prop.setter
+    def a_prop(self, x):
         pass
 
+    @typing.overload
+    def module_overload(a: None) -> None: ...
 
-def top_level_func():
-    """A top level function"""
+    @typing.overload
+    def module_overload(a: int) -> int: ...
 
-    def inner_func():
-        """A inner function"""
+    def module_overload(a):
+        """overloaded method implementation"""
         pass
 
+    @overload
+    def simple_overload(a: None) -> None: ...
 
-class Bar(object):
-    """Bar class"""
+    @overload
+    def simple_overload(a: int) -> int: ...
 
-    def method_bar(self):
-        """a method that does bar"""
+    def simple_overload(a):
+        """overloaded method implementation"""
+        pass
 
-        class InnerBar(object):
-            """an inner class"""
 
-            pass
+def documented_top_level_func():
+    """A documented top level function"""
 
+    def documented_inner_func():
+        """A documented inner function"""
+        pass
 
-class _SemiprivateClass(object):
-    """a semiprivate class"""
 
-    pass
+def undocumented_top_level_func():
+    def undocumented_inner_func():
+        pass
+
+
+class Bar:
+    def method_bar(self):
+        class InnerBar:
+            pass
 
 
-class __PrivateClass(object):
-    """a private class"""
+class _SemiprivateClass:
+    pass
+
 
+class __PrivateClass:
     pass
```

### Comparing `interrogate-1.5.0/tests/functional/test_cli.py` & `interrogate-1.6.0/tests/functional/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,117 +29,120 @@
 
 def test_run_no_paths(runner, monkeypatch, tmpdir):
     """Assume current working directory if no paths are given."""
     monkeypatch.setattr(os, "getcwd", lambda: SAMPLE_DIR)
 
     result = runner.invoke(cli.main, [])
 
-    assert "actual: 46.4%" in result.output
+    assert "actual: 50.0%" in result.output
     assert 1 == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
         # no flags
-        ([], 46.4, 1),
+        ([], 50.0, 1),
         # ignore init module
-        (["-I"], 46.3, 1),
+        (["-I"], 50.0, 1),
         # ignore module docs
-        (["-M"], 46.0, 1),
+        (["-M"], 50.0, 1),
         # ignore semiprivate docs
-        (["-s"], 46.9, 1),
+        (["-s"], 50.8, 1),
         # ignore private docs
-        (["-p"], 48.0, 1),
+        (["-p"], 51.6, 1),
         # ignore property getter/setter decorators
-        (["-P"], 46.2, 1),
+        (["-P"], 50.0, 1),
         # ignore property setter decorators
-        (["-S"], 46.3, 1),
+        (["-S"], 50.0, 1),
         # ignore magic method docs
-        (["-m"], 46.2, 1),
+        (["-m"], 50.0, 1),
         # ignore init method docs
-        (["-i"], 45.3, 1),
+        (["-i"], 49.2, 1),
         # ignore nested funcs
-        (["-n"], 45.3, 1),
+        (["-n"], 49.2, 1),
         # ignore nested classes
-        (["-C"], 47.2, 1),
+        (["-C"], 50.8, 1),
+        # ignore @typing.overload-decorated functions
+        (["-O"], 50.0, 1),
         # ignore regex
-        (["-r", "^get$"], 46.2, 1),
+        (["-r", "^get$"], 50.0, 1),
         # whitelist regex
         (["-w", "^get$"], 50.0, 1),
         # exclude file
-        (["-e", os.path.join(SAMPLE_DIR, "partial.py")], 55.9, 1),
+        (["-e", os.path.join(SAMPLE_DIR, "partial.py")], 62.5, 1),
         # exclude file which doesn't exist
-        (["-e", os.path.join(SAMPLE_DIR, "does.not.exist")], 46.4, 1),
+        (["-e", os.path.join(SAMPLE_DIR, "does.not.exist")], 50.0, 1),
         # fail under
-        (["-f", "40"], 46.4, 0),
+        (["-f", "40"], 50.0, 0),
     ),
 )
 def test_run_shortflags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with single short flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
 
-    exp_partial_output = "actual: {:.1f}%".format(exp_result)
+    exp_partial_output = f"actual: {exp_result:.1f}%"
     assert exp_partial_output in result.output
     assert exp_exit_code == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
-        (["--ignore-init-module"], 46.3, 1),
-        (["--ignore-module"], 46.0, 1),
-        (["--ignore-semiprivate"], 46.9, 1),
-        (["--ignore-private"], 48.0, 1),
-        (["--ignore-property-decorators"], 46.2, 1),
-        (["--ignore-setters"], 46.3, 1),
-        (["--ignore-magic"], 46.2, 1),
-        (["--ignore-init-method"], 45.3, 1),
-        (["--ignore-nested-functions"], 45.3, 1),
-        (["--ignore-nested-classes"], 47.2, 1),
-        (["--ignore-regex", "^get$"], 46.2, 1),
+        (["--ignore-init-module"], 50.0, 1),
+        (["--ignore-module"], 50.0, 1),
+        (["--ignore-semiprivate"], 50.8, 1),
+        (["--ignore-private"], 51.6, 1),
+        (["--ignore-property-decorators"], 50.0, 1),
+        (["--ignore-setters"], 50.0, 1),
+        (["--ignore-magic"], 50.0, 1),
+        (["--ignore-init-method"], 49.2, 1),
+        (["--ignore-nested-functions"], 49.2, 1),
+        (["--ignore-nested-classes"], 50.8, 1),
+        (["--ignore-overloaded-functions"], 50.0, 1),
+        (["--ignore-regex", "^get$"], 50.0, 1),
         (["--whitelist-regex", "^get$"], 50.0, 1),
-        (["--exclude", os.path.join(SAMPLE_DIR, "partial.py")], 55.9, 1),
-        (["--fail-under", "40"], 46.4, 0),
+        (["--exclude", os.path.join(SAMPLE_DIR, "partial.py")], 62.5, 1),
+        (["--fail-under", "40"], 50.0, 0),
     ),
 )
 def test_run_longflags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with single long flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
 
-    exp_partial_output = "actual: {:.1f}%".format(exp_result)
+    exp_partial_output = f"actual: {exp_result:.1f}%"
     assert exp_partial_output in result.output
     assert exp_exit_code == result.exit_code
 
 
 @pytest.mark.parametrize(
     "flags,exp_result,exp_exit_code",
     (
-        (["-i", "-I", "-r" "^method_foo$"], 45.8, 1),
-        (["-s", "-p", "-M"], 48.6, 1),
-        (["-m", "-f", "45"], 46.2, 0),
+        (["-i", "-I", "-r" "^method_foo$"], 50.0, 1),
+        (["-s", "-p", "-M"], 53.1, 1),
+        (["-m", "-f", "45"], 50.0, 0),
     ),
 )
 def test_run_multiple_flags(flags, exp_result, exp_exit_code, runner):
     """Test CLI with a hodge-podge of flags"""
     cli_inputs = flags + [SAMPLE_DIR]
     result = runner.invoke(cli.main, cli_inputs)
 
-    exp_partial_output = "actual: {:.1f}%".format(exp_result)
+    exp_partial_output = f"actual: {exp_result:.1f}%"
     assert exp_partial_output in result.output
     assert exp_exit_code == result.exit_code
 
 
 @pytest.mark.parametrize("quiet", (True, False))
 def test_generate_badge(quiet, runner, tmp_path):
     """Test expected SVG output when creating a status badge."""
     expected_output_path = os.path.join(FIXTURES, "expected_badge.svg")
-    with open(expected_output_path, "r") as f:
+    with open(expected_output_path) as f:
         expected_output = f.read()
 
     expected_output = expected_output.replace("\n", "")
 
     tmpdir = tmp_path / "testing"
     tmpdir.mkdir()
     expected_path = tmpdir / "interrogate_badge.svg"
@@ -156,15 +159,15 @@
     result = runner.invoke(cli.main, cli_inputs)
     assert 0 == result.exit_code
     if quiet:
         assert "" == result.output
     else:
         assert str(expected_path) in result.output
 
-    with open(str(expected_path), "r") as f:
+    with open(str(expected_path)) as f:
         actual_output = f.read()
         actual_output = actual_output.replace("\n", "")
 
     assert expected_output == actual_output
 
 
 def test_incompatible_options_badge_format(runner):
```

### Comparing `interrogate-1.5.0/tests/functional/test_coverage.py` & `interrogate-1.6.0/tests/functional/test_coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,44 +40,58 @@
             (0, 0, 0, "100.0"),
         ),
         (
             [
                 SAMPLE_DIR,
             ],
             {},
-            (56, 26, 30, "46.4"),
+            (68, 34, 34, "50.0"),
         ),
-        ([os.path.join(SAMPLE_DIR, "partial.py")], {}, (22, 7, 15, "31.8")),
+        ([os.path.join(SAMPLE_DIR, "partial.py")], {}, (28, 9, 19, "32.1")),
         (
             [
                 os.path.join(SAMPLE_DIR, "full.py"),
             ],
             {"ignore_nested_functions": True},
-            (17, 17, 0, "100.0"),
+            (23, 23, 0, "100.0"),
         ),
         (
             [
                 os.path.join(SAMPLE_DIR, "partial.py"),
             ],
             {"ignore_nested_functions": True},
-            (20, 6, 14, "30.0"),
+            (26, 8, 18, "30.8"),
+        ),
+        (
+            [
+                os.path.join(SAMPLE_DIR, "full.py"),
+            ],
+            {"ignore_overloaded_functions": True},
+            (20, 20, 0, "100.0"),
+        ),
+        (
+            [
+                os.path.join(SAMPLE_DIR, "partial.py"),
+            ],
+            {"ignore_overloaded_functions": True},
+            (24, 9, 15, "37.5"),
         ),
     ),
 )
 def test_coverage_simple(paths, conf, exp_results, mocker):
     """Happy path - get expected results given a file or directory"""
     conf = config.InterrogateConfig(**conf)
     interrogate_coverage = coverage.InterrogateCoverage(paths=paths, conf=conf)
 
     results = interrogate_coverage.get_coverage()
 
     assert exp_results[0] == results.total
     assert exp_results[1] == results.covered
     assert exp_results[2] == results.missing
-    assert exp_results[3] == "{:.1f}".format(results.perc_covered)
+    assert exp_results[3] == f"{results.perc_covered:.1f}"
 
 
 def test_coverage_errors(capsys):
     """Exit when no Python files are found."""
     path = os.path.join(SAMPLE_DIR, "ignoreme.txt")
     interrogate_coverage = coverage.InterrogateCoverage(paths=[path])
 
@@ -112,15 +126,15 @@
         results=results, output=None, verbosity=level
     )
 
     captured = capsys.readouterr()
     expected_fixture = os.path.join(FIXTURES, exp_fixture_file)
     if IS_WINDOWS:
         expected_fixture = os.path.join(FIXTURES, "windows", exp_fixture_file)
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected_out = f.read()
 
     assert expected_out in captured.out
     assert "omitted due to complete coverage" not in captured.out
 
 
 @pytest.mark.parametrize(
@@ -144,15 +158,15 @@
         results=results, output=None, verbosity=level
     )
 
     captured = capsys.readouterr()
     expected_fixture = os.path.join(FIXTURES, exp_fixture_file)
     if IS_WINDOWS:
         expected_fixture = os.path.join(FIXTURES, "windows", exp_fixture_file)
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected_out = f.read()
 
     assert expected_out in captured.out
 
 
 @pytest.mark.parametrize("level", (1, 2))
 def test_print_results_omit_none(level, capsys, monkeypatch):
@@ -183,15 +197,15 @@
     )
 
     captured = capsys.readouterr()
     exp_fixture_file = "expected_summary_skip_covered_all.txt"
     expected_fixture = os.path.join(FIXTURES, exp_fixture_file)
     if IS_WINDOWS:
         expected_fixture = os.path.join(FIXTURES, "windows", exp_fixture_file)
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected_out = f.read()
 
     assert expected_out in captured.out
 
 
 def test_print_results_omit_all_detailed(capsys, monkeypatch):
     """Show no detail view when all files are omitted from skipping covered"""
@@ -234,15 +248,15 @@
         results=results, output=None, verbosity=level
     )
 
     captured = capsys.readouterr()
     expected_fixture = os.path.join(FIXTURES, exp_fixture_file)
     if IS_WINDOWS:
         expected_fixture = os.path.join(FIXTURES, "windows", exp_fixture_file)
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected_out = f.read()
 
     assert expected_out in captured.out
 
 
 def test_print_results_single_file(capsys, monkeypatch):
     """Results for a single file should still list the filename."""
@@ -259,15 +273,15 @@
     )
 
     if IS_WINDOWS:
         expected_fixture = os.path.join(
             FIXTURES, "windows", "expected_detailed_single_file.txt"
         )
 
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected_out = f.read()
 
     assert expected_out in captured.out
     # I don't want to deal with path mocking out just to get tests to run
     # everywhere
     if not IS_WINDOWS:
         assert "tests/functional/sample/" in captured.out
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/100.svg` & `interrogate-1.6.0/docs/_static/interrogate_badge.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/99.png` & `interrogate-1.6.0/tests/unit/fixtures/default-style/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/default-style/no_logo.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/no_logo.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/99.png` & `interrogate-1.6.0/tests/unit/fixtures/flat/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/60.svg`

 * *Files 2% similar despite different names*

```diff
@@ -1,359 +1,359 @@
 00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3133 3522 2068  k" width="135" h
+00000050: 6b22 2077 6964 7468 3d22 3134 3022 2068  k" width="140" h
 00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 696e 7465 7272 6f67 6174 653a 2031  ="interrogate: 1
-00000090: 3030 2522 3e0a 2020 2020 3c74 6974 6c65  00%">.    <title
-000000a0: 3e69 6e74 6572 726f 6761 7465 3a20 3130  >interrogate: 10
-000000b0: 3025 3c2f 7469 746c 653e 0a20 2020 203c  0%</title>.    <
-000000c0: 6720 7368 6170 652d 7265 6e64 6572 696e  g shape-renderin
-000000d0: 673d 2263 7269 7370 4564 6765 7322 3e0a  g="crispEdges">.
-000000e0: 2020 2020 2020 2020 3c72 6563 7420 7769          <rect wi
-000000f0: 6474 683d 2239 3322 2068 6569 6768 743d  dth="93" height=
-00000100: 2232 3022 2066 696c 6c3d 2223 3535 3522  "20" fill="#555"
-00000110: 2f3e 0a20 2020 2020 2020 203c 7265 6374  />.        <rect
-00000120: 2078 3d22 3933 2220 7769 6474 683d 2234   x="93" width="4
-00000130: 3222 2068 6569 6768 743d 2232 3022 2066  2" height="20" f
-00000140: 696c 6c3d 2223 3463 3122 2f3e 0a20 2020  ill="#4c1"/>.   
-00000150: 203c 2f67 3e0a 2020 2020 3c67 2066 696c   </g>.    <g fil
-00000160: 6c3d 2223 6666 6622 2074 6578 742d 616e  l="#fff" text-an
-00000170: 6368 6f72 3d22 6d69 6464 6c65 2220 666f  chor="middle" fo
-00000180: 6e74 2d66 616d 696c 793d 2256 6572 6461  nt-family="Verda
-00000190: 6e61 2c47 656e 6576 612c 4465 6a61 5675  na,Geneva,DejaVu
-000001a0: 2053 616e 732c 7361 6e73 2d73 6572 6966   Sans,sans-serif
-000001b0: 2220 7465 7874 2d72 656e 6465 7269 6e67  " text-rendering
-000001c0: 3d22 6765 6f6d 6574 7269 6350 7265 6369  ="geometricPreci
-000001d0: 7369 6f6e 2220 666f 6e74 2d73 697a 653d  sion" font-size=
-000001e0: 2231 3130 223e 0a20 2020 2020 2020 203c  "110">.        <
-000001f0: 7465 7874 2078 3d22 3539 3022 2079 3d22  text x="590" y="
-00000200: 3134 3022 2074 7261 6e73 666f 726d 3d22  140" transform="
-00000210: 7363 616c 6528 2e31 2922 2066 696c 6c3d  scale(.1)" fill=
-00000220: 2223 6666 6622 2074 6578 744c 656e 6774  "#fff" textLengt
-00000230: 683d 2236 3130 223e 696e 7465 7272 6f67  h="610">interrog
-00000240: 6174 653c 2f74 6578 743e 0a20 2020 2020  ate</text>.     
-00000250: 2020 203c 7465 7874 2078 3d22 3131 3430     <text x="1140
-00000260: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
-00000270: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
-00000280: 6669 6c6c 3d22 2366 6666 2220 7465 7874  fill="#fff" text
-00000290: 4c65 6e67 7468 3d22 3333 3022 2064 6174  Length="330" dat
-000002a0: 612d 696e 7465 7272 6f67 6174 653d 2272  a-interrogate="r
-000002b0: 6573 756c 7422 3e31 3030 253c 2f74 6578  esult">100%</tex
-000002c0: 743e 0a20 2020 203c 2f67 3e0a 2020 2020  t>.    </g>.    
-000002d0: 3c67 2069 643d 226c 6f67 6f2d 7069 6e6b  <g id="logo-pink
-000002e0: 2220 7472 616e 7366 6f72 6d3d 226d 6174  " transform="mat
-000002f0: 7269 7828 302e 3835 3438 3736 2c30 2c30  rix(0.854876,0,0
-00000300: 2c30 2e38 3534 3837 362c 2d36 2e37 3335  ,0.854876,-6.735
-00000310: 3134 2c30 2e38 3737 3132 3429 223e 0a20  14,0.877124)">. 
-00000320: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00000330: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-00000340: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-00000350: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
-00000360: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-00000370: 2020 3c70 6174 6820 643d 224d 3530 2c36    <path d="M50,6
-00000380: 342e 3235 4335 322e 3736 2c36 342e 3235  4.25C52.76,64.25
-00000390: 2035 352c 3631 2e31 3320 3535 2c35 392e   55,61.13 55,59.
-000003a0: 3735 4335 352c 3538 2e33 3720 3532 2e37  75C55,58.37 52.7
-000003b0: 362c 3537 2e32 3520 3530 2c35 372e 3235  6,57.25 50,57.25
-000003c0: 4334 372e 3234 2c35 372e 3235 2034 352c  C47.24,57.25 45,
-000003d0: 3538 2e33 3720 3435 2c35 392e 3735 4334  58.37 45,59.75C4
-000003e0: 352c 3631 2e31 3320 3437 2e32 342c 3634  5,61.13 47.24,64
-000003f0: 2e32 3520 3530 2c36 342e 3235 5a22 2073  .25 50,64.25Z" s
-00000400: 7479 6c65 3d22 6669 6c6c 3a72 6762 2832  tyle="fill:rgb(2
-00000410: 3232 2c31 3230 2c31 3630 293b 6669 6c6c  22,120,160);fill
-00000420: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 222f  -rule:nonzero;"/
-00000430: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-00000440: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00000450: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-00000460: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-00000470: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
-00000480: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-00000490: 2020 3c70 6174 6820 643d 224d 3838 2c34    <path d="M88,4
-000004a0: 392e 3035 4338 362e 3530 362c 3433 2e34  9.05C86.506,43.4
-000004b0: 3735 2038 332e 3031 382c 3338 2e36 3338  75 83.018,38.638
-000004c0: 2037 382e 322c 3335 2e34 3643 3732 2e39   78.2,35.46C72.9
-000004d0: 3639 2c33 322e 3030 3220 3636 2e35 3339  69,32.002 66.539
-000004e0: 2c33 302e 3834 3420 3630 2e34 332c 3332  ,30.844 60.43,32
-000004f0: 2e32 3643 3536 2e35 3736 2c33 332e 3134  .26C56.576,33.14
-00000500: 3520 3532 2e39 3935 2c33 342e 3935 3820  5 52.995,34.958 
-00000510: 3530 2c33 372e 3534 4334 362e 3939 382c  50,37.54C46.998,
-00000520: 3334 2e39 3538 2034 332e 3431 312c 3333  34.958 43.411,33
-00000530: 2e31 3439 2033 392e 3535 2c33 322e 3237  .149 39.55,32.27
-00000540: 4333 332e 3434 312c 3330 2e38 3533 2032  C33.441,30.853 2
-00000550: 372e 3031 312c 3332 2e30 3131 2032 312e  7.011,32.011 21.
-00000560: 3738 2c33 352e 3437 4331 362e 3937 2c33  78,35.47C16.97,3
-00000570: 382e 3635 3220 3133 2e34 3839 2c34 332e  8.652 13.489,43.
-00000580: 3438 3920 3132 2c34 392e 3036 4c31 322c  489 12,49.06L12,
-00000590: 3439 2e31 3343 3131 2e38 322c 3439 2e37  49.13C11.82,49.7
-000005a0: 3920 3131 2e36 362c 3530 2e34 3620 3131  9 11.66,50.46 11
-000005b0: 2e35 332c 3531 2e31 3343 3131 2e31 3436  .53,51.13C11.146
-000005c0: 2c35 332e 3230 3720 3131 2e30 3231 2c35  ,53.207 11.021,5
-000005d0: 352e 3332 3320 3131 2e31 362c 3537 2e34  5.323 11.16,57.4
-000005e0: 3343 3131 2e31 362c 3538 2e30 3320 3131  3C11.16,58.03 11
-000005f0: 2e32 362c 3538 2e36 3320 3131 2e33 342c  .26,58.63 11.34,
-00000600: 3539 2e32 3343 3131 2e33 342c 3539 2e35  59.23C11.34,59.5
-00000610: 3120 3131 2e34 332c 3539 2e37 3920 3131  1 11.43,59.79 11
-00000620: 2e34 382c 3630 2e30 3743 3131 2e35 332c  .48,60.07C11.53,
-00000630: 3630 2e33 3520 3131 2e35 382c 3630 2e36  60.35 11.58,60.6
-00000640: 3820 3131 2e36 342c 3630 2e39 3843 3131  8 11.64,60.98C11
-00000650: 2e37 2c36 312e 3238 2031 312e 382c 3631  .7,61.28 11.8,61
-00000660: 2e36 3920 3131 2e38 392c 3632 2e30 3543  .69 11.89,62.05C
-00000670: 3131 2e39 382c 3632 2e34 3120 3131 2e39  11.98,62.41 11.9
-00000680: 392c 3632 2e34 3720 3132 2e30 352c 3632  9,62.47 12.05,62
-00000690: 2e36 3843 3132 2e31 362c 3633 2e30 3720  .68C12.16,63.07 
-000006a0: 3132 2e32 382c 3633 2e34 3620 3132 2e34  12.28,63.46 12.4
-000006b0: 312c 3633 2e38 344c 3132 2e35 382c 3634  1,63.84L12.58,64
-000006c0: 2e33 3443 3132 2e37 322c 3634 2e37 3420  .34C12.72,64.74 
-000006d0: 3132 2e38 382c 3635 2e31 3420 3133 2e30  12.88,65.14 13.0
-000006e0: 342c 3635 2e35 334c 3133 2e32 332c 3635  4,65.53L13.23,65
-000006f0: 2e39 3843 3133 2e34 3033 2c36 362e 3337  .98C13.403,66.37
-00000700: 3320 3133 2e35 3833 2c36 362e 3736 3720  3 13.583,66.767 
-00000710: 3133 2e37 372c 3637 2e31 364c 3133 2e39  13.77,67.16L13.9
-00000720: 392c 3637 2e35 3943 3134 2e31 392c 3637  9,67.59C14.19,67
-00000730: 2e39 3720 3134 2e33 392c 3638 2e33 3520  .97 14.39,68.35 
-00000740: 3134 2e36 312c 3638 2e37 334c 3134 2e38  14.61,68.73L14.8
-00000750: 372c 3639 2e31 3543 3135 2e31 2c36 392e  7,69.15C15.1,69.
-00000760: 3532 2031 352e 3333 2c36 392e 3839 2031  52 15.33,69.89 1
-00000770: 352e 3538 2c37 302e 3236 4c31 352e 3538  5.58,70.26L15.58
-00000780: 2c37 302e 3332 4c31 352e 3939 2c37 302e  ,70.32L15.99,70.
-00000790: 3933 4331 362e 3134 2c37 312e 3134 2031  93C16.14,71.14 1
-000007a0: 362e 3239 2c37 312e 3336 2031 362e 3435  6.29,71.36 16.45
-000007b0: 2c37 312e 3537 4332 302e 3230 362c 3735  ,71.57C20.206,75
-000007c0: 2e38 3320 3235 2e30 3836 2c37 382e 3935  .83 25.086,78.95
-000007d0: 2033 302e 3533 2c38 302e 3537 4333 362e   30.53,80.57C36.
-000007e0: 3833 392c 3832 2e34 3820 3433 2e34 312c  839,82.48 43.41,
-000007f0: 3833 2e33 3835 2035 302c 3833 2e32 3543  83.385 50,83.25C
-00000800: 3536 2e35 3939 2c38 332e 3337 3420 3633  56.599,83.374 63
-00000810: 2e31 3737 2c38 322e 3435 3620 3639 2e34  .177,82.456 69.4
-00000820: 392c 3830 2e35 3343 3734 2e36 3434 2c37  9,80.53C74.644,7
-00000830: 382e 3937 3820 3739 2e33 3033 2c37 362e  8.978 79.303,76.
-00000840: 3130 3220 3833 2c37 322e 3139 4338 332e  102 83,72.19C83.
-00000850: 3334 2c37 312e 3738 2038 332e 3635 2c37  34,71.78 83.65,7
-00000860: 312e 3335 2038 342c 3730 2e39 324c 3834  1.35 84,70.92L84
-00000870: 2e31 382c 3730 2e36 364c 3834 2e33 332c  .18,70.66L84.33,
-00000880: 3730 2e34 344c 3834 2e34 312c 3730 2e33  70.44L84.41,70.3
-00000890: 3243 3834 2e35 352c 3730 2e31 3220 3834  2C84.55,70.12 84
-000008a0: 2e36 372c 3639 2e39 2038 342e 3831 2c36  .67,69.9 84.81,6
-000008b0: 392e 3743 3835 2e30 372c 3639 2e33 2038  9.7C85.07,69.3 8
-000008c0: 352e 3332 2c36 382e 3839 2038 352e 3535  5.32,68.89 85.55
-000008d0: 2c36 382e 3438 4338 352e 3738 2c36 382e  ,68.48C85.78,68.
-000008e0: 3037 2038 362e 3032 2c36 372e 3635 2038  07 86.02,67.65 8
-000008f0: 362e 3233 2c36 372e 3232 4338 362e 3331  6.23,67.22C86.31
-00000900: 2c36 372e 3035 2038 362e 3339 2c36 362e  ,67.05 86.39,66.
-00000910: 3838 2038 362e 3437 2c36 362e 3743 3836  88 86.47,66.7C86
-00000920: 2e36 372c 3636 2e32 3820 3836 2e38 352c  .67,66.28 86.85,
-00000930: 3635 2e38 3720 3837 2e30 332c 3635 2e34  65.87 87.03,65.4
-00000940: 344c 3837 2e32 332c 3634 2e39 3243 3837  4L87.23,64.92C87
-00000950: 2e33 3937 2c36 342e 3438 3720 3837 2e35  .397,64.487 87.5
-00000960: 352c 3634 2e30 3520 3837 2e36 392c 3633  5,64.05 87.69,63
-00000970: 2e36 314c 3837 2e38 352c 3633 2e30 3943  .61L87.85,63.09C
-00000980: 3837 2e39 382c 3632 2e36 3420 3838 2e31  87.98,62.64 88.1
-00000990: 2c36 322e 3139 2038 382e 3231 2c36 312e  ,62.19 88.21,61.
-000009a0: 3734 4338 382e 3231 2c36 312e 3537 2038  74C88.21,61.57 8
-000009b0: 382e 332c 3631 2e33 3920 3838 2e33 332c  8.3,61.39 88.33,
-000009c0: 3631 2e32 3243 3838 2e34 332c 3630 2e37  61.22C88.43,60.7
-000009d0: 3520 3838 2e35 322c 3630 2e32 3220 3838  5 88.52,60.22 88
-000009e0: 2e36 2c35 392e 3739 4338 382e 362c 3539  .6,59.79C88.6,59
-000009f0: 2e36 3420 3838 2e36 362c 3539 2e34 3920  .64 88.66,59.49 
-00000a00: 3838 2e36 382c 3539 2e33 3343 3838 2e37  88.68,59.33C88.7
-00000a10: 372c 3538 2e37 3120 3838 2e38 342c 3538  7,58.71 88.84,58
-00000a20: 2e30 3820 3838 2e38 382c 3537 2e34 354c  .08 88.88,57.45L
-00000a30: 3838 2e38 382c 3534 2e31 3743 3838 2e38  88.88,54.17C88.8
-00000a40: 3137 2c35 332e 3136 3420 3838 2e36 3933  17,53.164 88.693
-00000a50: 2c35 322e 3136 3220 3838 2e35 312c 3531  ,52.162 88.51,51
-00000a60: 2e31 3743 3838 2e33 382c 3530 2e35 2038  .17C88.38,50.5 8
-00000a70: 382e 3233 2c34 392e 3834 2038 382e 3035  8.23,49.84 88.05
-00000a80: 2c34 392e 3137 4c38 382c 3439 2e30 355a  ,49.17L88,49.05Z
-00000a90: 4d38 352e 3839 2c35 362e 3434 4c38 352e  M85.89,56.44L85.
-00000aa0: 3839 2c35 372e 3233 4338 352e 3839 2c35  89,57.23C85.89,5
-00000ab0: 372e 3738 2038 352e 3739 2c35 382e 3332  7.78 85.79,58.32
-00000ac0: 2038 352e 3732 2c35 382e 3836 4338 352e   85.72,58.86C85.
-00000ad0: 3732 2c35 392e 3031 2038 352e 3732 2c35  72,59.01 85.72,5
-00000ae0: 392e 3135 2038 352e 3635 2c35 392e 3343  9.15 85.65,59.3C
-00000af0: 3835 2e35 392c 3539 2e37 2038 352e 3531  85.59,59.7 85.51
-00000b00: 2c36 302e 3131 2038 352e 3433 2c36 302e  ,60.11 85.43,60.
-00000b10: 3531 4c38 352e 3332 2c36 302e 3939 4338  51L85.32,60.99C8
-00000b20: 352e 3233 2c36 312e 3338 2038 352e 3132  5.23,61.38 85.12
-00000b30: 2c36 312e 3737 2038 352e 3031 2c36 322e  ,61.77 85.01,62.
-00000b40: 3136 4338 352e 3031 2c36 322e 3331 2038  16C85.01,62.31 8
-00000b50: 342e 3933 2c36 322e 3436 2038 342e 3838  4.93,62.46 84.88
-00000b60: 2c36 322e 3643 3834 2e37 342c 3633 2e30  ,62.6C84.74,63.0
-00000b70: 3420 3834 2e35 392c 3633 2e34 3720 3834  4 84.59,63.47 84
-00000b80: 2e34 322c 3633 2e39 4c38 342e 3237 2c36  .42,63.9L84.27,6
-00000b90: 342e 3238 4338 342e 312c 3634 2e37 3120  4.28C84.1,64.71 
-00000ba0: 3833 2e39 312c 3635 2e31 3420 3833 2e37  83.91,65.14 83.7
-00000bb0: 312c 3635 2e35 3643 3833 2e35 312c 3635  1,65.56C83.51,65
-00000bc0: 2e39 3820 3833 2e34 332c 3636 2e31 3220  .98 83.43,66.12 
-00000bd0: 3833 2e32 382c 3636 2e34 4c38 332e 3031  83.28,66.4L83.01
-00000be0: 2c36 362e 3931 4338 322e 3833 2c36 372e  ,66.91C82.83,67.
-00000bf0: 3232 3320 3832 2e36 3433 2c36 372e 3533  223 82.643,67.53
-00000c00: 3720 3832 2e34 352c 3637 2e38 354c 3832  7 82.45,67.85L82
-00000c10: 2e33 352c 3638 2e30 3143 3739 2e31 3231  .35,68.01C79.121
-00000c20: 2c36 382e 3034 3720 3735 2e39 3138 2c36  ,68.047 75.918,6
-00000c30: 372e 3433 3420 3732 2e39 332c 3636 2e32  7.434 72.93,66.2
-00000c40: 3143 3634 2e32 372c 3632 2e37 3420 3539  1C64.27,62.74 59
-00000c50: 2c35 352e 3532 2036 312e 3138 2c35 302e  ,55.52 61.18,50.
-00000c60: 3131 4336 322e 3138 2c34 372e 3620 3634  11C62.18,47.6 64
-00000c70: 2e37 2c34 352e 3832 2036 382e 3236 2c34  .7,45.82 68.26,4
-00000c80: 352e 3131 4337 322e 3438 392c 3434 2e33  5.11C72.489,44.3
-00000c90: 3935 2037 362e 3833 352c 3434 2e39 3038  95 76.835,44.908
-00000ca0: 2038 302e 3738 2c34 362e 3539 4338 322e   80.78,46.59C82.
-00000cb0: 3134 312c 3437 2e31 3434 2038 332e 3435  141,47.144 83.45
-00000cc0: 332c 3437 2e38 3133 2038 342e 372c 3438  3,47.813 84.7,48
-00000cd0: 2e35 3943 3834 2e37 362c 3438 2e37 3620  .59C84.76,48.76 
-00000ce0: 3834 2e38 322c 3438 2e39 3320 3834 2e38  84.82,48.93 84.8
-00000cf0: 382c 3439 2e31 4338 342e 3934 2c34 392e  8,49.1C84.94,49.
-00000d00: 3237 2038 352e 3035 2c34 392e 3633 2038  27 85.05,49.63 8
-00000d10: 352e 3132 2c34 392e 3943 3835 2e32 382c  5.12,49.9C85.28,
-00000d20: 3530 2e35 2038 352e 3434 2c35 312e 3120  50.5 85.44,51.1 
-00000d30: 3835 2e35 352c 3531 2e37 3343 3835 2e36  85.55,51.73C85.6
-00000d40: 3931 2c35 322e 3530 3720 3835 2e37 3932  91,52.507 85.792
-00000d50: 2c35 332e 3239 3220 3835 2e38 352c 3534  ,53.292 85.85,54
-00000d60: 2e30 384c 3835 2e38 352c 3535 2e38 3943  .08L85.85,55.89C
-00000d70: 3835 2e38 352c 3536 2e31 3220 3835 2e39  85.85,56.12 85.9
-00000d80: 312c 3536 2e32 3520 3835 2e39 312c 3536  1,56.25 85.91,56
-00000d90: 2e34 354c 3835 2e38 392c 3536 2e34 345a  .45L85.89,56.44Z
-00000da0: 4d31 372e 3636 2c36 3843 3136 2e36 3638  M17.66,68C16.668
-00000db0: 2c36 362e 3433 3520 3135 2e38 3639 2c36  ,66.435 15.869,6
-00000dc0: 342e 3735 3620 3135 2e32 382c 3633 4c31  4.756 15.28,63L1
-00000dd0: 352e 3137 2c36 322e 3638 4331 352e 3036  5.17,62.68C15.06
-00000de0: 2c36 322e 3335 2031 342e 3936 2c36 322e  ,62.35 14.96,62.
-00000df0: 3031 2031 342e 3837 2c36 312e 3638 4331  01 14.87,61.68C1
-00000e00: 342e 3832 332c 3631 2e34 3933 2031 342e  4.823,61.493 14.
-00000e10: 3737 372c 3631 2e33 3120 3134 2e37 332c  777,61.31 14.73,
-00000e20: 3631 2e31 3343 3134 2e36 362c 3630 2e38  61.13C14.66,60.8
-00000e30: 3420 3134 2e35 392c 3630 2e35 3520 3134  4 14.59,60.55 14
-00000e40: 2e35 332c 3630 2e32 3743 3134 2e34 372c  .53,60.27C14.47,
-00000e50: 3539 2e39 3920 3134 2e34 332c 3539 2e37  59.99 14.43,59.7
-00000e60: 3220 3134 2e33 382c 3539 2e34 3443 3134  2 14.38,59.44C14
-00000e70: 2e33 332c 3539 2e31 3620 3134 2e33 2c35  .33,59.16 14.3,5
-00000e80: 3920 3134 2e32 372c 3538 2e37 3843 3134  9 14.27,58.78C14
-00000e90: 2e32 2c35 382e 3237 2031 342e 3135 2c35  .2,58.27 14.15,5
-00000ea0: 372e 3738 2031 342e 3131 2c35 372e 3233  7.78 14.11,57.23
-00000eb0: 4c31 342e 3131 2c35 372e 3033 4331 342e  L14.11,57.03C14.
-00000ec0: 3030 382c 3535 2e32 3336 2031 342e 3132  008,55.236 14.12
-00000ed0: 322c 3533 2e34 3337 2031 342e 3435 2c35  2,53.437 14.45,5
-00000ee0: 312e 3637 4331 342e 3536 2c35 312e 3036  1.67C14.56,51.06
-00000ef0: 2031 342e 3731 2c35 302e 3436 2031 342e   14.71,50.46 14.
-00000f00: 3838 2c34 392e 3837 4331 342e 3936 2c34  88,49.87C14.96,4
-00000f10: 392e 3539 2031 352e 3034 2c34 392e 3332  9.59 15.04,49.32
-00000f20: 2031 352e 3133 2c34 392e 3035 4331 352e   15.13,49.05C15.
-00000f30: 3232 2c34 382e 3738 2031 352e 3234 2c34  22,48.78 15.24,4
-00000f40: 382e 3732 2031 352e 332c 3438 2e35 3543  8.72 15.3,48.55C
-00000f50: 3136 2e35 3438 2c34 372e 3737 3420 3137  16.548,47.774 17
-00000f60: 2e38 3539 2c34 372e 3130 3520 3139 2e32  .859,47.105 19.2
-00000f70: 322c 3436 2e35 3543 3237 2e38 362c 3433  2,46.55C27.86,43
-00000f80: 2e30 3920 3336 2e36 352c 3434 2e36 3720  .09 36.65,44.67 
-00000f90: 3338 2e38 322c 3530 2e30 3843 3430 2e39  38.82,50.08C40.9
-00000fa0: 392c 3535 2e34 3920 3335 2e37 332c 3632  9,55.49 35.73,62
-00000fb0: 2e37 3420 3237 2e30 392c 3636 2e32 4332  .74 27.09,66.2C2
-00000fc0: 342e 3130 312c 3637 2e34 3331 2032 302e  4.101,67.431 20.
-00000fd0: 3839 332c 3638 2e30 3433 2031 372e 3636  893,68.043 17.66
-00000fe0: 2c36 385a 4d36 382e 3537 2c37 372e 3638  ,68ZM68.57,77.68
-00000ff0: 4336 322e 3535 342c 3739 2e35 3038 2035  C62.554,79.508 5
-00001000: 362e 3238 372c 3830 2e33 3736 2035 302c  6.287,80.376 50,
-00001010: 3830 2e32 3543 3433 2e37 3337 2c38 302e  80.25C43.737,80.
-00001020: 3337 2033 372e 3439 352c 3739 2e35 3036  37 37.495,79.506
-00001030: 2033 312e 352c 3737 2e36 3943 3237 2e31   31.5,77.69C27.1
-00001040: 3835 2c37 362e 3338 2032 332e 3234 332c  85,76.38 23.243,
-00001050: 3734 2e30 3632 2032 302c 3730 2e39 3343  74.062 20,70.93C
-00001060: 3232 2e38 3135 2c37 302e 3730 3620 3235  22.815,70.706 25
-00001070: 2e35 382c 3730 2e30 3535 2032 382e 322c  .58,70.055 28.2,
-00001080: 3639 4333 382e 3337 2c36 342e 3932 2034  69C38.37,64.92 4
-00001090: 342e 3339 2c35 3620 3431 2e36 2c34 3943  4.39,56 41.6,49C
-000010a0: 3338 2e38 312c 3432 2032 382e 3237 2c33  38.81,42 28.27,3
-000010b0: 392e 3732 2031 382e 312c 3433 2e38 4c31  9.72 18.1,43.8L1
-000010c0: 372e 3433 2c34 342e 3039 4331 382e 3937  7.43,44.09C18.97
-000010d0: 332c 3431 2e36 3438 2032 312e 3031 392c  3,41.648 21.019,
-000010e0: 3339 2e35 3631 2032 332e 3433 2c33 372e  39.561 23.43,37.
-000010f0: 3937 4332 362e 3637 312c 3335 2e38 3234  97C26.671,35.824
-00001100: 2033 302e 3437 332c 3334 2e36 3820 3334   30.473,34.68 34
-00001110: 2e33 362c 3334 2e36 3843 3335 2e38 3834  .36,34.68C35.884
-00001120: 2c33 342e 3638 3120 3337 2e34 3034 2c33  ,34.681 37.404,3
-00001130: 342e 3835 3220 3338 2e38 392c 3335 2e31  4.852 38.89,35.1
-00001140: 3943 3432 2e36 3934 2c33 362e 3034 3920  9C42.694,36.049 
-00001150: 3436 2e31 3931 2c33 372e 3933 3520 3439  46.191,37.935 49
-00001160: 2c34 302e 3634 4c35 302c 3431 2e36 344c  ,40.64L50,41.64L
-00001170: 3531 2c34 302e 3634 4335 332e 3739 372c  51,40.64C53.797,
-00001180: 3337 2e39 3337 2035 372e 3237 392c 3336  37.937 57.279,36
-00001190: 2e30 3439 2036 312e 3037 2c33 352e 3138  .049 61.07,35.18
-000011a0: 4336 362e 3430 322c 3333 2e39 3437 2037  C66.402,33.947 7
-000011b0: 322e 3031 342c 3334 2e39 3638 2037 362e  2.014,34.968 76.
-000011c0: 3537 2c33 3843 3738 2e39 382c 3339 2e35  57,38C78.98,39.5
-000011d0: 3838 2038 312e 3032 362c 3431 2e36 3731  88 81.026,41.671
-000011e0: 2038 322e 3537 2c34 342e 3131 4c38 312e   82.57,44.11L81.
-000011f0: 392c 3433 2e38 3243 3737 2e34 3039 2c34  9,43.82C77.409,4
-00001200: 312e 3932 3120 3732 2e34 3634 2c34 312e  1.921 72.464,41.
-00001210: 3335 3520 3637 2e36 362c 3432 2e31 3943  355 67.66,42.19C
-00001220: 3633 2e30 382c 3433 2e31 3220 3539 2e37  63.08,43.12 59.7
-00001230: 392c 3435 2e35 3420 3538 2e33 392c 3439  9,45.54 58.39,49
-00001240: 2e30 3243 3535 2e36 2c35 352e 3937 2036  .02C55.6,55.97 6
-00001250: 312e 3632 2c36 342e 3934 2037 312e 3739  1.62,64.94 71.79
-00001260: 2c36 392e 3032 4337 342e 3431 342c 3730  ,69.02C74.414,70
-00001270: 2e30 3720 3737 2e31 3832 2c37 302e 3731  .07 77.182,70.71
-00001280: 3420 3830 2c37 302e 3933 4337 362e 3737  4 80,70.93C76.77
-00001290: 362c 3734 2e30 3520 3732 2e38 3539 2c37  6,74.05 72.859,7
-000012a0: 362e 3336 3320 3638 2e35 372c 3737 2e36  6.363 68.57,77.6
-000012b0: 385a 2220 7374 796c 653d 2266 696c 6c3a  8Z" style="fill:
-000012c0: 7267 6228 3232 322c 3132 302c 3136 3029  rgb(222,120,160)
-000012d0: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
-000012e0: 726f 3b22 2f3e 0a20 2020 2020 2020 203c  ro;"/>.        <
-000012f0: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
-00001300: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
-00001310: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
-00001320: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
-00001330: 362e 3638 3538 3229 223e 0a20 2020 2020  6.68582)">.     
-00001340: 2020 2020 2020 203c 6369 7263 6c65 2063         <circle c
-00001350: 783d 2237 312e 3333 2220 6379 3d22 3536  x="71.33" cy="56
-00001360: 2220 723d 2235 2e31 3622 2073 7479 6c65  " r="5.16" style
-00001370: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
-00001380: 3230 2c31 3630 293b 222f 3e0a 2020 2020  20,160);"/>.    
-00001390: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
-000013a0: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
-000013b0: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
-000013c0: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
-000013d0: 3232 392c 2d36 2e36 3835 3832 2922 3e0a  229,-6.68582)">.
-000013e0: 2020 2020 2020 2020 2020 2020 3c63 6972              <cir
-000013f0: 636c 6520 6378 3d22 3238 2e36 3722 2063  cle cx="28.67" c
-00001400: 793d 2235 3622 2072 3d22 352e 3136 2220  y="56" r="5.16" 
-00001410: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
-00001420: 3232 322c 3132 302c 3136 3029 3b22 2f3e  222,120,160);"/>
-00001430: 0a20 2020 2020 2020 203c 2f67 3e0a 2020  .        </g>.  
-00001440: 2020 2020 2020 3c67 2074 7261 6e73 666f        <g transfo
-00001450: 726d 3d22 6d61 7472 6978 2830 2e32 3939  rm="matrix(0.299
-00001460: 3031 322c 302c 302c 302e 3239 3930 3132  012,0,0,0.299012
-00001470: 2c39 2e37 3032 3239 2c2d 362e 3638 3538  ,9.70229,-6.6858
-00001480: 3229 223e 0a20 2020 2020 2020 2020 2020  2)">.           
-00001490: 203c 7061 7468 2064 3d22 4d35 382c 3636   <path d="M58,66
-000014a0: 4335 352e 3931 322c 3638 2e31 3631 2035  C55.912,68.161 5
-000014b0: 332e 3030 332c 3639 2e33 3339 2035 302c  3.003,69.339 50,
-000014c0: 3639 2e32 3443 3436 2e39 3937 2c36 392e  69.24C46.997,69.
-000014d0: 3333 3920 3434 2e30 3838 2c36 382e 3136  339 44.088,68.16
-000014e0: 3120 3432 2c36 3643 3431 2e37 3134 2c36  1 42,66C41.714,6
-000014f0: 352e 3637 3720 3431 2e33 3032 2c36 352e  5.677 41.302,65.
-00001500: 3439 3120 3430 2e38 372c 3635 2e34 3931  491 40.87,65.491
-00001510: 4334 302e 3034 322c 3635 2e34 3931 2033  C40.042,65.491 3
-00001520: 392e 3336 312c 3636 2e31 3732 2033 392e  9.361,66.172 39.
-00001530: 3336 312c 3637 4333 392e 3336 312c 3637  361,67C39.361,67
-00001540: 2e33 3638 2033 392e 3439 362c 3637 2e37  .368 39.496,67.7
-00001550: 3234 2033 392e 3734 2c36 3843 3432 2e34  24 39.74,68C42.4
-00001560: 3033 2c37 302e 3830 3420 3436 2e31 3334  03,70.804 46.134
-00001570: 2c37 322e 3335 2035 302c 3732 2e32 3543  ,72.35 50,72.25C
-00001580: 3533 2e38 3632 2c37 322e 3334 3720 3537  53.862,72.347 57
-00001590: 2e35 392c 3730 2e38 3032 2036 302e 3235  .59,70.802 60.25
-000015a0: 2c36 3843 3630 2e34 3935 2c36 372e 3732  ,68C60.495,67.72
-000015b0: 3520 3630 2e36 332c 3637 2e33 3639 2036  5 60.63,67.369 6
-000015c0: 302e 3633 2c36 3743 3630 2e36 332c 3636  0.63,67C60.63,66
-000015d0: 2e31 3734 2035 392e 3935 312c 3635 2e34  .174 59.951,65.4
-000015e0: 3935 2035 392e 3132 352c 3635 2e34 3935  95 59.125,65.495
-000015f0: 4335 382e 3639 352c 3635 2e34 3935 2035  C58.695,65.495 5
-00001600: 382e 3238 352c 3635 2e36 3739 2035 382c  8.285,65.679 58,
-00001610: 3636 5a22 2073 7479 6c65 3d22 6669 6c6c  66Z" style="fill
-00001620: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
-00001630: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
-00001640: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
-00001650: 3c2f 673e 0a20 2020 203c 2f67 3e0a 3c2f  </g>.    </g>.</
-00001660: 7376 673e 0a                             svg>.
+00000080: 3d22 696e 7465 7272 6f67 6174 653a 2036  ="interrogate: 6
+00000090: 302e 3025 223e 0a20 2020 203c 7469 746c  0.0%">.    <titl
+000000a0: 653e 696e 7465 7272 6f67 6174 653a 2036  e>interrogate: 6
+000000b0: 302e 3025 3c2f 7469 746c 653e 0a20 2020  0.0%</title>.   
+000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
+000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
+000000f0: 7769 6474 683d 2239 3322 2068 6569 6768  width="93" heigh
+00000100: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
+00000110: 3522 2f3e 0a20 2020 2020 2020 203c 7265  5"/>.        <re
+00000120: 6374 2078 3d22 3933 2220 7769 6474 683d  ct x="93" width=
+00000130: 2234 3722 2068 6569 6768 743d 2232 3022  "47" height="20"
+00000140: 2066 696c 6c3d 2223 6466 6233 3137 222f   fill="#dfb317"/
+00000150: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
+00000160: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
+00000170: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00000180: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
+00000190: 5665 7264 616e 612c 4765 6e65 7661 2c44  Verdana,Geneva,D
+000001a0: 656a 6156 7520 5361 6e73 2c73 616e 732d  ejaVu Sans,sans-
+000001b0: 7365 7269 6622 2074 6578 742d 7265 6e64  serif" text-rend
+000001c0: 6572 696e 673d 2267 656f 6d65 7472 6963  ering="geometric
+000001d0: 5072 6563 6973 696f 6e22 2066 6f6e 742d  Precision" font-
+000001e0: 7369 7a65 3d22 3131 3022 3e0a 2020 2020  size="110">.    
+000001f0: 2020 2020 3c74 6578 7420 783d 2235 3930      <text x="590
+00000200: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
+00000210: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
+00000220: 6669 6c6c 3d22 2366 6666 2220 7465 7874  fill="#fff" text
+00000230: 4c65 6e67 7468 3d22 3631 3022 3e69 6e74  Length="610">int
+00000240: 6572 726f 6761 7465 3c2f 7465 7874 3e0a  errogate</text>.
+00000250: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
+00000260: 2231 3136 3022 2079 3d22 3134 3022 2074  "1160" y="140" t
+00000270: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
+00000280: 2e31 2922 2066 696c 6c3d 2223 6666 6622  .1)" fill="#fff"
+00000290: 2074 6578 744c 656e 6774 683d 2233 3730   textLength="370
+000002a0: 2220 6461 7461 2d69 6e74 6572 726f 6761  " data-interroga
+000002b0: 7465 3d22 7265 7375 6c74 223e 3630 2e30  te="result">60.0
+000002c0: 253c 2f74 6578 743e 0a20 2020 203c 2f67  %</text>.    </g
+000002d0: 3e0a 2020 2020 3c67 2069 643d 226c 6f67  >.    <g id="log
+000002e0: 6f2d 7069 6e6b 2220 7472 616e 7366 6f72  o-pink" transfor
+000002f0: 6d3d 226d 6174 7269 7828 302e 3835 3438  m="matrix(0.8548
+00000300: 3736 2c30 2c30 2c30 2e38 3534 3837 362c  76,0,0,0.854876,
+00000310: 2d36 2e37 3335 3134 2c30 2e38 3737 3132  -6.73514,0.87712
+00000320: 3429 223e 0a20 2020 2020 2020 203c 6720  4)">.        <g 
+00000330: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+00000340: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+00000350: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00000360: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
+00000370: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+00000380: 224d 3530 2c36 342e 3235 4335 322e 3736  "M50,64.25C52.76
+00000390: 2c36 342e 3235 2035 352c 3631 2e31 3320  ,64.25 55,61.13 
+000003a0: 3535 2c35 392e 3735 4335 352c 3538 2e33  55,59.75C55,58.3
+000003b0: 3720 3532 2e37 362c 3537 2e32 3520 3530  7 52.76,57.25 50
+000003c0: 2c35 372e 3235 4334 372e 3234 2c35 372e  ,57.25C47.24,57.
+000003d0: 3235 2034 352c 3538 2e33 3720 3435 2c35  25 45,58.37 45,5
+000003e0: 392e 3735 4334 352c 3631 2e31 3320 3437  9.75C45,61.13 47
+000003f0: 2e32 342c 3634 2e32 3520 3530 2c36 342e  .24,64.25 50,64.
+00000400: 3235 5a22 2073 7479 6c65 3d22 6669 6c6c  25Z" style="fill
+00000410: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
+00000420: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
+00000430: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
+00000440: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
+00000450: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+00000460: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+00000470: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00000480: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
+00000490: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+000004a0: 224d 3838 2c34 392e 3035 4338 362e 3530  "M88,49.05C86.50
+000004b0: 362c 3433 2e34 3735 2038 332e 3031 382c  6,43.475 83.018,
+000004c0: 3338 2e36 3338 2037 382e 322c 3335 2e34  38.638 78.2,35.4
+000004d0: 3643 3732 2e39 3639 2c33 322e 3030 3220  6C72.969,32.002 
+000004e0: 3636 2e35 3339 2c33 302e 3834 3420 3630  66.539,30.844 60
+000004f0: 2e34 332c 3332 2e32 3643 3536 2e35 3736  .43,32.26C56.576
+00000500: 2c33 332e 3134 3520 3532 2e39 3935 2c33  ,33.145 52.995,3
+00000510: 342e 3935 3820 3530 2c33 372e 3534 4334  4.958 50,37.54C4
+00000520: 362e 3939 382c 3334 2e39 3538 2034 332e  6.998,34.958 43.
+00000530: 3431 312c 3333 2e31 3439 2033 392e 3535  411,33.149 39.55
+00000540: 2c33 322e 3237 4333 332e 3434 312c 3330  ,32.27C33.441,30
+00000550: 2e38 3533 2032 372e 3031 312c 3332 2e30  .853 27.011,32.0
+00000560: 3131 2032 312e 3738 2c33 352e 3437 4331  11 21.78,35.47C1
+00000570: 362e 3937 2c33 382e 3635 3220 3133 2e34  6.97,38.652 13.4
+00000580: 3839 2c34 332e 3438 3920 3132 2c34 392e  89,43.489 12,49.
+00000590: 3036 4c31 322c 3439 2e31 3343 3131 2e38  06L12,49.13C11.8
+000005a0: 322c 3439 2e37 3920 3131 2e36 362c 3530  2,49.79 11.66,50
+000005b0: 2e34 3620 3131 2e35 332c 3531 2e31 3343  .46 11.53,51.13C
+000005c0: 3131 2e31 3436 2c35 332e 3230 3720 3131  11.146,53.207 11
+000005d0: 2e30 3231 2c35 352e 3332 3320 3131 2e31  .021,55.323 11.1
+000005e0: 362c 3537 2e34 3343 3131 2e31 362c 3538  6,57.43C11.16,58
+000005f0: 2e30 3320 3131 2e32 362c 3538 2e36 3320  .03 11.26,58.63 
+00000600: 3131 2e33 342c 3539 2e32 3343 3131 2e33  11.34,59.23C11.3
+00000610: 342c 3539 2e35 3120 3131 2e34 332c 3539  4,59.51 11.43,59
+00000620: 2e37 3920 3131 2e34 382c 3630 2e30 3743  .79 11.48,60.07C
+00000630: 3131 2e35 332c 3630 2e33 3520 3131 2e35  11.53,60.35 11.5
+00000640: 382c 3630 2e36 3820 3131 2e36 342c 3630  8,60.68 11.64,60
+00000650: 2e39 3843 3131 2e37 2c36 312e 3238 2031  .98C11.7,61.28 1
+00000660: 312e 382c 3631 2e36 3920 3131 2e38 392c  1.8,61.69 11.89,
+00000670: 3632 2e30 3543 3131 2e39 382c 3632 2e34  62.05C11.98,62.4
+00000680: 3120 3131 2e39 392c 3632 2e34 3720 3132  1 11.99,62.47 12
+00000690: 2e30 352c 3632 2e36 3843 3132 2e31 362c  .05,62.68C12.16,
+000006a0: 3633 2e30 3720 3132 2e32 382c 3633 2e34  63.07 12.28,63.4
+000006b0: 3620 3132 2e34 312c 3633 2e38 344c 3132  6 12.41,63.84L12
+000006c0: 2e35 382c 3634 2e33 3443 3132 2e37 322c  .58,64.34C12.72,
+000006d0: 3634 2e37 3420 3132 2e38 382c 3635 2e31  64.74 12.88,65.1
+000006e0: 3420 3133 2e30 342c 3635 2e35 334c 3133  4 13.04,65.53L13
+000006f0: 2e32 332c 3635 2e39 3843 3133 2e34 3033  .23,65.98C13.403
+00000700: 2c36 362e 3337 3320 3133 2e35 3833 2c36  ,66.373 13.583,6
+00000710: 362e 3736 3720 3133 2e37 372c 3637 2e31  6.767 13.77,67.1
+00000720: 364c 3133 2e39 392c 3637 2e35 3943 3134  6L13.99,67.59C14
+00000730: 2e31 392c 3637 2e39 3720 3134 2e33 392c  .19,67.97 14.39,
+00000740: 3638 2e33 3520 3134 2e36 312c 3638 2e37  68.35 14.61,68.7
+00000750: 334c 3134 2e38 372c 3639 2e31 3543 3135  3L14.87,69.15C15
+00000760: 2e31 2c36 392e 3532 2031 352e 3333 2c36  .1,69.52 15.33,6
+00000770: 392e 3839 2031 352e 3538 2c37 302e 3236  9.89 15.58,70.26
+00000780: 4c31 352e 3538 2c37 302e 3332 4c31 352e  L15.58,70.32L15.
+00000790: 3939 2c37 302e 3933 4331 362e 3134 2c37  99,70.93C16.14,7
+000007a0: 312e 3134 2031 362e 3239 2c37 312e 3336  1.14 16.29,71.36
+000007b0: 2031 362e 3435 2c37 312e 3537 4332 302e   16.45,71.57C20.
+000007c0: 3230 362c 3735 2e38 3320 3235 2e30 3836  206,75.83 25.086
+000007d0: 2c37 382e 3935 2033 302e 3533 2c38 302e  ,78.95 30.53,80.
+000007e0: 3537 4333 362e 3833 392c 3832 2e34 3820  57C36.839,82.48 
+000007f0: 3433 2e34 312c 3833 2e33 3835 2035 302c  43.41,83.385 50,
+00000800: 3833 2e32 3543 3536 2e35 3939 2c38 332e  83.25C56.599,83.
+00000810: 3337 3420 3633 2e31 3737 2c38 322e 3435  374 63.177,82.45
+00000820: 3620 3639 2e34 392c 3830 2e35 3343 3734  6 69.49,80.53C74
+00000830: 2e36 3434 2c37 382e 3937 3820 3739 2e33  .644,78.978 79.3
+00000840: 3033 2c37 362e 3130 3220 3833 2c37 322e  03,76.102 83,72.
+00000850: 3139 4338 332e 3334 2c37 312e 3738 2038  19C83.34,71.78 8
+00000860: 332e 3635 2c37 312e 3335 2038 342c 3730  3.65,71.35 84,70
+00000870: 2e39 324c 3834 2e31 382c 3730 2e36 364c  .92L84.18,70.66L
+00000880: 3834 2e33 332c 3730 2e34 344c 3834 2e34  84.33,70.44L84.4
+00000890: 312c 3730 2e33 3243 3834 2e35 352c 3730  1,70.32C84.55,70
+000008a0: 2e31 3220 3834 2e36 372c 3639 2e39 2038  .12 84.67,69.9 8
+000008b0: 342e 3831 2c36 392e 3743 3835 2e30 372c  4.81,69.7C85.07,
+000008c0: 3639 2e33 2038 352e 3332 2c36 382e 3839  69.3 85.32,68.89
+000008d0: 2038 352e 3535 2c36 382e 3438 4338 352e   85.55,68.48C85.
+000008e0: 3738 2c36 382e 3037 2038 362e 3032 2c36  78,68.07 86.02,6
+000008f0: 372e 3635 2038 362e 3233 2c36 372e 3232  7.65 86.23,67.22
+00000900: 4338 362e 3331 2c36 372e 3035 2038 362e  C86.31,67.05 86.
+00000910: 3339 2c36 362e 3838 2038 362e 3437 2c36  39,66.88 86.47,6
+00000920: 362e 3743 3836 2e36 372c 3636 2e32 3820  6.7C86.67,66.28 
+00000930: 3836 2e38 352c 3635 2e38 3720 3837 2e30  86.85,65.87 87.0
+00000940: 332c 3635 2e34 344c 3837 2e32 332c 3634  3,65.44L87.23,64
+00000950: 2e39 3243 3837 2e33 3937 2c36 342e 3438  .92C87.397,64.48
+00000960: 3720 3837 2e35 352c 3634 2e30 3520 3837  7 87.55,64.05 87
+00000970: 2e36 392c 3633 2e36 314c 3837 2e38 352c  .69,63.61L87.85,
+00000980: 3633 2e30 3943 3837 2e39 382c 3632 2e36  63.09C87.98,62.6
+00000990: 3420 3838 2e31 2c36 322e 3139 2038 382e  4 88.1,62.19 88.
+000009a0: 3231 2c36 312e 3734 4338 382e 3231 2c36  21,61.74C88.21,6
+000009b0: 312e 3537 2038 382e 332c 3631 2e33 3920  1.57 88.3,61.39 
+000009c0: 3838 2e33 332c 3631 2e32 3243 3838 2e34  88.33,61.22C88.4
+000009d0: 332c 3630 2e37 3520 3838 2e35 322c 3630  3,60.75 88.52,60
+000009e0: 2e32 3220 3838 2e36 2c35 392e 3739 4338  .22 88.6,59.79C8
+000009f0: 382e 362c 3539 2e36 3420 3838 2e36 362c  8.6,59.64 88.66,
+00000a00: 3539 2e34 3920 3838 2e36 382c 3539 2e33  59.49 88.68,59.3
+00000a10: 3343 3838 2e37 372c 3538 2e37 3120 3838  3C88.77,58.71 88
+00000a20: 2e38 342c 3538 2e30 3820 3838 2e38 382c  .84,58.08 88.88,
+00000a30: 3537 2e34 354c 3838 2e38 382c 3534 2e31  57.45L88.88,54.1
+00000a40: 3743 3838 2e38 3137 2c35 332e 3136 3420  7C88.817,53.164 
+00000a50: 3838 2e36 3933 2c35 322e 3136 3220 3838  88.693,52.162 88
+00000a60: 2e35 312c 3531 2e31 3743 3838 2e33 382c  .51,51.17C88.38,
+00000a70: 3530 2e35 2038 382e 3233 2c34 392e 3834  50.5 88.23,49.84
+00000a80: 2038 382e 3035 2c34 392e 3137 4c38 382c   88.05,49.17L88,
+00000a90: 3439 2e30 355a 4d38 352e 3839 2c35 362e  49.05ZM85.89,56.
+00000aa0: 3434 4c38 352e 3839 2c35 372e 3233 4338  44L85.89,57.23C8
+00000ab0: 352e 3839 2c35 372e 3738 2038 352e 3739  5.89,57.78 85.79
+00000ac0: 2c35 382e 3332 2038 352e 3732 2c35 382e  ,58.32 85.72,58.
+00000ad0: 3836 4338 352e 3732 2c35 392e 3031 2038  86C85.72,59.01 8
+00000ae0: 352e 3732 2c35 392e 3135 2038 352e 3635  5.72,59.15 85.65
+00000af0: 2c35 392e 3343 3835 2e35 392c 3539 2e37  ,59.3C85.59,59.7
+00000b00: 2038 352e 3531 2c36 302e 3131 2038 352e   85.51,60.11 85.
+00000b10: 3433 2c36 302e 3531 4c38 352e 3332 2c36  43,60.51L85.32,6
+00000b20: 302e 3939 4338 352e 3233 2c36 312e 3338  0.99C85.23,61.38
+00000b30: 2038 352e 3132 2c36 312e 3737 2038 352e   85.12,61.77 85.
+00000b40: 3031 2c36 322e 3136 4338 352e 3031 2c36  01,62.16C85.01,6
+00000b50: 322e 3331 2038 342e 3933 2c36 322e 3436  2.31 84.93,62.46
+00000b60: 2038 342e 3838 2c36 322e 3643 3834 2e37   84.88,62.6C84.7
+00000b70: 342c 3633 2e30 3420 3834 2e35 392c 3633  4,63.04 84.59,63
+00000b80: 2e34 3720 3834 2e34 322c 3633 2e39 4c38  .47 84.42,63.9L8
+00000b90: 342e 3237 2c36 342e 3238 4338 342e 312c  4.27,64.28C84.1,
+00000ba0: 3634 2e37 3120 3833 2e39 312c 3635 2e31  64.71 83.91,65.1
+00000bb0: 3420 3833 2e37 312c 3635 2e35 3643 3833  4 83.71,65.56C83
+00000bc0: 2e35 312c 3635 2e39 3820 3833 2e34 332c  .51,65.98 83.43,
+00000bd0: 3636 2e31 3220 3833 2e32 382c 3636 2e34  66.12 83.28,66.4
+00000be0: 4c38 332e 3031 2c36 362e 3931 4338 322e  L83.01,66.91C82.
+00000bf0: 3833 2c36 372e 3232 3320 3832 2e36 3433  83,67.223 82.643
+00000c00: 2c36 372e 3533 3720 3832 2e34 352c 3637  ,67.537 82.45,67
+00000c10: 2e38 354c 3832 2e33 352c 3638 2e30 3143  .85L82.35,68.01C
+00000c20: 3739 2e31 3231 2c36 382e 3034 3720 3735  79.121,68.047 75
+00000c30: 2e39 3138 2c36 372e 3433 3420 3732 2e39  .918,67.434 72.9
+00000c40: 332c 3636 2e32 3143 3634 2e32 372c 3632  3,66.21C64.27,62
+00000c50: 2e37 3420 3539 2c35 352e 3532 2036 312e  .74 59,55.52 61.
+00000c60: 3138 2c35 302e 3131 4336 322e 3138 2c34  18,50.11C62.18,4
+00000c70: 372e 3620 3634 2e37 2c34 352e 3832 2036  7.6 64.7,45.82 6
+00000c80: 382e 3236 2c34 352e 3131 4337 322e 3438  8.26,45.11C72.48
+00000c90: 392c 3434 2e33 3935 2037 362e 3833 352c  9,44.395 76.835,
+00000ca0: 3434 2e39 3038 2038 302e 3738 2c34 362e  44.908 80.78,46.
+00000cb0: 3539 4338 322e 3134 312c 3437 2e31 3434  59C82.141,47.144
+00000cc0: 2038 332e 3435 332c 3437 2e38 3133 2038   83.453,47.813 8
+00000cd0: 342e 372c 3438 2e35 3943 3834 2e37 362c  4.7,48.59C84.76,
+00000ce0: 3438 2e37 3620 3834 2e38 322c 3438 2e39  48.76 84.82,48.9
+00000cf0: 3320 3834 2e38 382c 3439 2e31 4338 342e  3 84.88,49.1C84.
+00000d00: 3934 2c34 392e 3237 2038 352e 3035 2c34  94,49.27 85.05,4
+00000d10: 392e 3633 2038 352e 3132 2c34 392e 3943  9.63 85.12,49.9C
+00000d20: 3835 2e32 382c 3530 2e35 2038 352e 3434  85.28,50.5 85.44
+00000d30: 2c35 312e 3120 3835 2e35 352c 3531 2e37  ,51.1 85.55,51.7
+00000d40: 3343 3835 2e36 3931 2c35 322e 3530 3720  3C85.691,52.507 
+00000d50: 3835 2e37 3932 2c35 332e 3239 3220 3835  85.792,53.292 85
+00000d60: 2e38 352c 3534 2e30 384c 3835 2e38 352c  .85,54.08L85.85,
+00000d70: 3535 2e38 3943 3835 2e38 352c 3536 2e31  55.89C85.85,56.1
+00000d80: 3220 3835 2e39 312c 3536 2e32 3520 3835  2 85.91,56.25 85
+00000d90: 2e39 312c 3536 2e34 354c 3835 2e38 392c  .91,56.45L85.89,
+00000da0: 3536 2e34 345a 4d31 372e 3636 2c36 3843  56.44ZM17.66,68C
+00000db0: 3136 2e36 3638 2c36 362e 3433 3520 3135  16.668,66.435 15
+00000dc0: 2e38 3639 2c36 342e 3735 3620 3135 2e32  .869,64.756 15.2
+00000dd0: 382c 3633 4c31 352e 3137 2c36 322e 3638  8,63L15.17,62.68
+00000de0: 4331 352e 3036 2c36 322e 3335 2031 342e  C15.06,62.35 14.
+00000df0: 3936 2c36 322e 3031 2031 342e 3837 2c36  96,62.01 14.87,6
+00000e00: 312e 3638 4331 342e 3832 332c 3631 2e34  1.68C14.823,61.4
+00000e10: 3933 2031 342e 3737 372c 3631 2e33 3120  93 14.777,61.31 
+00000e20: 3134 2e37 332c 3631 2e31 3343 3134 2e36  14.73,61.13C14.6
+00000e30: 362c 3630 2e38 3420 3134 2e35 392c 3630  6,60.84 14.59,60
+00000e40: 2e35 3520 3134 2e35 332c 3630 2e32 3743  .55 14.53,60.27C
+00000e50: 3134 2e34 372c 3539 2e39 3920 3134 2e34  14.47,59.99 14.4
+00000e60: 332c 3539 2e37 3220 3134 2e33 382c 3539  3,59.72 14.38,59
+00000e70: 2e34 3443 3134 2e33 332c 3539 2e31 3620  .44C14.33,59.16 
+00000e80: 3134 2e33 2c35 3920 3134 2e32 372c 3538  14.3,59 14.27,58
+00000e90: 2e37 3843 3134 2e32 2c35 382e 3237 2031  .78C14.2,58.27 1
+00000ea0: 342e 3135 2c35 372e 3738 2031 342e 3131  4.15,57.78 14.11
+00000eb0: 2c35 372e 3233 4c31 342e 3131 2c35 372e  ,57.23L14.11,57.
+00000ec0: 3033 4331 342e 3030 382c 3535 2e32 3336  03C14.008,55.236
+00000ed0: 2031 342e 3132 322c 3533 2e34 3337 2031   14.122,53.437 1
+00000ee0: 342e 3435 2c35 312e 3637 4331 342e 3536  4.45,51.67C14.56
+00000ef0: 2c35 312e 3036 2031 342e 3731 2c35 302e  ,51.06 14.71,50.
+00000f00: 3436 2031 342e 3838 2c34 392e 3837 4331  46 14.88,49.87C1
+00000f10: 342e 3936 2c34 392e 3539 2031 352e 3034  4.96,49.59 15.04
+00000f20: 2c34 392e 3332 2031 352e 3133 2c34 392e  ,49.32 15.13,49.
+00000f30: 3035 4331 352e 3232 2c34 382e 3738 2031  05C15.22,48.78 1
+00000f40: 352e 3234 2c34 382e 3732 2031 352e 332c  5.24,48.72 15.3,
+00000f50: 3438 2e35 3543 3136 2e35 3438 2c34 372e  48.55C16.548,47.
+00000f60: 3737 3420 3137 2e38 3539 2c34 372e 3130  774 17.859,47.10
+00000f70: 3520 3139 2e32 322c 3436 2e35 3543 3237  5 19.22,46.55C27
+00000f80: 2e38 362c 3433 2e30 3920 3336 2e36 352c  .86,43.09 36.65,
+00000f90: 3434 2e36 3720 3338 2e38 322c 3530 2e30  44.67 38.82,50.0
+00000fa0: 3843 3430 2e39 392c 3535 2e34 3920 3335  8C40.99,55.49 35
+00000fb0: 2e37 332c 3632 2e37 3420 3237 2e30 392c  .73,62.74 27.09,
+00000fc0: 3636 2e32 4332 342e 3130 312c 3637 2e34  66.2C24.101,67.4
+00000fd0: 3331 2032 302e 3839 332c 3638 2e30 3433  31 20.893,68.043
+00000fe0: 2031 372e 3636 2c36 385a 4d36 382e 3537   17.66,68ZM68.57
+00000ff0: 2c37 372e 3638 4336 322e 3535 342c 3739  ,77.68C62.554,79
+00001000: 2e35 3038 2035 362e 3238 372c 3830 2e33  .508 56.287,80.3
+00001010: 3736 2035 302c 3830 2e32 3543 3433 2e37  76 50,80.25C43.7
+00001020: 3337 2c38 302e 3337 2033 372e 3439 352c  37,80.37 37.495,
+00001030: 3739 2e35 3036 2033 312e 352c 3737 2e36  79.506 31.5,77.6
+00001040: 3943 3237 2e31 3835 2c37 362e 3338 2032  9C27.185,76.38 2
+00001050: 332e 3234 332c 3734 2e30 3632 2032 302c  3.243,74.062 20,
+00001060: 3730 2e39 3343 3232 2e38 3135 2c37 302e  70.93C22.815,70.
+00001070: 3730 3620 3235 2e35 382c 3730 2e30 3535  706 25.58,70.055
+00001080: 2032 382e 322c 3639 4333 382e 3337 2c36   28.2,69C38.37,6
+00001090: 342e 3932 2034 342e 3339 2c35 3620 3431  4.92 44.39,56 41
+000010a0: 2e36 2c34 3943 3338 2e38 312c 3432 2032  .6,49C38.81,42 2
+000010b0: 382e 3237 2c33 392e 3732 2031 382e 312c  8.27,39.72 18.1,
+000010c0: 3433 2e38 4c31 372e 3433 2c34 342e 3039  43.8L17.43,44.09
+000010d0: 4331 382e 3937 332c 3431 2e36 3438 2032  C18.973,41.648 2
+000010e0: 312e 3031 392c 3339 2e35 3631 2032 332e  1.019,39.561 23.
+000010f0: 3433 2c33 372e 3937 4332 362e 3637 312c  43,37.97C26.671,
+00001100: 3335 2e38 3234 2033 302e 3437 332c 3334  35.824 30.473,34
+00001110: 2e36 3820 3334 2e33 362c 3334 2e36 3843  .68 34.36,34.68C
+00001120: 3335 2e38 3834 2c33 342e 3638 3120 3337  35.884,34.681 37
+00001130: 2e34 3034 2c33 342e 3835 3220 3338 2e38  .404,34.852 38.8
+00001140: 392c 3335 2e31 3943 3432 2e36 3934 2c33  9,35.19C42.694,3
+00001150: 362e 3034 3920 3436 2e31 3931 2c33 372e  6.049 46.191,37.
+00001160: 3933 3520 3439 2c34 302e 3634 4c35 302c  935 49,40.64L50,
+00001170: 3431 2e36 344c 3531 2c34 302e 3634 4335  41.64L51,40.64C5
+00001180: 332e 3739 372c 3337 2e39 3337 2035 372e  3.797,37.937 57.
+00001190: 3237 392c 3336 2e30 3439 2036 312e 3037  279,36.049 61.07
+000011a0: 2c33 352e 3138 4336 362e 3430 322c 3333  ,35.18C66.402,33
+000011b0: 2e39 3437 2037 322e 3031 342c 3334 2e39  .947 72.014,34.9
+000011c0: 3638 2037 362e 3537 2c33 3843 3738 2e39  68 76.57,38C78.9
+000011d0: 382c 3339 2e35 3838 2038 312e 3032 362c  8,39.588 81.026,
+000011e0: 3431 2e36 3731 2038 322e 3537 2c34 342e  41.671 82.57,44.
+000011f0: 3131 4c38 312e 392c 3433 2e38 3243 3737  11L81.9,43.82C77
+00001200: 2e34 3039 2c34 312e 3932 3120 3732 2e34  .409,41.921 72.4
+00001210: 3634 2c34 312e 3335 3520 3637 2e36 362c  64,41.355 67.66,
+00001220: 3432 2e31 3943 3633 2e30 382c 3433 2e31  42.19C63.08,43.1
+00001230: 3220 3539 2e37 392c 3435 2e35 3420 3538  2 59.79,45.54 58
+00001240: 2e33 392c 3439 2e30 3243 3535 2e36 2c35  .39,49.02C55.6,5
+00001250: 352e 3937 2036 312e 3632 2c36 342e 3934  5.97 61.62,64.94
+00001260: 2037 312e 3739 2c36 392e 3032 4337 342e   71.79,69.02C74.
+00001270: 3431 342c 3730 2e30 3720 3737 2e31 3832  414,70.07 77.182
+00001280: 2c37 302e 3731 3420 3830 2c37 302e 3933  ,70.714 80,70.93
+00001290: 4337 362e 3737 362c 3734 2e30 3520 3732  C76.776,74.05 72
+000012a0: 2e38 3539 2c37 362e 3336 3320 3638 2e35  .859,76.363 68.5
+000012b0: 372c 3737 2e36 385a 2220 7374 796c 653d  7,77.68Z" style=
+000012c0: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
+000012d0: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
+000012e0: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
+000012f0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00001300: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00001310: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+00001320: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+00001330: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
+00001340: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
+00001350: 7263 6c65 2063 783d 2237 312e 3333 2220  rcle cx="71.33" 
+00001360: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
+00001370: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
+00001380: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
+00001390: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
+000013a0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
+000013b0: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
+000013c0: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
+000013d0: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
+000013e0: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
+000013f0: 2020 3c63 6972 636c 6520 6378 3d22 3238    <circle cx="28
+00001400: 2e36 3722 2063 793d 2235 3622 2072 3d22  .67" cy="56" r="
+00001410: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
+00001420: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
+00001430: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
+00001440: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
+00001450: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00001460: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
+00001470: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
+00001480: 362e 3638 3538 3229 223e 0a20 2020 2020  6.68582)">.     
+00001490: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
+000014a0: 4d35 382c 3636 4335 352e 3931 322c 3638  M58,66C55.912,68
+000014b0: 2e31 3631 2035 332e 3030 332c 3639 2e33  .161 53.003,69.3
+000014c0: 3339 2035 302c 3639 2e32 3443 3436 2e39  39 50,69.24C46.9
+000014d0: 3937 2c36 392e 3333 3920 3434 2e30 3838  97,69.339 44.088
+000014e0: 2c36 382e 3136 3120 3432 2c36 3643 3431  ,68.161 42,66C41
+000014f0: 2e37 3134 2c36 352e 3637 3720 3431 2e33  .714,65.677 41.3
+00001500: 3032 2c36 352e 3439 3120 3430 2e38 372c  02,65.491 40.87,
+00001510: 3635 2e34 3931 4334 302e 3034 322c 3635  65.491C40.042,65
+00001520: 2e34 3931 2033 392e 3336 312c 3636 2e31  .491 39.361,66.1
+00001530: 3732 2033 392e 3336 312c 3637 4333 392e  72 39.361,67C39.
+00001540: 3336 312c 3637 2e33 3638 2033 392e 3439  361,67.368 39.49
+00001550: 362c 3637 2e37 3234 2033 392e 3734 2c36  6,67.724 39.74,6
+00001560: 3843 3432 2e34 3033 2c37 302e 3830 3420  8C42.403,70.804 
+00001570: 3436 2e31 3334 2c37 322e 3335 2035 302c  46.134,72.35 50,
+00001580: 3732 2e32 3543 3533 2e38 3632 2c37 322e  72.25C53.862,72.
+00001590: 3334 3720 3537 2e35 392c 3730 2e38 3032  347 57.59,70.802
+000015a0: 2036 302e 3235 2c36 3843 3630 2e34 3935   60.25,68C60.495
+000015b0: 2c36 372e 3732 3520 3630 2e36 332c 3637  ,67.725 60.63,67
+000015c0: 2e33 3639 2036 302e 3633 2c36 3743 3630  .369 60.63,67C60
+000015d0: 2e36 332c 3636 2e31 3734 2035 392e 3935  .63,66.174 59.95
+000015e0: 312c 3635 2e34 3935 2035 392e 3132 352c  1,65.495 59.125,
+000015f0: 3635 2e34 3935 4335 382e 3639 352c 3635  65.495C58.695,65
+00001600: 2e34 3935 2035 382e 3238 352c 3635 2e36  .495 58.285,65.6
+00001610: 3739 2035 382c 3636 5a22 2073 7479 6c65  79 58,66Z" style
+00001620: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
+00001630: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
+00001640: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
+00001650: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
+00001660: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/90.svg`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
 00000050: 6b22 2077 6964 7468 3d22 3134 3022 2068  k" width="140" h
 00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 696e 7465 7272 6f67 6174 653a 2036  ="interrogate: 6
+00000080: 3d22 696e 7465 7272 6f67 6174 653a 2039  ="interrogate: 9
 00000090: 302e 3025 223e 0a20 2020 203c 7469 746c  0.0%">.    <titl
-000000a0: 653e 696e 7465 7272 6f67 6174 653a 2036  e>interrogate: 6
+000000a0: 653e 696e 7465 7272 6f67 6174 653a 2039  e>interrogate: 9
 000000b0: 302e 3025 3c2f 7469 746c 653e 0a20 2020  0.0%</title>.   
 000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
 000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
 000000f0: 7769 6474 683d 2239 3322 2068 6569 6768  width="93" heigh
 00000100: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
 00000110: 3522 2f3e 0a20 2020 2020 2020 203c 7265  5"/>.        <re
 00000120: 6374 2078 3d22 3933 2220 7769 6474 683d  ct x="93" width=
 00000130: 2234 3722 2068 6569 6768 743d 2232 3022  "47" height="20"
-00000140: 2066 696c 6c3d 2223 6466 6233 3137 222f   fill="#dfb317"/
+00000140: 2066 696c 6c3d 2223 3937 4341 3030 222f   fill="#97CA00"/
 00000150: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00000160: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
 00000170: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
 00000180: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
 00000190: 5665 7264 616e 612c 4765 6e65 7661 2c44  Verdana,Geneva,D
 000001a0: 656a 6156 7520 5361 6e73 2c73 616e 732d  ejaVu Sans,sans-
 000001b0: 7365 7269 6622 2074 6578 742d 7265 6e64  serif" text-rend
@@ -37,15 +37,15 @@
 00000240: 6572 726f 6761 7465 3c2f 7465 7874 3e0a  errogate</text>.
 00000250: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
 00000260: 2231 3136 3022 2079 3d22 3134 3022 2074  "1160" y="140" t
 00000270: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
 00000280: 2e31 2922 2066 696c 6c3d 2223 6666 6622  .1)" fill="#fff"
 00000290: 2074 6578 744c 656e 6774 683d 2233 3730   textLength="370
 000002a0: 2220 6461 7461 2d69 6e74 6572 726f 6761  " data-interroga
-000002b0: 7465 3d22 7265 7375 6c74 223e 3630 2e30  te="result">60.0
+000002b0: 7465 3d22 7265 7375 6c74 223e 3930 2e30  te="result">90.0
 000002c0: 253c 2f74 6578 743e 0a20 2020 203c 2f67  %</text>.    </g
 000002d0: 3e0a 2020 2020 3c67 2069 643d 226c 6f67  >.    <g id="log
 000002e0: 6f2d 7069 6e6b 2220 7472 616e 7366 6f72  o-pink" transfor
 000002f0: 6d3d 226d 6174 7269 7828 302e 3835 3438  m="matrix(0.8548
 00000300: 3736 2c30 2c30 2c30 2e38 3534 3837 362c  76,0,0,0.854876,
 00000310: 2d36 2e37 3335 3134 2c30 2e38 3737 3132  -6.73514,0.87712
 00000320: 3429 223e 0a20 2020 2020 2020 203c 6720  4)">.        <g
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/99.svg`

 * *Files 1% similar despite different names*

```diff
@@ -3,357 +3,357 @@
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
 00000050: 6b22 2077 6964 7468 3d22 3134 3022 2068  k" width="140" h
 00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
 00000080: 3d22 696e 7465 7272 6f67 6174 653a 2039  ="interrogate: 9
-00000090: 302e 3025 223e 0a20 2020 203c 7469 746c  0.0%">.    <titl
+00000090: 392e 3925 223e 0a20 2020 203c 7469 746c  9.9%">.    <titl
 000000a0: 653e 696e 7465 7272 6f67 6174 653a 2039  e>interrogate: 9
-000000b0: 302e 3025 3c2f 7469 746c 653e 0a20 2020  0.0%</title>.   
+000000b0: 392e 3925 3c2f 7469 746c 653e 0a20 2020  9.9%</title>.   
 000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
 000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
 000000f0: 7769 6474 683d 2239 3322 2068 6569 6768  width="93" heigh
 00000100: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
 00000110: 3522 2f3e 0a20 2020 2020 2020 203c 7265  5"/>.        <re
 00000120: 6374 2078 3d22 3933 2220 7769 6474 683d  ct x="93" width=
 00000130: 2234 3722 2068 6569 6768 743d 2232 3022  "47" height="20"
-00000140: 2066 696c 6c3d 2223 3937 4341 3030 222f   fill="#97CA00"/
-00000150: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
-00000160: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
-00000170: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
-00000180: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
-00000190: 5665 7264 616e 612c 4765 6e65 7661 2c44  Verdana,Geneva,D
-000001a0: 656a 6156 7520 5361 6e73 2c73 616e 732d  ejaVu Sans,sans-
-000001b0: 7365 7269 6622 2074 6578 742d 7265 6e64  serif" text-rend
-000001c0: 6572 696e 673d 2267 656f 6d65 7472 6963  ering="geometric
-000001d0: 5072 6563 6973 696f 6e22 2066 6f6e 742d  Precision" font-
-000001e0: 7369 7a65 3d22 3131 3022 3e0a 2020 2020  size="110">.    
-000001f0: 2020 2020 3c74 6578 7420 783d 2235 3930      <text x="590
-00000200: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
-00000210: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
-00000220: 6669 6c6c 3d22 2366 6666 2220 7465 7874  fill="#fff" text
-00000230: 4c65 6e67 7468 3d22 3631 3022 3e69 6e74  Length="610">int
-00000240: 6572 726f 6761 7465 3c2f 7465 7874 3e0a  errogate</text>.
-00000250: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
-00000260: 2231 3136 3022 2079 3d22 3134 3022 2074  "1160" y="140" t
-00000270: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00000280: 2e31 2922 2066 696c 6c3d 2223 6666 6622  .1)" fill="#fff"
-00000290: 2074 6578 744c 656e 6774 683d 2233 3730   textLength="370
-000002a0: 2220 6461 7461 2d69 6e74 6572 726f 6761  " data-interroga
-000002b0: 7465 3d22 7265 7375 6c74 223e 3930 2e30  te="result">90.0
-000002c0: 253c 2f74 6578 743e 0a20 2020 203c 2f67  %</text>.    </g
-000002d0: 3e0a 2020 2020 3c67 2069 643d 226c 6f67  >.    <g id="log
-000002e0: 6f2d 7069 6e6b 2220 7472 616e 7366 6f72  o-pink" transfor
-000002f0: 6d3d 226d 6174 7269 7828 302e 3835 3438  m="matrix(0.8548
-00000300: 3736 2c30 2c30 2c30 2e38 3534 3837 362c  76,0,0,0.854876,
-00000310: 2d36 2e37 3335 3134 2c30 2e38 3737 3132  -6.73514,0.87712
-00000320: 3429 223e 0a20 2020 2020 2020 203c 6720  4)">.        <g 
-00000330: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00000340: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-00000350: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00000360: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
-00000370: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-00000380: 224d 3530 2c36 342e 3235 4335 322e 3736  "M50,64.25C52.76
-00000390: 2c36 342e 3235 2035 352c 3631 2e31 3320  ,64.25 55,61.13 
-000003a0: 3535 2c35 392e 3735 4335 352c 3538 2e33  55,59.75C55,58.3
-000003b0: 3720 3532 2e37 362c 3537 2e32 3520 3530  7 52.76,57.25 50
-000003c0: 2c35 372e 3235 4334 372e 3234 2c35 372e  ,57.25C47.24,57.
-000003d0: 3235 2034 352c 3538 2e33 3720 3435 2c35  25 45,58.37 45,5
-000003e0: 392e 3735 4334 352c 3631 2e31 3320 3437  9.75C45,61.13 47
-000003f0: 2e32 342c 3634 2e32 3520 3530 2c36 342e  .24,64.25 50,64.
-00000400: 3235 5a22 2073 7479 6c65 3d22 6669 6c6c  25Z" style="fill
-00000410: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
-00000420: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
-00000430: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
-00000440: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
-00000450: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00000460: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-00000470: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00000480: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
-00000490: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-000004a0: 224d 3838 2c34 392e 3035 4338 362e 3530  "M88,49.05C86.50
-000004b0: 362c 3433 2e34 3735 2038 332e 3031 382c  6,43.475 83.018,
-000004c0: 3338 2e36 3338 2037 382e 322c 3335 2e34  38.638 78.2,35.4
-000004d0: 3643 3732 2e39 3639 2c33 322e 3030 3220  6C72.969,32.002 
-000004e0: 3636 2e35 3339 2c33 302e 3834 3420 3630  66.539,30.844 60
-000004f0: 2e34 332c 3332 2e32 3643 3536 2e35 3736  .43,32.26C56.576
-00000500: 2c33 332e 3134 3520 3532 2e39 3935 2c33  ,33.145 52.995,3
-00000510: 342e 3935 3820 3530 2c33 372e 3534 4334  4.958 50,37.54C4
-00000520: 362e 3939 382c 3334 2e39 3538 2034 332e  6.998,34.958 43.
-00000530: 3431 312c 3333 2e31 3439 2033 392e 3535  411,33.149 39.55
-00000540: 2c33 322e 3237 4333 332e 3434 312c 3330  ,32.27C33.441,30
-00000550: 2e38 3533 2032 372e 3031 312c 3332 2e30  .853 27.011,32.0
-00000560: 3131 2032 312e 3738 2c33 352e 3437 4331  11 21.78,35.47C1
-00000570: 362e 3937 2c33 382e 3635 3220 3133 2e34  6.97,38.652 13.4
-00000580: 3839 2c34 332e 3438 3920 3132 2c34 392e  89,43.489 12,49.
-00000590: 3036 4c31 322c 3439 2e31 3343 3131 2e38  06L12,49.13C11.8
-000005a0: 322c 3439 2e37 3920 3131 2e36 362c 3530  2,49.79 11.66,50
-000005b0: 2e34 3620 3131 2e35 332c 3531 2e31 3343  .46 11.53,51.13C
-000005c0: 3131 2e31 3436 2c35 332e 3230 3720 3131  11.146,53.207 11
-000005d0: 2e30 3231 2c35 352e 3332 3320 3131 2e31  .021,55.323 11.1
-000005e0: 362c 3537 2e34 3343 3131 2e31 362c 3538  6,57.43C11.16,58
-000005f0: 2e30 3320 3131 2e32 362c 3538 2e36 3320  .03 11.26,58.63 
-00000600: 3131 2e33 342c 3539 2e32 3343 3131 2e33  11.34,59.23C11.3
-00000610: 342c 3539 2e35 3120 3131 2e34 332c 3539  4,59.51 11.43,59
-00000620: 2e37 3920 3131 2e34 382c 3630 2e30 3743  .79 11.48,60.07C
-00000630: 3131 2e35 332c 3630 2e33 3520 3131 2e35  11.53,60.35 11.5
-00000640: 382c 3630 2e36 3820 3131 2e36 342c 3630  8,60.68 11.64,60
-00000650: 2e39 3843 3131 2e37 2c36 312e 3238 2031  .98C11.7,61.28 1
-00000660: 312e 382c 3631 2e36 3920 3131 2e38 392c  1.8,61.69 11.89,
-00000670: 3632 2e30 3543 3131 2e39 382c 3632 2e34  62.05C11.98,62.4
-00000680: 3120 3131 2e39 392c 3632 2e34 3720 3132  1 11.99,62.47 12
-00000690: 2e30 352c 3632 2e36 3843 3132 2e31 362c  .05,62.68C12.16,
-000006a0: 3633 2e30 3720 3132 2e32 382c 3633 2e34  63.07 12.28,63.4
-000006b0: 3620 3132 2e34 312c 3633 2e38 344c 3132  6 12.41,63.84L12
-000006c0: 2e35 382c 3634 2e33 3443 3132 2e37 322c  .58,64.34C12.72,
-000006d0: 3634 2e37 3420 3132 2e38 382c 3635 2e31  64.74 12.88,65.1
-000006e0: 3420 3133 2e30 342c 3635 2e35 334c 3133  4 13.04,65.53L13
-000006f0: 2e32 332c 3635 2e39 3843 3133 2e34 3033  .23,65.98C13.403
-00000700: 2c36 362e 3337 3320 3133 2e35 3833 2c36  ,66.373 13.583,6
-00000710: 362e 3736 3720 3133 2e37 372c 3637 2e31  6.767 13.77,67.1
-00000720: 364c 3133 2e39 392c 3637 2e35 3943 3134  6L13.99,67.59C14
-00000730: 2e31 392c 3637 2e39 3720 3134 2e33 392c  .19,67.97 14.39,
-00000740: 3638 2e33 3520 3134 2e36 312c 3638 2e37  68.35 14.61,68.7
-00000750: 334c 3134 2e38 372c 3639 2e31 3543 3135  3L14.87,69.15C15
-00000760: 2e31 2c36 392e 3532 2031 352e 3333 2c36  .1,69.52 15.33,6
-00000770: 392e 3839 2031 352e 3538 2c37 302e 3236  9.89 15.58,70.26
-00000780: 4c31 352e 3538 2c37 302e 3332 4c31 352e  L15.58,70.32L15.
-00000790: 3939 2c37 302e 3933 4331 362e 3134 2c37  99,70.93C16.14,7
-000007a0: 312e 3134 2031 362e 3239 2c37 312e 3336  1.14 16.29,71.36
-000007b0: 2031 362e 3435 2c37 312e 3537 4332 302e   16.45,71.57C20.
-000007c0: 3230 362c 3735 2e38 3320 3235 2e30 3836  206,75.83 25.086
-000007d0: 2c37 382e 3935 2033 302e 3533 2c38 302e  ,78.95 30.53,80.
-000007e0: 3537 4333 362e 3833 392c 3832 2e34 3820  57C36.839,82.48 
-000007f0: 3433 2e34 312c 3833 2e33 3835 2035 302c  43.41,83.385 50,
-00000800: 3833 2e32 3543 3536 2e35 3939 2c38 332e  83.25C56.599,83.
-00000810: 3337 3420 3633 2e31 3737 2c38 322e 3435  374 63.177,82.45
-00000820: 3620 3639 2e34 392c 3830 2e35 3343 3734  6 69.49,80.53C74
-00000830: 2e36 3434 2c37 382e 3937 3820 3739 2e33  .644,78.978 79.3
-00000840: 3033 2c37 362e 3130 3220 3833 2c37 322e  03,76.102 83,72.
-00000850: 3139 4338 332e 3334 2c37 312e 3738 2038  19C83.34,71.78 8
-00000860: 332e 3635 2c37 312e 3335 2038 342c 3730  3.65,71.35 84,70
-00000870: 2e39 324c 3834 2e31 382c 3730 2e36 364c  .92L84.18,70.66L
-00000880: 3834 2e33 332c 3730 2e34 344c 3834 2e34  84.33,70.44L84.4
-00000890: 312c 3730 2e33 3243 3834 2e35 352c 3730  1,70.32C84.55,70
-000008a0: 2e31 3220 3834 2e36 372c 3639 2e39 2038  .12 84.67,69.9 8
-000008b0: 342e 3831 2c36 392e 3743 3835 2e30 372c  4.81,69.7C85.07,
-000008c0: 3639 2e33 2038 352e 3332 2c36 382e 3839  69.3 85.32,68.89
-000008d0: 2038 352e 3535 2c36 382e 3438 4338 352e   85.55,68.48C85.
-000008e0: 3738 2c36 382e 3037 2038 362e 3032 2c36  78,68.07 86.02,6
-000008f0: 372e 3635 2038 362e 3233 2c36 372e 3232  7.65 86.23,67.22
-00000900: 4338 362e 3331 2c36 372e 3035 2038 362e  C86.31,67.05 86.
-00000910: 3339 2c36 362e 3838 2038 362e 3437 2c36  39,66.88 86.47,6
-00000920: 362e 3743 3836 2e36 372c 3636 2e32 3820  6.7C86.67,66.28 
-00000930: 3836 2e38 352c 3635 2e38 3720 3837 2e30  86.85,65.87 87.0
-00000940: 332c 3635 2e34 344c 3837 2e32 332c 3634  3,65.44L87.23,64
-00000950: 2e39 3243 3837 2e33 3937 2c36 342e 3438  .92C87.397,64.48
-00000960: 3720 3837 2e35 352c 3634 2e30 3520 3837  7 87.55,64.05 87
-00000970: 2e36 392c 3633 2e36 314c 3837 2e38 352c  .69,63.61L87.85,
-00000980: 3633 2e30 3943 3837 2e39 382c 3632 2e36  63.09C87.98,62.6
-00000990: 3420 3838 2e31 2c36 322e 3139 2038 382e  4 88.1,62.19 88.
-000009a0: 3231 2c36 312e 3734 4338 382e 3231 2c36  21,61.74C88.21,6
-000009b0: 312e 3537 2038 382e 332c 3631 2e33 3920  1.57 88.3,61.39 
-000009c0: 3838 2e33 332c 3631 2e32 3243 3838 2e34  88.33,61.22C88.4
-000009d0: 332c 3630 2e37 3520 3838 2e35 322c 3630  3,60.75 88.52,60
-000009e0: 2e32 3220 3838 2e36 2c35 392e 3739 4338  .22 88.6,59.79C8
-000009f0: 382e 362c 3539 2e36 3420 3838 2e36 362c  8.6,59.64 88.66,
-00000a00: 3539 2e34 3920 3838 2e36 382c 3539 2e33  59.49 88.68,59.3
-00000a10: 3343 3838 2e37 372c 3538 2e37 3120 3838  3C88.77,58.71 88
-00000a20: 2e38 342c 3538 2e30 3820 3838 2e38 382c  .84,58.08 88.88,
-00000a30: 3537 2e34 354c 3838 2e38 382c 3534 2e31  57.45L88.88,54.1
-00000a40: 3743 3838 2e38 3137 2c35 332e 3136 3420  7C88.817,53.164 
-00000a50: 3838 2e36 3933 2c35 322e 3136 3220 3838  88.693,52.162 88
-00000a60: 2e35 312c 3531 2e31 3743 3838 2e33 382c  .51,51.17C88.38,
-00000a70: 3530 2e35 2038 382e 3233 2c34 392e 3834  50.5 88.23,49.84
-00000a80: 2038 382e 3035 2c34 392e 3137 4c38 382c   88.05,49.17L88,
-00000a90: 3439 2e30 355a 4d38 352e 3839 2c35 362e  49.05ZM85.89,56.
-00000aa0: 3434 4c38 352e 3839 2c35 372e 3233 4338  44L85.89,57.23C8
-00000ab0: 352e 3839 2c35 372e 3738 2038 352e 3739  5.89,57.78 85.79
-00000ac0: 2c35 382e 3332 2038 352e 3732 2c35 382e  ,58.32 85.72,58.
-00000ad0: 3836 4338 352e 3732 2c35 392e 3031 2038  86C85.72,59.01 8
-00000ae0: 352e 3732 2c35 392e 3135 2038 352e 3635  5.72,59.15 85.65
-00000af0: 2c35 392e 3343 3835 2e35 392c 3539 2e37  ,59.3C85.59,59.7
-00000b00: 2038 352e 3531 2c36 302e 3131 2038 352e   85.51,60.11 85.
-00000b10: 3433 2c36 302e 3531 4c38 352e 3332 2c36  43,60.51L85.32,6
-00000b20: 302e 3939 4338 352e 3233 2c36 312e 3338  0.99C85.23,61.38
-00000b30: 2038 352e 3132 2c36 312e 3737 2038 352e   85.12,61.77 85.
-00000b40: 3031 2c36 322e 3136 4338 352e 3031 2c36  01,62.16C85.01,6
-00000b50: 322e 3331 2038 342e 3933 2c36 322e 3436  2.31 84.93,62.46
-00000b60: 2038 342e 3838 2c36 322e 3643 3834 2e37   84.88,62.6C84.7
-00000b70: 342c 3633 2e30 3420 3834 2e35 392c 3633  4,63.04 84.59,63
-00000b80: 2e34 3720 3834 2e34 322c 3633 2e39 4c38  .47 84.42,63.9L8
-00000b90: 342e 3237 2c36 342e 3238 4338 342e 312c  4.27,64.28C84.1,
-00000ba0: 3634 2e37 3120 3833 2e39 312c 3635 2e31  64.71 83.91,65.1
-00000bb0: 3420 3833 2e37 312c 3635 2e35 3643 3833  4 83.71,65.56C83
-00000bc0: 2e35 312c 3635 2e39 3820 3833 2e34 332c  .51,65.98 83.43,
-00000bd0: 3636 2e31 3220 3833 2e32 382c 3636 2e34  66.12 83.28,66.4
-00000be0: 4c38 332e 3031 2c36 362e 3931 4338 322e  L83.01,66.91C82.
-00000bf0: 3833 2c36 372e 3232 3320 3832 2e36 3433  83,67.223 82.643
-00000c00: 2c36 372e 3533 3720 3832 2e34 352c 3637  ,67.537 82.45,67
-00000c10: 2e38 354c 3832 2e33 352c 3638 2e30 3143  .85L82.35,68.01C
-00000c20: 3739 2e31 3231 2c36 382e 3034 3720 3735  79.121,68.047 75
-00000c30: 2e39 3138 2c36 372e 3433 3420 3732 2e39  .918,67.434 72.9
-00000c40: 332c 3636 2e32 3143 3634 2e32 372c 3632  3,66.21C64.27,62
-00000c50: 2e37 3420 3539 2c35 352e 3532 2036 312e  .74 59,55.52 61.
-00000c60: 3138 2c35 302e 3131 4336 322e 3138 2c34  18,50.11C62.18,4
-00000c70: 372e 3620 3634 2e37 2c34 352e 3832 2036  7.6 64.7,45.82 6
-00000c80: 382e 3236 2c34 352e 3131 4337 322e 3438  8.26,45.11C72.48
-00000c90: 392c 3434 2e33 3935 2037 362e 3833 352c  9,44.395 76.835,
-00000ca0: 3434 2e39 3038 2038 302e 3738 2c34 362e  44.908 80.78,46.
-00000cb0: 3539 4338 322e 3134 312c 3437 2e31 3434  59C82.141,47.144
-00000cc0: 2038 332e 3435 332c 3437 2e38 3133 2038   83.453,47.813 8
-00000cd0: 342e 372c 3438 2e35 3943 3834 2e37 362c  4.7,48.59C84.76,
-00000ce0: 3438 2e37 3620 3834 2e38 322c 3438 2e39  48.76 84.82,48.9
-00000cf0: 3320 3834 2e38 382c 3439 2e31 4338 342e  3 84.88,49.1C84.
-00000d00: 3934 2c34 392e 3237 2038 352e 3035 2c34  94,49.27 85.05,4
-00000d10: 392e 3633 2038 352e 3132 2c34 392e 3943  9.63 85.12,49.9C
-00000d20: 3835 2e32 382c 3530 2e35 2038 352e 3434  85.28,50.5 85.44
-00000d30: 2c35 312e 3120 3835 2e35 352c 3531 2e37  ,51.1 85.55,51.7
-00000d40: 3343 3835 2e36 3931 2c35 322e 3530 3720  3C85.691,52.507 
-00000d50: 3835 2e37 3932 2c35 332e 3239 3220 3835  85.792,53.292 85
-00000d60: 2e38 352c 3534 2e30 384c 3835 2e38 352c  .85,54.08L85.85,
-00000d70: 3535 2e38 3943 3835 2e38 352c 3536 2e31  55.89C85.85,56.1
-00000d80: 3220 3835 2e39 312c 3536 2e32 3520 3835  2 85.91,56.25 85
-00000d90: 2e39 312c 3536 2e34 354c 3835 2e38 392c  .91,56.45L85.89,
-00000da0: 3536 2e34 345a 4d31 372e 3636 2c36 3843  56.44ZM17.66,68C
-00000db0: 3136 2e36 3638 2c36 362e 3433 3520 3135  16.668,66.435 15
-00000dc0: 2e38 3639 2c36 342e 3735 3620 3135 2e32  .869,64.756 15.2
-00000dd0: 382c 3633 4c31 352e 3137 2c36 322e 3638  8,63L15.17,62.68
-00000de0: 4331 352e 3036 2c36 322e 3335 2031 342e  C15.06,62.35 14.
-00000df0: 3936 2c36 322e 3031 2031 342e 3837 2c36  96,62.01 14.87,6
-00000e00: 312e 3638 4331 342e 3832 332c 3631 2e34  1.68C14.823,61.4
-00000e10: 3933 2031 342e 3737 372c 3631 2e33 3120  93 14.777,61.31 
-00000e20: 3134 2e37 332c 3631 2e31 3343 3134 2e36  14.73,61.13C14.6
-00000e30: 362c 3630 2e38 3420 3134 2e35 392c 3630  6,60.84 14.59,60
-00000e40: 2e35 3520 3134 2e35 332c 3630 2e32 3743  .55 14.53,60.27C
-00000e50: 3134 2e34 372c 3539 2e39 3920 3134 2e34  14.47,59.99 14.4
-00000e60: 332c 3539 2e37 3220 3134 2e33 382c 3539  3,59.72 14.38,59
-00000e70: 2e34 3443 3134 2e33 332c 3539 2e31 3620  .44C14.33,59.16 
-00000e80: 3134 2e33 2c35 3920 3134 2e32 372c 3538  14.3,59 14.27,58
-00000e90: 2e37 3843 3134 2e32 2c35 382e 3237 2031  .78C14.2,58.27 1
-00000ea0: 342e 3135 2c35 372e 3738 2031 342e 3131  4.15,57.78 14.11
-00000eb0: 2c35 372e 3233 4c31 342e 3131 2c35 372e  ,57.23L14.11,57.
-00000ec0: 3033 4331 342e 3030 382c 3535 2e32 3336  03C14.008,55.236
-00000ed0: 2031 342e 3132 322c 3533 2e34 3337 2031   14.122,53.437 1
-00000ee0: 342e 3435 2c35 312e 3637 4331 342e 3536  4.45,51.67C14.56
-00000ef0: 2c35 312e 3036 2031 342e 3731 2c35 302e  ,51.06 14.71,50.
-00000f00: 3436 2031 342e 3838 2c34 392e 3837 4331  46 14.88,49.87C1
-00000f10: 342e 3936 2c34 392e 3539 2031 352e 3034  4.96,49.59 15.04
-00000f20: 2c34 392e 3332 2031 352e 3133 2c34 392e  ,49.32 15.13,49.
-00000f30: 3035 4331 352e 3232 2c34 382e 3738 2031  05C15.22,48.78 1
-00000f40: 352e 3234 2c34 382e 3732 2031 352e 332c  5.24,48.72 15.3,
-00000f50: 3438 2e35 3543 3136 2e35 3438 2c34 372e  48.55C16.548,47.
-00000f60: 3737 3420 3137 2e38 3539 2c34 372e 3130  774 17.859,47.10
-00000f70: 3520 3139 2e32 322c 3436 2e35 3543 3237  5 19.22,46.55C27
-00000f80: 2e38 362c 3433 2e30 3920 3336 2e36 352c  .86,43.09 36.65,
-00000f90: 3434 2e36 3720 3338 2e38 322c 3530 2e30  44.67 38.82,50.0
-00000fa0: 3843 3430 2e39 392c 3535 2e34 3920 3335  8C40.99,55.49 35
-00000fb0: 2e37 332c 3632 2e37 3420 3237 2e30 392c  .73,62.74 27.09,
-00000fc0: 3636 2e32 4332 342e 3130 312c 3637 2e34  66.2C24.101,67.4
-00000fd0: 3331 2032 302e 3839 332c 3638 2e30 3433  31 20.893,68.043
-00000fe0: 2031 372e 3636 2c36 385a 4d36 382e 3537   17.66,68ZM68.57
-00000ff0: 2c37 372e 3638 4336 322e 3535 342c 3739  ,77.68C62.554,79
-00001000: 2e35 3038 2035 362e 3238 372c 3830 2e33  .508 56.287,80.3
-00001010: 3736 2035 302c 3830 2e32 3543 3433 2e37  76 50,80.25C43.7
-00001020: 3337 2c38 302e 3337 2033 372e 3439 352c  37,80.37 37.495,
-00001030: 3739 2e35 3036 2033 312e 352c 3737 2e36  79.506 31.5,77.6
-00001040: 3943 3237 2e31 3835 2c37 362e 3338 2032  9C27.185,76.38 2
-00001050: 332e 3234 332c 3734 2e30 3632 2032 302c  3.243,74.062 20,
-00001060: 3730 2e39 3343 3232 2e38 3135 2c37 302e  70.93C22.815,70.
-00001070: 3730 3620 3235 2e35 382c 3730 2e30 3535  706 25.58,70.055
-00001080: 2032 382e 322c 3639 4333 382e 3337 2c36   28.2,69C38.37,6
-00001090: 342e 3932 2034 342e 3339 2c35 3620 3431  4.92 44.39,56 41
-000010a0: 2e36 2c34 3943 3338 2e38 312c 3432 2032  .6,49C38.81,42 2
-000010b0: 382e 3237 2c33 392e 3732 2031 382e 312c  8.27,39.72 18.1,
-000010c0: 3433 2e38 4c31 372e 3433 2c34 342e 3039  43.8L17.43,44.09
-000010d0: 4331 382e 3937 332c 3431 2e36 3438 2032  C18.973,41.648 2
-000010e0: 312e 3031 392c 3339 2e35 3631 2032 332e  1.019,39.561 23.
-000010f0: 3433 2c33 372e 3937 4332 362e 3637 312c  43,37.97C26.671,
-00001100: 3335 2e38 3234 2033 302e 3437 332c 3334  35.824 30.473,34
-00001110: 2e36 3820 3334 2e33 362c 3334 2e36 3843  .68 34.36,34.68C
-00001120: 3335 2e38 3834 2c33 342e 3638 3120 3337  35.884,34.681 37
-00001130: 2e34 3034 2c33 342e 3835 3220 3338 2e38  .404,34.852 38.8
-00001140: 392c 3335 2e31 3943 3432 2e36 3934 2c33  9,35.19C42.694,3
-00001150: 362e 3034 3920 3436 2e31 3931 2c33 372e  6.049 46.191,37.
-00001160: 3933 3520 3439 2c34 302e 3634 4c35 302c  935 49,40.64L50,
-00001170: 3431 2e36 344c 3531 2c34 302e 3634 4335  41.64L51,40.64C5
-00001180: 332e 3739 372c 3337 2e39 3337 2035 372e  3.797,37.937 57.
-00001190: 3237 392c 3336 2e30 3439 2036 312e 3037  279,36.049 61.07
-000011a0: 2c33 352e 3138 4336 362e 3430 322c 3333  ,35.18C66.402,33
-000011b0: 2e39 3437 2037 322e 3031 342c 3334 2e39  .947 72.014,34.9
-000011c0: 3638 2037 362e 3537 2c33 3843 3738 2e39  68 76.57,38C78.9
-000011d0: 382c 3339 2e35 3838 2038 312e 3032 362c  8,39.588 81.026,
-000011e0: 3431 2e36 3731 2038 322e 3537 2c34 342e  41.671 82.57,44.
-000011f0: 3131 4c38 312e 392c 3433 2e38 3243 3737  11L81.9,43.82C77
-00001200: 2e34 3039 2c34 312e 3932 3120 3732 2e34  .409,41.921 72.4
-00001210: 3634 2c34 312e 3335 3520 3637 2e36 362c  64,41.355 67.66,
-00001220: 3432 2e31 3943 3633 2e30 382c 3433 2e31  42.19C63.08,43.1
-00001230: 3220 3539 2e37 392c 3435 2e35 3420 3538  2 59.79,45.54 58
-00001240: 2e33 392c 3439 2e30 3243 3535 2e36 2c35  .39,49.02C55.6,5
-00001250: 352e 3937 2036 312e 3632 2c36 342e 3934  5.97 61.62,64.94
-00001260: 2037 312e 3739 2c36 392e 3032 4337 342e   71.79,69.02C74.
-00001270: 3431 342c 3730 2e30 3720 3737 2e31 3832  414,70.07 77.182
-00001280: 2c37 302e 3731 3420 3830 2c37 302e 3933  ,70.714 80,70.93
-00001290: 4337 362e 3737 362c 3734 2e30 3520 3732  C76.776,74.05 72
-000012a0: 2e38 3539 2c37 362e 3336 3320 3638 2e35  .859,76.363 68.5
-000012b0: 372c 3737 2e36 385a 2220 7374 796c 653d  7,77.68Z" style=
-000012c0: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
-000012d0: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
-000012e0: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
-000012f0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00001300: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00001310: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-00001320: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-00001330: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
-00001340: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
-00001350: 7263 6c65 2063 783d 2237 312e 3333 2220  rcle cx="71.33" 
-00001360: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
-00001370: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
-00001380: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
-00001390: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-000013a0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-000013b0: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-000013c0: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-000013d0: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
-000013e0: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-000013f0: 2020 3c63 6972 636c 6520 6378 3d22 3238    <circle cx="28
-00001400: 2e36 3722 2063 793d 2235 3622 2072 3d22  .67" cy="56" r="
-00001410: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
-00001420: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
-00001430: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
-00001440: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
-00001450: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
-00001460: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
-00001470: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
-00001480: 362e 3638 3538 3229 223e 0a20 2020 2020  6.68582)">.     
-00001490: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
-000014a0: 4d35 382c 3636 4335 352e 3931 322c 3638  M58,66C55.912,68
-000014b0: 2e31 3631 2035 332e 3030 332c 3639 2e33  .161 53.003,69.3
-000014c0: 3339 2035 302c 3639 2e32 3443 3436 2e39  39 50,69.24C46.9
-000014d0: 3937 2c36 392e 3333 3920 3434 2e30 3838  97,69.339 44.088
-000014e0: 2c36 382e 3136 3120 3432 2c36 3643 3431  ,68.161 42,66C41
-000014f0: 2e37 3134 2c36 352e 3637 3720 3431 2e33  .714,65.677 41.3
-00001500: 3032 2c36 352e 3439 3120 3430 2e38 372c  02,65.491 40.87,
-00001510: 3635 2e34 3931 4334 302e 3034 322c 3635  65.491C40.042,65
-00001520: 2e34 3931 2033 392e 3336 312c 3636 2e31  .491 39.361,66.1
-00001530: 3732 2033 392e 3336 312c 3637 4333 392e  72 39.361,67C39.
-00001540: 3336 312c 3637 2e33 3638 2033 392e 3439  361,67.368 39.49
-00001550: 362c 3637 2e37 3234 2033 392e 3734 2c36  6,67.724 39.74,6
-00001560: 3843 3432 2e34 3033 2c37 302e 3830 3420  8C42.403,70.804 
-00001570: 3436 2e31 3334 2c37 322e 3335 2035 302c  46.134,72.35 50,
-00001580: 3732 2e32 3543 3533 2e38 3632 2c37 322e  72.25C53.862,72.
-00001590: 3334 3720 3537 2e35 392c 3730 2e38 3032  347 57.59,70.802
-000015a0: 2036 302e 3235 2c36 3843 3630 2e34 3935   60.25,68C60.495
-000015b0: 2c36 372e 3732 3520 3630 2e36 332c 3637  ,67.725 60.63,67
-000015c0: 2e33 3639 2036 302e 3633 2c36 3743 3630  .369 60.63,67C60
-000015d0: 2e36 332c 3636 2e31 3734 2035 392e 3935  .63,66.174 59.95
-000015e0: 312c 3635 2e34 3935 2035 392e 3132 352c  1,65.495 59.125,
-000015f0: 3635 2e34 3935 4335 382e 3639 352c 3635  65.495C58.695,65
-00001600: 2e34 3935 2035 382e 3238 352c 3635 2e36  .495 58.285,65.6
-00001610: 3739 2035 382c 3636 5a22 2073 7479 6c65  79 58,66Z" style
-00001620: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
-00001630: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
-00001640: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
-00001650: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
-00001660: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
+00000140: 2066 696c 6c3d 2223 3463 3122 2f3e 0a20   fill="#4c1"/>. 
+00000150: 2020 203c 2f67 3e0a 2020 2020 3c67 2066     </g>.    <g f
+00000160: 696c 6c3d 2223 6666 6622 2074 6578 742d  ill="#fff" text-
+00000170: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
+00000180: 666f 6e74 2d66 616d 696c 793d 2256 6572  font-family="Ver
+00000190: 6461 6e61 2c47 656e 6576 612c 4465 6a61  dana,Geneva,Deja
+000001a0: 5675 2053 616e 732c 7361 6e73 2d73 6572  Vu Sans,sans-ser
+000001b0: 6966 2220 7465 7874 2d72 656e 6465 7269  if" text-renderi
+000001c0: 6e67 3d22 6765 6f6d 6574 7269 6350 7265  ng="geometricPre
+000001d0: 6369 7369 6f6e 2220 666f 6e74 2d73 697a  cision" font-siz
+000001e0: 653d 2231 3130 223e 0a20 2020 2020 2020  e="110">.       
+000001f0: 203c 7465 7874 2078 3d22 3539 3022 2079   <text x="590" y
+00000200: 3d22 3134 3022 2074 7261 6e73 666f 726d  ="140" transform
+00000210: 3d22 7363 616c 6528 2e31 2922 2066 696c  ="scale(.1)" fil
+00000220: 6c3d 2223 6666 6622 2074 6578 744c 656e  l="#fff" textLen
+00000230: 6774 683d 2236 3130 223e 696e 7465 7272  gth="610">interr
+00000240: 6f67 6174 653c 2f74 6578 743e 0a20 2020  ogate</text>.   
+00000250: 2020 2020 203c 7465 7874 2078 3d22 3131       <text x="11
+00000260: 3630 2220 793d 2231 3430 2220 7472 616e  60" y="140" tran
+00000270: 7366 6f72 6d3d 2273 6361 6c65 282e 3129  sform="scale(.1)
+00000280: 2220 6669 6c6c 3d22 2366 6666 2220 7465  " fill="#fff" te
+00000290: 7874 4c65 6e67 7468 3d22 3337 3022 2064  xtLength="370" d
+000002a0: 6174 612d 696e 7465 7272 6f67 6174 653d  ata-interrogate=
+000002b0: 2272 6573 756c 7422 3e39 392e 3925 3c2f  "result">99.9%</
+000002c0: 7465 7874 3e0a 2020 2020 3c2f 673e 0a20  text>.    </g>. 
+000002d0: 2020 203c 6720 6964 3d22 6c6f 676f 2d70     <g id="logo-p
+000002e0: 696e 6b22 2074 7261 6e73 666f 726d 3d22  ink" transform="
+000002f0: 6d61 7472 6978 2830 2e38 3534 3837 362c  matrix(0.854876,
+00000300: 302c 302c 302e 3835 3438 3736 2c2d 362e  0,0,0.854876,-6.
+00000310: 3733 3531 342c 302e 3837 3731 3234 2922  73514,0.877124)"
+00000320: 3e0a 2020 2020 2020 2020 3c67 2074 7261  >.        <g tra
+00000330: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
+00000340: 2e32 3939 3031 322c 302c 302c 302e 3239  .299012,0,0,0.29
+00000350: 3930 3132 2c39 2e37 3032 3239 2c2d 362e  9012,9.70229,-6.
+00000360: 3638 3538 3229 223e 0a20 2020 2020 2020  68582)">.       
+00000370: 2020 2020 203c 7061 7468 2064 3d22 4d35       <path d="M5
+00000380: 302c 3634 2e32 3543 3532 2e37 362c 3634  0,64.25C52.76,64
+00000390: 2e32 3520 3535 2c36 312e 3133 2035 352c  .25 55,61.13 55,
+000003a0: 3539 2e37 3543 3535 2c35 382e 3337 2035  59.75C55,58.37 5
+000003b0: 322e 3736 2c35 372e 3235 2035 302c 3537  2.76,57.25 50,57
+000003c0: 2e32 3543 3437 2e32 342c 3537 2e32 3520  .25C47.24,57.25 
+000003d0: 3435 2c35 382e 3337 2034 352c 3539 2e37  45,58.37 45,59.7
+000003e0: 3543 3435 2c36 312e 3133 2034 372e 3234  5C45,61.13 47.24
+000003f0: 2c36 342e 3235 2035 302c 3634 2e32 355a  ,64.25 50,64.25Z
+00000400: 2220 7374 796c 653d 2266 696c 6c3a 7267  " style="fill:rg
+00000410: 6228 3232 322c 3132 302c 3136 3029 3b66  b(222,120,160);f
+00000420: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+00000430: 3b22 2f3e 0a20 2020 2020 2020 203c 2f67  ;"/>.        </g
+00000440: 3e0a 2020 2020 2020 2020 3c67 2074 7261  >.        <g tra
+00000450: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
+00000460: 2e32 3939 3031 322c 302c 302c 302e 3239  .299012,0,0,0.29
+00000470: 3930 3132 2c39 2e37 3032 3239 2c2d 362e  9012,9.70229,-6.
+00000480: 3638 3538 3229 223e 0a20 2020 2020 2020  68582)">.       
+00000490: 2020 2020 203c 7061 7468 2064 3d22 4d38       <path d="M8
+000004a0: 382c 3439 2e30 3543 3836 2e35 3036 2c34  8,49.05C86.506,4
+000004b0: 332e 3437 3520 3833 2e30 3138 2c33 382e  3.475 83.018,38.
+000004c0: 3633 3820 3738 2e32 2c33 352e 3436 4337  638 78.2,35.46C7
+000004d0: 322e 3936 392c 3332 2e30 3032 2036 362e  2.969,32.002 66.
+000004e0: 3533 392c 3330 2e38 3434 2036 302e 3433  539,30.844 60.43
+000004f0: 2c33 322e 3236 4335 362e 3537 362c 3333  ,32.26C56.576,33
+00000500: 2e31 3435 2035 322e 3939 352c 3334 2e39  .145 52.995,34.9
+00000510: 3538 2035 302c 3337 2e35 3443 3436 2e39  58 50,37.54C46.9
+00000520: 3938 2c33 342e 3935 3820 3433 2e34 3131  98,34.958 43.411
+00000530: 2c33 332e 3134 3920 3339 2e35 352c 3332  ,33.149 39.55,32
+00000540: 2e32 3743 3333 2e34 3431 2c33 302e 3835  .27C33.441,30.85
+00000550: 3320 3237 2e30 3131 2c33 322e 3031 3120  3 27.011,32.011 
+00000560: 3231 2e37 382c 3335 2e34 3743 3136 2e39  21.78,35.47C16.9
+00000570: 372c 3338 2e36 3532 2031 332e 3438 392c  7,38.652 13.489,
+00000580: 3433 2e34 3839 2031 322c 3439 2e30 364c  43.489 12,49.06L
+00000590: 3132 2c34 392e 3133 4331 312e 3832 2c34  12,49.13C11.82,4
+000005a0: 392e 3739 2031 312e 3636 2c35 302e 3436  9.79 11.66,50.46
+000005b0: 2031 312e 3533 2c35 312e 3133 4331 312e   11.53,51.13C11.
+000005c0: 3134 362c 3533 2e32 3037 2031 312e 3032  146,53.207 11.02
+000005d0: 312c 3535 2e33 3233 2031 312e 3136 2c35  1,55.323 11.16,5
+000005e0: 372e 3433 4331 312e 3136 2c35 382e 3033  7.43C11.16,58.03
+000005f0: 2031 312e 3236 2c35 382e 3633 2031 312e   11.26,58.63 11.
+00000600: 3334 2c35 392e 3233 4331 312e 3334 2c35  34,59.23C11.34,5
+00000610: 392e 3531 2031 312e 3433 2c35 392e 3739  9.51 11.43,59.79
+00000620: 2031 312e 3438 2c36 302e 3037 4331 312e   11.48,60.07C11.
+00000630: 3533 2c36 302e 3335 2031 312e 3538 2c36  53,60.35 11.58,6
+00000640: 302e 3638 2031 312e 3634 2c36 302e 3938  0.68 11.64,60.98
+00000650: 4331 312e 372c 3631 2e32 3820 3131 2e38  C11.7,61.28 11.8
+00000660: 2c36 312e 3639 2031 312e 3839 2c36 322e  ,61.69 11.89,62.
+00000670: 3035 4331 312e 3938 2c36 322e 3431 2031  05C11.98,62.41 1
+00000680: 312e 3939 2c36 322e 3437 2031 322e 3035  1.99,62.47 12.05
+00000690: 2c36 322e 3638 4331 322e 3136 2c36 332e  ,62.68C12.16,63.
+000006a0: 3037 2031 322e 3238 2c36 332e 3436 2031  07 12.28,63.46 1
+000006b0: 322e 3431 2c36 332e 3834 4c31 322e 3538  2.41,63.84L12.58
+000006c0: 2c36 342e 3334 4331 322e 3732 2c36 342e  ,64.34C12.72,64.
+000006d0: 3734 2031 322e 3838 2c36 352e 3134 2031  74 12.88,65.14 1
+000006e0: 332e 3034 2c36 352e 3533 4c31 332e 3233  3.04,65.53L13.23
+000006f0: 2c36 352e 3938 4331 332e 3430 332c 3636  ,65.98C13.403,66
+00000700: 2e33 3733 2031 332e 3538 332c 3636 2e37  .373 13.583,66.7
+00000710: 3637 2031 332e 3737 2c36 372e 3136 4c31  67 13.77,67.16L1
+00000720: 332e 3939 2c36 372e 3539 4331 342e 3139  3.99,67.59C14.19
+00000730: 2c36 372e 3937 2031 342e 3339 2c36 382e  ,67.97 14.39,68.
+00000740: 3335 2031 342e 3631 2c36 382e 3733 4c31  35 14.61,68.73L1
+00000750: 342e 3837 2c36 392e 3135 4331 352e 312c  4.87,69.15C15.1,
+00000760: 3639 2e35 3220 3135 2e33 332c 3639 2e38  69.52 15.33,69.8
+00000770: 3920 3135 2e35 382c 3730 2e32 364c 3135  9 15.58,70.26L15
+00000780: 2e35 382c 3730 2e33 324c 3135 2e39 392c  .58,70.32L15.99,
+00000790: 3730 2e39 3343 3136 2e31 342c 3731 2e31  70.93C16.14,71.1
+000007a0: 3420 3136 2e32 392c 3731 2e33 3620 3136  4 16.29,71.36 16
+000007b0: 2e34 352c 3731 2e35 3743 3230 2e32 3036  .45,71.57C20.206
+000007c0: 2c37 352e 3833 2032 352e 3038 362c 3738  ,75.83 25.086,78
+000007d0: 2e39 3520 3330 2e35 332c 3830 2e35 3743  .95 30.53,80.57C
+000007e0: 3336 2e38 3339 2c38 322e 3438 2034 332e  36.839,82.48 43.
+000007f0: 3431 2c38 332e 3338 3520 3530 2c38 332e  41,83.385 50,83.
+00000800: 3235 4335 362e 3539 392c 3833 2e33 3734  25C56.599,83.374
+00000810: 2036 332e 3137 372c 3832 2e34 3536 2036   63.177,82.456 6
+00000820: 392e 3439 2c38 302e 3533 4337 342e 3634  9.49,80.53C74.64
+00000830: 342c 3738 2e39 3738 2037 392e 3330 332c  4,78.978 79.303,
+00000840: 3736 2e31 3032 2038 332c 3732 2e31 3943  76.102 83,72.19C
+00000850: 3833 2e33 342c 3731 2e37 3820 3833 2e36  83.34,71.78 83.6
+00000860: 352c 3731 2e33 3520 3834 2c37 302e 3932  5,71.35 84,70.92
+00000870: 4c38 342e 3138 2c37 302e 3636 4c38 342e  L84.18,70.66L84.
+00000880: 3333 2c37 302e 3434 4c38 342e 3431 2c37  33,70.44L84.41,7
+00000890: 302e 3332 4338 342e 3535 2c37 302e 3132  0.32C84.55,70.12
+000008a0: 2038 342e 3637 2c36 392e 3920 3834 2e38   84.67,69.9 84.8
+000008b0: 312c 3639 2e37 4338 352e 3037 2c36 392e  1,69.7C85.07,69.
+000008c0: 3320 3835 2e33 322c 3638 2e38 3920 3835  3 85.32,68.89 85
+000008d0: 2e35 352c 3638 2e34 3843 3835 2e37 382c  .55,68.48C85.78,
+000008e0: 3638 2e30 3720 3836 2e30 322c 3637 2e36  68.07 86.02,67.6
+000008f0: 3520 3836 2e32 332c 3637 2e32 3243 3836  5 86.23,67.22C86
+00000900: 2e33 312c 3637 2e30 3520 3836 2e33 392c  .31,67.05 86.39,
+00000910: 3636 2e38 3820 3836 2e34 372c 3636 2e37  66.88 86.47,66.7
+00000920: 4338 362e 3637 2c36 362e 3238 2038 362e  C86.67,66.28 86.
+00000930: 3835 2c36 352e 3837 2038 372e 3033 2c36  85,65.87 87.03,6
+00000940: 352e 3434 4c38 372e 3233 2c36 342e 3932  5.44L87.23,64.92
+00000950: 4338 372e 3339 372c 3634 2e34 3837 2038  C87.397,64.487 8
+00000960: 372e 3535 2c36 342e 3035 2038 372e 3639  7.55,64.05 87.69
+00000970: 2c36 332e 3631 4c38 372e 3835 2c36 332e  ,63.61L87.85,63.
+00000980: 3039 4338 372e 3938 2c36 322e 3634 2038  09C87.98,62.64 8
+00000990: 382e 312c 3632 2e31 3920 3838 2e32 312c  8.1,62.19 88.21,
+000009a0: 3631 2e37 3443 3838 2e32 312c 3631 2e35  61.74C88.21,61.5
+000009b0: 3720 3838 2e33 2c36 312e 3339 2038 382e  7 88.3,61.39 88.
+000009c0: 3333 2c36 312e 3232 4338 382e 3433 2c36  33,61.22C88.43,6
+000009d0: 302e 3735 2038 382e 3532 2c36 302e 3232  0.75 88.52,60.22
+000009e0: 2038 382e 362c 3539 2e37 3943 3838 2e36   88.6,59.79C88.6
+000009f0: 2c35 392e 3634 2038 382e 3636 2c35 392e  ,59.64 88.66,59.
+00000a00: 3439 2038 382e 3638 2c35 392e 3333 4338  49 88.68,59.33C8
+00000a10: 382e 3737 2c35 382e 3731 2038 382e 3834  8.77,58.71 88.84
+00000a20: 2c35 382e 3038 2038 382e 3838 2c35 372e  ,58.08 88.88,57.
+00000a30: 3435 4c38 382e 3838 2c35 342e 3137 4338  45L88.88,54.17C8
+00000a40: 382e 3831 372c 3533 2e31 3634 2038 382e  8.817,53.164 88.
+00000a50: 3639 332c 3532 2e31 3632 2038 382e 3531  693,52.162 88.51
+00000a60: 2c35 312e 3137 4338 382e 3338 2c35 302e  ,51.17C88.38,50.
+00000a70: 3520 3838 2e32 332c 3439 2e38 3420 3838  5 88.23,49.84 88
+00000a80: 2e30 352c 3439 2e31 374c 3838 2c34 392e  .05,49.17L88,49.
+00000a90: 3035 5a4d 3835 2e38 392c 3536 2e34 344c  05ZM85.89,56.44L
+00000aa0: 3835 2e38 392c 3537 2e32 3343 3835 2e38  85.89,57.23C85.8
+00000ab0: 392c 3537 2e37 3820 3835 2e37 392c 3538  9,57.78 85.79,58
+00000ac0: 2e33 3220 3835 2e37 322c 3538 2e38 3643  .32 85.72,58.86C
+00000ad0: 3835 2e37 322c 3539 2e30 3120 3835 2e37  85.72,59.01 85.7
+00000ae0: 322c 3539 2e31 3520 3835 2e36 352c 3539  2,59.15 85.65,59
+00000af0: 2e33 4338 352e 3539 2c35 392e 3720 3835  .3C85.59,59.7 85
+00000b00: 2e35 312c 3630 2e31 3120 3835 2e34 332c  .51,60.11 85.43,
+00000b10: 3630 2e35 314c 3835 2e33 322c 3630 2e39  60.51L85.32,60.9
+00000b20: 3943 3835 2e32 332c 3631 2e33 3820 3835  9C85.23,61.38 85
+00000b30: 2e31 322c 3631 2e37 3720 3835 2e30 312c  .12,61.77 85.01,
+00000b40: 3632 2e31 3643 3835 2e30 312c 3632 2e33  62.16C85.01,62.3
+00000b50: 3120 3834 2e39 332c 3632 2e34 3620 3834  1 84.93,62.46 84
+00000b60: 2e38 382c 3632 2e36 4338 342e 3734 2c36  .88,62.6C84.74,6
+00000b70: 332e 3034 2038 342e 3539 2c36 332e 3437  3.04 84.59,63.47
+00000b80: 2038 342e 3432 2c36 332e 394c 3834 2e32   84.42,63.9L84.2
+00000b90: 372c 3634 2e32 3843 3834 2e31 2c36 342e  7,64.28C84.1,64.
+00000ba0: 3731 2038 332e 3931 2c36 352e 3134 2038  71 83.91,65.14 8
+00000bb0: 332e 3731 2c36 352e 3536 4338 332e 3531  3.71,65.56C83.51
+00000bc0: 2c36 352e 3938 2038 332e 3433 2c36 362e  ,65.98 83.43,66.
+00000bd0: 3132 2038 332e 3238 2c36 362e 344c 3833  12 83.28,66.4L83
+00000be0: 2e30 312c 3636 2e39 3143 3832 2e38 332c  .01,66.91C82.83,
+00000bf0: 3637 2e32 3233 2038 322e 3634 332c 3637  67.223 82.643,67
+00000c00: 2e35 3337 2038 322e 3435 2c36 372e 3835  .537 82.45,67.85
+00000c10: 4c38 322e 3335 2c36 382e 3031 4337 392e  L82.35,68.01C79.
+00000c20: 3132 312c 3638 2e30 3437 2037 352e 3931  121,68.047 75.91
+00000c30: 382c 3637 2e34 3334 2037 322e 3933 2c36  8,67.434 72.93,6
+00000c40: 362e 3231 4336 342e 3237 2c36 322e 3734  6.21C64.27,62.74
+00000c50: 2035 392c 3535 2e35 3220 3631 2e31 382c   59,55.52 61.18,
+00000c60: 3530 2e31 3143 3632 2e31 382c 3437 2e36  50.11C62.18,47.6
+00000c70: 2036 342e 372c 3435 2e38 3220 3638 2e32   64.7,45.82 68.2
+00000c80: 362c 3435 2e31 3143 3732 2e34 3839 2c34  6,45.11C72.489,4
+00000c90: 342e 3339 3520 3736 2e38 3335 2c34 342e  4.395 76.835,44.
+00000ca0: 3930 3820 3830 2e37 382c 3436 2e35 3943  908 80.78,46.59C
+00000cb0: 3832 2e31 3431 2c34 372e 3134 3420 3833  82.141,47.144 83
+00000cc0: 2e34 3533 2c34 372e 3831 3320 3834 2e37  .453,47.813 84.7
+00000cd0: 2c34 382e 3539 4338 342e 3736 2c34 382e  ,48.59C84.76,48.
+00000ce0: 3736 2038 342e 3832 2c34 382e 3933 2038  76 84.82,48.93 8
+00000cf0: 342e 3838 2c34 392e 3143 3834 2e39 342c  4.88,49.1C84.94,
+00000d00: 3439 2e32 3720 3835 2e30 352c 3439 2e36  49.27 85.05,49.6
+00000d10: 3320 3835 2e31 322c 3439 2e39 4338 352e  3 85.12,49.9C85.
+00000d20: 3238 2c35 302e 3520 3835 2e34 342c 3531  28,50.5 85.44,51
+00000d30: 2e31 2038 352e 3535 2c35 312e 3733 4338  .1 85.55,51.73C8
+00000d40: 352e 3639 312c 3532 2e35 3037 2038 352e  5.691,52.507 85.
+00000d50: 3739 322c 3533 2e32 3932 2038 352e 3835  792,53.292 85.85
+00000d60: 2c35 342e 3038 4c38 352e 3835 2c35 352e  ,54.08L85.85,55.
+00000d70: 3839 4338 352e 3835 2c35 362e 3132 2038  89C85.85,56.12 8
+00000d80: 352e 3931 2c35 362e 3235 2038 352e 3931  5.91,56.25 85.91
+00000d90: 2c35 362e 3435 4c38 352e 3839 2c35 362e  ,56.45L85.89,56.
+00000da0: 3434 5a4d 3137 2e36 362c 3638 4331 362e  44ZM17.66,68C16.
+00000db0: 3636 382c 3636 2e34 3335 2031 352e 3836  668,66.435 15.86
+00000dc0: 392c 3634 2e37 3536 2031 352e 3238 2c36  9,64.756 15.28,6
+00000dd0: 334c 3135 2e31 372c 3632 2e36 3843 3135  3L15.17,62.68C15
+00000de0: 2e30 362c 3632 2e33 3520 3134 2e39 362c  .06,62.35 14.96,
+00000df0: 3632 2e30 3120 3134 2e38 372c 3631 2e36  62.01 14.87,61.6
+00000e00: 3843 3134 2e38 3233 2c36 312e 3439 3320  8C14.823,61.493 
+00000e10: 3134 2e37 3737 2c36 312e 3331 2031 342e  14.777,61.31 14.
+00000e20: 3733 2c36 312e 3133 4331 342e 3636 2c36  73,61.13C14.66,6
+00000e30: 302e 3834 2031 342e 3539 2c36 302e 3535  0.84 14.59,60.55
+00000e40: 2031 342e 3533 2c36 302e 3237 4331 342e   14.53,60.27C14.
+00000e50: 3437 2c35 392e 3939 2031 342e 3433 2c35  47,59.99 14.43,5
+00000e60: 392e 3732 2031 342e 3338 2c35 392e 3434  9.72 14.38,59.44
+00000e70: 4331 342e 3333 2c35 392e 3136 2031 342e  C14.33,59.16 14.
+00000e80: 332c 3539 2031 342e 3237 2c35 382e 3738  3,59 14.27,58.78
+00000e90: 4331 342e 322c 3538 2e32 3720 3134 2e31  C14.2,58.27 14.1
+00000ea0: 352c 3537 2e37 3820 3134 2e31 312c 3537  5,57.78 14.11,57
+00000eb0: 2e32 334c 3134 2e31 312c 3537 2e30 3343  .23L14.11,57.03C
+00000ec0: 3134 2e30 3038 2c35 352e 3233 3620 3134  14.008,55.236 14
+00000ed0: 2e31 3232 2c35 332e 3433 3720 3134 2e34  .122,53.437 14.4
+00000ee0: 352c 3531 2e36 3743 3134 2e35 362c 3531  5,51.67C14.56,51
+00000ef0: 2e30 3620 3134 2e37 312c 3530 2e34 3620  .06 14.71,50.46 
+00000f00: 3134 2e38 382c 3439 2e38 3743 3134 2e39  14.88,49.87C14.9
+00000f10: 362c 3439 2e35 3920 3135 2e30 342c 3439  6,49.59 15.04,49
+00000f20: 2e33 3220 3135 2e31 332c 3439 2e30 3543  .32 15.13,49.05C
+00000f30: 3135 2e32 322c 3438 2e37 3820 3135 2e32  15.22,48.78 15.2
+00000f40: 342c 3438 2e37 3220 3135 2e33 2c34 382e  4,48.72 15.3,48.
+00000f50: 3535 4331 362e 3534 382c 3437 2e37 3734  55C16.548,47.774
+00000f60: 2031 372e 3835 392c 3437 2e31 3035 2031   17.859,47.105 1
+00000f70: 392e 3232 2c34 362e 3535 4332 372e 3836  9.22,46.55C27.86
+00000f80: 2c34 332e 3039 2033 362e 3635 2c34 342e  ,43.09 36.65,44.
+00000f90: 3637 2033 382e 3832 2c35 302e 3038 4334  67 38.82,50.08C4
+00000fa0: 302e 3939 2c35 352e 3439 2033 352e 3733  0.99,55.49 35.73
+00000fb0: 2c36 322e 3734 2032 372e 3039 2c36 362e  ,62.74 27.09,66.
+00000fc0: 3243 3234 2e31 3031 2c36 372e 3433 3120  2C24.101,67.431 
+00000fd0: 3230 2e38 3933 2c36 382e 3034 3320 3137  20.893,68.043 17
+00000fe0: 2e36 362c 3638 5a4d 3638 2e35 372c 3737  .66,68ZM68.57,77
+00000ff0: 2e36 3843 3632 2e35 3534 2c37 392e 3530  .68C62.554,79.50
+00001000: 3820 3536 2e32 3837 2c38 302e 3337 3620  8 56.287,80.376 
+00001010: 3530 2c38 302e 3235 4334 332e 3733 372c  50,80.25C43.737,
+00001020: 3830 2e33 3720 3337 2e34 3935 2c37 392e  80.37 37.495,79.
+00001030: 3530 3620 3331 2e35 2c37 372e 3639 4332  506 31.5,77.69C2
+00001040: 372e 3138 352c 3736 2e33 3820 3233 2e32  7.185,76.38 23.2
+00001050: 3433 2c37 342e 3036 3220 3230 2c37 302e  43,74.062 20,70.
+00001060: 3933 4332 322e 3831 352c 3730 2e37 3036  93C22.815,70.706
+00001070: 2032 352e 3538 2c37 302e 3035 3520 3238   25.58,70.055 28
+00001080: 2e32 2c36 3943 3338 2e33 372c 3634 2e39  .2,69C38.37,64.9
+00001090: 3220 3434 2e33 392c 3536 2034 312e 362c  2 44.39,56 41.6,
+000010a0: 3439 4333 382e 3831 2c34 3220 3238 2e32  49C38.81,42 28.2
+000010b0: 372c 3339 2e37 3220 3138 2e31 2c34 332e  7,39.72 18.1,43.
+000010c0: 384c 3137 2e34 332c 3434 2e30 3943 3138  8L17.43,44.09C18
+000010d0: 2e39 3733 2c34 312e 3634 3820 3231 2e30  .973,41.648 21.0
+000010e0: 3139 2c33 392e 3536 3120 3233 2e34 332c  19,39.561 23.43,
+000010f0: 3337 2e39 3743 3236 2e36 3731 2c33 352e  37.97C26.671,35.
+00001100: 3832 3420 3330 2e34 3733 2c33 342e 3638  824 30.473,34.68
+00001110: 2033 342e 3336 2c33 342e 3638 4333 352e   34.36,34.68C35.
+00001120: 3838 342c 3334 2e36 3831 2033 372e 3430  884,34.681 37.40
+00001130: 342c 3334 2e38 3532 2033 382e 3839 2c33  4,34.852 38.89,3
+00001140: 352e 3139 4334 322e 3639 342c 3336 2e30  5.19C42.694,36.0
+00001150: 3439 2034 362e 3139 312c 3337 2e39 3335  49 46.191,37.935
+00001160: 2034 392c 3430 2e36 344c 3530 2c34 312e   49,40.64L50,41.
+00001170: 3634 4c35 312c 3430 2e36 3443 3533 2e37  64L51,40.64C53.7
+00001180: 3937 2c33 372e 3933 3720 3537 2e32 3739  97,37.937 57.279
+00001190: 2c33 362e 3034 3920 3631 2e30 372c 3335  ,36.049 61.07,35
+000011a0: 2e31 3843 3636 2e34 3032 2c33 332e 3934  .18C66.402,33.94
+000011b0: 3720 3732 2e30 3134 2c33 342e 3936 3820  7 72.014,34.968 
+000011c0: 3736 2e35 372c 3338 4337 382e 3938 2c33  76.57,38C78.98,3
+000011d0: 392e 3538 3820 3831 2e30 3236 2c34 312e  9.588 81.026,41.
+000011e0: 3637 3120 3832 2e35 372c 3434 2e31 314c  671 82.57,44.11L
+000011f0: 3831 2e39 2c34 332e 3832 4337 372e 3430  81.9,43.82C77.40
+00001200: 392c 3431 2e39 3231 2037 322e 3436 342c  9,41.921 72.464,
+00001210: 3431 2e33 3535 2036 372e 3636 2c34 322e  41.355 67.66,42.
+00001220: 3139 4336 332e 3038 2c34 332e 3132 2035  19C63.08,43.12 5
+00001230: 392e 3739 2c34 352e 3534 2035 382e 3339  9.79,45.54 58.39
+00001240: 2c34 392e 3032 4335 352e 362c 3535 2e39  ,49.02C55.6,55.9
+00001250: 3720 3631 2e36 322c 3634 2e39 3420 3731  7 61.62,64.94 71
+00001260: 2e37 392c 3639 2e30 3243 3734 2e34 3134  .79,69.02C74.414
+00001270: 2c37 302e 3037 2037 372e 3138 322c 3730  ,70.07 77.182,70
+00001280: 2e37 3134 2038 302c 3730 2e39 3343 3736  .714 80,70.93C76
+00001290: 2e37 3736 2c37 342e 3035 2037 322e 3835  .776,74.05 72.85
+000012a0: 392c 3736 2e33 3633 2036 382e 3537 2c37  9,76.363 68.57,7
+000012b0: 372e 3638 5a22 2073 7479 6c65 3d22 6669  7.68Z" style="fi
+000012c0: 6c6c 3a72 6762 2832 3232 2c31 3230 2c31  ll:rgb(222,120,1
+000012d0: 3630 293b 6669 6c6c 2d72 756c 653a 6e6f  60);fill-rule:no
+000012e0: 6e7a 6572 6f3b 222f 3e0a 2020 2020 2020  nzero;"/>.      
+000012f0: 2020 3c2f 673e 0a20 2020 2020 2020 203c    </g>.        <
+00001300: 6720 7472 616e 7366 6f72 6d3d 226d 6174  g transform="mat
+00001310: 7269 7828 302e 3239 3930 3132 2c30 2c30  rix(0.299012,0,0
+00001320: 2c30 2e32 3939 3031 322c 392e 3730 3232  ,0.299012,9.7022
+00001330: 392c 2d36 2e36 3835 3832 2922 3e0a 2020  9,-6.68582)">.  
+00001340: 2020 2020 2020 2020 2020 3c63 6972 636c            <circl
+00001350: 6520 6378 3d22 3731 2e33 3322 2063 793d  e cx="71.33" cy=
+00001360: 2235 3622 2072 3d22 352e 3136 2220 7374  "56" r="5.16" st
+00001370: 796c 653d 2266 696c 6c3a 7267 6228 3232  yle="fill:rgb(22
+00001380: 322c 3132 302c 3136 3029 3b22 2f3e 0a20  2,120,160);"/>. 
+00001390: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
+000013a0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+000013b0: 3d22 6d61 7472 6978 2830 2e32 3939 3031  ="matrix(0.29901
+000013c0: 322c 302c 302c 302e 3239 3930 3132 2c39  2,0,0,0.299012,9
+000013d0: 2e37 3032 3239 2c2d 362e 3638 3538 3229  .70229,-6.68582)
+000013e0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+000013f0: 6369 7263 6c65 2063 783d 2232 382e 3637  circle cx="28.67
+00001400: 2220 6379 3d22 3536 2220 723d 2235 2e31  " cy="56" r="5.1
+00001410: 3622 2073 7479 6c65 3d22 6669 6c6c 3a72  6" style="fill:r
+00001420: 6762 2832 3232 2c31 3230 2c31 3630 293b  gb(222,120,160);
+00001430: 222f 3e0a 2020 2020 2020 2020 3c2f 673e  "/>.        </g>
+00001440: 0a20 2020 2020 2020 203c 6720 7472 616e  .        <g tran
+00001450: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
+00001460: 3239 3930 3132 2c30 2c30 2c30 2e32 3939  299012,0,0,0.299
+00001470: 3031 322c 392e 3730 3232 392c 2d36 2e36  012,9.70229,-6.6
+00001480: 3835 3832 2922 3e0a 2020 2020 2020 2020  8582)">.        
+00001490: 2020 2020 3c70 6174 6820 643d 224d 3538      <path d="M58
+000014a0: 2c36 3643 3535 2e39 3132 2c36 382e 3136  ,66C55.912,68.16
+000014b0: 3120 3533 2e30 3033 2c36 392e 3333 3920  1 53.003,69.339 
+000014c0: 3530 2c36 392e 3234 4334 362e 3939 372c  50,69.24C46.997,
+000014d0: 3639 2e33 3339 2034 342e 3038 382c 3638  69.339 44.088,68
+000014e0: 2e31 3631 2034 322c 3636 4334 312e 3731  .161 42,66C41.71
+000014f0: 342c 3635 2e36 3737 2034 312e 3330 322c  4,65.677 41.302,
+00001500: 3635 2e34 3931 2034 302e 3837 2c36 352e  65.491 40.87,65.
+00001510: 3439 3143 3430 2e30 3432 2c36 352e 3439  491C40.042,65.49
+00001520: 3120 3339 2e33 3631 2c36 362e 3137 3220  1 39.361,66.172 
+00001530: 3339 2e33 3631 2c36 3743 3339 2e33 3631  39.361,67C39.361
+00001540: 2c36 372e 3336 3820 3339 2e34 3936 2c36  ,67.368 39.496,6
+00001550: 372e 3732 3420 3339 2e37 342c 3638 4334  7.724 39.74,68C4
+00001560: 322e 3430 332c 3730 2e38 3034 2034 362e  2.403,70.804 46.
+00001570: 3133 342c 3732 2e33 3520 3530 2c37 322e  134,72.35 50,72.
+00001580: 3235 4335 332e 3836 322c 3732 2e33 3437  25C53.862,72.347
+00001590: 2035 372e 3539 2c37 302e 3830 3220 3630   57.59,70.802 60
+000015a0: 2e32 352c 3638 4336 302e 3439 352c 3637  .25,68C60.495,67
+000015b0: 2e37 3235 2036 302e 3633 2c36 372e 3336  .725 60.63,67.36
+000015c0: 3920 3630 2e36 332c 3637 4336 302e 3633  9 60.63,67C60.63
+000015d0: 2c36 362e 3137 3420 3539 2e39 3531 2c36  ,66.174 59.951,6
+000015e0: 352e 3439 3520 3539 2e31 3235 2c36 352e  5.495 59.125,65.
+000015f0: 3439 3543 3538 2e36 3935 2c36 352e 3439  495C58.695,65.49
+00001600: 3520 3538 2e32 3835 2c36 352e 3637 3920  5 58.285,65.679 
+00001610: 3538 2c36 365a 2220 7374 796c 653d 2266  58,66Z" style="f
+00001620: 696c 6c3a 7267 6228 3232 322c 3132 302c  ill:rgb(222,120,
+00001630: 3136 3029 3b66 696c 6c2d 7275 6c65 3a6e  160);fill-rule:n
+00001640: 6f6e 7a65 726f 3b22 2f3e 0a20 2020 2020  onzero;"/>.     
+00001650: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
+00001660: 0a3c 2f73 7667 3e0a                      .</svg>.
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/99.png` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square/default.svg`

 * *Files 2% similar despite different names*

```diff
@@ -1,359 +1,359 @@
 00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3134 3022 2068  k" width="140" h
+00000050: 6b22 2077 6964 7468 3d22 3133 3222 2068  k" width="132" h
 00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 696e 7465 7272 6f67 6174 653a 2039  ="interrogate: 9
-00000090: 392e 3925 223e 0a20 2020 203c 7469 746c  9.9%">.    <titl
-000000a0: 653e 696e 7465 7272 6f67 6174 653a 2039  e>interrogate: 9
-000000b0: 392e 3925 3c2f 7469 746c 653e 0a20 2020  9.9%</title>.   
+00000080: 3d22 696e 7465 7272 6f67 6174 653a 202d  ="interrogate: -
+00000090: 312e 3025 223e 0a20 2020 203c 7469 746c  1.0%">.    <titl
+000000a0: 653e 696e 7465 7272 6f67 6174 653a 202d  e>interrogate: -
+000000b0: 312e 3025 3c2f 7469 746c 653e 0a20 2020  1.0%</title>.   
 000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
 000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
 000000f0: 7769 6474 683d 2239 3322 2068 6569 6768  width="93" heigh
 00000100: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
 00000110: 3522 2f3e 0a20 2020 2020 2020 203c 7265  5"/>.        <re
 00000120: 6374 2078 3d22 3933 2220 7769 6474 683d  ct x="93" width=
-00000130: 2234 3722 2068 6569 6768 743d 2232 3022  "47" height="20"
-00000140: 2066 696c 6c3d 2223 3463 3122 2f3e 0a20   fill="#4c1"/>. 
-00000150: 2020 203c 2f67 3e0a 2020 2020 3c67 2066     </g>.    <g f
-00000160: 696c 6c3d 2223 6666 6622 2074 6578 742d  ill="#fff" text-
-00000170: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
-00000180: 666f 6e74 2d66 616d 696c 793d 2256 6572  font-family="Ver
-00000190: 6461 6e61 2c47 656e 6576 612c 4465 6a61  dana,Geneva,Deja
-000001a0: 5675 2053 616e 732c 7361 6e73 2d73 6572  Vu Sans,sans-ser
-000001b0: 6966 2220 7465 7874 2d72 656e 6465 7269  if" text-renderi
-000001c0: 6e67 3d22 6765 6f6d 6574 7269 6350 7265  ng="geometricPre
-000001d0: 6369 7369 6f6e 2220 666f 6e74 2d73 697a  cision" font-siz
-000001e0: 653d 2231 3130 223e 0a20 2020 2020 2020  e="110">.       
-000001f0: 203c 7465 7874 2078 3d22 3539 3022 2079   <text x="590" y
-00000200: 3d22 3134 3022 2074 7261 6e73 666f 726d  ="140" transform
-00000210: 3d22 7363 616c 6528 2e31 2922 2066 696c  ="scale(.1)" fil
-00000220: 6c3d 2223 6666 6622 2074 6578 744c 656e  l="#fff" textLen
-00000230: 6774 683d 2236 3130 223e 696e 7465 7272  gth="610">interr
-00000240: 6f67 6174 653c 2f74 6578 743e 0a20 2020  ogate</text>.   
-00000250: 2020 2020 203c 7465 7874 2078 3d22 3131       <text x="11
-00000260: 3630 2220 793d 2231 3430 2220 7472 616e  60" y="140" tran
-00000270: 7366 6f72 6d3d 2273 6361 6c65 282e 3129  sform="scale(.1)
-00000280: 2220 6669 6c6c 3d22 2366 6666 2220 7465  " fill="#fff" te
-00000290: 7874 4c65 6e67 7468 3d22 3337 3022 2064  xtLength="370" d
-000002a0: 6174 612d 696e 7465 7272 6f67 6174 653d  ata-interrogate=
-000002b0: 2272 6573 756c 7422 3e39 392e 3925 3c2f  "result">99.9%</
-000002c0: 7465 7874 3e0a 2020 2020 3c2f 673e 0a20  text>.    </g>. 
-000002d0: 2020 203c 6720 6964 3d22 6c6f 676f 2d70     <g id="logo-p
-000002e0: 696e 6b22 2074 7261 6e73 666f 726d 3d22  ink" transform="
-000002f0: 6d61 7472 6978 2830 2e38 3534 3837 362c  matrix(0.854876,
-00000300: 302c 302c 302e 3835 3438 3736 2c2d 362e  0,0,0.854876,-6.
-00000310: 3733 3531 342c 302e 3837 3731 3234 2922  73514,0.877124)"
-00000320: 3e0a 2020 2020 2020 2020 3c67 2074 7261  >.        <g tra
-00000330: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
-00000340: 2e32 3939 3031 322c 302c 302c 302e 3239  .299012,0,0,0.29
-00000350: 3930 3132 2c39 2e37 3032 3239 2c2d 362e  9012,9.70229,-6.
-00000360: 3638 3538 3229 223e 0a20 2020 2020 2020  68582)">.       
-00000370: 2020 2020 203c 7061 7468 2064 3d22 4d35       <path d="M5
-00000380: 302c 3634 2e32 3543 3532 2e37 362c 3634  0,64.25C52.76,64
-00000390: 2e32 3520 3535 2c36 312e 3133 2035 352c  .25 55,61.13 55,
-000003a0: 3539 2e37 3543 3535 2c35 382e 3337 2035  59.75C55,58.37 5
-000003b0: 322e 3736 2c35 372e 3235 2035 302c 3537  2.76,57.25 50,57
-000003c0: 2e32 3543 3437 2e32 342c 3537 2e32 3520  .25C47.24,57.25 
-000003d0: 3435 2c35 382e 3337 2034 352c 3539 2e37  45,58.37 45,59.7
-000003e0: 3543 3435 2c36 312e 3133 2034 372e 3234  5C45,61.13 47.24
-000003f0: 2c36 342e 3235 2035 302c 3634 2e32 355a  ,64.25 50,64.25Z
-00000400: 2220 7374 796c 653d 2266 696c 6c3a 7267  " style="fill:rg
-00000410: 6228 3232 322c 3132 302c 3136 3029 3b66  b(222,120,160);f
-00000420: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
-00000430: 3b22 2f3e 0a20 2020 2020 2020 203c 2f67  ;"/>.        </g
-00000440: 3e0a 2020 2020 2020 2020 3c67 2074 7261  >.        <g tra
-00000450: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
-00000460: 2e32 3939 3031 322c 302c 302c 302e 3239  .299012,0,0,0.29
-00000470: 3930 3132 2c39 2e37 3032 3239 2c2d 362e  9012,9.70229,-6.
-00000480: 3638 3538 3229 223e 0a20 2020 2020 2020  68582)">.       
-00000490: 2020 2020 203c 7061 7468 2064 3d22 4d38       <path d="M8
-000004a0: 382c 3439 2e30 3543 3836 2e35 3036 2c34  8,49.05C86.506,4
-000004b0: 332e 3437 3520 3833 2e30 3138 2c33 382e  3.475 83.018,38.
-000004c0: 3633 3820 3738 2e32 2c33 352e 3436 4337  638 78.2,35.46C7
-000004d0: 322e 3936 392c 3332 2e30 3032 2036 362e  2.969,32.002 66.
-000004e0: 3533 392c 3330 2e38 3434 2036 302e 3433  539,30.844 60.43
-000004f0: 2c33 322e 3236 4335 362e 3537 362c 3333  ,32.26C56.576,33
-00000500: 2e31 3435 2035 322e 3939 352c 3334 2e39  .145 52.995,34.9
-00000510: 3538 2035 302c 3337 2e35 3443 3436 2e39  58 50,37.54C46.9
-00000520: 3938 2c33 342e 3935 3820 3433 2e34 3131  98,34.958 43.411
-00000530: 2c33 332e 3134 3920 3339 2e35 352c 3332  ,33.149 39.55,32
-00000540: 2e32 3743 3333 2e34 3431 2c33 302e 3835  .27C33.441,30.85
-00000550: 3320 3237 2e30 3131 2c33 322e 3031 3120  3 27.011,32.011 
-00000560: 3231 2e37 382c 3335 2e34 3743 3136 2e39  21.78,35.47C16.9
-00000570: 372c 3338 2e36 3532 2031 332e 3438 392c  7,38.652 13.489,
-00000580: 3433 2e34 3839 2031 322c 3439 2e30 364c  43.489 12,49.06L
-00000590: 3132 2c34 392e 3133 4331 312e 3832 2c34  12,49.13C11.82,4
-000005a0: 392e 3739 2031 312e 3636 2c35 302e 3436  9.79 11.66,50.46
-000005b0: 2031 312e 3533 2c35 312e 3133 4331 312e   11.53,51.13C11.
-000005c0: 3134 362c 3533 2e32 3037 2031 312e 3032  146,53.207 11.02
-000005d0: 312c 3535 2e33 3233 2031 312e 3136 2c35  1,55.323 11.16,5
-000005e0: 372e 3433 4331 312e 3136 2c35 382e 3033  7.43C11.16,58.03
-000005f0: 2031 312e 3236 2c35 382e 3633 2031 312e   11.26,58.63 11.
-00000600: 3334 2c35 392e 3233 4331 312e 3334 2c35  34,59.23C11.34,5
-00000610: 392e 3531 2031 312e 3433 2c35 392e 3739  9.51 11.43,59.79
-00000620: 2031 312e 3438 2c36 302e 3037 4331 312e   11.48,60.07C11.
-00000630: 3533 2c36 302e 3335 2031 312e 3538 2c36  53,60.35 11.58,6
-00000640: 302e 3638 2031 312e 3634 2c36 302e 3938  0.68 11.64,60.98
-00000650: 4331 312e 372c 3631 2e32 3820 3131 2e38  C11.7,61.28 11.8
-00000660: 2c36 312e 3639 2031 312e 3839 2c36 322e  ,61.69 11.89,62.
-00000670: 3035 4331 312e 3938 2c36 322e 3431 2031  05C11.98,62.41 1
-00000680: 312e 3939 2c36 322e 3437 2031 322e 3035  1.99,62.47 12.05
-00000690: 2c36 322e 3638 4331 322e 3136 2c36 332e  ,62.68C12.16,63.
-000006a0: 3037 2031 322e 3238 2c36 332e 3436 2031  07 12.28,63.46 1
-000006b0: 322e 3431 2c36 332e 3834 4c31 322e 3538  2.41,63.84L12.58
-000006c0: 2c36 342e 3334 4331 322e 3732 2c36 342e  ,64.34C12.72,64.
-000006d0: 3734 2031 322e 3838 2c36 352e 3134 2031  74 12.88,65.14 1
-000006e0: 332e 3034 2c36 352e 3533 4c31 332e 3233  3.04,65.53L13.23
-000006f0: 2c36 352e 3938 4331 332e 3430 332c 3636  ,65.98C13.403,66
-00000700: 2e33 3733 2031 332e 3538 332c 3636 2e37  .373 13.583,66.7
-00000710: 3637 2031 332e 3737 2c36 372e 3136 4c31  67 13.77,67.16L1
-00000720: 332e 3939 2c36 372e 3539 4331 342e 3139  3.99,67.59C14.19
-00000730: 2c36 372e 3937 2031 342e 3339 2c36 382e  ,67.97 14.39,68.
-00000740: 3335 2031 342e 3631 2c36 382e 3733 4c31  35 14.61,68.73L1
-00000750: 342e 3837 2c36 392e 3135 4331 352e 312c  4.87,69.15C15.1,
-00000760: 3639 2e35 3220 3135 2e33 332c 3639 2e38  69.52 15.33,69.8
-00000770: 3920 3135 2e35 382c 3730 2e32 364c 3135  9 15.58,70.26L15
-00000780: 2e35 382c 3730 2e33 324c 3135 2e39 392c  .58,70.32L15.99,
-00000790: 3730 2e39 3343 3136 2e31 342c 3731 2e31  70.93C16.14,71.1
-000007a0: 3420 3136 2e32 392c 3731 2e33 3620 3136  4 16.29,71.36 16
-000007b0: 2e34 352c 3731 2e35 3743 3230 2e32 3036  .45,71.57C20.206
-000007c0: 2c37 352e 3833 2032 352e 3038 362c 3738  ,75.83 25.086,78
-000007d0: 2e39 3520 3330 2e35 332c 3830 2e35 3743  .95 30.53,80.57C
-000007e0: 3336 2e38 3339 2c38 322e 3438 2034 332e  36.839,82.48 43.
-000007f0: 3431 2c38 332e 3338 3520 3530 2c38 332e  41,83.385 50,83.
-00000800: 3235 4335 362e 3539 392c 3833 2e33 3734  25C56.599,83.374
-00000810: 2036 332e 3137 372c 3832 2e34 3536 2036   63.177,82.456 6
-00000820: 392e 3439 2c38 302e 3533 4337 342e 3634  9.49,80.53C74.64
-00000830: 342c 3738 2e39 3738 2037 392e 3330 332c  4,78.978 79.303,
-00000840: 3736 2e31 3032 2038 332c 3732 2e31 3943  76.102 83,72.19C
-00000850: 3833 2e33 342c 3731 2e37 3820 3833 2e36  83.34,71.78 83.6
-00000860: 352c 3731 2e33 3520 3834 2c37 302e 3932  5,71.35 84,70.92
-00000870: 4c38 342e 3138 2c37 302e 3636 4c38 342e  L84.18,70.66L84.
-00000880: 3333 2c37 302e 3434 4c38 342e 3431 2c37  33,70.44L84.41,7
-00000890: 302e 3332 4338 342e 3535 2c37 302e 3132  0.32C84.55,70.12
-000008a0: 2038 342e 3637 2c36 392e 3920 3834 2e38   84.67,69.9 84.8
-000008b0: 312c 3639 2e37 4338 352e 3037 2c36 392e  1,69.7C85.07,69.
-000008c0: 3320 3835 2e33 322c 3638 2e38 3920 3835  3 85.32,68.89 85
-000008d0: 2e35 352c 3638 2e34 3843 3835 2e37 382c  .55,68.48C85.78,
-000008e0: 3638 2e30 3720 3836 2e30 322c 3637 2e36  68.07 86.02,67.6
-000008f0: 3520 3836 2e32 332c 3637 2e32 3243 3836  5 86.23,67.22C86
-00000900: 2e33 312c 3637 2e30 3520 3836 2e33 392c  .31,67.05 86.39,
-00000910: 3636 2e38 3820 3836 2e34 372c 3636 2e37  66.88 86.47,66.7
-00000920: 4338 362e 3637 2c36 362e 3238 2038 362e  C86.67,66.28 86.
-00000930: 3835 2c36 352e 3837 2038 372e 3033 2c36  85,65.87 87.03,6
-00000940: 352e 3434 4c38 372e 3233 2c36 342e 3932  5.44L87.23,64.92
-00000950: 4338 372e 3339 372c 3634 2e34 3837 2038  C87.397,64.487 8
-00000960: 372e 3535 2c36 342e 3035 2038 372e 3639  7.55,64.05 87.69
-00000970: 2c36 332e 3631 4c38 372e 3835 2c36 332e  ,63.61L87.85,63.
-00000980: 3039 4338 372e 3938 2c36 322e 3634 2038  09C87.98,62.64 8
-00000990: 382e 312c 3632 2e31 3920 3838 2e32 312c  8.1,62.19 88.21,
-000009a0: 3631 2e37 3443 3838 2e32 312c 3631 2e35  61.74C88.21,61.5
-000009b0: 3720 3838 2e33 2c36 312e 3339 2038 382e  7 88.3,61.39 88.
-000009c0: 3333 2c36 312e 3232 4338 382e 3433 2c36  33,61.22C88.43,6
-000009d0: 302e 3735 2038 382e 3532 2c36 302e 3232  0.75 88.52,60.22
-000009e0: 2038 382e 362c 3539 2e37 3943 3838 2e36   88.6,59.79C88.6
-000009f0: 2c35 392e 3634 2038 382e 3636 2c35 392e  ,59.64 88.66,59.
-00000a00: 3439 2038 382e 3638 2c35 392e 3333 4338  49 88.68,59.33C8
-00000a10: 382e 3737 2c35 382e 3731 2038 382e 3834  8.77,58.71 88.84
-00000a20: 2c35 382e 3038 2038 382e 3838 2c35 372e  ,58.08 88.88,57.
-00000a30: 3435 4c38 382e 3838 2c35 342e 3137 4338  45L88.88,54.17C8
-00000a40: 382e 3831 372c 3533 2e31 3634 2038 382e  8.817,53.164 88.
-00000a50: 3639 332c 3532 2e31 3632 2038 382e 3531  693,52.162 88.51
-00000a60: 2c35 312e 3137 4338 382e 3338 2c35 302e  ,51.17C88.38,50.
-00000a70: 3520 3838 2e32 332c 3439 2e38 3420 3838  5 88.23,49.84 88
-00000a80: 2e30 352c 3439 2e31 374c 3838 2c34 392e  .05,49.17L88,49.
-00000a90: 3035 5a4d 3835 2e38 392c 3536 2e34 344c  05ZM85.89,56.44L
-00000aa0: 3835 2e38 392c 3537 2e32 3343 3835 2e38  85.89,57.23C85.8
-00000ab0: 392c 3537 2e37 3820 3835 2e37 392c 3538  9,57.78 85.79,58
-00000ac0: 2e33 3220 3835 2e37 322c 3538 2e38 3643  .32 85.72,58.86C
-00000ad0: 3835 2e37 322c 3539 2e30 3120 3835 2e37  85.72,59.01 85.7
-00000ae0: 322c 3539 2e31 3520 3835 2e36 352c 3539  2,59.15 85.65,59
-00000af0: 2e33 4338 352e 3539 2c35 392e 3720 3835  .3C85.59,59.7 85
-00000b00: 2e35 312c 3630 2e31 3120 3835 2e34 332c  .51,60.11 85.43,
-00000b10: 3630 2e35 314c 3835 2e33 322c 3630 2e39  60.51L85.32,60.9
-00000b20: 3943 3835 2e32 332c 3631 2e33 3820 3835  9C85.23,61.38 85
-00000b30: 2e31 322c 3631 2e37 3720 3835 2e30 312c  .12,61.77 85.01,
-00000b40: 3632 2e31 3643 3835 2e30 312c 3632 2e33  62.16C85.01,62.3
-00000b50: 3120 3834 2e39 332c 3632 2e34 3620 3834  1 84.93,62.46 84
-00000b60: 2e38 382c 3632 2e36 4338 342e 3734 2c36  .88,62.6C84.74,6
-00000b70: 332e 3034 2038 342e 3539 2c36 332e 3437  3.04 84.59,63.47
-00000b80: 2038 342e 3432 2c36 332e 394c 3834 2e32   84.42,63.9L84.2
-00000b90: 372c 3634 2e32 3843 3834 2e31 2c36 342e  7,64.28C84.1,64.
-00000ba0: 3731 2038 332e 3931 2c36 352e 3134 2038  71 83.91,65.14 8
-00000bb0: 332e 3731 2c36 352e 3536 4338 332e 3531  3.71,65.56C83.51
-00000bc0: 2c36 352e 3938 2038 332e 3433 2c36 362e  ,65.98 83.43,66.
-00000bd0: 3132 2038 332e 3238 2c36 362e 344c 3833  12 83.28,66.4L83
-00000be0: 2e30 312c 3636 2e39 3143 3832 2e38 332c  .01,66.91C82.83,
-00000bf0: 3637 2e32 3233 2038 322e 3634 332c 3637  67.223 82.643,67
-00000c00: 2e35 3337 2038 322e 3435 2c36 372e 3835  .537 82.45,67.85
-00000c10: 4c38 322e 3335 2c36 382e 3031 4337 392e  L82.35,68.01C79.
-00000c20: 3132 312c 3638 2e30 3437 2037 352e 3931  121,68.047 75.91
-00000c30: 382c 3637 2e34 3334 2037 322e 3933 2c36  8,67.434 72.93,6
-00000c40: 362e 3231 4336 342e 3237 2c36 322e 3734  6.21C64.27,62.74
-00000c50: 2035 392c 3535 2e35 3220 3631 2e31 382c   59,55.52 61.18,
-00000c60: 3530 2e31 3143 3632 2e31 382c 3437 2e36  50.11C62.18,47.6
-00000c70: 2036 342e 372c 3435 2e38 3220 3638 2e32   64.7,45.82 68.2
-00000c80: 362c 3435 2e31 3143 3732 2e34 3839 2c34  6,45.11C72.489,4
-00000c90: 342e 3339 3520 3736 2e38 3335 2c34 342e  4.395 76.835,44.
-00000ca0: 3930 3820 3830 2e37 382c 3436 2e35 3943  908 80.78,46.59C
-00000cb0: 3832 2e31 3431 2c34 372e 3134 3420 3833  82.141,47.144 83
-00000cc0: 2e34 3533 2c34 372e 3831 3320 3834 2e37  .453,47.813 84.7
-00000cd0: 2c34 382e 3539 4338 342e 3736 2c34 382e  ,48.59C84.76,48.
-00000ce0: 3736 2038 342e 3832 2c34 382e 3933 2038  76 84.82,48.93 8
-00000cf0: 342e 3838 2c34 392e 3143 3834 2e39 342c  4.88,49.1C84.94,
-00000d00: 3439 2e32 3720 3835 2e30 352c 3439 2e36  49.27 85.05,49.6
-00000d10: 3320 3835 2e31 322c 3439 2e39 4338 352e  3 85.12,49.9C85.
-00000d20: 3238 2c35 302e 3520 3835 2e34 342c 3531  28,50.5 85.44,51
-00000d30: 2e31 2038 352e 3535 2c35 312e 3733 4338  .1 85.55,51.73C8
-00000d40: 352e 3639 312c 3532 2e35 3037 2038 352e  5.691,52.507 85.
-00000d50: 3739 322c 3533 2e32 3932 2038 352e 3835  792,53.292 85.85
-00000d60: 2c35 342e 3038 4c38 352e 3835 2c35 352e  ,54.08L85.85,55.
-00000d70: 3839 4338 352e 3835 2c35 362e 3132 2038  89C85.85,56.12 8
-00000d80: 352e 3931 2c35 362e 3235 2038 352e 3931  5.91,56.25 85.91
-00000d90: 2c35 362e 3435 4c38 352e 3839 2c35 362e  ,56.45L85.89,56.
-00000da0: 3434 5a4d 3137 2e36 362c 3638 4331 362e  44ZM17.66,68C16.
-00000db0: 3636 382c 3636 2e34 3335 2031 352e 3836  668,66.435 15.86
-00000dc0: 392c 3634 2e37 3536 2031 352e 3238 2c36  9,64.756 15.28,6
-00000dd0: 334c 3135 2e31 372c 3632 2e36 3843 3135  3L15.17,62.68C15
-00000de0: 2e30 362c 3632 2e33 3520 3134 2e39 362c  .06,62.35 14.96,
-00000df0: 3632 2e30 3120 3134 2e38 372c 3631 2e36  62.01 14.87,61.6
-00000e00: 3843 3134 2e38 3233 2c36 312e 3439 3320  8C14.823,61.493 
-00000e10: 3134 2e37 3737 2c36 312e 3331 2031 342e  14.777,61.31 14.
-00000e20: 3733 2c36 312e 3133 4331 342e 3636 2c36  73,61.13C14.66,6
-00000e30: 302e 3834 2031 342e 3539 2c36 302e 3535  0.84 14.59,60.55
-00000e40: 2031 342e 3533 2c36 302e 3237 4331 342e   14.53,60.27C14.
-00000e50: 3437 2c35 392e 3939 2031 342e 3433 2c35  47,59.99 14.43,5
-00000e60: 392e 3732 2031 342e 3338 2c35 392e 3434  9.72 14.38,59.44
-00000e70: 4331 342e 3333 2c35 392e 3136 2031 342e  C14.33,59.16 14.
-00000e80: 332c 3539 2031 342e 3237 2c35 382e 3738  3,59 14.27,58.78
-00000e90: 4331 342e 322c 3538 2e32 3720 3134 2e31  C14.2,58.27 14.1
-00000ea0: 352c 3537 2e37 3820 3134 2e31 312c 3537  5,57.78 14.11,57
-00000eb0: 2e32 334c 3134 2e31 312c 3537 2e30 3343  .23L14.11,57.03C
-00000ec0: 3134 2e30 3038 2c35 352e 3233 3620 3134  14.008,55.236 14
-00000ed0: 2e31 3232 2c35 332e 3433 3720 3134 2e34  .122,53.437 14.4
-00000ee0: 352c 3531 2e36 3743 3134 2e35 362c 3531  5,51.67C14.56,51
-00000ef0: 2e30 3620 3134 2e37 312c 3530 2e34 3620  .06 14.71,50.46 
-00000f00: 3134 2e38 382c 3439 2e38 3743 3134 2e39  14.88,49.87C14.9
-00000f10: 362c 3439 2e35 3920 3135 2e30 342c 3439  6,49.59 15.04,49
-00000f20: 2e33 3220 3135 2e31 332c 3439 2e30 3543  .32 15.13,49.05C
-00000f30: 3135 2e32 322c 3438 2e37 3820 3135 2e32  15.22,48.78 15.2
-00000f40: 342c 3438 2e37 3220 3135 2e33 2c34 382e  4,48.72 15.3,48.
-00000f50: 3535 4331 362e 3534 382c 3437 2e37 3734  55C16.548,47.774
-00000f60: 2031 372e 3835 392c 3437 2e31 3035 2031   17.859,47.105 1
-00000f70: 392e 3232 2c34 362e 3535 4332 372e 3836  9.22,46.55C27.86
-00000f80: 2c34 332e 3039 2033 362e 3635 2c34 342e  ,43.09 36.65,44.
-00000f90: 3637 2033 382e 3832 2c35 302e 3038 4334  67 38.82,50.08C4
-00000fa0: 302e 3939 2c35 352e 3439 2033 352e 3733  0.99,55.49 35.73
-00000fb0: 2c36 322e 3734 2032 372e 3039 2c36 362e  ,62.74 27.09,66.
-00000fc0: 3243 3234 2e31 3031 2c36 372e 3433 3120  2C24.101,67.431 
-00000fd0: 3230 2e38 3933 2c36 382e 3034 3320 3137  20.893,68.043 17
-00000fe0: 2e36 362c 3638 5a4d 3638 2e35 372c 3737  .66,68ZM68.57,77
-00000ff0: 2e36 3843 3632 2e35 3534 2c37 392e 3530  .68C62.554,79.50
-00001000: 3820 3536 2e32 3837 2c38 302e 3337 3620  8 56.287,80.376 
-00001010: 3530 2c38 302e 3235 4334 332e 3733 372c  50,80.25C43.737,
-00001020: 3830 2e33 3720 3337 2e34 3935 2c37 392e  80.37 37.495,79.
-00001030: 3530 3620 3331 2e35 2c37 372e 3639 4332  506 31.5,77.69C2
-00001040: 372e 3138 352c 3736 2e33 3820 3233 2e32  7.185,76.38 23.2
-00001050: 3433 2c37 342e 3036 3220 3230 2c37 302e  43,74.062 20,70.
-00001060: 3933 4332 322e 3831 352c 3730 2e37 3036  93C22.815,70.706
-00001070: 2032 352e 3538 2c37 302e 3035 3520 3238   25.58,70.055 28
-00001080: 2e32 2c36 3943 3338 2e33 372c 3634 2e39  .2,69C38.37,64.9
-00001090: 3220 3434 2e33 392c 3536 2034 312e 362c  2 44.39,56 41.6,
-000010a0: 3439 4333 382e 3831 2c34 3220 3238 2e32  49C38.81,42 28.2
-000010b0: 372c 3339 2e37 3220 3138 2e31 2c34 332e  7,39.72 18.1,43.
-000010c0: 384c 3137 2e34 332c 3434 2e30 3943 3138  8L17.43,44.09C18
-000010d0: 2e39 3733 2c34 312e 3634 3820 3231 2e30  .973,41.648 21.0
-000010e0: 3139 2c33 392e 3536 3120 3233 2e34 332c  19,39.561 23.43,
-000010f0: 3337 2e39 3743 3236 2e36 3731 2c33 352e  37.97C26.671,35.
-00001100: 3832 3420 3330 2e34 3733 2c33 342e 3638  824 30.473,34.68
-00001110: 2033 342e 3336 2c33 342e 3638 4333 352e   34.36,34.68C35.
-00001120: 3838 342c 3334 2e36 3831 2033 372e 3430  884,34.681 37.40
-00001130: 342c 3334 2e38 3532 2033 382e 3839 2c33  4,34.852 38.89,3
-00001140: 352e 3139 4334 322e 3639 342c 3336 2e30  5.19C42.694,36.0
-00001150: 3439 2034 362e 3139 312c 3337 2e39 3335  49 46.191,37.935
-00001160: 2034 392c 3430 2e36 344c 3530 2c34 312e   49,40.64L50,41.
-00001170: 3634 4c35 312c 3430 2e36 3443 3533 2e37  64L51,40.64C53.7
-00001180: 3937 2c33 372e 3933 3720 3537 2e32 3739  97,37.937 57.279
-00001190: 2c33 362e 3034 3920 3631 2e30 372c 3335  ,36.049 61.07,35
-000011a0: 2e31 3843 3636 2e34 3032 2c33 332e 3934  .18C66.402,33.94
-000011b0: 3720 3732 2e30 3134 2c33 342e 3936 3820  7 72.014,34.968 
-000011c0: 3736 2e35 372c 3338 4337 382e 3938 2c33  76.57,38C78.98,3
-000011d0: 392e 3538 3820 3831 2e30 3236 2c34 312e  9.588 81.026,41.
-000011e0: 3637 3120 3832 2e35 372c 3434 2e31 314c  671 82.57,44.11L
-000011f0: 3831 2e39 2c34 332e 3832 4337 372e 3430  81.9,43.82C77.40
-00001200: 392c 3431 2e39 3231 2037 322e 3436 342c  9,41.921 72.464,
-00001210: 3431 2e33 3535 2036 372e 3636 2c34 322e  41.355 67.66,42.
-00001220: 3139 4336 332e 3038 2c34 332e 3132 2035  19C63.08,43.12 5
-00001230: 392e 3739 2c34 352e 3534 2035 382e 3339  9.79,45.54 58.39
-00001240: 2c34 392e 3032 4335 352e 362c 3535 2e39  ,49.02C55.6,55.9
-00001250: 3720 3631 2e36 322c 3634 2e39 3420 3731  7 61.62,64.94 71
-00001260: 2e37 392c 3639 2e30 3243 3734 2e34 3134  .79,69.02C74.414
-00001270: 2c37 302e 3037 2037 372e 3138 322c 3730  ,70.07 77.182,70
-00001280: 2e37 3134 2038 302c 3730 2e39 3343 3736  .714 80,70.93C76
-00001290: 2e37 3736 2c37 342e 3035 2037 322e 3835  .776,74.05 72.85
-000012a0: 392c 3736 2e33 3633 2036 382e 3537 2c37  9,76.363 68.57,7
-000012b0: 372e 3638 5a22 2073 7479 6c65 3d22 6669  7.68Z" style="fi
-000012c0: 6c6c 3a72 6762 2832 3232 2c31 3230 2c31  ll:rgb(222,120,1
-000012d0: 3630 293b 6669 6c6c 2d72 756c 653a 6e6f  60);fill-rule:no
-000012e0: 6e7a 6572 6f3b 222f 3e0a 2020 2020 2020  nzero;"/>.      
-000012f0: 2020 3c2f 673e 0a20 2020 2020 2020 203c    </g>.        <
-00001300: 6720 7472 616e 7366 6f72 6d3d 226d 6174  g transform="mat
-00001310: 7269 7828 302e 3239 3930 3132 2c30 2c30  rix(0.299012,0,0
-00001320: 2c30 2e32 3939 3031 322c 392e 3730 3232  ,0.299012,9.7022
-00001330: 392c 2d36 2e36 3835 3832 2922 3e0a 2020  9,-6.68582)">.  
-00001340: 2020 2020 2020 2020 2020 3c63 6972 636c            <circl
-00001350: 6520 6378 3d22 3731 2e33 3322 2063 793d  e cx="71.33" cy=
-00001360: 2235 3622 2072 3d22 352e 3136 2220 7374  "56" r="5.16" st
-00001370: 796c 653d 2266 696c 6c3a 7267 6228 3232  yle="fill:rgb(22
-00001380: 322c 3132 302c 3136 3029 3b22 2f3e 0a20  2,120,160);"/>. 
-00001390: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
-000013a0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
-000013b0: 3d22 6d61 7472 6978 2830 2e32 3939 3031  ="matrix(0.29901
-000013c0: 322c 302c 302c 302e 3239 3930 3132 2c39  2,0,0,0.299012,9
-000013d0: 2e37 3032 3239 2c2d 362e 3638 3538 3229  .70229,-6.68582)
-000013e0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-000013f0: 6369 7263 6c65 2063 783d 2232 382e 3637  circle cx="28.67
-00001400: 2220 6379 3d22 3536 2220 723d 2235 2e31  " cy="56" r="5.1
-00001410: 3622 2073 7479 6c65 3d22 6669 6c6c 3a72  6" style="fill:r
-00001420: 6762 2832 3232 2c31 3230 2c31 3630 293b  gb(222,120,160);
-00001430: 222f 3e0a 2020 2020 2020 2020 3c2f 673e  "/>.        </g>
-00001440: 0a20 2020 2020 2020 203c 6720 7472 616e  .        <g tran
-00001450: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
-00001460: 3239 3930 3132 2c30 2c30 2c30 2e32 3939  299012,0,0,0.299
-00001470: 3031 322c 392e 3730 3232 392c 2d36 2e36  012,9.70229,-6.6
-00001480: 3835 3832 2922 3e0a 2020 2020 2020 2020  8582)">.        
-00001490: 2020 2020 3c70 6174 6820 643d 224d 3538      <path d="M58
-000014a0: 2c36 3643 3535 2e39 3132 2c36 382e 3136  ,66C55.912,68.16
-000014b0: 3120 3533 2e30 3033 2c36 392e 3333 3920  1 53.003,69.339 
-000014c0: 3530 2c36 392e 3234 4334 362e 3939 372c  50,69.24C46.997,
-000014d0: 3639 2e33 3339 2034 342e 3038 382c 3638  69.339 44.088,68
-000014e0: 2e31 3631 2034 322c 3636 4334 312e 3731  .161 42,66C41.71
-000014f0: 342c 3635 2e36 3737 2034 312e 3330 322c  4,65.677 41.302,
-00001500: 3635 2e34 3931 2034 302e 3837 2c36 352e  65.491 40.87,65.
-00001510: 3439 3143 3430 2e30 3432 2c36 352e 3439  491C40.042,65.49
-00001520: 3120 3339 2e33 3631 2c36 362e 3137 3220  1 39.361,66.172 
-00001530: 3339 2e33 3631 2c36 3743 3339 2e33 3631  39.361,67C39.361
-00001540: 2c36 372e 3336 3820 3339 2e34 3936 2c36  ,67.368 39.496,6
-00001550: 372e 3732 3420 3339 2e37 342c 3638 4334  7.724 39.74,68C4
-00001560: 322e 3430 332c 3730 2e38 3034 2034 362e  2.403,70.804 46.
-00001570: 3133 342c 3732 2e33 3520 3530 2c37 322e  134,72.35 50,72.
-00001580: 3235 4335 332e 3836 322c 3732 2e33 3437  25C53.862,72.347
-00001590: 2035 372e 3539 2c37 302e 3830 3220 3630   57.59,70.802 60
-000015a0: 2e32 352c 3638 4336 302e 3439 352c 3637  .25,68C60.495,67
-000015b0: 2e37 3235 2036 302e 3633 2c36 372e 3336  .725 60.63,67.36
-000015c0: 3920 3630 2e36 332c 3637 4336 302e 3633  9 60.63,67C60.63
-000015d0: 2c36 362e 3137 3420 3539 2e39 3531 2c36  ,66.174 59.951,6
-000015e0: 352e 3439 3520 3539 2e31 3235 2c36 352e  5.495 59.125,65.
-000015f0: 3439 3543 3538 2e36 3935 2c36 352e 3439  495C58.695,65.49
-00001600: 3520 3538 2e32 3835 2c36 352e 3637 3920  5 58.285,65.679 
-00001610: 3538 2c36 365a 2220 7374 796c 653d 2266  58,66Z" style="f
-00001620: 696c 6c3a 7267 6228 3232 322c 3132 302c  ill:rgb(222,120,
-00001630: 3136 3029 3b66 696c 6c2d 7275 6c65 3a6e  160);fill-rule:n
-00001640: 6f6e 7a65 726f 3b22 2f3e 0a20 2020 2020  onzero;"/>.     
-00001650: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
-00001660: 0a3c 2f73 7667 3e0a                      .</svg>.
+00000130: 2233 3922 2068 6569 6768 743d 2232 3022  "39" height="20"
+00000140: 2066 696c 6c3d 2223 3966 3966 3966 222f   fill="#9f9f9f"/
+00000150: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
+00000160: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
+00000170: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00000180: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
+00000190: 5665 7264 616e 612c 4765 6e65 7661 2c44  Verdana,Geneva,D
+000001a0: 656a 6156 7520 5361 6e73 2c73 616e 732d  ejaVu Sans,sans-
+000001b0: 7365 7269 6622 2074 6578 742d 7265 6e64  serif" text-rend
+000001c0: 6572 696e 673d 2267 656f 6d65 7472 6963  ering="geometric
+000001d0: 5072 6563 6973 696f 6e22 2066 6f6e 742d  Precision" font-
+000001e0: 7369 7a65 3d22 3131 3022 3e0a 2020 2020  size="110">.    
+000001f0: 2020 2020 3c74 6578 7420 783d 2235 3930      <text x="590
+00000200: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
+00000210: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
+00000220: 6669 6c6c 3d22 2366 6666 2220 7465 7874  fill="#fff" text
+00000230: 4c65 6e67 7468 3d22 3631 3022 3e69 6e74  Length="610">int
+00000240: 6572 726f 6761 7465 3c2f 7465 7874 3e0a  errogate</text>.
+00000250: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
+00000260: 2231 3132 3022 2079 3d22 3134 3022 2074  "1120" y="140" t
+00000270: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
+00000280: 2e31 2922 2066 696c 6c3d 2223 6666 6622  .1)" fill="#fff"
+00000290: 2074 6578 744c 656e 6774 683d 2232 3930   textLength="290
+000002a0: 2220 6461 7461 2d69 6e74 6572 726f 6761  " data-interroga
+000002b0: 7465 3d22 7265 7375 6c74 223e 2d31 2e30  te="result">-1.0
+000002c0: 253c 2f74 6578 743e 0a20 2020 203c 2f67  %</text>.    </g
+000002d0: 3e0a 2020 2020 3c67 2069 643d 226c 6f67  >.    <g id="log
+000002e0: 6f2d 7069 6e6b 2220 7472 616e 7366 6f72  o-pink" transfor
+000002f0: 6d3d 226d 6174 7269 7828 302e 3835 3438  m="matrix(0.8548
+00000300: 3736 2c30 2c30 2c30 2e38 3534 3837 362c  76,0,0,0.854876,
+00000310: 2d36 2e37 3335 3134 2c30 2e38 3737 3132  -6.73514,0.87712
+00000320: 3429 223e 0a20 2020 2020 2020 203c 6720  4)">.        <g 
+00000330: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+00000340: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+00000350: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00000360: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
+00000370: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+00000380: 224d 3530 2c36 342e 3235 4335 322e 3736  "M50,64.25C52.76
+00000390: 2c36 342e 3235 2035 352c 3631 2e31 3320  ,64.25 55,61.13 
+000003a0: 3535 2c35 392e 3735 4335 352c 3538 2e33  55,59.75C55,58.3
+000003b0: 3720 3532 2e37 362c 3537 2e32 3520 3530  7 52.76,57.25 50
+000003c0: 2c35 372e 3235 4334 372e 3234 2c35 372e  ,57.25C47.24,57.
+000003d0: 3235 2034 352c 3538 2e33 3720 3435 2c35  25 45,58.37 45,5
+000003e0: 392e 3735 4334 352c 3631 2e31 3320 3437  9.75C45,61.13 47
+000003f0: 2e32 342c 3634 2e32 3520 3530 2c36 342e  .24,64.25 50,64.
+00000400: 3235 5a22 2073 7479 6c65 3d22 6669 6c6c  25Z" style="fill
+00000410: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
+00000420: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
+00000430: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
+00000440: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
+00000450: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+00000460: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+00000470: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00000480: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
+00000490: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+000004a0: 224d 3838 2c34 392e 3035 4338 362e 3530  "M88,49.05C86.50
+000004b0: 362c 3433 2e34 3735 2038 332e 3031 382c  6,43.475 83.018,
+000004c0: 3338 2e36 3338 2037 382e 322c 3335 2e34  38.638 78.2,35.4
+000004d0: 3643 3732 2e39 3639 2c33 322e 3030 3220  6C72.969,32.002 
+000004e0: 3636 2e35 3339 2c33 302e 3834 3420 3630  66.539,30.844 60
+000004f0: 2e34 332c 3332 2e32 3643 3536 2e35 3736  .43,32.26C56.576
+00000500: 2c33 332e 3134 3520 3532 2e39 3935 2c33  ,33.145 52.995,3
+00000510: 342e 3935 3820 3530 2c33 372e 3534 4334  4.958 50,37.54C4
+00000520: 362e 3939 382c 3334 2e39 3538 2034 332e  6.998,34.958 43.
+00000530: 3431 312c 3333 2e31 3439 2033 392e 3535  411,33.149 39.55
+00000540: 2c33 322e 3237 4333 332e 3434 312c 3330  ,32.27C33.441,30
+00000550: 2e38 3533 2032 372e 3031 312c 3332 2e30  .853 27.011,32.0
+00000560: 3131 2032 312e 3738 2c33 352e 3437 4331  11 21.78,35.47C1
+00000570: 362e 3937 2c33 382e 3635 3220 3133 2e34  6.97,38.652 13.4
+00000580: 3839 2c34 332e 3438 3920 3132 2c34 392e  89,43.489 12,49.
+00000590: 3036 4c31 322c 3439 2e31 3343 3131 2e38  06L12,49.13C11.8
+000005a0: 322c 3439 2e37 3920 3131 2e36 362c 3530  2,49.79 11.66,50
+000005b0: 2e34 3620 3131 2e35 332c 3531 2e31 3343  .46 11.53,51.13C
+000005c0: 3131 2e31 3436 2c35 332e 3230 3720 3131  11.146,53.207 11
+000005d0: 2e30 3231 2c35 352e 3332 3320 3131 2e31  .021,55.323 11.1
+000005e0: 362c 3537 2e34 3343 3131 2e31 362c 3538  6,57.43C11.16,58
+000005f0: 2e30 3320 3131 2e32 362c 3538 2e36 3320  .03 11.26,58.63 
+00000600: 3131 2e33 342c 3539 2e32 3343 3131 2e33  11.34,59.23C11.3
+00000610: 342c 3539 2e35 3120 3131 2e34 332c 3539  4,59.51 11.43,59
+00000620: 2e37 3920 3131 2e34 382c 3630 2e30 3743  .79 11.48,60.07C
+00000630: 3131 2e35 332c 3630 2e33 3520 3131 2e35  11.53,60.35 11.5
+00000640: 382c 3630 2e36 3820 3131 2e36 342c 3630  8,60.68 11.64,60
+00000650: 2e39 3843 3131 2e37 2c36 312e 3238 2031  .98C11.7,61.28 1
+00000660: 312e 382c 3631 2e36 3920 3131 2e38 392c  1.8,61.69 11.89,
+00000670: 3632 2e30 3543 3131 2e39 382c 3632 2e34  62.05C11.98,62.4
+00000680: 3120 3131 2e39 392c 3632 2e34 3720 3132  1 11.99,62.47 12
+00000690: 2e30 352c 3632 2e36 3843 3132 2e31 362c  .05,62.68C12.16,
+000006a0: 3633 2e30 3720 3132 2e32 382c 3633 2e34  63.07 12.28,63.4
+000006b0: 3620 3132 2e34 312c 3633 2e38 344c 3132  6 12.41,63.84L12
+000006c0: 2e35 382c 3634 2e33 3443 3132 2e37 322c  .58,64.34C12.72,
+000006d0: 3634 2e37 3420 3132 2e38 382c 3635 2e31  64.74 12.88,65.1
+000006e0: 3420 3133 2e30 342c 3635 2e35 334c 3133  4 13.04,65.53L13
+000006f0: 2e32 332c 3635 2e39 3843 3133 2e34 3033  .23,65.98C13.403
+00000700: 2c36 362e 3337 3320 3133 2e35 3833 2c36  ,66.373 13.583,6
+00000710: 362e 3736 3720 3133 2e37 372c 3637 2e31  6.767 13.77,67.1
+00000720: 364c 3133 2e39 392c 3637 2e35 3943 3134  6L13.99,67.59C14
+00000730: 2e31 392c 3637 2e39 3720 3134 2e33 392c  .19,67.97 14.39,
+00000740: 3638 2e33 3520 3134 2e36 312c 3638 2e37  68.35 14.61,68.7
+00000750: 334c 3134 2e38 372c 3639 2e31 3543 3135  3L14.87,69.15C15
+00000760: 2e31 2c36 392e 3532 2031 352e 3333 2c36  .1,69.52 15.33,6
+00000770: 392e 3839 2031 352e 3538 2c37 302e 3236  9.89 15.58,70.26
+00000780: 4c31 352e 3538 2c37 302e 3332 4c31 352e  L15.58,70.32L15.
+00000790: 3939 2c37 302e 3933 4331 362e 3134 2c37  99,70.93C16.14,7
+000007a0: 312e 3134 2031 362e 3239 2c37 312e 3336  1.14 16.29,71.36
+000007b0: 2031 362e 3435 2c37 312e 3537 4332 302e   16.45,71.57C20.
+000007c0: 3230 362c 3735 2e38 3320 3235 2e30 3836  206,75.83 25.086
+000007d0: 2c37 382e 3935 2033 302e 3533 2c38 302e  ,78.95 30.53,80.
+000007e0: 3537 4333 362e 3833 392c 3832 2e34 3820  57C36.839,82.48 
+000007f0: 3433 2e34 312c 3833 2e33 3835 2035 302c  43.41,83.385 50,
+00000800: 3833 2e32 3543 3536 2e35 3939 2c38 332e  83.25C56.599,83.
+00000810: 3337 3420 3633 2e31 3737 2c38 322e 3435  374 63.177,82.45
+00000820: 3620 3639 2e34 392c 3830 2e35 3343 3734  6 69.49,80.53C74
+00000830: 2e36 3434 2c37 382e 3937 3820 3739 2e33  .644,78.978 79.3
+00000840: 3033 2c37 362e 3130 3220 3833 2c37 322e  03,76.102 83,72.
+00000850: 3139 4338 332e 3334 2c37 312e 3738 2038  19C83.34,71.78 8
+00000860: 332e 3635 2c37 312e 3335 2038 342c 3730  3.65,71.35 84,70
+00000870: 2e39 324c 3834 2e31 382c 3730 2e36 364c  .92L84.18,70.66L
+00000880: 3834 2e33 332c 3730 2e34 344c 3834 2e34  84.33,70.44L84.4
+00000890: 312c 3730 2e33 3243 3834 2e35 352c 3730  1,70.32C84.55,70
+000008a0: 2e31 3220 3834 2e36 372c 3639 2e39 2038  .12 84.67,69.9 8
+000008b0: 342e 3831 2c36 392e 3743 3835 2e30 372c  4.81,69.7C85.07,
+000008c0: 3639 2e33 2038 352e 3332 2c36 382e 3839  69.3 85.32,68.89
+000008d0: 2038 352e 3535 2c36 382e 3438 4338 352e   85.55,68.48C85.
+000008e0: 3738 2c36 382e 3037 2038 362e 3032 2c36  78,68.07 86.02,6
+000008f0: 372e 3635 2038 362e 3233 2c36 372e 3232  7.65 86.23,67.22
+00000900: 4338 362e 3331 2c36 372e 3035 2038 362e  C86.31,67.05 86.
+00000910: 3339 2c36 362e 3838 2038 362e 3437 2c36  39,66.88 86.47,6
+00000920: 362e 3743 3836 2e36 372c 3636 2e32 3820  6.7C86.67,66.28 
+00000930: 3836 2e38 352c 3635 2e38 3720 3837 2e30  86.85,65.87 87.0
+00000940: 332c 3635 2e34 344c 3837 2e32 332c 3634  3,65.44L87.23,64
+00000950: 2e39 3243 3837 2e33 3937 2c36 342e 3438  .92C87.397,64.48
+00000960: 3720 3837 2e35 352c 3634 2e30 3520 3837  7 87.55,64.05 87
+00000970: 2e36 392c 3633 2e36 314c 3837 2e38 352c  .69,63.61L87.85,
+00000980: 3633 2e30 3943 3837 2e39 382c 3632 2e36  63.09C87.98,62.6
+00000990: 3420 3838 2e31 2c36 322e 3139 2038 382e  4 88.1,62.19 88.
+000009a0: 3231 2c36 312e 3734 4338 382e 3231 2c36  21,61.74C88.21,6
+000009b0: 312e 3537 2038 382e 332c 3631 2e33 3920  1.57 88.3,61.39 
+000009c0: 3838 2e33 332c 3631 2e32 3243 3838 2e34  88.33,61.22C88.4
+000009d0: 332c 3630 2e37 3520 3838 2e35 322c 3630  3,60.75 88.52,60
+000009e0: 2e32 3220 3838 2e36 2c35 392e 3739 4338  .22 88.6,59.79C8
+000009f0: 382e 362c 3539 2e36 3420 3838 2e36 362c  8.6,59.64 88.66,
+00000a00: 3539 2e34 3920 3838 2e36 382c 3539 2e33  59.49 88.68,59.3
+00000a10: 3343 3838 2e37 372c 3538 2e37 3120 3838  3C88.77,58.71 88
+00000a20: 2e38 342c 3538 2e30 3820 3838 2e38 382c  .84,58.08 88.88,
+00000a30: 3537 2e34 354c 3838 2e38 382c 3534 2e31  57.45L88.88,54.1
+00000a40: 3743 3838 2e38 3137 2c35 332e 3136 3420  7C88.817,53.164 
+00000a50: 3838 2e36 3933 2c35 322e 3136 3220 3838  88.693,52.162 88
+00000a60: 2e35 312c 3531 2e31 3743 3838 2e33 382c  .51,51.17C88.38,
+00000a70: 3530 2e35 2038 382e 3233 2c34 392e 3834  50.5 88.23,49.84
+00000a80: 2038 382e 3035 2c34 392e 3137 4c38 382c   88.05,49.17L88,
+00000a90: 3439 2e30 355a 4d38 352e 3839 2c35 362e  49.05ZM85.89,56.
+00000aa0: 3434 4c38 352e 3839 2c35 372e 3233 4338  44L85.89,57.23C8
+00000ab0: 352e 3839 2c35 372e 3738 2038 352e 3739  5.89,57.78 85.79
+00000ac0: 2c35 382e 3332 2038 352e 3732 2c35 382e  ,58.32 85.72,58.
+00000ad0: 3836 4338 352e 3732 2c35 392e 3031 2038  86C85.72,59.01 8
+00000ae0: 352e 3732 2c35 392e 3135 2038 352e 3635  5.72,59.15 85.65
+00000af0: 2c35 392e 3343 3835 2e35 392c 3539 2e37  ,59.3C85.59,59.7
+00000b00: 2038 352e 3531 2c36 302e 3131 2038 352e   85.51,60.11 85.
+00000b10: 3433 2c36 302e 3531 4c38 352e 3332 2c36  43,60.51L85.32,6
+00000b20: 302e 3939 4338 352e 3233 2c36 312e 3338  0.99C85.23,61.38
+00000b30: 2038 352e 3132 2c36 312e 3737 2038 352e   85.12,61.77 85.
+00000b40: 3031 2c36 322e 3136 4338 352e 3031 2c36  01,62.16C85.01,6
+00000b50: 322e 3331 2038 342e 3933 2c36 322e 3436  2.31 84.93,62.46
+00000b60: 2038 342e 3838 2c36 322e 3643 3834 2e37   84.88,62.6C84.7
+00000b70: 342c 3633 2e30 3420 3834 2e35 392c 3633  4,63.04 84.59,63
+00000b80: 2e34 3720 3834 2e34 322c 3633 2e39 4c38  .47 84.42,63.9L8
+00000b90: 342e 3237 2c36 342e 3238 4338 342e 312c  4.27,64.28C84.1,
+00000ba0: 3634 2e37 3120 3833 2e39 312c 3635 2e31  64.71 83.91,65.1
+00000bb0: 3420 3833 2e37 312c 3635 2e35 3643 3833  4 83.71,65.56C83
+00000bc0: 2e35 312c 3635 2e39 3820 3833 2e34 332c  .51,65.98 83.43,
+00000bd0: 3636 2e31 3220 3833 2e32 382c 3636 2e34  66.12 83.28,66.4
+00000be0: 4c38 332e 3031 2c36 362e 3931 4338 322e  L83.01,66.91C82.
+00000bf0: 3833 2c36 372e 3232 3320 3832 2e36 3433  83,67.223 82.643
+00000c00: 2c36 372e 3533 3720 3832 2e34 352c 3637  ,67.537 82.45,67
+00000c10: 2e38 354c 3832 2e33 352c 3638 2e30 3143  .85L82.35,68.01C
+00000c20: 3739 2e31 3231 2c36 382e 3034 3720 3735  79.121,68.047 75
+00000c30: 2e39 3138 2c36 372e 3433 3420 3732 2e39  .918,67.434 72.9
+00000c40: 332c 3636 2e32 3143 3634 2e32 372c 3632  3,66.21C64.27,62
+00000c50: 2e37 3420 3539 2c35 352e 3532 2036 312e  .74 59,55.52 61.
+00000c60: 3138 2c35 302e 3131 4336 322e 3138 2c34  18,50.11C62.18,4
+00000c70: 372e 3620 3634 2e37 2c34 352e 3832 2036  7.6 64.7,45.82 6
+00000c80: 382e 3236 2c34 352e 3131 4337 322e 3438  8.26,45.11C72.48
+00000c90: 392c 3434 2e33 3935 2037 362e 3833 352c  9,44.395 76.835,
+00000ca0: 3434 2e39 3038 2038 302e 3738 2c34 362e  44.908 80.78,46.
+00000cb0: 3539 4338 322e 3134 312c 3437 2e31 3434  59C82.141,47.144
+00000cc0: 2038 332e 3435 332c 3437 2e38 3133 2038   83.453,47.813 8
+00000cd0: 342e 372c 3438 2e35 3943 3834 2e37 362c  4.7,48.59C84.76,
+00000ce0: 3438 2e37 3620 3834 2e38 322c 3438 2e39  48.76 84.82,48.9
+00000cf0: 3320 3834 2e38 382c 3439 2e31 4338 342e  3 84.88,49.1C84.
+00000d00: 3934 2c34 392e 3237 2038 352e 3035 2c34  94,49.27 85.05,4
+00000d10: 392e 3633 2038 352e 3132 2c34 392e 3943  9.63 85.12,49.9C
+00000d20: 3835 2e32 382c 3530 2e35 2038 352e 3434  85.28,50.5 85.44
+00000d30: 2c35 312e 3120 3835 2e35 352c 3531 2e37  ,51.1 85.55,51.7
+00000d40: 3343 3835 2e36 3931 2c35 322e 3530 3720  3C85.691,52.507 
+00000d50: 3835 2e37 3932 2c35 332e 3239 3220 3835  85.792,53.292 85
+00000d60: 2e38 352c 3534 2e30 384c 3835 2e38 352c  .85,54.08L85.85,
+00000d70: 3535 2e38 3943 3835 2e38 352c 3536 2e31  55.89C85.85,56.1
+00000d80: 3220 3835 2e39 312c 3536 2e32 3520 3835  2 85.91,56.25 85
+00000d90: 2e39 312c 3536 2e34 354c 3835 2e38 392c  .91,56.45L85.89,
+00000da0: 3536 2e34 345a 4d31 372e 3636 2c36 3843  56.44ZM17.66,68C
+00000db0: 3136 2e36 3638 2c36 362e 3433 3520 3135  16.668,66.435 15
+00000dc0: 2e38 3639 2c36 342e 3735 3620 3135 2e32  .869,64.756 15.2
+00000dd0: 382c 3633 4c31 352e 3137 2c36 322e 3638  8,63L15.17,62.68
+00000de0: 4331 352e 3036 2c36 322e 3335 2031 342e  C15.06,62.35 14.
+00000df0: 3936 2c36 322e 3031 2031 342e 3837 2c36  96,62.01 14.87,6
+00000e00: 312e 3638 4331 342e 3832 332c 3631 2e34  1.68C14.823,61.4
+00000e10: 3933 2031 342e 3737 372c 3631 2e33 3120  93 14.777,61.31 
+00000e20: 3134 2e37 332c 3631 2e31 3343 3134 2e36  14.73,61.13C14.6
+00000e30: 362c 3630 2e38 3420 3134 2e35 392c 3630  6,60.84 14.59,60
+00000e40: 2e35 3520 3134 2e35 332c 3630 2e32 3743  .55 14.53,60.27C
+00000e50: 3134 2e34 372c 3539 2e39 3920 3134 2e34  14.47,59.99 14.4
+00000e60: 332c 3539 2e37 3220 3134 2e33 382c 3539  3,59.72 14.38,59
+00000e70: 2e34 3443 3134 2e33 332c 3539 2e31 3620  .44C14.33,59.16 
+00000e80: 3134 2e33 2c35 3920 3134 2e32 372c 3538  14.3,59 14.27,58
+00000e90: 2e37 3843 3134 2e32 2c35 382e 3237 2031  .78C14.2,58.27 1
+00000ea0: 342e 3135 2c35 372e 3738 2031 342e 3131  4.15,57.78 14.11
+00000eb0: 2c35 372e 3233 4c31 342e 3131 2c35 372e  ,57.23L14.11,57.
+00000ec0: 3033 4331 342e 3030 382c 3535 2e32 3336  03C14.008,55.236
+00000ed0: 2031 342e 3132 322c 3533 2e34 3337 2031   14.122,53.437 1
+00000ee0: 342e 3435 2c35 312e 3637 4331 342e 3536  4.45,51.67C14.56
+00000ef0: 2c35 312e 3036 2031 342e 3731 2c35 302e  ,51.06 14.71,50.
+00000f00: 3436 2031 342e 3838 2c34 392e 3837 4331  46 14.88,49.87C1
+00000f10: 342e 3936 2c34 392e 3539 2031 352e 3034  4.96,49.59 15.04
+00000f20: 2c34 392e 3332 2031 352e 3133 2c34 392e  ,49.32 15.13,49.
+00000f30: 3035 4331 352e 3232 2c34 382e 3738 2031  05C15.22,48.78 1
+00000f40: 352e 3234 2c34 382e 3732 2031 352e 332c  5.24,48.72 15.3,
+00000f50: 3438 2e35 3543 3136 2e35 3438 2c34 372e  48.55C16.548,47.
+00000f60: 3737 3420 3137 2e38 3539 2c34 372e 3130  774 17.859,47.10
+00000f70: 3520 3139 2e32 322c 3436 2e35 3543 3237  5 19.22,46.55C27
+00000f80: 2e38 362c 3433 2e30 3920 3336 2e36 352c  .86,43.09 36.65,
+00000f90: 3434 2e36 3720 3338 2e38 322c 3530 2e30  44.67 38.82,50.0
+00000fa0: 3843 3430 2e39 392c 3535 2e34 3920 3335  8C40.99,55.49 35
+00000fb0: 2e37 332c 3632 2e37 3420 3237 2e30 392c  .73,62.74 27.09,
+00000fc0: 3636 2e32 4332 342e 3130 312c 3637 2e34  66.2C24.101,67.4
+00000fd0: 3331 2032 302e 3839 332c 3638 2e30 3433  31 20.893,68.043
+00000fe0: 2031 372e 3636 2c36 385a 4d36 382e 3537   17.66,68ZM68.57
+00000ff0: 2c37 372e 3638 4336 322e 3535 342c 3739  ,77.68C62.554,79
+00001000: 2e35 3038 2035 362e 3238 372c 3830 2e33  .508 56.287,80.3
+00001010: 3736 2035 302c 3830 2e32 3543 3433 2e37  76 50,80.25C43.7
+00001020: 3337 2c38 302e 3337 2033 372e 3439 352c  37,80.37 37.495,
+00001030: 3739 2e35 3036 2033 312e 352c 3737 2e36  79.506 31.5,77.6
+00001040: 3943 3237 2e31 3835 2c37 362e 3338 2032  9C27.185,76.38 2
+00001050: 332e 3234 332c 3734 2e30 3632 2032 302c  3.243,74.062 20,
+00001060: 3730 2e39 3343 3232 2e38 3135 2c37 302e  70.93C22.815,70.
+00001070: 3730 3620 3235 2e35 382c 3730 2e30 3535  706 25.58,70.055
+00001080: 2032 382e 322c 3639 4333 382e 3337 2c36   28.2,69C38.37,6
+00001090: 342e 3932 2034 342e 3339 2c35 3620 3431  4.92 44.39,56 41
+000010a0: 2e36 2c34 3943 3338 2e38 312c 3432 2032  .6,49C38.81,42 2
+000010b0: 382e 3237 2c33 392e 3732 2031 382e 312c  8.27,39.72 18.1,
+000010c0: 3433 2e38 4c31 372e 3433 2c34 342e 3039  43.8L17.43,44.09
+000010d0: 4331 382e 3937 332c 3431 2e36 3438 2032  C18.973,41.648 2
+000010e0: 312e 3031 392c 3339 2e35 3631 2032 332e  1.019,39.561 23.
+000010f0: 3433 2c33 372e 3937 4332 362e 3637 312c  43,37.97C26.671,
+00001100: 3335 2e38 3234 2033 302e 3437 332c 3334  35.824 30.473,34
+00001110: 2e36 3820 3334 2e33 362c 3334 2e36 3843  .68 34.36,34.68C
+00001120: 3335 2e38 3834 2c33 342e 3638 3120 3337  35.884,34.681 37
+00001130: 2e34 3034 2c33 342e 3835 3220 3338 2e38  .404,34.852 38.8
+00001140: 392c 3335 2e31 3943 3432 2e36 3934 2c33  9,35.19C42.694,3
+00001150: 362e 3034 3920 3436 2e31 3931 2c33 372e  6.049 46.191,37.
+00001160: 3933 3520 3439 2c34 302e 3634 4c35 302c  935 49,40.64L50,
+00001170: 3431 2e36 344c 3531 2c34 302e 3634 4335  41.64L51,40.64C5
+00001180: 332e 3739 372c 3337 2e39 3337 2035 372e  3.797,37.937 57.
+00001190: 3237 392c 3336 2e30 3439 2036 312e 3037  279,36.049 61.07
+000011a0: 2c33 352e 3138 4336 362e 3430 322c 3333  ,35.18C66.402,33
+000011b0: 2e39 3437 2037 322e 3031 342c 3334 2e39  .947 72.014,34.9
+000011c0: 3638 2037 362e 3537 2c33 3843 3738 2e39  68 76.57,38C78.9
+000011d0: 382c 3339 2e35 3838 2038 312e 3032 362c  8,39.588 81.026,
+000011e0: 3431 2e36 3731 2038 322e 3537 2c34 342e  41.671 82.57,44.
+000011f0: 3131 4c38 312e 392c 3433 2e38 3243 3737  11L81.9,43.82C77
+00001200: 2e34 3039 2c34 312e 3932 3120 3732 2e34  .409,41.921 72.4
+00001210: 3634 2c34 312e 3335 3520 3637 2e36 362c  64,41.355 67.66,
+00001220: 3432 2e31 3943 3633 2e30 382c 3433 2e31  42.19C63.08,43.1
+00001230: 3220 3539 2e37 392c 3435 2e35 3420 3538  2 59.79,45.54 58
+00001240: 2e33 392c 3439 2e30 3243 3535 2e36 2c35  .39,49.02C55.6,5
+00001250: 352e 3937 2036 312e 3632 2c36 342e 3934  5.97 61.62,64.94
+00001260: 2037 312e 3739 2c36 392e 3032 4337 342e   71.79,69.02C74.
+00001270: 3431 342c 3730 2e30 3720 3737 2e31 3832  414,70.07 77.182
+00001280: 2c37 302e 3731 3420 3830 2c37 302e 3933  ,70.714 80,70.93
+00001290: 4337 362e 3737 362c 3734 2e30 3520 3732  C76.776,74.05 72
+000012a0: 2e38 3539 2c37 362e 3336 3320 3638 2e35  .859,76.363 68.5
+000012b0: 372c 3737 2e36 385a 2220 7374 796c 653d  7,77.68Z" style=
+000012c0: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
+000012d0: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
+000012e0: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
+000012f0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00001300: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00001310: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+00001320: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+00001330: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
+00001340: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
+00001350: 7263 6c65 2063 783d 2237 312e 3333 2220  rcle cx="71.33" 
+00001360: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
+00001370: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
+00001380: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
+00001390: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
+000013a0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
+000013b0: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
+000013c0: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
+000013d0: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
+000013e0: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
+000013f0: 2020 3c63 6972 636c 6520 6378 3d22 3238    <circle cx="28
+00001400: 2e36 3722 2063 793d 2235 3622 2072 3d22  .67" cy="56" r="
+00001410: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
+00001420: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
+00001430: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
+00001440: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
+00001450: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00001460: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
+00001470: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
+00001480: 362e 3638 3538 3229 223e 0a20 2020 2020  6.68582)">.     
+00001490: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
+000014a0: 4d35 382c 3636 4335 352e 3931 322c 3638  M58,66C55.912,68
+000014b0: 2e31 3631 2035 332e 3030 332c 3639 2e33  .161 53.003,69.3
+000014c0: 3339 2035 302c 3639 2e32 3443 3436 2e39  39 50,69.24C46.9
+000014d0: 3937 2c36 392e 3333 3920 3434 2e30 3838  97,69.339 44.088
+000014e0: 2c36 382e 3136 3120 3432 2c36 3643 3431  ,68.161 42,66C41
+000014f0: 2e37 3134 2c36 352e 3637 3720 3431 2e33  .714,65.677 41.3
+00001500: 3032 2c36 352e 3439 3120 3430 2e38 372c  02,65.491 40.87,
+00001510: 3635 2e34 3931 4334 302e 3034 322c 3635  65.491C40.042,65
+00001520: 2e34 3931 2033 392e 3336 312c 3636 2e31  .491 39.361,66.1
+00001530: 3732 2033 392e 3336 312c 3637 4333 392e  72 39.361,67C39.
+00001540: 3336 312c 3637 2e33 3638 2033 392e 3439  361,67.368 39.49
+00001550: 362c 3637 2e37 3234 2033 392e 3734 2c36  6,67.724 39.74,6
+00001560: 3843 3432 2e34 3033 2c37 302e 3830 3420  8C42.403,70.804 
+00001570: 3436 2e31 3334 2c37 322e 3335 2035 302c  46.134,72.35 50,
+00001580: 3732 2e32 3543 3533 2e38 3632 2c37 322e  72.25C53.862,72.
+00001590: 3334 3720 3537 2e35 392c 3730 2e38 3032  347 57.59,70.802
+000015a0: 2036 302e 3235 2c36 3843 3630 2e34 3935   60.25,68C60.495
+000015b0: 2c36 372e 3732 3520 3630 2e36 332c 3637  ,67.725 60.63,67
+000015c0: 2e33 3639 2036 302e 3633 2c36 3743 3630  .369 60.63,67C60
+000015d0: 2e36 332c 3636 2e31 3734 2035 392e 3935  .63,66.174 59.95
+000015e0: 312c 3635 2e34 3935 2035 392e 3132 352c  1,65.495 59.125,
+000015f0: 3635 2e34 3935 4335 382e 3639 352c 3635  65.495C58.695,65
+00001600: 2e34 3935 2035 382e 3238 352c 3635 2e36  .495 58.285,65.6
+00001610: 3739 2035 382c 3636 5a22 2073 7479 6c65  79 58,66Z" style
+00001620: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
+00001630: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
+00001640: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
+00001650: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
+00001660: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.svg`

 * *Files 4% similar despite different names*

```diff
@@ -1,359 +1,361 @@
 00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3133 3222 2068  k" width="132" h
-00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
+00000050: 6b22 2077 6964 7468 3d22 3230 3022 2068  k" width="200" h
+00000060: 6569 6768 743d 2232 3822 2072 6f6c 653d  eight="28" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 696e 7465 7272 6f67 6174 653a 202d  ="interrogate: -
-00000090: 312e 3025 223e 0a20 2020 203c 7469 746c  1.0%">.    <titl
-000000a0: 653e 696e 7465 7272 6f67 6174 653a 202d  e>interrogate: -
-000000b0: 312e 3025 3c2f 7469 746c 653e 0a20 2020  1.0%</title>.   
+00000080: 3d22 494e 5445 5252 4f47 4154 453a 2039  ="INTERROGATE: 9
+00000090: 392e 3925 223e 0a20 2020 203c 7469 746c  9.9%">.    <titl
+000000a0: 653e 494e 5445 5252 4f47 4154 453a 2039  e>INTERROGATE: 9
+000000b0: 392e 3925 3c2f 7469 746c 653e 0a20 2020  9.9%</title>.   
 000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
 000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
-000000f0: 7769 6474 683d 2239 3322 2068 6569 6768  width="93" heigh
-00000100: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
-00000110: 3522 2f3e 0a20 2020 2020 2020 203c 7265  5"/>.        <re
-00000120: 6374 2078 3d22 3933 2220 7769 6474 683d  ct x="93" width=
-00000130: 2233 3922 2068 6569 6768 743d 2232 3022  "39" height="20"
-00000140: 2066 696c 6c3d 2223 3966 3966 3966 222f   fill="#9f9f9f"/
-00000150: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
-00000160: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
-00000170: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
-00000180: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
-00000190: 5665 7264 616e 612c 4765 6e65 7661 2c44  Verdana,Geneva,D
-000001a0: 656a 6156 7520 5361 6e73 2c73 616e 732d  ejaVu Sans,sans-
-000001b0: 7365 7269 6622 2074 6578 742d 7265 6e64  serif" text-rend
-000001c0: 6572 696e 673d 2267 656f 6d65 7472 6963  ering="geometric
-000001d0: 5072 6563 6973 696f 6e22 2066 6f6e 742d  Precision" font-
-000001e0: 7369 7a65 3d22 3131 3022 3e0a 2020 2020  size="110">.    
-000001f0: 2020 2020 3c74 6578 7420 783d 2235 3930      <text x="590
-00000200: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
-00000210: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
-00000220: 6669 6c6c 3d22 2366 6666 2220 7465 7874  fill="#fff" text
-00000230: 4c65 6e67 7468 3d22 3631 3022 3e69 6e74  Length="610">int
-00000240: 6572 726f 6761 7465 3c2f 7465 7874 3e0a  errogate</text>.
-00000250: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
-00000260: 2231 3132 3022 2079 3d22 3134 3022 2074  "1120" y="140" t
-00000270: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00000280: 2e31 2922 2066 696c 6c3d 2223 6666 6622  .1)" fill="#fff"
-00000290: 2074 6578 744c 656e 6774 683d 2232 3930   textLength="290
-000002a0: 2220 6461 7461 2d69 6e74 6572 726f 6761  " data-interroga
-000002b0: 7465 3d22 7265 7375 6c74 223e 2d31 2e30  te="result">-1.0
-000002c0: 253c 2f74 6578 743e 0a20 2020 203c 2f67  %</text>.    </g
-000002d0: 3e0a 2020 2020 3c67 2069 643d 226c 6f67  >.    <g id="log
-000002e0: 6f2d 7069 6e6b 2220 7472 616e 7366 6f72  o-pink" transfor
-000002f0: 6d3d 226d 6174 7269 7828 302e 3835 3438  m="matrix(0.8548
-00000300: 3736 2c30 2c30 2c30 2e38 3534 3837 362c  76,0,0,0.854876,
-00000310: 2d36 2e37 3335 3134 2c30 2e38 3737 3132  -6.73514,0.87712
-00000320: 3429 223e 0a20 2020 2020 2020 203c 6720  4)">.        <g 
-00000330: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00000340: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-00000350: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00000360: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
-00000370: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-00000380: 224d 3530 2c36 342e 3235 4335 322e 3736  "M50,64.25C52.76
-00000390: 2c36 342e 3235 2035 352c 3631 2e31 3320  ,64.25 55,61.13 
-000003a0: 3535 2c35 392e 3735 4335 352c 3538 2e33  55,59.75C55,58.3
-000003b0: 3720 3532 2e37 362c 3537 2e32 3520 3530  7 52.76,57.25 50
-000003c0: 2c35 372e 3235 4334 372e 3234 2c35 372e  ,57.25C47.24,57.
-000003d0: 3235 2034 352c 3538 2e33 3720 3435 2c35  25 45,58.37 45,5
-000003e0: 392e 3735 4334 352c 3631 2e31 3320 3437  9.75C45,61.13 47
-000003f0: 2e32 342c 3634 2e32 3520 3530 2c36 342e  .24,64.25 50,64.
-00000400: 3235 5a22 2073 7479 6c65 3d22 6669 6c6c  25Z" style="fill
-00000410: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
-00000420: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
-00000430: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
-00000440: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
-00000450: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00000460: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-00000470: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00000480: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
-00000490: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-000004a0: 224d 3838 2c34 392e 3035 4338 362e 3530  "M88,49.05C86.50
-000004b0: 362c 3433 2e34 3735 2038 332e 3031 382c  6,43.475 83.018,
-000004c0: 3338 2e36 3338 2037 382e 322c 3335 2e34  38.638 78.2,35.4
-000004d0: 3643 3732 2e39 3639 2c33 322e 3030 3220  6C72.969,32.002 
-000004e0: 3636 2e35 3339 2c33 302e 3834 3420 3630  66.539,30.844 60
-000004f0: 2e34 332c 3332 2e32 3643 3536 2e35 3736  .43,32.26C56.576
-00000500: 2c33 332e 3134 3520 3532 2e39 3935 2c33  ,33.145 52.995,3
-00000510: 342e 3935 3820 3530 2c33 372e 3534 4334  4.958 50,37.54C4
-00000520: 362e 3939 382c 3334 2e39 3538 2034 332e  6.998,34.958 43.
-00000530: 3431 312c 3333 2e31 3439 2033 392e 3535  411,33.149 39.55
-00000540: 2c33 322e 3237 4333 332e 3434 312c 3330  ,32.27C33.441,30
-00000550: 2e38 3533 2032 372e 3031 312c 3332 2e30  .853 27.011,32.0
-00000560: 3131 2032 312e 3738 2c33 352e 3437 4331  11 21.78,35.47C1
-00000570: 362e 3937 2c33 382e 3635 3220 3133 2e34  6.97,38.652 13.4
-00000580: 3839 2c34 332e 3438 3920 3132 2c34 392e  89,43.489 12,49.
-00000590: 3036 4c31 322c 3439 2e31 3343 3131 2e38  06L12,49.13C11.8
-000005a0: 322c 3439 2e37 3920 3131 2e36 362c 3530  2,49.79 11.66,50
-000005b0: 2e34 3620 3131 2e35 332c 3531 2e31 3343  .46 11.53,51.13C
-000005c0: 3131 2e31 3436 2c35 332e 3230 3720 3131  11.146,53.207 11
-000005d0: 2e30 3231 2c35 352e 3332 3320 3131 2e31  .021,55.323 11.1
-000005e0: 362c 3537 2e34 3343 3131 2e31 362c 3538  6,57.43C11.16,58
-000005f0: 2e30 3320 3131 2e32 362c 3538 2e36 3320  .03 11.26,58.63 
-00000600: 3131 2e33 342c 3539 2e32 3343 3131 2e33  11.34,59.23C11.3
-00000610: 342c 3539 2e35 3120 3131 2e34 332c 3539  4,59.51 11.43,59
-00000620: 2e37 3920 3131 2e34 382c 3630 2e30 3743  .79 11.48,60.07C
-00000630: 3131 2e35 332c 3630 2e33 3520 3131 2e35  11.53,60.35 11.5
-00000640: 382c 3630 2e36 3820 3131 2e36 342c 3630  8,60.68 11.64,60
-00000650: 2e39 3843 3131 2e37 2c36 312e 3238 2031  .98C11.7,61.28 1
-00000660: 312e 382c 3631 2e36 3920 3131 2e38 392c  1.8,61.69 11.89,
-00000670: 3632 2e30 3543 3131 2e39 382c 3632 2e34  62.05C11.98,62.4
-00000680: 3120 3131 2e39 392c 3632 2e34 3720 3132  1 11.99,62.47 12
-00000690: 2e30 352c 3632 2e36 3843 3132 2e31 362c  .05,62.68C12.16,
-000006a0: 3633 2e30 3720 3132 2e32 382c 3633 2e34  63.07 12.28,63.4
-000006b0: 3620 3132 2e34 312c 3633 2e38 344c 3132  6 12.41,63.84L12
-000006c0: 2e35 382c 3634 2e33 3443 3132 2e37 322c  .58,64.34C12.72,
-000006d0: 3634 2e37 3420 3132 2e38 382c 3635 2e31  64.74 12.88,65.1
-000006e0: 3420 3133 2e30 342c 3635 2e35 334c 3133  4 13.04,65.53L13
-000006f0: 2e32 332c 3635 2e39 3843 3133 2e34 3033  .23,65.98C13.403
-00000700: 2c36 362e 3337 3320 3133 2e35 3833 2c36  ,66.373 13.583,6
-00000710: 362e 3736 3720 3133 2e37 372c 3637 2e31  6.767 13.77,67.1
-00000720: 364c 3133 2e39 392c 3637 2e35 3943 3134  6L13.99,67.59C14
-00000730: 2e31 392c 3637 2e39 3720 3134 2e33 392c  .19,67.97 14.39,
-00000740: 3638 2e33 3520 3134 2e36 312c 3638 2e37  68.35 14.61,68.7
-00000750: 334c 3134 2e38 372c 3639 2e31 3543 3135  3L14.87,69.15C15
-00000760: 2e31 2c36 392e 3532 2031 352e 3333 2c36  .1,69.52 15.33,6
-00000770: 392e 3839 2031 352e 3538 2c37 302e 3236  9.89 15.58,70.26
-00000780: 4c31 352e 3538 2c37 302e 3332 4c31 352e  L15.58,70.32L15.
-00000790: 3939 2c37 302e 3933 4331 362e 3134 2c37  99,70.93C16.14,7
-000007a0: 312e 3134 2031 362e 3239 2c37 312e 3336  1.14 16.29,71.36
-000007b0: 2031 362e 3435 2c37 312e 3537 4332 302e   16.45,71.57C20.
-000007c0: 3230 362c 3735 2e38 3320 3235 2e30 3836  206,75.83 25.086
-000007d0: 2c37 382e 3935 2033 302e 3533 2c38 302e  ,78.95 30.53,80.
-000007e0: 3537 4333 362e 3833 392c 3832 2e34 3820  57C36.839,82.48 
-000007f0: 3433 2e34 312c 3833 2e33 3835 2035 302c  43.41,83.385 50,
-00000800: 3833 2e32 3543 3536 2e35 3939 2c38 332e  83.25C56.599,83.
-00000810: 3337 3420 3633 2e31 3737 2c38 322e 3435  374 63.177,82.45
-00000820: 3620 3639 2e34 392c 3830 2e35 3343 3734  6 69.49,80.53C74
-00000830: 2e36 3434 2c37 382e 3937 3820 3739 2e33  .644,78.978 79.3
-00000840: 3033 2c37 362e 3130 3220 3833 2c37 322e  03,76.102 83,72.
-00000850: 3139 4338 332e 3334 2c37 312e 3738 2038  19C83.34,71.78 8
-00000860: 332e 3635 2c37 312e 3335 2038 342c 3730  3.65,71.35 84,70
-00000870: 2e39 324c 3834 2e31 382c 3730 2e36 364c  .92L84.18,70.66L
-00000880: 3834 2e33 332c 3730 2e34 344c 3834 2e34  84.33,70.44L84.4
-00000890: 312c 3730 2e33 3243 3834 2e35 352c 3730  1,70.32C84.55,70
-000008a0: 2e31 3220 3834 2e36 372c 3639 2e39 2038  .12 84.67,69.9 8
-000008b0: 342e 3831 2c36 392e 3743 3835 2e30 372c  4.81,69.7C85.07,
-000008c0: 3639 2e33 2038 352e 3332 2c36 382e 3839  69.3 85.32,68.89
-000008d0: 2038 352e 3535 2c36 382e 3438 4338 352e   85.55,68.48C85.
-000008e0: 3738 2c36 382e 3037 2038 362e 3032 2c36  78,68.07 86.02,6
-000008f0: 372e 3635 2038 362e 3233 2c36 372e 3232  7.65 86.23,67.22
-00000900: 4338 362e 3331 2c36 372e 3035 2038 362e  C86.31,67.05 86.
-00000910: 3339 2c36 362e 3838 2038 362e 3437 2c36  39,66.88 86.47,6
-00000920: 362e 3743 3836 2e36 372c 3636 2e32 3820  6.7C86.67,66.28 
-00000930: 3836 2e38 352c 3635 2e38 3720 3837 2e30  86.85,65.87 87.0
-00000940: 332c 3635 2e34 344c 3837 2e32 332c 3634  3,65.44L87.23,64
-00000950: 2e39 3243 3837 2e33 3937 2c36 342e 3438  .92C87.397,64.48
-00000960: 3720 3837 2e35 352c 3634 2e30 3520 3837  7 87.55,64.05 87
-00000970: 2e36 392c 3633 2e36 314c 3837 2e38 352c  .69,63.61L87.85,
-00000980: 3633 2e30 3943 3837 2e39 382c 3632 2e36  63.09C87.98,62.6
-00000990: 3420 3838 2e31 2c36 322e 3139 2038 382e  4 88.1,62.19 88.
-000009a0: 3231 2c36 312e 3734 4338 382e 3231 2c36  21,61.74C88.21,6
-000009b0: 312e 3537 2038 382e 332c 3631 2e33 3920  1.57 88.3,61.39 
-000009c0: 3838 2e33 332c 3631 2e32 3243 3838 2e34  88.33,61.22C88.4
-000009d0: 332c 3630 2e37 3520 3838 2e35 322c 3630  3,60.75 88.52,60
-000009e0: 2e32 3220 3838 2e36 2c35 392e 3739 4338  .22 88.6,59.79C8
-000009f0: 382e 362c 3539 2e36 3420 3838 2e36 362c  8.6,59.64 88.66,
-00000a00: 3539 2e34 3920 3838 2e36 382c 3539 2e33  59.49 88.68,59.3
-00000a10: 3343 3838 2e37 372c 3538 2e37 3120 3838  3C88.77,58.71 88
-00000a20: 2e38 342c 3538 2e30 3820 3838 2e38 382c  .84,58.08 88.88,
-00000a30: 3537 2e34 354c 3838 2e38 382c 3534 2e31  57.45L88.88,54.1
-00000a40: 3743 3838 2e38 3137 2c35 332e 3136 3420  7C88.817,53.164 
-00000a50: 3838 2e36 3933 2c35 322e 3136 3220 3838  88.693,52.162 88
-00000a60: 2e35 312c 3531 2e31 3743 3838 2e33 382c  .51,51.17C88.38,
-00000a70: 3530 2e35 2038 382e 3233 2c34 392e 3834  50.5 88.23,49.84
-00000a80: 2038 382e 3035 2c34 392e 3137 4c38 382c   88.05,49.17L88,
-00000a90: 3439 2e30 355a 4d38 352e 3839 2c35 362e  49.05ZM85.89,56.
-00000aa0: 3434 4c38 352e 3839 2c35 372e 3233 4338  44L85.89,57.23C8
-00000ab0: 352e 3839 2c35 372e 3738 2038 352e 3739  5.89,57.78 85.79
-00000ac0: 2c35 382e 3332 2038 352e 3732 2c35 382e  ,58.32 85.72,58.
-00000ad0: 3836 4338 352e 3732 2c35 392e 3031 2038  86C85.72,59.01 8
-00000ae0: 352e 3732 2c35 392e 3135 2038 352e 3635  5.72,59.15 85.65
-00000af0: 2c35 392e 3343 3835 2e35 392c 3539 2e37  ,59.3C85.59,59.7
-00000b00: 2038 352e 3531 2c36 302e 3131 2038 352e   85.51,60.11 85.
-00000b10: 3433 2c36 302e 3531 4c38 352e 3332 2c36  43,60.51L85.32,6
-00000b20: 302e 3939 4338 352e 3233 2c36 312e 3338  0.99C85.23,61.38
-00000b30: 2038 352e 3132 2c36 312e 3737 2038 352e   85.12,61.77 85.
-00000b40: 3031 2c36 322e 3136 4338 352e 3031 2c36  01,62.16C85.01,6
-00000b50: 322e 3331 2038 342e 3933 2c36 322e 3436  2.31 84.93,62.46
-00000b60: 2038 342e 3838 2c36 322e 3643 3834 2e37   84.88,62.6C84.7
-00000b70: 342c 3633 2e30 3420 3834 2e35 392c 3633  4,63.04 84.59,63
-00000b80: 2e34 3720 3834 2e34 322c 3633 2e39 4c38  .47 84.42,63.9L8
-00000b90: 342e 3237 2c36 342e 3238 4338 342e 312c  4.27,64.28C84.1,
-00000ba0: 3634 2e37 3120 3833 2e39 312c 3635 2e31  64.71 83.91,65.1
-00000bb0: 3420 3833 2e37 312c 3635 2e35 3643 3833  4 83.71,65.56C83
-00000bc0: 2e35 312c 3635 2e39 3820 3833 2e34 332c  .51,65.98 83.43,
-00000bd0: 3636 2e31 3220 3833 2e32 382c 3636 2e34  66.12 83.28,66.4
-00000be0: 4c38 332e 3031 2c36 362e 3931 4338 322e  L83.01,66.91C82.
-00000bf0: 3833 2c36 372e 3232 3320 3832 2e36 3433  83,67.223 82.643
-00000c00: 2c36 372e 3533 3720 3832 2e34 352c 3637  ,67.537 82.45,67
-00000c10: 2e38 354c 3832 2e33 352c 3638 2e30 3143  .85L82.35,68.01C
-00000c20: 3739 2e31 3231 2c36 382e 3034 3720 3735  79.121,68.047 75
-00000c30: 2e39 3138 2c36 372e 3433 3420 3732 2e39  .918,67.434 72.9
-00000c40: 332c 3636 2e32 3143 3634 2e32 372c 3632  3,66.21C64.27,62
-00000c50: 2e37 3420 3539 2c35 352e 3532 2036 312e  .74 59,55.52 61.
-00000c60: 3138 2c35 302e 3131 4336 322e 3138 2c34  18,50.11C62.18,4
-00000c70: 372e 3620 3634 2e37 2c34 352e 3832 2036  7.6 64.7,45.82 6
-00000c80: 382e 3236 2c34 352e 3131 4337 322e 3438  8.26,45.11C72.48
-00000c90: 392c 3434 2e33 3935 2037 362e 3833 352c  9,44.395 76.835,
-00000ca0: 3434 2e39 3038 2038 302e 3738 2c34 362e  44.908 80.78,46.
-00000cb0: 3539 4338 322e 3134 312c 3437 2e31 3434  59C82.141,47.144
-00000cc0: 2038 332e 3435 332c 3437 2e38 3133 2038   83.453,47.813 8
-00000cd0: 342e 372c 3438 2e35 3943 3834 2e37 362c  4.7,48.59C84.76,
-00000ce0: 3438 2e37 3620 3834 2e38 322c 3438 2e39  48.76 84.82,48.9
-00000cf0: 3320 3834 2e38 382c 3439 2e31 4338 342e  3 84.88,49.1C84.
-00000d00: 3934 2c34 392e 3237 2038 352e 3035 2c34  94,49.27 85.05,4
-00000d10: 392e 3633 2038 352e 3132 2c34 392e 3943  9.63 85.12,49.9C
-00000d20: 3835 2e32 382c 3530 2e35 2038 352e 3434  85.28,50.5 85.44
-00000d30: 2c35 312e 3120 3835 2e35 352c 3531 2e37  ,51.1 85.55,51.7
-00000d40: 3343 3835 2e36 3931 2c35 322e 3530 3720  3C85.691,52.507 
-00000d50: 3835 2e37 3932 2c35 332e 3239 3220 3835  85.792,53.292 85
-00000d60: 2e38 352c 3534 2e30 384c 3835 2e38 352c  .85,54.08L85.85,
-00000d70: 3535 2e38 3943 3835 2e38 352c 3536 2e31  55.89C85.85,56.1
-00000d80: 3220 3835 2e39 312c 3536 2e32 3520 3835  2 85.91,56.25 85
-00000d90: 2e39 312c 3536 2e34 354c 3835 2e38 392c  .91,56.45L85.89,
-00000da0: 3536 2e34 345a 4d31 372e 3636 2c36 3843  56.44ZM17.66,68C
-00000db0: 3136 2e36 3638 2c36 362e 3433 3520 3135  16.668,66.435 15
-00000dc0: 2e38 3639 2c36 342e 3735 3620 3135 2e32  .869,64.756 15.2
-00000dd0: 382c 3633 4c31 352e 3137 2c36 322e 3638  8,63L15.17,62.68
-00000de0: 4331 352e 3036 2c36 322e 3335 2031 342e  C15.06,62.35 14.
-00000df0: 3936 2c36 322e 3031 2031 342e 3837 2c36  96,62.01 14.87,6
-00000e00: 312e 3638 4331 342e 3832 332c 3631 2e34  1.68C14.823,61.4
-00000e10: 3933 2031 342e 3737 372c 3631 2e33 3120  93 14.777,61.31 
-00000e20: 3134 2e37 332c 3631 2e31 3343 3134 2e36  14.73,61.13C14.6
-00000e30: 362c 3630 2e38 3420 3134 2e35 392c 3630  6,60.84 14.59,60
-00000e40: 2e35 3520 3134 2e35 332c 3630 2e32 3743  .55 14.53,60.27C
-00000e50: 3134 2e34 372c 3539 2e39 3920 3134 2e34  14.47,59.99 14.4
-00000e60: 332c 3539 2e37 3220 3134 2e33 382c 3539  3,59.72 14.38,59
-00000e70: 2e34 3443 3134 2e33 332c 3539 2e31 3620  .44C14.33,59.16 
-00000e80: 3134 2e33 2c35 3920 3134 2e32 372c 3538  14.3,59 14.27,58
-00000e90: 2e37 3843 3134 2e32 2c35 382e 3237 2031  .78C14.2,58.27 1
-00000ea0: 342e 3135 2c35 372e 3738 2031 342e 3131  4.15,57.78 14.11
-00000eb0: 2c35 372e 3233 4c31 342e 3131 2c35 372e  ,57.23L14.11,57.
-00000ec0: 3033 4331 342e 3030 382c 3535 2e32 3336  03C14.008,55.236
-00000ed0: 2031 342e 3132 322c 3533 2e34 3337 2031   14.122,53.437 1
-00000ee0: 342e 3435 2c35 312e 3637 4331 342e 3536  4.45,51.67C14.56
-00000ef0: 2c35 312e 3036 2031 342e 3731 2c35 302e  ,51.06 14.71,50.
-00000f00: 3436 2031 342e 3838 2c34 392e 3837 4331  46 14.88,49.87C1
-00000f10: 342e 3936 2c34 392e 3539 2031 352e 3034  4.96,49.59 15.04
-00000f20: 2c34 392e 3332 2031 352e 3133 2c34 392e  ,49.32 15.13,49.
-00000f30: 3035 4331 352e 3232 2c34 382e 3738 2031  05C15.22,48.78 1
-00000f40: 352e 3234 2c34 382e 3732 2031 352e 332c  5.24,48.72 15.3,
-00000f50: 3438 2e35 3543 3136 2e35 3438 2c34 372e  48.55C16.548,47.
-00000f60: 3737 3420 3137 2e38 3539 2c34 372e 3130  774 17.859,47.10
-00000f70: 3520 3139 2e32 322c 3436 2e35 3543 3237  5 19.22,46.55C27
-00000f80: 2e38 362c 3433 2e30 3920 3336 2e36 352c  .86,43.09 36.65,
-00000f90: 3434 2e36 3720 3338 2e38 322c 3530 2e30  44.67 38.82,50.0
-00000fa0: 3843 3430 2e39 392c 3535 2e34 3920 3335  8C40.99,55.49 35
-00000fb0: 2e37 332c 3632 2e37 3420 3237 2e30 392c  .73,62.74 27.09,
-00000fc0: 3636 2e32 4332 342e 3130 312c 3637 2e34  66.2C24.101,67.4
-00000fd0: 3331 2032 302e 3839 332c 3638 2e30 3433  31 20.893,68.043
-00000fe0: 2031 372e 3636 2c36 385a 4d36 382e 3537   17.66,68ZM68.57
-00000ff0: 2c37 372e 3638 4336 322e 3535 342c 3739  ,77.68C62.554,79
-00001000: 2e35 3038 2035 362e 3238 372c 3830 2e33  .508 56.287,80.3
-00001010: 3736 2035 302c 3830 2e32 3543 3433 2e37  76 50,80.25C43.7
-00001020: 3337 2c38 302e 3337 2033 372e 3439 352c  37,80.37 37.495,
-00001030: 3739 2e35 3036 2033 312e 352c 3737 2e36  79.506 31.5,77.6
-00001040: 3943 3237 2e31 3835 2c37 362e 3338 2032  9C27.185,76.38 2
-00001050: 332e 3234 332c 3734 2e30 3632 2032 302c  3.243,74.062 20,
-00001060: 3730 2e39 3343 3232 2e38 3135 2c37 302e  70.93C22.815,70.
-00001070: 3730 3620 3235 2e35 382c 3730 2e30 3535  706 25.58,70.055
-00001080: 2032 382e 322c 3639 4333 382e 3337 2c36   28.2,69C38.37,6
-00001090: 342e 3932 2034 342e 3339 2c35 3620 3431  4.92 44.39,56 41
-000010a0: 2e36 2c34 3943 3338 2e38 312c 3432 2032  .6,49C38.81,42 2
-000010b0: 382e 3237 2c33 392e 3732 2031 382e 312c  8.27,39.72 18.1,
-000010c0: 3433 2e38 4c31 372e 3433 2c34 342e 3039  43.8L17.43,44.09
-000010d0: 4331 382e 3937 332c 3431 2e36 3438 2032  C18.973,41.648 2
-000010e0: 312e 3031 392c 3339 2e35 3631 2032 332e  1.019,39.561 23.
-000010f0: 3433 2c33 372e 3937 4332 362e 3637 312c  43,37.97C26.671,
-00001100: 3335 2e38 3234 2033 302e 3437 332c 3334  35.824 30.473,34
-00001110: 2e36 3820 3334 2e33 362c 3334 2e36 3843  .68 34.36,34.68C
-00001120: 3335 2e38 3834 2c33 342e 3638 3120 3337  35.884,34.681 37
-00001130: 2e34 3034 2c33 342e 3835 3220 3338 2e38  .404,34.852 38.8
-00001140: 392c 3335 2e31 3943 3432 2e36 3934 2c33  9,35.19C42.694,3
-00001150: 362e 3034 3920 3436 2e31 3931 2c33 372e  6.049 46.191,37.
-00001160: 3933 3520 3439 2c34 302e 3634 4c35 302c  935 49,40.64L50,
-00001170: 3431 2e36 344c 3531 2c34 302e 3634 4335  41.64L51,40.64C5
-00001180: 332e 3739 372c 3337 2e39 3337 2035 372e  3.797,37.937 57.
-00001190: 3237 392c 3336 2e30 3439 2036 312e 3037  279,36.049 61.07
-000011a0: 2c33 352e 3138 4336 362e 3430 322c 3333  ,35.18C66.402,33
-000011b0: 2e39 3437 2037 322e 3031 342c 3334 2e39  .947 72.014,34.9
-000011c0: 3638 2037 362e 3537 2c33 3843 3738 2e39  68 76.57,38C78.9
-000011d0: 382c 3339 2e35 3838 2038 312e 3032 362c  8,39.588 81.026,
-000011e0: 3431 2e36 3731 2038 322e 3537 2c34 342e  41.671 82.57,44.
-000011f0: 3131 4c38 312e 392c 3433 2e38 3243 3737  11L81.9,43.82C77
-00001200: 2e34 3039 2c34 312e 3932 3120 3732 2e34  .409,41.921 72.4
-00001210: 3634 2c34 312e 3335 3520 3637 2e36 362c  64,41.355 67.66,
-00001220: 3432 2e31 3943 3633 2e30 382c 3433 2e31  42.19C63.08,43.1
-00001230: 3220 3539 2e37 392c 3435 2e35 3420 3538  2 59.79,45.54 58
-00001240: 2e33 392c 3439 2e30 3243 3535 2e36 2c35  .39,49.02C55.6,5
-00001250: 352e 3937 2036 312e 3632 2c36 342e 3934  5.97 61.62,64.94
-00001260: 2037 312e 3739 2c36 392e 3032 4337 342e   71.79,69.02C74.
-00001270: 3431 342c 3730 2e30 3720 3737 2e31 3832  414,70.07 77.182
-00001280: 2c37 302e 3731 3420 3830 2c37 302e 3933  ,70.714 80,70.93
-00001290: 4337 362e 3737 362c 3734 2e30 3520 3732  C76.776,74.05 72
-000012a0: 2e38 3539 2c37 362e 3336 3320 3638 2e35  .859,76.363 68.5
-000012b0: 372c 3737 2e36 385a 2220 7374 796c 653d  7,77.68Z" style=
-000012c0: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
-000012d0: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
-000012e0: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
-000012f0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00001300: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00001310: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-00001320: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-00001330: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
-00001340: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
-00001350: 7263 6c65 2063 783d 2237 312e 3333 2220  rcle cx="71.33" 
-00001360: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
-00001370: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
-00001380: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
-00001390: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-000013a0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-000013b0: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-000013c0: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-000013d0: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
-000013e0: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-000013f0: 2020 3c63 6972 636c 6520 6378 3d22 3238    <circle cx="28
-00001400: 2e36 3722 2063 793d 2235 3622 2072 3d22  .67" cy="56" r="
-00001410: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
-00001420: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
-00001430: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
-00001440: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
-00001450: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
-00001460: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
-00001470: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
-00001480: 362e 3638 3538 3229 223e 0a20 2020 2020  6.68582)">.     
-00001490: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
-000014a0: 4d35 382c 3636 4335 352e 3931 322c 3638  M58,66C55.912,68
-000014b0: 2e31 3631 2035 332e 3030 332c 3639 2e33  .161 53.003,69.3
-000014c0: 3339 2035 302c 3639 2e32 3443 3436 2e39  39 50,69.24C46.9
-000014d0: 3937 2c36 392e 3333 3920 3434 2e30 3838  97,69.339 44.088
-000014e0: 2c36 382e 3136 3120 3432 2c36 3643 3431  ,68.161 42,66C41
-000014f0: 2e37 3134 2c36 352e 3637 3720 3431 2e33  .714,65.677 41.3
-00001500: 3032 2c36 352e 3439 3120 3430 2e38 372c  02,65.491 40.87,
-00001510: 3635 2e34 3931 4334 302e 3034 322c 3635  65.491C40.042,65
-00001520: 2e34 3931 2033 392e 3336 312c 3636 2e31  .491 39.361,66.1
-00001530: 3732 2033 392e 3336 312c 3637 4333 392e  72 39.361,67C39.
-00001540: 3336 312c 3637 2e33 3638 2033 392e 3439  361,67.368 39.49
-00001550: 362c 3637 2e37 3234 2033 392e 3734 2c36  6,67.724 39.74,6
-00001560: 3843 3432 2e34 3033 2c37 302e 3830 3420  8C42.403,70.804 
-00001570: 3436 2e31 3334 2c37 322e 3335 2035 302c  46.134,72.35 50,
-00001580: 3732 2e32 3543 3533 2e38 3632 2c37 322e  72.25C53.862,72.
-00001590: 3334 3720 3537 2e35 392c 3730 2e38 3032  347 57.59,70.802
-000015a0: 2036 302e 3235 2c36 3843 3630 2e34 3935   60.25,68C60.495
-000015b0: 2c36 372e 3732 3520 3630 2e36 332c 3637  ,67.725 60.63,67
-000015c0: 2e33 3639 2036 302e 3633 2c36 3743 3630  .369 60.63,67C60
-000015d0: 2e36 332c 3636 2e31 3734 2035 392e 3935  .63,66.174 59.95
-000015e0: 312c 3635 2e34 3935 2035 392e 3132 352c  1,65.495 59.125,
-000015f0: 3635 2e34 3935 4335 382e 3639 352c 3635  65.495C58.695,65
-00001600: 2e34 3935 2035 382e 3238 352c 3635 2e36  .495 58.285,65.6
-00001610: 3739 2035 382c 3636 5a22 2073 7479 6c65  79 58,66Z" style
-00001620: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
-00001630: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
-00001640: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
-00001650: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
-00001660: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
+000000f0: 7769 6474 683d 2231 3332 2e37 3522 2068  width="132.75" h
+00000100: 6569 6768 743d 2232 3822 2066 696c 6c3d  eight="28" fill=
+00000110: 2223 3535 3522 2f3e 0a20 2020 2020 2020  "#555"/>.       
+00000120: 203c 7265 6374 2078 3d22 3133 322e 3735   <rect x="132.75
+00000130: 2220 7769 6474 683d 2236 372e 3235 2220  " width="67.25" 
+00000140: 6865 6967 6874 3d22 3238 2220 6669 6c6c  height="28" fill
+00000150: 3d22 2334 6331 222f 3e0a 2020 2020 3c2f  ="#4c1"/>.    </
+00000160: 673e 0a20 2020 203c 6720 6669 6c6c 3d22  g>.    <g fill="
+00000170: 2366 6666 2220 7465 7874 2d61 6e63 686f  #fff" text-ancho
+00000180: 723d 226d 6964 646c 6522 2066 6f6e 742d  r="middle" font-
+00000190: 6661 6d69 6c79 3d22 5665 7264 616e 612c  family="Verdana,
+000001a0: 4765 6e65 7661 2c44 656a 6156 7520 5361  Geneva,DejaVu Sa
+000001b0: 6e73 2c73 616e 732d 7365 7269 6622 2074  ns,sans-serif" t
+000001c0: 6578 742d 7265 6e64 6572 696e 673d 2267  ext-rendering="g
+000001d0: 656f 6d65 7472 6963 5072 6563 6973 696f  eometricPrecisio
+000001e0: 6e22 2066 6f6e 742d 7369 7a65 3d22 3130  n" font-size="10
+000001f0: 3022 3e0a 2020 2020 2020 2020 3c74 6578  0">.        <tex
+00000200: 7420 7472 616e 7366 6f72 6d3d 2273 6361  t transform="sca
+00000210: 6c65 282e 3129 2220 783d 2237 3730 2e37  le(.1)" x="770.7
+00000220: 3522 2079 3d22 3137 3522 2074 6578 744c  5" y="175" textL
+00000230: 656e 6774 683d 2238 3637 2e35 2220 6669  ength="867.5" fi
+00000240: 6c6c 3d22 2366 6666 223e 494e 5445 5252  ll="#fff">INTERR
+00000250: 4f47 4154 453c 2f74 6578 743e 0a20 2020  OGATE</text>.   
+00000260: 2020 2020 203c 7465 7874 2074 7261 6e73       <text trans
+00000270: 666f 726d 3d22 7363 616c 6528 2e31 2922  form="scale(.1)"
+00000280: 2078 3d22 3136 3630 2e37 3522 2079 3d22   x="1660.75" y="
+00000290: 3137 3522 2074 6578 744c 656e 6774 683d  175" textLength=
+000002a0: 2234 3332 2e35 2220 6669 6c6c 3d22 2366  "432.5" fill="#f
+000002b0: 6666 2220 666f 6e74 2d77 6569 6768 743d  ff" font-weight=
+000002c0: 2262 6f6c 6422 2064 6174 612d 696e 7465  "bold" data-inte
+000002d0: 7272 6f67 6174 653d 2272 6573 756c 7422  rrogate="result"
+000002e0: 3e39 392e 3925 3c2f 7465 7874 3e0a 2020  >99.9%</text>.  
+000002f0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
+00000300: 3d22 6c6f 676f 2d70 696e 6b22 2074 7261  ="logo-pink" tra
+00000310: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
+00000320: 2e38 3534 3837 362c 302c 302c 302e 3835  .854876,0,0,0.85
+00000330: 3438 3736 2c2d 342e 3733 3531 342c 302e  4876,-4.73514,0.
+00000340: 3837 3731 3234 2922 3e0a 2020 2020 2020  877124)">.      
+00000350: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00000360: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+00000370: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+00000380: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
+00000390: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
+000003a0: 7468 2064 3d22 4d35 302c 3634 2e32 3543  th d="M50,64.25C
+000003b0: 3532 2e37 362c 3634 2e32 3520 3535 2c36  52.76,64.25 55,6
+000003c0: 312e 3133 2035 352c 3539 2e37 3543 3535  1.13 55,59.75C55
+000003d0: 2c35 382e 3337 2035 322e 3736 2c35 372e  ,58.37 52.76,57.
+000003e0: 3235 2035 302c 3537 2e32 3543 3437 2e32  25 50,57.25C47.2
+000003f0: 342c 3537 2e32 3520 3435 2c35 382e 3337  4,57.25 45,58.37
+00000400: 2034 352c 3539 2e37 3543 3435 2c36 312e   45,59.75C45,61.
+00000410: 3133 2034 372e 3234 2c36 342e 3235 2035  13 47.24,64.25 5
+00000420: 302c 3634 2e32 355a 2220 7374 796c 653d  0,64.25Z" style=
+00000430: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
+00000440: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
+00000450: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
+00000460: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00000470: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00000480: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+00000490: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+000004a0: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
+000004b0: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
+000004c0: 7468 2064 3d22 4d38 382c 3439 2e30 3543  th d="M88,49.05C
+000004d0: 3836 2e35 3036 2c34 332e 3437 3520 3833  86.506,43.475 83
+000004e0: 2e30 3138 2c33 382e 3633 3820 3738 2e32  .018,38.638 78.2
+000004f0: 2c33 352e 3436 4337 322e 3936 392c 3332  ,35.46C72.969,32
+00000500: 2e30 3032 2036 362e 3533 392c 3330 2e38  .002 66.539,30.8
+00000510: 3434 2036 302e 3433 2c33 322e 3236 4335  44 60.43,32.26C5
+00000520: 362e 3537 362c 3333 2e31 3435 2035 322e  6.576,33.145 52.
+00000530: 3939 352c 3334 2e39 3538 2035 302c 3337  995,34.958 50,37
+00000540: 2e35 3443 3436 2e39 3938 2c33 342e 3935  .54C46.998,34.95
+00000550: 3820 3433 2e34 3131 2c33 332e 3134 3920  8 43.411,33.149 
+00000560: 3339 2e35 352c 3332 2e32 3743 3333 2e34  39.55,32.27C33.4
+00000570: 3431 2c33 302e 3835 3320 3237 2e30 3131  41,30.853 27.011
+00000580: 2c33 322e 3031 3120 3231 2e37 382c 3335  ,32.011 21.78,35
+00000590: 2e34 3743 3136 2e39 372c 3338 2e36 3532  .47C16.97,38.652
+000005a0: 2031 332e 3438 392c 3433 2e34 3839 2031   13.489,43.489 1
+000005b0: 322c 3439 2e30 364c 3132 2c34 392e 3133  2,49.06L12,49.13
+000005c0: 4331 312e 3832 2c34 392e 3739 2031 312e  C11.82,49.79 11.
+000005d0: 3636 2c35 302e 3436 2031 312e 3533 2c35  66,50.46 11.53,5
+000005e0: 312e 3133 4331 312e 3134 362c 3533 2e32  1.13C11.146,53.2
+000005f0: 3037 2031 312e 3032 312c 3535 2e33 3233  07 11.021,55.323
+00000600: 2031 312e 3136 2c35 372e 3433 4331 312e   11.16,57.43C11.
+00000610: 3136 2c35 382e 3033 2031 312e 3236 2c35  16,58.03 11.26,5
+00000620: 382e 3633 2031 312e 3334 2c35 392e 3233  8.63 11.34,59.23
+00000630: 4331 312e 3334 2c35 392e 3531 2031 312e  C11.34,59.51 11.
+00000640: 3433 2c35 392e 3739 2031 312e 3438 2c36  43,59.79 11.48,6
+00000650: 302e 3037 4331 312e 3533 2c36 302e 3335  0.07C11.53,60.35
+00000660: 2031 312e 3538 2c36 302e 3638 2031 312e   11.58,60.68 11.
+00000670: 3634 2c36 302e 3938 4331 312e 372c 3631  64,60.98C11.7,61
+00000680: 2e32 3820 3131 2e38 2c36 312e 3639 2031  .28 11.8,61.69 1
+00000690: 312e 3839 2c36 322e 3035 4331 312e 3938  1.89,62.05C11.98
+000006a0: 2c36 322e 3431 2031 312e 3939 2c36 322e  ,62.41 11.99,62.
+000006b0: 3437 2031 322e 3035 2c36 322e 3638 4331  47 12.05,62.68C1
+000006c0: 322e 3136 2c36 332e 3037 2031 322e 3238  2.16,63.07 12.28
+000006d0: 2c36 332e 3436 2031 322e 3431 2c36 332e  ,63.46 12.41,63.
+000006e0: 3834 4c31 322e 3538 2c36 342e 3334 4331  84L12.58,64.34C1
+000006f0: 322e 3732 2c36 342e 3734 2031 322e 3838  2.72,64.74 12.88
+00000700: 2c36 352e 3134 2031 332e 3034 2c36 352e  ,65.14 13.04,65.
+00000710: 3533 4c31 332e 3233 2c36 352e 3938 4331  53L13.23,65.98C1
+00000720: 332e 3430 332c 3636 2e33 3733 2031 332e  3.403,66.373 13.
+00000730: 3538 332c 3636 2e37 3637 2031 332e 3737  583,66.767 13.77
+00000740: 2c36 372e 3136 4c31 332e 3939 2c36 372e  ,67.16L13.99,67.
+00000750: 3539 4331 342e 3139 2c36 372e 3937 2031  59C14.19,67.97 1
+00000760: 342e 3339 2c36 382e 3335 2031 342e 3631  4.39,68.35 14.61
+00000770: 2c36 382e 3733 4c31 342e 3837 2c36 392e  ,68.73L14.87,69.
+00000780: 3135 4331 352e 312c 3639 2e35 3220 3135  15C15.1,69.52 15
+00000790: 2e33 332c 3639 2e38 3920 3135 2e35 382c  .33,69.89 15.58,
+000007a0: 3730 2e32 364c 3135 2e35 382c 3730 2e33  70.26L15.58,70.3
+000007b0: 324c 3135 2e39 392c 3730 2e39 3343 3136  2L15.99,70.93C16
+000007c0: 2e31 342c 3731 2e31 3420 3136 2e32 392c  .14,71.14 16.29,
+000007d0: 3731 2e33 3620 3136 2e34 352c 3731 2e35  71.36 16.45,71.5
+000007e0: 3743 3230 2e32 3036 2c37 352e 3833 2032  7C20.206,75.83 2
+000007f0: 352e 3038 362c 3738 2e39 3520 3330 2e35  5.086,78.95 30.5
+00000800: 332c 3830 2e35 3743 3336 2e38 3339 2c38  3,80.57C36.839,8
+00000810: 322e 3438 2034 332e 3431 2c38 332e 3338  2.48 43.41,83.38
+00000820: 3520 3530 2c38 332e 3235 4335 362e 3539  5 50,83.25C56.59
+00000830: 392c 3833 2e33 3734 2036 332e 3137 372c  9,83.374 63.177,
+00000840: 3832 2e34 3536 2036 392e 3439 2c38 302e  82.456 69.49,80.
+00000850: 3533 4337 342e 3634 342c 3738 2e39 3738  53C74.644,78.978
+00000860: 2037 392e 3330 332c 3736 2e31 3032 2038   79.303,76.102 8
+00000870: 332c 3732 2e31 3943 3833 2e33 342c 3731  3,72.19C83.34,71
+00000880: 2e37 3820 3833 2e36 352c 3731 2e33 3520  .78 83.65,71.35 
+00000890: 3834 2c37 302e 3932 4c38 342e 3138 2c37  84,70.92L84.18,7
+000008a0: 302e 3636 4c38 342e 3333 2c37 302e 3434  0.66L84.33,70.44
+000008b0: 4c38 342e 3431 2c37 302e 3332 4338 342e  L84.41,70.32C84.
+000008c0: 3535 2c37 302e 3132 2038 342e 3637 2c36  55,70.12 84.67,6
+000008d0: 392e 3920 3834 2e38 312c 3639 2e37 4338  9.9 84.81,69.7C8
+000008e0: 352e 3037 2c36 392e 3320 3835 2e33 322c  5.07,69.3 85.32,
+000008f0: 3638 2e38 3920 3835 2e35 352c 3638 2e34  68.89 85.55,68.4
+00000900: 3843 3835 2e37 382c 3638 2e30 3720 3836  8C85.78,68.07 86
+00000910: 2e30 322c 3637 2e36 3520 3836 2e32 332c  .02,67.65 86.23,
+00000920: 3637 2e32 3243 3836 2e33 312c 3637 2e30  67.22C86.31,67.0
+00000930: 3520 3836 2e33 392c 3636 2e38 3820 3836  5 86.39,66.88 86
+00000940: 2e34 372c 3636 2e37 4338 362e 3637 2c36  .47,66.7C86.67,6
+00000950: 362e 3238 2038 362e 3835 2c36 352e 3837  6.28 86.85,65.87
+00000960: 2038 372e 3033 2c36 352e 3434 4c38 372e   87.03,65.44L87.
+00000970: 3233 2c36 342e 3932 4338 372e 3339 372c  23,64.92C87.397,
+00000980: 3634 2e34 3837 2038 372e 3535 2c36 342e  64.487 87.55,64.
+00000990: 3035 2038 372e 3639 2c36 332e 3631 4c38  05 87.69,63.61L8
+000009a0: 372e 3835 2c36 332e 3039 4338 372e 3938  7.85,63.09C87.98
+000009b0: 2c36 322e 3634 2038 382e 312c 3632 2e31  ,62.64 88.1,62.1
+000009c0: 3920 3838 2e32 312c 3631 2e37 3443 3838  9 88.21,61.74C88
+000009d0: 2e32 312c 3631 2e35 3720 3838 2e33 2c36  .21,61.57 88.3,6
+000009e0: 312e 3339 2038 382e 3333 2c36 312e 3232  1.39 88.33,61.22
+000009f0: 4338 382e 3433 2c36 302e 3735 2038 382e  C88.43,60.75 88.
+00000a00: 3532 2c36 302e 3232 2038 382e 362c 3539  52,60.22 88.6,59
+00000a10: 2e37 3943 3838 2e36 2c35 392e 3634 2038  .79C88.6,59.64 8
+00000a20: 382e 3636 2c35 392e 3439 2038 382e 3638  8.66,59.49 88.68
+00000a30: 2c35 392e 3333 4338 382e 3737 2c35 382e  ,59.33C88.77,58.
+00000a40: 3731 2038 382e 3834 2c35 382e 3038 2038  71 88.84,58.08 8
+00000a50: 382e 3838 2c35 372e 3435 4c38 382e 3838  8.88,57.45L88.88
+00000a60: 2c35 342e 3137 4338 382e 3831 372c 3533  ,54.17C88.817,53
+00000a70: 2e31 3634 2038 382e 3639 332c 3532 2e31  .164 88.693,52.1
+00000a80: 3632 2038 382e 3531 2c35 312e 3137 4338  62 88.51,51.17C8
+00000a90: 382e 3338 2c35 302e 3520 3838 2e32 332c  8.38,50.5 88.23,
+00000aa0: 3439 2e38 3420 3838 2e30 352c 3439 2e31  49.84 88.05,49.1
+00000ab0: 374c 3838 2c34 392e 3035 5a4d 3835 2e38  7L88,49.05ZM85.8
+00000ac0: 392c 3536 2e34 344c 3835 2e38 392c 3537  9,56.44L85.89,57
+00000ad0: 2e32 3343 3835 2e38 392c 3537 2e37 3820  .23C85.89,57.78 
+00000ae0: 3835 2e37 392c 3538 2e33 3220 3835 2e37  85.79,58.32 85.7
+00000af0: 322c 3538 2e38 3643 3835 2e37 322c 3539  2,58.86C85.72,59
+00000b00: 2e30 3120 3835 2e37 322c 3539 2e31 3520  .01 85.72,59.15 
+00000b10: 3835 2e36 352c 3539 2e33 4338 352e 3539  85.65,59.3C85.59
+00000b20: 2c35 392e 3720 3835 2e35 312c 3630 2e31  ,59.7 85.51,60.1
+00000b30: 3120 3835 2e34 332c 3630 2e35 314c 3835  1 85.43,60.51L85
+00000b40: 2e33 322c 3630 2e39 3943 3835 2e32 332c  .32,60.99C85.23,
+00000b50: 3631 2e33 3820 3835 2e31 322c 3631 2e37  61.38 85.12,61.7
+00000b60: 3720 3835 2e30 312c 3632 2e31 3643 3835  7 85.01,62.16C85
+00000b70: 2e30 312c 3632 2e33 3120 3834 2e39 332c  .01,62.31 84.93,
+00000b80: 3632 2e34 3620 3834 2e38 382c 3632 2e36  62.46 84.88,62.6
+00000b90: 4338 342e 3734 2c36 332e 3034 2038 342e  C84.74,63.04 84.
+00000ba0: 3539 2c36 332e 3437 2038 342e 3432 2c36  59,63.47 84.42,6
+00000bb0: 332e 394c 3834 2e32 372c 3634 2e32 3843  3.9L84.27,64.28C
+00000bc0: 3834 2e31 2c36 342e 3731 2038 332e 3931  84.1,64.71 83.91
+00000bd0: 2c36 352e 3134 2038 332e 3731 2c36 352e  ,65.14 83.71,65.
+00000be0: 3536 4338 332e 3531 2c36 352e 3938 2038  56C83.51,65.98 8
+00000bf0: 332e 3433 2c36 362e 3132 2038 332e 3238  3.43,66.12 83.28
+00000c00: 2c36 362e 344c 3833 2e30 312c 3636 2e39  ,66.4L83.01,66.9
+00000c10: 3143 3832 2e38 332c 3637 2e32 3233 2038  1C82.83,67.223 8
+00000c20: 322e 3634 332c 3637 2e35 3337 2038 322e  2.643,67.537 82.
+00000c30: 3435 2c36 372e 3835 4c38 322e 3335 2c36  45,67.85L82.35,6
+00000c40: 382e 3031 4337 392e 3132 312c 3638 2e30  8.01C79.121,68.0
+00000c50: 3437 2037 352e 3931 382c 3637 2e34 3334  47 75.918,67.434
+00000c60: 2037 322e 3933 2c36 362e 3231 4336 342e   72.93,66.21C64.
+00000c70: 3237 2c36 322e 3734 2035 392c 3535 2e35  27,62.74 59,55.5
+00000c80: 3220 3631 2e31 382c 3530 2e31 3143 3632  2 61.18,50.11C62
+00000c90: 2e31 382c 3437 2e36 2036 342e 372c 3435  .18,47.6 64.7,45
+00000ca0: 2e38 3220 3638 2e32 362c 3435 2e31 3143  .82 68.26,45.11C
+00000cb0: 3732 2e34 3839 2c34 342e 3339 3520 3736  72.489,44.395 76
+00000cc0: 2e38 3335 2c34 342e 3930 3820 3830 2e37  .835,44.908 80.7
+00000cd0: 382c 3436 2e35 3943 3832 2e31 3431 2c34  8,46.59C82.141,4
+00000ce0: 372e 3134 3420 3833 2e34 3533 2c34 372e  7.144 83.453,47.
+00000cf0: 3831 3320 3834 2e37 2c34 382e 3539 4338  813 84.7,48.59C8
+00000d00: 342e 3736 2c34 382e 3736 2038 342e 3832  4.76,48.76 84.82
+00000d10: 2c34 382e 3933 2038 342e 3838 2c34 392e  ,48.93 84.88,49.
+00000d20: 3143 3834 2e39 342c 3439 2e32 3720 3835  1C84.94,49.27 85
+00000d30: 2e30 352c 3439 2e36 3320 3835 2e31 322c  .05,49.63 85.12,
+00000d40: 3439 2e39 4338 352e 3238 2c35 302e 3520  49.9C85.28,50.5 
+00000d50: 3835 2e34 342c 3531 2e31 2038 352e 3535  85.44,51.1 85.55
+00000d60: 2c35 312e 3733 4338 352e 3639 312c 3532  ,51.73C85.691,52
+00000d70: 2e35 3037 2038 352e 3739 322c 3533 2e32  .507 85.792,53.2
+00000d80: 3932 2038 352e 3835 2c35 342e 3038 4c38  92 85.85,54.08L8
+00000d90: 352e 3835 2c35 352e 3839 4338 352e 3835  5.85,55.89C85.85
+00000da0: 2c35 362e 3132 2038 352e 3931 2c35 362e  ,56.12 85.91,56.
+00000db0: 3235 2038 352e 3931 2c35 362e 3435 4c38  25 85.91,56.45L8
+00000dc0: 352e 3839 2c35 362e 3434 5a4d 3137 2e36  5.89,56.44ZM17.6
+00000dd0: 362c 3638 4331 362e 3636 382c 3636 2e34  6,68C16.668,66.4
+00000de0: 3335 2031 352e 3836 392c 3634 2e37 3536  35 15.869,64.756
+00000df0: 2031 352e 3238 2c36 334c 3135 2e31 372c   15.28,63L15.17,
+00000e00: 3632 2e36 3843 3135 2e30 362c 3632 2e33  62.68C15.06,62.3
+00000e10: 3520 3134 2e39 362c 3632 2e30 3120 3134  5 14.96,62.01 14
+00000e20: 2e38 372c 3631 2e36 3843 3134 2e38 3233  .87,61.68C14.823
+00000e30: 2c36 312e 3439 3320 3134 2e37 3737 2c36  ,61.493 14.777,6
+00000e40: 312e 3331 2031 342e 3733 2c36 312e 3133  1.31 14.73,61.13
+00000e50: 4331 342e 3636 2c36 302e 3834 2031 342e  C14.66,60.84 14.
+00000e60: 3539 2c36 302e 3535 2031 342e 3533 2c36  59,60.55 14.53,6
+00000e70: 302e 3237 4331 342e 3437 2c35 392e 3939  0.27C14.47,59.99
+00000e80: 2031 342e 3433 2c35 392e 3732 2031 342e   14.43,59.72 14.
+00000e90: 3338 2c35 392e 3434 4331 342e 3333 2c35  38,59.44C14.33,5
+00000ea0: 392e 3136 2031 342e 332c 3539 2031 342e  9.16 14.3,59 14.
+00000eb0: 3237 2c35 382e 3738 4331 342e 322c 3538  27,58.78C14.2,58
+00000ec0: 2e32 3720 3134 2e31 352c 3537 2e37 3820  .27 14.15,57.78 
+00000ed0: 3134 2e31 312c 3537 2e32 334c 3134 2e31  14.11,57.23L14.1
+00000ee0: 312c 3537 2e30 3343 3134 2e30 3038 2c35  1,57.03C14.008,5
+00000ef0: 352e 3233 3620 3134 2e31 3232 2c35 332e  5.236 14.122,53.
+00000f00: 3433 3720 3134 2e34 352c 3531 2e36 3743  437 14.45,51.67C
+00000f10: 3134 2e35 362c 3531 2e30 3620 3134 2e37  14.56,51.06 14.7
+00000f20: 312c 3530 2e34 3620 3134 2e38 382c 3439  1,50.46 14.88,49
+00000f30: 2e38 3743 3134 2e39 362c 3439 2e35 3920  .87C14.96,49.59 
+00000f40: 3135 2e30 342c 3439 2e33 3220 3135 2e31  15.04,49.32 15.1
+00000f50: 332c 3439 2e30 3543 3135 2e32 322c 3438  3,49.05C15.22,48
+00000f60: 2e37 3820 3135 2e32 342c 3438 2e37 3220  .78 15.24,48.72 
+00000f70: 3135 2e33 2c34 382e 3535 4331 362e 3534  15.3,48.55C16.54
+00000f80: 382c 3437 2e37 3734 2031 372e 3835 392c  8,47.774 17.859,
+00000f90: 3437 2e31 3035 2031 392e 3232 2c34 362e  47.105 19.22,46.
+00000fa0: 3535 4332 372e 3836 2c34 332e 3039 2033  55C27.86,43.09 3
+00000fb0: 362e 3635 2c34 342e 3637 2033 382e 3832  6.65,44.67 38.82
+00000fc0: 2c35 302e 3038 4334 302e 3939 2c35 352e  ,50.08C40.99,55.
+00000fd0: 3439 2033 352e 3733 2c36 322e 3734 2032  49 35.73,62.74 2
+00000fe0: 372e 3039 2c36 362e 3243 3234 2e31 3031  7.09,66.2C24.101
+00000ff0: 2c36 372e 3433 3120 3230 2e38 3933 2c36  ,67.431 20.893,6
+00001000: 382e 3034 3320 3137 2e36 362c 3638 5a4d  8.043 17.66,68ZM
+00001010: 3638 2e35 372c 3737 2e36 3843 3632 2e35  68.57,77.68C62.5
+00001020: 3534 2c37 392e 3530 3820 3536 2e32 3837  54,79.508 56.287
+00001030: 2c38 302e 3337 3620 3530 2c38 302e 3235  ,80.376 50,80.25
+00001040: 4334 332e 3733 372c 3830 2e33 3720 3337  C43.737,80.37 37
+00001050: 2e34 3935 2c37 392e 3530 3620 3331 2e35  .495,79.506 31.5
+00001060: 2c37 372e 3639 4332 372e 3138 352c 3736  ,77.69C27.185,76
+00001070: 2e33 3820 3233 2e32 3433 2c37 342e 3036  .38 23.243,74.06
+00001080: 3220 3230 2c37 302e 3933 4332 322e 3831  2 20,70.93C22.81
+00001090: 352c 3730 2e37 3036 2032 352e 3538 2c37  5,70.706 25.58,7
+000010a0: 302e 3035 3520 3238 2e32 2c36 3943 3338  0.055 28.2,69C38
+000010b0: 2e33 372c 3634 2e39 3220 3434 2e33 392c  .37,64.92 44.39,
+000010c0: 3536 2034 312e 362c 3439 4333 382e 3831  56 41.6,49C38.81
+000010d0: 2c34 3220 3238 2e32 372c 3339 2e37 3220  ,42 28.27,39.72 
+000010e0: 3138 2e31 2c34 332e 384c 3137 2e34 332c  18.1,43.8L17.43,
+000010f0: 3434 2e30 3943 3138 2e39 3733 2c34 312e  44.09C18.973,41.
+00001100: 3634 3820 3231 2e30 3139 2c33 392e 3536  648 21.019,39.56
+00001110: 3120 3233 2e34 332c 3337 2e39 3743 3236  1 23.43,37.97C26
+00001120: 2e36 3731 2c33 352e 3832 3420 3330 2e34  .671,35.824 30.4
+00001130: 3733 2c33 342e 3638 2033 342e 3336 2c33  73,34.68 34.36,3
+00001140: 342e 3638 4333 352e 3838 342c 3334 2e36  4.68C35.884,34.6
+00001150: 3831 2033 372e 3430 342c 3334 2e38 3532  81 37.404,34.852
+00001160: 2033 382e 3839 2c33 352e 3139 4334 322e   38.89,35.19C42.
+00001170: 3639 342c 3336 2e30 3439 2034 362e 3139  694,36.049 46.19
+00001180: 312c 3337 2e39 3335 2034 392c 3430 2e36  1,37.935 49,40.6
+00001190: 344c 3530 2c34 312e 3634 4c35 312c 3430  4L50,41.64L51,40
+000011a0: 2e36 3443 3533 2e37 3937 2c33 372e 3933  .64C53.797,37.93
+000011b0: 3720 3537 2e32 3739 2c33 362e 3034 3920  7 57.279,36.049 
+000011c0: 3631 2e30 372c 3335 2e31 3843 3636 2e34  61.07,35.18C66.4
+000011d0: 3032 2c33 332e 3934 3720 3732 2e30 3134  02,33.947 72.014
+000011e0: 2c33 342e 3936 3820 3736 2e35 372c 3338  ,34.968 76.57,38
+000011f0: 4337 382e 3938 2c33 392e 3538 3820 3831  C78.98,39.588 81
+00001200: 2e30 3236 2c34 312e 3637 3120 3832 2e35  .026,41.671 82.5
+00001210: 372c 3434 2e31 314c 3831 2e39 2c34 332e  7,44.11L81.9,43.
+00001220: 3832 4337 372e 3430 392c 3431 2e39 3231  82C77.409,41.921
+00001230: 2037 322e 3436 342c 3431 2e33 3535 2036   72.464,41.355 6
+00001240: 372e 3636 2c34 322e 3139 4336 332e 3038  7.66,42.19C63.08
+00001250: 2c34 332e 3132 2035 392e 3739 2c34 352e  ,43.12 59.79,45.
+00001260: 3534 2035 382e 3339 2c34 392e 3032 4335  54 58.39,49.02C5
+00001270: 352e 362c 3535 2e39 3720 3631 2e36 322c  5.6,55.97 61.62,
+00001280: 3634 2e39 3420 3731 2e37 392c 3639 2e30  64.94 71.79,69.0
+00001290: 3243 3734 2e34 3134 2c37 302e 3037 2037  2C74.414,70.07 7
+000012a0: 372e 3138 322c 3730 2e37 3134 2038 302c  7.182,70.714 80,
+000012b0: 3730 2e39 3343 3736 2e37 3736 2c37 342e  70.93C76.776,74.
+000012c0: 3035 2037 322e 3835 392c 3736 2e33 3633  05 72.859,76.363
+000012d0: 2036 382e 3537 2c37 372e 3638 5a22 2073   68.57,77.68Z" s
+000012e0: 7479 6c65 3d22 6669 6c6c 3a72 6762 2832  tyle="fill:rgb(2
+000012f0: 3232 2c31 3230 2c31 3630 293b 6669 6c6c  22,120,160);fill
+00001300: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 222f  -rule:nonzero;"/
+00001310: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
+00001320: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
+00001330: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
+00001340: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
+00001350: 322c 392e 3730 3232 392c 2d31 2e37 3835  2,9.70229,-1.785
+00001360: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
+00001370: 2020 3c63 6972 636c 6520 6378 3d22 3731    <circle cx="71
+00001380: 2e33 3322 2063 793d 2235 3622 2072 3d22  .33" cy="56" r="
+00001390: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
+000013a0: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
+000013b0: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
+000013c0: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
+000013d0: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+000013e0: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
+000013f0: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
+00001400: 312e 3738 3538 3229 223e 0a20 2020 2020  1.78582)">.     
+00001410: 2020 2020 2020 203c 6369 7263 6c65 2063         <circle c
+00001420: 783d 2232 382e 3637 2220 6379 3d22 3536  x="28.67" cy="56
+00001430: 2220 723d 2235 2e31 3622 2073 7479 6c65  " r="5.16" style
+00001440: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
+00001450: 3230 2c31 3630 293b 222f 3e0a 2020 2020  20,160);"/>.    
+00001460: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+00001470: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
+00001480: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
+00001490: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
+000014a0: 3232 392c 2d31 2e37 3835 3832 2922 3e0a  229,-1.78582)">.
+000014b0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+000014c0: 6820 643d 224d 3538 2c36 3643 3535 2e39  h d="M58,66C55.9
+000014d0: 3132 2c36 382e 3136 3120 3533 2e30 3033  12,68.161 53.003
+000014e0: 2c36 392e 3333 3920 3530 2c36 392e 3234  ,69.339 50,69.24
+000014f0: 4334 362e 3939 372c 3639 2e33 3339 2034  C46.997,69.339 4
+00001500: 342e 3038 382c 3638 2e31 3631 2034 322c  4.088,68.161 42,
+00001510: 3636 4334 312e 3731 342c 3635 2e36 3737  66C41.714,65.677
+00001520: 2034 312e 3330 322c 3635 2e34 3931 2034   41.302,65.491 4
+00001530: 302e 3837 2c36 352e 3439 3143 3430 2e30  0.87,65.491C40.0
+00001540: 3432 2c36 352e 3439 3120 3339 2e33 3631  42,65.491 39.361
+00001550: 2c36 362e 3137 3220 3339 2e33 3631 2c36  ,66.172 39.361,6
+00001560: 3743 3339 2e33 3631 2c36 372e 3336 3820  7C39.361,67.368 
+00001570: 3339 2e34 3936 2c36 372e 3732 3420 3339  39.496,67.724 39
+00001580: 2e37 342c 3638 4334 322e 3430 332c 3730  .74,68C42.403,70
+00001590: 2e38 3034 2034 362e 3133 342c 3732 2e33  .804 46.134,72.3
+000015a0: 3520 3530 2c37 322e 3235 4335 332e 3836  5 50,72.25C53.86
+000015b0: 322c 3732 2e33 3437 2035 372e 3539 2c37  2,72.347 57.59,7
+000015c0: 302e 3830 3220 3630 2e32 352c 3638 4336  0.802 60.25,68C6
+000015d0: 302e 3439 352c 3637 2e37 3235 2036 302e  0.495,67.725 60.
+000015e0: 3633 2c36 372e 3336 3920 3630 2e36 332c  63,67.369 60.63,
+000015f0: 3637 4336 302e 3633 2c36 362e 3137 3420  67C60.63,66.174 
+00001600: 3539 2e39 3531 2c36 352e 3439 3520 3539  59.951,65.495 59
+00001610: 2e31 3235 2c36 352e 3439 3543 3538 2e36  .125,65.495C58.6
+00001620: 3935 2c36 352e 3439 3520 3538 2e32 3835  95,65.495 58.285
+00001630: 2c36 352e 3637 3920 3538 2c36 365a 2220  ,65.679 58,66Z" 
+00001640: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+00001650: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
+00001660: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
+00001670: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
+00001680: 2020 2020 3c2f 673e 0a3c 2f73 7667 3e0a      </g>.</svg>.
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/default-style/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/99.png` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/flat-square-modified/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/99.png` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/for-the-badge/default.svg`

 * *Files 1% similar despite different names*

```diff
@@ -2,360 +2,361 @@
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
 00000050: 6b22 2077 6964 7468 3d22 3230 3022 2068  k" width="200" h
 00000060: 6569 6768 743d 2232 3822 2072 6f6c 653d  eight="28" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 494e 5445 5252 4f47 4154 453a 2039  ="INTERROGATE: 9
-00000090: 392e 3925 223e 0a20 2020 203c 7469 746c  9.9%">.    <titl
-000000a0: 653e 494e 5445 5252 4f47 4154 453a 2039  e>INTERROGATE: 9
-000000b0: 392e 3925 3c2f 7469 746c 653e 0a20 2020  9.9%</title>.   
+00000080: 3d22 494e 5445 5252 4f47 4154 453a 202d  ="INTERROGATE: -
+00000090: 312e 3025 223e 0a20 2020 203c 7469 746c  1.0%">.    <titl
+000000a0: 653e 494e 5445 5252 4f47 4154 453a 202d  e>INTERROGATE: -
+000000b0: 312e 3025 3c2f 7469 746c 653e 0a20 2020  1.0%</title>.   
 000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
 000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
 000000f0: 7769 6474 683d 2231 3332 2e37 3522 2068  width="132.75" h
 00000100: 6569 6768 743d 2232 3822 2066 696c 6c3d  eight="28" fill=
 00000110: 2223 3535 3522 2f3e 0a20 2020 2020 2020  "#555"/>.       
 00000120: 203c 7265 6374 2078 3d22 3133 322e 3735   <rect x="132.75
 00000130: 2220 7769 6474 683d 2236 372e 3235 2220  " width="67.25" 
 00000140: 6865 6967 6874 3d22 3238 2220 6669 6c6c  height="28" fill
-00000150: 3d22 2334 6331 222f 3e0a 2020 2020 3c2f  ="#4c1"/>.    </
-00000160: 673e 0a20 2020 203c 6720 6669 6c6c 3d22  g>.    <g fill="
-00000170: 2366 6666 2220 7465 7874 2d61 6e63 686f  #fff" text-ancho
-00000180: 723d 226d 6964 646c 6522 2066 6f6e 742d  r="middle" font-
-00000190: 6661 6d69 6c79 3d22 5665 7264 616e 612c  family="Verdana,
-000001a0: 4765 6e65 7661 2c44 656a 6156 7520 5361  Geneva,DejaVu Sa
-000001b0: 6e73 2c73 616e 732d 7365 7269 6622 2074  ns,sans-serif" t
-000001c0: 6578 742d 7265 6e64 6572 696e 673d 2267  ext-rendering="g
-000001d0: 656f 6d65 7472 6963 5072 6563 6973 696f  eometricPrecisio
-000001e0: 6e22 2066 6f6e 742d 7369 7a65 3d22 3130  n" font-size="10
-000001f0: 3022 3e0a 2020 2020 2020 2020 3c74 6578  0">.        <tex
-00000200: 7420 7472 616e 7366 6f72 6d3d 2273 6361  t transform="sca
-00000210: 6c65 282e 3129 2220 783d 2237 3730 2e37  le(.1)" x="770.7
-00000220: 3522 2079 3d22 3137 3522 2074 6578 744c  5" y="175" textL
-00000230: 656e 6774 683d 2238 3637 2e35 2220 6669  ength="867.5" fi
-00000240: 6c6c 3d22 2366 6666 223e 494e 5445 5252  ll="#fff">INTERR
-00000250: 4f47 4154 453c 2f74 6578 743e 0a20 2020  OGATE</text>.   
-00000260: 2020 2020 203c 7465 7874 2074 7261 6e73       <text trans
-00000270: 666f 726d 3d22 7363 616c 6528 2e31 2922  form="scale(.1)"
-00000280: 2078 3d22 3136 3630 2e37 3522 2079 3d22   x="1660.75" y="
-00000290: 3137 3522 2074 6578 744c 656e 6774 683d  175" textLength=
-000002a0: 2234 3332 2e35 2220 6669 6c6c 3d22 2366  "432.5" fill="#f
-000002b0: 6666 2220 666f 6e74 2d77 6569 6768 743d  ff" font-weight=
-000002c0: 2262 6f6c 6422 2064 6174 612d 696e 7465  "bold" data-inte
-000002d0: 7272 6f67 6174 653d 2272 6573 756c 7422  rrogate="result"
-000002e0: 3e39 392e 3925 3c2f 7465 7874 3e0a 2020  >99.9%</text>.  
-000002f0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
-00000300: 3d22 6c6f 676f 2d70 696e 6b22 2074 7261  ="logo-pink" tra
-00000310: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
-00000320: 2e38 3534 3837 362c 302c 302c 302e 3835  .854876,0,0,0.85
-00000330: 3438 3736 2c2d 342e 3733 3531 342c 302e  4876,-4.73514,0.
-00000340: 3837 3731 3234 2922 3e0a 2020 2020 2020  877124)">.      
-00000350: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00000360: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-00000370: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-00000380: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
-00000390: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
-000003a0: 7468 2064 3d22 4d35 302c 3634 2e32 3543  th d="M50,64.25C
-000003b0: 3532 2e37 362c 3634 2e32 3520 3535 2c36  52.76,64.25 55,6
-000003c0: 312e 3133 2035 352c 3539 2e37 3543 3535  1.13 55,59.75C55
-000003d0: 2c35 382e 3337 2035 322e 3736 2c35 372e  ,58.37 52.76,57.
-000003e0: 3235 2035 302c 3537 2e32 3543 3437 2e32  25 50,57.25C47.2
-000003f0: 342c 3537 2e32 3520 3435 2c35 382e 3337  4,57.25 45,58.37
-00000400: 2034 352c 3539 2e37 3543 3435 2c36 312e   45,59.75C45,61.
-00000410: 3133 2034 372e 3234 2c36 342e 3235 2035  13 47.24,64.25 5
-00000420: 302c 3634 2e32 355a 2220 7374 796c 653d  0,64.25Z" style=
-00000430: 2266 696c 6c3a 7267 6228 3232 322c 3132  "fill:rgb(222,12
-00000440: 302c 3136 3029 3b66 696c 6c2d 7275 6c65  0,160);fill-rule
-00000450: 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20 2020  :nonzero;"/>.   
-00000460: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00000470: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00000480: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-00000490: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-000004a0: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
-000004b0: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
-000004c0: 7468 2064 3d22 4d38 382c 3439 2e30 3543  th d="M88,49.05C
-000004d0: 3836 2e35 3036 2c34 332e 3437 3520 3833  86.506,43.475 83
-000004e0: 2e30 3138 2c33 382e 3633 3820 3738 2e32  .018,38.638 78.2
-000004f0: 2c33 352e 3436 4337 322e 3936 392c 3332  ,35.46C72.969,32
-00000500: 2e30 3032 2036 362e 3533 392c 3330 2e38  .002 66.539,30.8
-00000510: 3434 2036 302e 3433 2c33 322e 3236 4335  44 60.43,32.26C5
-00000520: 362e 3537 362c 3333 2e31 3435 2035 322e  6.576,33.145 52.
-00000530: 3939 352c 3334 2e39 3538 2035 302c 3337  995,34.958 50,37
-00000540: 2e35 3443 3436 2e39 3938 2c33 342e 3935  .54C46.998,34.95
-00000550: 3820 3433 2e34 3131 2c33 332e 3134 3920  8 43.411,33.149 
-00000560: 3339 2e35 352c 3332 2e32 3743 3333 2e34  39.55,32.27C33.4
-00000570: 3431 2c33 302e 3835 3320 3237 2e30 3131  41,30.853 27.011
-00000580: 2c33 322e 3031 3120 3231 2e37 382c 3335  ,32.011 21.78,35
-00000590: 2e34 3743 3136 2e39 372c 3338 2e36 3532  .47C16.97,38.652
-000005a0: 2031 332e 3438 392c 3433 2e34 3839 2031   13.489,43.489 1
-000005b0: 322c 3439 2e30 364c 3132 2c34 392e 3133  2,49.06L12,49.13
-000005c0: 4331 312e 3832 2c34 392e 3739 2031 312e  C11.82,49.79 11.
-000005d0: 3636 2c35 302e 3436 2031 312e 3533 2c35  66,50.46 11.53,5
-000005e0: 312e 3133 4331 312e 3134 362c 3533 2e32  1.13C11.146,53.2
-000005f0: 3037 2031 312e 3032 312c 3535 2e33 3233  07 11.021,55.323
-00000600: 2031 312e 3136 2c35 372e 3433 4331 312e   11.16,57.43C11.
-00000610: 3136 2c35 382e 3033 2031 312e 3236 2c35  16,58.03 11.26,5
-00000620: 382e 3633 2031 312e 3334 2c35 392e 3233  8.63 11.34,59.23
-00000630: 4331 312e 3334 2c35 392e 3531 2031 312e  C11.34,59.51 11.
-00000640: 3433 2c35 392e 3739 2031 312e 3438 2c36  43,59.79 11.48,6
-00000650: 302e 3037 4331 312e 3533 2c36 302e 3335  0.07C11.53,60.35
-00000660: 2031 312e 3538 2c36 302e 3638 2031 312e   11.58,60.68 11.
-00000670: 3634 2c36 302e 3938 4331 312e 372c 3631  64,60.98C11.7,61
-00000680: 2e32 3820 3131 2e38 2c36 312e 3639 2031  .28 11.8,61.69 1
-00000690: 312e 3839 2c36 322e 3035 4331 312e 3938  1.89,62.05C11.98
-000006a0: 2c36 322e 3431 2031 312e 3939 2c36 322e  ,62.41 11.99,62.
-000006b0: 3437 2031 322e 3035 2c36 322e 3638 4331  47 12.05,62.68C1
-000006c0: 322e 3136 2c36 332e 3037 2031 322e 3238  2.16,63.07 12.28
-000006d0: 2c36 332e 3436 2031 322e 3431 2c36 332e  ,63.46 12.41,63.
-000006e0: 3834 4c31 322e 3538 2c36 342e 3334 4331  84L12.58,64.34C1
-000006f0: 322e 3732 2c36 342e 3734 2031 322e 3838  2.72,64.74 12.88
-00000700: 2c36 352e 3134 2031 332e 3034 2c36 352e  ,65.14 13.04,65.
-00000710: 3533 4c31 332e 3233 2c36 352e 3938 4331  53L13.23,65.98C1
-00000720: 332e 3430 332c 3636 2e33 3733 2031 332e  3.403,66.373 13.
-00000730: 3538 332c 3636 2e37 3637 2031 332e 3737  583,66.767 13.77
-00000740: 2c36 372e 3136 4c31 332e 3939 2c36 372e  ,67.16L13.99,67.
-00000750: 3539 4331 342e 3139 2c36 372e 3937 2031  59C14.19,67.97 1
-00000760: 342e 3339 2c36 382e 3335 2031 342e 3631  4.39,68.35 14.61
-00000770: 2c36 382e 3733 4c31 342e 3837 2c36 392e  ,68.73L14.87,69.
-00000780: 3135 4331 352e 312c 3639 2e35 3220 3135  15C15.1,69.52 15
-00000790: 2e33 332c 3639 2e38 3920 3135 2e35 382c  .33,69.89 15.58,
-000007a0: 3730 2e32 364c 3135 2e35 382c 3730 2e33  70.26L15.58,70.3
-000007b0: 324c 3135 2e39 392c 3730 2e39 3343 3136  2L15.99,70.93C16
-000007c0: 2e31 342c 3731 2e31 3420 3136 2e32 392c  .14,71.14 16.29,
-000007d0: 3731 2e33 3620 3136 2e34 352c 3731 2e35  71.36 16.45,71.5
-000007e0: 3743 3230 2e32 3036 2c37 352e 3833 2032  7C20.206,75.83 2
-000007f0: 352e 3038 362c 3738 2e39 3520 3330 2e35  5.086,78.95 30.5
-00000800: 332c 3830 2e35 3743 3336 2e38 3339 2c38  3,80.57C36.839,8
-00000810: 322e 3438 2034 332e 3431 2c38 332e 3338  2.48 43.41,83.38
-00000820: 3520 3530 2c38 332e 3235 4335 362e 3539  5 50,83.25C56.59
-00000830: 392c 3833 2e33 3734 2036 332e 3137 372c  9,83.374 63.177,
-00000840: 3832 2e34 3536 2036 392e 3439 2c38 302e  82.456 69.49,80.
-00000850: 3533 4337 342e 3634 342c 3738 2e39 3738  53C74.644,78.978
-00000860: 2037 392e 3330 332c 3736 2e31 3032 2038   79.303,76.102 8
-00000870: 332c 3732 2e31 3943 3833 2e33 342c 3731  3,72.19C83.34,71
-00000880: 2e37 3820 3833 2e36 352c 3731 2e33 3520  .78 83.65,71.35 
-00000890: 3834 2c37 302e 3932 4c38 342e 3138 2c37  84,70.92L84.18,7
-000008a0: 302e 3636 4c38 342e 3333 2c37 302e 3434  0.66L84.33,70.44
-000008b0: 4c38 342e 3431 2c37 302e 3332 4338 342e  L84.41,70.32C84.
-000008c0: 3535 2c37 302e 3132 2038 342e 3637 2c36  55,70.12 84.67,6
-000008d0: 392e 3920 3834 2e38 312c 3639 2e37 4338  9.9 84.81,69.7C8
-000008e0: 352e 3037 2c36 392e 3320 3835 2e33 322c  5.07,69.3 85.32,
-000008f0: 3638 2e38 3920 3835 2e35 352c 3638 2e34  68.89 85.55,68.4
-00000900: 3843 3835 2e37 382c 3638 2e30 3720 3836  8C85.78,68.07 86
-00000910: 2e30 322c 3637 2e36 3520 3836 2e32 332c  .02,67.65 86.23,
-00000920: 3637 2e32 3243 3836 2e33 312c 3637 2e30  67.22C86.31,67.0
-00000930: 3520 3836 2e33 392c 3636 2e38 3820 3836  5 86.39,66.88 86
-00000940: 2e34 372c 3636 2e37 4338 362e 3637 2c36  .47,66.7C86.67,6
-00000950: 362e 3238 2038 362e 3835 2c36 352e 3837  6.28 86.85,65.87
-00000960: 2038 372e 3033 2c36 352e 3434 4c38 372e   87.03,65.44L87.
-00000970: 3233 2c36 342e 3932 4338 372e 3339 372c  23,64.92C87.397,
-00000980: 3634 2e34 3837 2038 372e 3535 2c36 342e  64.487 87.55,64.
-00000990: 3035 2038 372e 3639 2c36 332e 3631 4c38  05 87.69,63.61L8
-000009a0: 372e 3835 2c36 332e 3039 4338 372e 3938  7.85,63.09C87.98
-000009b0: 2c36 322e 3634 2038 382e 312c 3632 2e31  ,62.64 88.1,62.1
-000009c0: 3920 3838 2e32 312c 3631 2e37 3443 3838  9 88.21,61.74C88
-000009d0: 2e32 312c 3631 2e35 3720 3838 2e33 2c36  .21,61.57 88.3,6
-000009e0: 312e 3339 2038 382e 3333 2c36 312e 3232  1.39 88.33,61.22
-000009f0: 4338 382e 3433 2c36 302e 3735 2038 382e  C88.43,60.75 88.
-00000a00: 3532 2c36 302e 3232 2038 382e 362c 3539  52,60.22 88.6,59
-00000a10: 2e37 3943 3838 2e36 2c35 392e 3634 2038  .79C88.6,59.64 8
-00000a20: 382e 3636 2c35 392e 3439 2038 382e 3638  8.66,59.49 88.68
-00000a30: 2c35 392e 3333 4338 382e 3737 2c35 382e  ,59.33C88.77,58.
-00000a40: 3731 2038 382e 3834 2c35 382e 3038 2038  71 88.84,58.08 8
-00000a50: 382e 3838 2c35 372e 3435 4c38 382e 3838  8.88,57.45L88.88
-00000a60: 2c35 342e 3137 4338 382e 3831 372c 3533  ,54.17C88.817,53
-00000a70: 2e31 3634 2038 382e 3639 332c 3532 2e31  .164 88.693,52.1
-00000a80: 3632 2038 382e 3531 2c35 312e 3137 4338  62 88.51,51.17C8
-00000a90: 382e 3338 2c35 302e 3520 3838 2e32 332c  8.38,50.5 88.23,
-00000aa0: 3439 2e38 3420 3838 2e30 352c 3439 2e31  49.84 88.05,49.1
-00000ab0: 374c 3838 2c34 392e 3035 5a4d 3835 2e38  7L88,49.05ZM85.8
-00000ac0: 392c 3536 2e34 344c 3835 2e38 392c 3537  9,56.44L85.89,57
-00000ad0: 2e32 3343 3835 2e38 392c 3537 2e37 3820  .23C85.89,57.78 
-00000ae0: 3835 2e37 392c 3538 2e33 3220 3835 2e37  85.79,58.32 85.7
-00000af0: 322c 3538 2e38 3643 3835 2e37 322c 3539  2,58.86C85.72,59
-00000b00: 2e30 3120 3835 2e37 322c 3539 2e31 3520  .01 85.72,59.15 
-00000b10: 3835 2e36 352c 3539 2e33 4338 352e 3539  85.65,59.3C85.59
-00000b20: 2c35 392e 3720 3835 2e35 312c 3630 2e31  ,59.7 85.51,60.1
-00000b30: 3120 3835 2e34 332c 3630 2e35 314c 3835  1 85.43,60.51L85
-00000b40: 2e33 322c 3630 2e39 3943 3835 2e32 332c  .32,60.99C85.23,
-00000b50: 3631 2e33 3820 3835 2e31 322c 3631 2e37  61.38 85.12,61.7
-00000b60: 3720 3835 2e30 312c 3632 2e31 3643 3835  7 85.01,62.16C85
-00000b70: 2e30 312c 3632 2e33 3120 3834 2e39 332c  .01,62.31 84.93,
-00000b80: 3632 2e34 3620 3834 2e38 382c 3632 2e36  62.46 84.88,62.6
-00000b90: 4338 342e 3734 2c36 332e 3034 2038 342e  C84.74,63.04 84.
-00000ba0: 3539 2c36 332e 3437 2038 342e 3432 2c36  59,63.47 84.42,6
-00000bb0: 332e 394c 3834 2e32 372c 3634 2e32 3843  3.9L84.27,64.28C
-00000bc0: 3834 2e31 2c36 342e 3731 2038 332e 3931  84.1,64.71 83.91
-00000bd0: 2c36 352e 3134 2038 332e 3731 2c36 352e  ,65.14 83.71,65.
-00000be0: 3536 4338 332e 3531 2c36 352e 3938 2038  56C83.51,65.98 8
-00000bf0: 332e 3433 2c36 362e 3132 2038 332e 3238  3.43,66.12 83.28
-00000c00: 2c36 362e 344c 3833 2e30 312c 3636 2e39  ,66.4L83.01,66.9
-00000c10: 3143 3832 2e38 332c 3637 2e32 3233 2038  1C82.83,67.223 8
-00000c20: 322e 3634 332c 3637 2e35 3337 2038 322e  2.643,67.537 82.
-00000c30: 3435 2c36 372e 3835 4c38 322e 3335 2c36  45,67.85L82.35,6
-00000c40: 382e 3031 4337 392e 3132 312c 3638 2e30  8.01C79.121,68.0
-00000c50: 3437 2037 352e 3931 382c 3637 2e34 3334  47 75.918,67.434
-00000c60: 2037 322e 3933 2c36 362e 3231 4336 342e   72.93,66.21C64.
-00000c70: 3237 2c36 322e 3734 2035 392c 3535 2e35  27,62.74 59,55.5
-00000c80: 3220 3631 2e31 382c 3530 2e31 3143 3632  2 61.18,50.11C62
-00000c90: 2e31 382c 3437 2e36 2036 342e 372c 3435  .18,47.6 64.7,45
-00000ca0: 2e38 3220 3638 2e32 362c 3435 2e31 3143  .82 68.26,45.11C
-00000cb0: 3732 2e34 3839 2c34 342e 3339 3520 3736  72.489,44.395 76
-00000cc0: 2e38 3335 2c34 342e 3930 3820 3830 2e37  .835,44.908 80.7
-00000cd0: 382c 3436 2e35 3943 3832 2e31 3431 2c34  8,46.59C82.141,4
-00000ce0: 372e 3134 3420 3833 2e34 3533 2c34 372e  7.144 83.453,47.
-00000cf0: 3831 3320 3834 2e37 2c34 382e 3539 4338  813 84.7,48.59C8
-00000d00: 342e 3736 2c34 382e 3736 2038 342e 3832  4.76,48.76 84.82
-00000d10: 2c34 382e 3933 2038 342e 3838 2c34 392e  ,48.93 84.88,49.
-00000d20: 3143 3834 2e39 342c 3439 2e32 3720 3835  1C84.94,49.27 85
-00000d30: 2e30 352c 3439 2e36 3320 3835 2e31 322c  .05,49.63 85.12,
-00000d40: 3439 2e39 4338 352e 3238 2c35 302e 3520  49.9C85.28,50.5 
-00000d50: 3835 2e34 342c 3531 2e31 2038 352e 3535  85.44,51.1 85.55
-00000d60: 2c35 312e 3733 4338 352e 3639 312c 3532  ,51.73C85.691,52
-00000d70: 2e35 3037 2038 352e 3739 322c 3533 2e32  .507 85.792,53.2
-00000d80: 3932 2038 352e 3835 2c35 342e 3038 4c38  92 85.85,54.08L8
-00000d90: 352e 3835 2c35 352e 3839 4338 352e 3835  5.85,55.89C85.85
-00000da0: 2c35 362e 3132 2038 352e 3931 2c35 362e  ,56.12 85.91,56.
-00000db0: 3235 2038 352e 3931 2c35 362e 3435 4c38  25 85.91,56.45L8
-00000dc0: 352e 3839 2c35 362e 3434 5a4d 3137 2e36  5.89,56.44ZM17.6
-00000dd0: 362c 3638 4331 362e 3636 382c 3636 2e34  6,68C16.668,66.4
-00000de0: 3335 2031 352e 3836 392c 3634 2e37 3536  35 15.869,64.756
-00000df0: 2031 352e 3238 2c36 334c 3135 2e31 372c   15.28,63L15.17,
-00000e00: 3632 2e36 3843 3135 2e30 362c 3632 2e33  62.68C15.06,62.3
-00000e10: 3520 3134 2e39 362c 3632 2e30 3120 3134  5 14.96,62.01 14
-00000e20: 2e38 372c 3631 2e36 3843 3134 2e38 3233  .87,61.68C14.823
-00000e30: 2c36 312e 3439 3320 3134 2e37 3737 2c36  ,61.493 14.777,6
-00000e40: 312e 3331 2031 342e 3733 2c36 312e 3133  1.31 14.73,61.13
-00000e50: 4331 342e 3636 2c36 302e 3834 2031 342e  C14.66,60.84 14.
-00000e60: 3539 2c36 302e 3535 2031 342e 3533 2c36  59,60.55 14.53,6
-00000e70: 302e 3237 4331 342e 3437 2c35 392e 3939  0.27C14.47,59.99
-00000e80: 2031 342e 3433 2c35 392e 3732 2031 342e   14.43,59.72 14.
-00000e90: 3338 2c35 392e 3434 4331 342e 3333 2c35  38,59.44C14.33,5
-00000ea0: 392e 3136 2031 342e 332c 3539 2031 342e  9.16 14.3,59 14.
-00000eb0: 3237 2c35 382e 3738 4331 342e 322c 3538  27,58.78C14.2,58
-00000ec0: 2e32 3720 3134 2e31 352c 3537 2e37 3820  .27 14.15,57.78 
-00000ed0: 3134 2e31 312c 3537 2e32 334c 3134 2e31  14.11,57.23L14.1
-00000ee0: 312c 3537 2e30 3343 3134 2e30 3038 2c35  1,57.03C14.008,5
-00000ef0: 352e 3233 3620 3134 2e31 3232 2c35 332e  5.236 14.122,53.
-00000f00: 3433 3720 3134 2e34 352c 3531 2e36 3743  437 14.45,51.67C
-00000f10: 3134 2e35 362c 3531 2e30 3620 3134 2e37  14.56,51.06 14.7
-00000f20: 312c 3530 2e34 3620 3134 2e38 382c 3439  1,50.46 14.88,49
-00000f30: 2e38 3743 3134 2e39 362c 3439 2e35 3920  .87C14.96,49.59 
-00000f40: 3135 2e30 342c 3439 2e33 3220 3135 2e31  15.04,49.32 15.1
-00000f50: 332c 3439 2e30 3543 3135 2e32 322c 3438  3,49.05C15.22,48
-00000f60: 2e37 3820 3135 2e32 342c 3438 2e37 3220  .78 15.24,48.72 
-00000f70: 3135 2e33 2c34 382e 3535 4331 362e 3534  15.3,48.55C16.54
-00000f80: 382c 3437 2e37 3734 2031 372e 3835 392c  8,47.774 17.859,
-00000f90: 3437 2e31 3035 2031 392e 3232 2c34 362e  47.105 19.22,46.
-00000fa0: 3535 4332 372e 3836 2c34 332e 3039 2033  55C27.86,43.09 3
-00000fb0: 362e 3635 2c34 342e 3637 2033 382e 3832  6.65,44.67 38.82
-00000fc0: 2c35 302e 3038 4334 302e 3939 2c35 352e  ,50.08C40.99,55.
-00000fd0: 3439 2033 352e 3733 2c36 322e 3734 2032  49 35.73,62.74 2
-00000fe0: 372e 3039 2c36 362e 3243 3234 2e31 3031  7.09,66.2C24.101
-00000ff0: 2c36 372e 3433 3120 3230 2e38 3933 2c36  ,67.431 20.893,6
-00001000: 382e 3034 3320 3137 2e36 362c 3638 5a4d  8.043 17.66,68ZM
-00001010: 3638 2e35 372c 3737 2e36 3843 3632 2e35  68.57,77.68C62.5
-00001020: 3534 2c37 392e 3530 3820 3536 2e32 3837  54,79.508 56.287
-00001030: 2c38 302e 3337 3620 3530 2c38 302e 3235  ,80.376 50,80.25
-00001040: 4334 332e 3733 372c 3830 2e33 3720 3337  C43.737,80.37 37
-00001050: 2e34 3935 2c37 392e 3530 3620 3331 2e35  .495,79.506 31.5
-00001060: 2c37 372e 3639 4332 372e 3138 352c 3736  ,77.69C27.185,76
-00001070: 2e33 3820 3233 2e32 3433 2c37 342e 3036  .38 23.243,74.06
-00001080: 3220 3230 2c37 302e 3933 4332 322e 3831  2 20,70.93C22.81
-00001090: 352c 3730 2e37 3036 2032 352e 3538 2c37  5,70.706 25.58,7
-000010a0: 302e 3035 3520 3238 2e32 2c36 3943 3338  0.055 28.2,69C38
-000010b0: 2e33 372c 3634 2e39 3220 3434 2e33 392c  .37,64.92 44.39,
-000010c0: 3536 2034 312e 362c 3439 4333 382e 3831  56 41.6,49C38.81
-000010d0: 2c34 3220 3238 2e32 372c 3339 2e37 3220  ,42 28.27,39.72 
-000010e0: 3138 2e31 2c34 332e 384c 3137 2e34 332c  18.1,43.8L17.43,
-000010f0: 3434 2e30 3943 3138 2e39 3733 2c34 312e  44.09C18.973,41.
-00001100: 3634 3820 3231 2e30 3139 2c33 392e 3536  648 21.019,39.56
-00001110: 3120 3233 2e34 332c 3337 2e39 3743 3236  1 23.43,37.97C26
-00001120: 2e36 3731 2c33 352e 3832 3420 3330 2e34  .671,35.824 30.4
-00001130: 3733 2c33 342e 3638 2033 342e 3336 2c33  73,34.68 34.36,3
-00001140: 342e 3638 4333 352e 3838 342c 3334 2e36  4.68C35.884,34.6
-00001150: 3831 2033 372e 3430 342c 3334 2e38 3532  81 37.404,34.852
-00001160: 2033 382e 3839 2c33 352e 3139 4334 322e   38.89,35.19C42.
-00001170: 3639 342c 3336 2e30 3439 2034 362e 3139  694,36.049 46.19
-00001180: 312c 3337 2e39 3335 2034 392c 3430 2e36  1,37.935 49,40.6
-00001190: 344c 3530 2c34 312e 3634 4c35 312c 3430  4L50,41.64L51,40
-000011a0: 2e36 3443 3533 2e37 3937 2c33 372e 3933  .64C53.797,37.93
-000011b0: 3720 3537 2e32 3739 2c33 362e 3034 3920  7 57.279,36.049 
-000011c0: 3631 2e30 372c 3335 2e31 3843 3636 2e34  61.07,35.18C66.4
-000011d0: 3032 2c33 332e 3934 3720 3732 2e30 3134  02,33.947 72.014
-000011e0: 2c33 342e 3936 3820 3736 2e35 372c 3338  ,34.968 76.57,38
-000011f0: 4337 382e 3938 2c33 392e 3538 3820 3831  C78.98,39.588 81
-00001200: 2e30 3236 2c34 312e 3637 3120 3832 2e35  .026,41.671 82.5
-00001210: 372c 3434 2e31 314c 3831 2e39 2c34 332e  7,44.11L81.9,43.
-00001220: 3832 4337 372e 3430 392c 3431 2e39 3231  82C77.409,41.921
-00001230: 2037 322e 3436 342c 3431 2e33 3535 2036   72.464,41.355 6
-00001240: 372e 3636 2c34 322e 3139 4336 332e 3038  7.66,42.19C63.08
-00001250: 2c34 332e 3132 2035 392e 3739 2c34 352e  ,43.12 59.79,45.
-00001260: 3534 2035 382e 3339 2c34 392e 3032 4335  54 58.39,49.02C5
-00001270: 352e 362c 3535 2e39 3720 3631 2e36 322c  5.6,55.97 61.62,
-00001280: 3634 2e39 3420 3731 2e37 392c 3639 2e30  64.94 71.79,69.0
-00001290: 3243 3734 2e34 3134 2c37 302e 3037 2037  2C74.414,70.07 7
-000012a0: 372e 3138 322c 3730 2e37 3134 2038 302c  7.182,70.714 80,
-000012b0: 3730 2e39 3343 3736 2e37 3736 2c37 342e  70.93C76.776,74.
-000012c0: 3035 2037 322e 3835 392c 3736 2e33 3633  05 72.859,76.363
-000012d0: 2036 382e 3537 2c37 372e 3638 5a22 2073   68.57,77.68Z" s
-000012e0: 7479 6c65 3d22 6669 6c6c 3a72 6762 2832  tyle="fill:rgb(2
-000012f0: 3232 2c31 3230 2c31 3630 293b 6669 6c6c  22,120,160);fill
-00001300: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 222f  -rule:nonzero;"/
-00001310: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-00001320: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00001330: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-00001340: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-00001350: 322c 392e 3730 3232 392c 2d31 2e37 3835  2,9.70229,-1.785
-00001360: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-00001370: 2020 3c63 6972 636c 6520 6378 3d22 3731    <circle cx="71
-00001380: 2e33 3322 2063 793d 2235 3622 2072 3d22  .33" cy="56" r="
-00001390: 352e 3136 2220 7374 796c 653d 2266 696c  5.16" style="fil
-000013a0: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
-000013b0: 3029 3b22 2f3e 0a20 2020 2020 2020 203c  0);"/>.        <
-000013c0: 2f67 3e0a 2020 2020 2020 2020 3c67 2074  /g>.        <g t
-000013d0: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
-000013e0: 2830 2e32 3939 3031 322c 302c 302c 302e  (0.299012,0,0,0.
-000013f0: 3239 3930 3132 2c39 2e37 3032 3239 2c2d  299012,9.70229,-
-00001400: 312e 3738 3538 3229 223e 0a20 2020 2020  1.78582)">.     
-00001410: 2020 2020 2020 203c 6369 7263 6c65 2063         <circle c
-00001420: 783d 2232 382e 3637 2220 6379 3d22 3536  x="28.67" cy="56
-00001430: 2220 723d 2235 2e31 3622 2073 7479 6c65  " r="5.16" style
-00001440: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
-00001450: 3230 2c31 3630 293b 222f 3e0a 2020 2020  20,160);"/>.    
-00001460: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
-00001470: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
-00001480: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
-00001490: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
-000014a0: 3232 392c 2d31 2e37 3835 3832 2922 3e0a  229,-1.78582)">.
-000014b0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-000014c0: 6820 643d 224d 3538 2c36 3643 3535 2e39  h d="M58,66C55.9
-000014d0: 3132 2c36 382e 3136 3120 3533 2e30 3033  12,68.161 53.003
-000014e0: 2c36 392e 3333 3920 3530 2c36 392e 3234  ,69.339 50,69.24
-000014f0: 4334 362e 3939 372c 3639 2e33 3339 2034  C46.997,69.339 4
-00001500: 342e 3038 382c 3638 2e31 3631 2034 322c  4.088,68.161 42,
-00001510: 3636 4334 312e 3731 342c 3635 2e36 3737  66C41.714,65.677
-00001520: 2034 312e 3330 322c 3635 2e34 3931 2034   41.302,65.491 4
-00001530: 302e 3837 2c36 352e 3439 3143 3430 2e30  0.87,65.491C40.0
-00001540: 3432 2c36 352e 3439 3120 3339 2e33 3631  42,65.491 39.361
-00001550: 2c36 362e 3137 3220 3339 2e33 3631 2c36  ,66.172 39.361,6
-00001560: 3743 3339 2e33 3631 2c36 372e 3336 3820  7C39.361,67.368 
-00001570: 3339 2e34 3936 2c36 372e 3732 3420 3339  39.496,67.724 39
-00001580: 2e37 342c 3638 4334 322e 3430 332c 3730  .74,68C42.403,70
-00001590: 2e38 3034 2034 362e 3133 342c 3732 2e33  .804 46.134,72.3
-000015a0: 3520 3530 2c37 322e 3235 4335 332e 3836  5 50,72.25C53.86
-000015b0: 322c 3732 2e33 3437 2035 372e 3539 2c37  2,72.347 57.59,7
-000015c0: 302e 3830 3220 3630 2e32 352c 3638 4336  0.802 60.25,68C6
-000015d0: 302e 3439 352c 3637 2e37 3235 2036 302e  0.495,67.725 60.
-000015e0: 3633 2c36 372e 3336 3920 3630 2e36 332c  63,67.369 60.63,
-000015f0: 3637 4336 302e 3633 2c36 362e 3137 3420  67C60.63,66.174 
-00001600: 3539 2e39 3531 2c36 352e 3439 3520 3539  59.951,65.495 59
-00001610: 2e31 3235 2c36 352e 3439 3543 3538 2e36  .125,65.495C58.6
-00001620: 3935 2c36 352e 3439 3520 3538 2e32 3835  95,65.495 58.285
-00001630: 2c36 352e 3637 3920 3538 2c36 365a 2220  ,65.679 58,66Z" 
-00001640: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
-00001650: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
-00001660: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
-00001670: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
-00001680: 2020 2020 3c2f 673e 0a3c 2f73 7667 3e0a      </g>.</svg>.
+00000150: 3d22 2339 6639 6639 6622 2f3e 0a20 2020  ="#9f9f9f"/>.   
+00000160: 203c 2f67 3e0a 2020 2020 3c67 2066 696c   </g>.    <g fil
+00000170: 6c3d 2223 6666 6622 2074 6578 742d 616e  l="#fff" text-an
+00000180: 6368 6f72 3d22 6d69 6464 6c65 2220 666f  chor="middle" fo
+00000190: 6e74 2d66 616d 696c 793d 2256 6572 6461  nt-family="Verda
+000001a0: 6e61 2c47 656e 6576 612c 4465 6a61 5675  na,Geneva,DejaVu
+000001b0: 2053 616e 732c 7361 6e73 2d73 6572 6966   Sans,sans-serif
+000001c0: 2220 7465 7874 2d72 656e 6465 7269 6e67  " text-rendering
+000001d0: 3d22 6765 6f6d 6574 7269 6350 7265 6369  ="geometricPreci
+000001e0: 7369 6f6e 2220 666f 6e74 2d73 697a 653d  sion" font-size=
+000001f0: 2231 3030 223e 0a20 2020 2020 2020 203c  "100">.        <
+00000200: 7465 7874 2074 7261 6e73 666f 726d 3d22  text transform="
+00000210: 7363 616c 6528 2e31 2922 2078 3d22 3737  scale(.1)" x="77
+00000220: 302e 3735 2220 793d 2231 3735 2220 7465  0.75" y="175" te
+00000230: 7874 4c65 6e67 7468 3d22 3836 372e 3522  xtLength="867.5"
+00000240: 2066 696c 6c3d 2223 6666 6622 3e49 4e54   fill="#fff">INT
+00000250: 4552 524f 4741 5445 3c2f 7465 7874 3e0a  ERROGATE</text>.
+00000260: 2020 2020 2020 2020 3c74 6578 7420 7472          <text tr
+00000270: 616e 7366 6f72 6d3d 2273 6361 6c65 282e  ansform="scale(.
+00000280: 3129 2220 783d 2231 3638 302e 3735 2220  1)" x="1680.75" 
+00000290: 793d 2231 3735 2220 7465 7874 4c65 6e67  y="175" textLeng
+000002a0: 7468 3d22 3335 3022 2066 696c 6c3d 2223  th="350" fill="#
+000002b0: 6666 6622 2066 6f6e 742d 7765 6967 6874  fff" font-weight
+000002c0: 3d22 626f 6c64 2220 6461 7461 2d69 6e74  ="bold" data-int
+000002d0: 6572 726f 6761 7465 3d22 7265 7375 6c74  errogate="result
+000002e0: 223e 2d31 2e30 253c 2f74 6578 743e 0a20  ">-1.0%</text>. 
+000002f0: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
+00000300: 643d 226c 6f67 6f2d 7069 6e6b 2220 7472  d="logo-pink" tr
+00000310: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+00000320: 302e 3835 3438 3736 2c30 2c30 2c30 2e38  0.854876,0,0,0.8
+00000330: 3534 3837 362c 2d34 2e37 3335 3134 2c30  54876,-4.73514,0
+00000340: 2e38 3737 3132 3429 223e 0a20 2020 2020  .877124)">.     
+00000350: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00000360: 226d 6174 7269 7828 302e 3239 3930 3132  "matrix(0.299012
+00000370: 2c30 2c30 2c30 2e32 3939 3031 322c 392e  ,0,0,0.299012,9.
+00000380: 3730 3232 392c 2d31 2e37 3835 3832 2922  70229,-1.78582)"
+00000390: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+000003a0: 6174 6820 643d 224d 3530 2c36 342e 3235  ath d="M50,64.25
+000003b0: 4335 322e 3736 2c36 342e 3235 2035 352c  C52.76,64.25 55,
+000003c0: 3631 2e31 3320 3535 2c35 392e 3735 4335  61.13 55,59.75C5
+000003d0: 352c 3538 2e33 3720 3532 2e37 362c 3537  5,58.37 52.76,57
+000003e0: 2e32 3520 3530 2c35 372e 3235 4334 372e  .25 50,57.25C47.
+000003f0: 3234 2c35 372e 3235 2034 352c 3538 2e33  24,57.25 45,58.3
+00000400: 3720 3435 2c35 392e 3735 4334 352c 3631  7 45,59.75C45,61
+00000410: 2e31 3320 3437 2e32 342c 3634 2e32 3520  .13 47.24,64.25 
+00000420: 3530 2c36 342e 3235 5a22 2073 7479 6c65  50,64.25Z" style
+00000430: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
+00000440: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
+00000450: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
+00000460: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
+00000470: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00000480: 226d 6174 7269 7828 302e 3239 3930 3132  "matrix(0.299012
+00000490: 2c30 2c30 2c30 2e32 3939 3031 322c 392e  ,0,0,0.299012,9.
+000004a0: 3730 3232 392c 2d31 2e37 3835 3832 2922  70229,-1.78582)"
+000004b0: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+000004c0: 6174 6820 643d 224d 3838 2c34 392e 3035  ath d="M88,49.05
+000004d0: 4338 362e 3530 362c 3433 2e34 3735 2038  C86.506,43.475 8
+000004e0: 332e 3031 382c 3338 2e36 3338 2037 382e  3.018,38.638 78.
+000004f0: 322c 3335 2e34 3643 3732 2e39 3639 2c33  2,35.46C72.969,3
+00000500: 322e 3030 3220 3636 2e35 3339 2c33 302e  2.002 66.539,30.
+00000510: 3834 3420 3630 2e34 332c 3332 2e32 3643  844 60.43,32.26C
+00000520: 3536 2e35 3736 2c33 332e 3134 3520 3532  56.576,33.145 52
+00000530: 2e39 3935 2c33 342e 3935 3820 3530 2c33  .995,34.958 50,3
+00000540: 372e 3534 4334 362e 3939 382c 3334 2e39  7.54C46.998,34.9
+00000550: 3538 2034 332e 3431 312c 3333 2e31 3439  58 43.411,33.149
+00000560: 2033 392e 3535 2c33 322e 3237 4333 332e   39.55,32.27C33.
+00000570: 3434 312c 3330 2e38 3533 2032 372e 3031  441,30.853 27.01
+00000580: 312c 3332 2e30 3131 2032 312e 3738 2c33  1,32.011 21.78,3
+00000590: 352e 3437 4331 362e 3937 2c33 382e 3635  5.47C16.97,38.65
+000005a0: 3220 3133 2e34 3839 2c34 332e 3438 3920  2 13.489,43.489 
+000005b0: 3132 2c34 392e 3036 4c31 322c 3439 2e31  12,49.06L12,49.1
+000005c0: 3343 3131 2e38 322c 3439 2e37 3920 3131  3C11.82,49.79 11
+000005d0: 2e36 362c 3530 2e34 3620 3131 2e35 332c  .66,50.46 11.53,
+000005e0: 3531 2e31 3343 3131 2e31 3436 2c35 332e  51.13C11.146,53.
+000005f0: 3230 3720 3131 2e30 3231 2c35 352e 3332  207 11.021,55.32
+00000600: 3320 3131 2e31 362c 3537 2e34 3343 3131  3 11.16,57.43C11
+00000610: 2e31 362c 3538 2e30 3320 3131 2e32 362c  .16,58.03 11.26,
+00000620: 3538 2e36 3320 3131 2e33 342c 3539 2e32  58.63 11.34,59.2
+00000630: 3343 3131 2e33 342c 3539 2e35 3120 3131  3C11.34,59.51 11
+00000640: 2e34 332c 3539 2e37 3920 3131 2e34 382c  .43,59.79 11.48,
+00000650: 3630 2e30 3743 3131 2e35 332c 3630 2e33  60.07C11.53,60.3
+00000660: 3520 3131 2e35 382c 3630 2e36 3820 3131  5 11.58,60.68 11
+00000670: 2e36 342c 3630 2e39 3843 3131 2e37 2c36  .64,60.98C11.7,6
+00000680: 312e 3238 2031 312e 382c 3631 2e36 3920  1.28 11.8,61.69 
+00000690: 3131 2e38 392c 3632 2e30 3543 3131 2e39  11.89,62.05C11.9
+000006a0: 382c 3632 2e34 3120 3131 2e39 392c 3632  8,62.41 11.99,62
+000006b0: 2e34 3720 3132 2e30 352c 3632 2e36 3843  .47 12.05,62.68C
+000006c0: 3132 2e31 362c 3633 2e30 3720 3132 2e32  12.16,63.07 12.2
+000006d0: 382c 3633 2e34 3620 3132 2e34 312c 3633  8,63.46 12.41,63
+000006e0: 2e38 344c 3132 2e35 382c 3634 2e33 3443  .84L12.58,64.34C
+000006f0: 3132 2e37 322c 3634 2e37 3420 3132 2e38  12.72,64.74 12.8
+00000700: 382c 3635 2e31 3420 3133 2e30 342c 3635  8,65.14 13.04,65
+00000710: 2e35 334c 3133 2e32 332c 3635 2e39 3843  .53L13.23,65.98C
+00000720: 3133 2e34 3033 2c36 362e 3337 3320 3133  13.403,66.373 13
+00000730: 2e35 3833 2c36 362e 3736 3720 3133 2e37  .583,66.767 13.7
+00000740: 372c 3637 2e31 364c 3133 2e39 392c 3637  7,67.16L13.99,67
+00000750: 2e35 3943 3134 2e31 392c 3637 2e39 3720  .59C14.19,67.97 
+00000760: 3134 2e33 392c 3638 2e33 3520 3134 2e36  14.39,68.35 14.6
+00000770: 312c 3638 2e37 334c 3134 2e38 372c 3639  1,68.73L14.87,69
+00000780: 2e31 3543 3135 2e31 2c36 392e 3532 2031  .15C15.1,69.52 1
+00000790: 352e 3333 2c36 392e 3839 2031 352e 3538  5.33,69.89 15.58
+000007a0: 2c37 302e 3236 4c31 352e 3538 2c37 302e  ,70.26L15.58,70.
+000007b0: 3332 4c31 352e 3939 2c37 302e 3933 4331  32L15.99,70.93C1
+000007c0: 362e 3134 2c37 312e 3134 2031 362e 3239  6.14,71.14 16.29
+000007d0: 2c37 312e 3336 2031 362e 3435 2c37 312e  ,71.36 16.45,71.
+000007e0: 3537 4332 302e 3230 362c 3735 2e38 3320  57C20.206,75.83 
+000007f0: 3235 2e30 3836 2c37 382e 3935 2033 302e  25.086,78.95 30.
+00000800: 3533 2c38 302e 3537 4333 362e 3833 392c  53,80.57C36.839,
+00000810: 3832 2e34 3820 3433 2e34 312c 3833 2e33  82.48 43.41,83.3
+00000820: 3835 2035 302c 3833 2e32 3543 3536 2e35  85 50,83.25C56.5
+00000830: 3939 2c38 332e 3337 3420 3633 2e31 3737  99,83.374 63.177
+00000840: 2c38 322e 3435 3620 3639 2e34 392c 3830  ,82.456 69.49,80
+00000850: 2e35 3343 3734 2e36 3434 2c37 382e 3937  .53C74.644,78.97
+00000860: 3820 3739 2e33 3033 2c37 362e 3130 3220  8 79.303,76.102 
+00000870: 3833 2c37 322e 3139 4338 332e 3334 2c37  83,72.19C83.34,7
+00000880: 312e 3738 2038 332e 3635 2c37 312e 3335  1.78 83.65,71.35
+00000890: 2038 342c 3730 2e39 324c 3834 2e31 382c   84,70.92L84.18,
+000008a0: 3730 2e36 364c 3834 2e33 332c 3730 2e34  70.66L84.33,70.4
+000008b0: 344c 3834 2e34 312c 3730 2e33 3243 3834  4L84.41,70.32C84
+000008c0: 2e35 352c 3730 2e31 3220 3834 2e36 372c  .55,70.12 84.67,
+000008d0: 3639 2e39 2038 342e 3831 2c36 392e 3743  69.9 84.81,69.7C
+000008e0: 3835 2e30 372c 3639 2e33 2038 352e 3332  85.07,69.3 85.32
+000008f0: 2c36 382e 3839 2038 352e 3535 2c36 382e  ,68.89 85.55,68.
+00000900: 3438 4338 352e 3738 2c36 382e 3037 2038  48C85.78,68.07 8
+00000910: 362e 3032 2c36 372e 3635 2038 362e 3233  6.02,67.65 86.23
+00000920: 2c36 372e 3232 4338 362e 3331 2c36 372e  ,67.22C86.31,67.
+00000930: 3035 2038 362e 3339 2c36 362e 3838 2038  05 86.39,66.88 8
+00000940: 362e 3437 2c36 362e 3743 3836 2e36 372c  6.47,66.7C86.67,
+00000950: 3636 2e32 3820 3836 2e38 352c 3635 2e38  66.28 86.85,65.8
+00000960: 3720 3837 2e30 332c 3635 2e34 344c 3837  7 87.03,65.44L87
+00000970: 2e32 332c 3634 2e39 3243 3837 2e33 3937  .23,64.92C87.397
+00000980: 2c36 342e 3438 3720 3837 2e35 352c 3634  ,64.487 87.55,64
+00000990: 2e30 3520 3837 2e36 392c 3633 2e36 314c  .05 87.69,63.61L
+000009a0: 3837 2e38 352c 3633 2e30 3943 3837 2e39  87.85,63.09C87.9
+000009b0: 382c 3632 2e36 3420 3838 2e31 2c36 322e  8,62.64 88.1,62.
+000009c0: 3139 2038 382e 3231 2c36 312e 3734 4338  19 88.21,61.74C8
+000009d0: 382e 3231 2c36 312e 3537 2038 382e 332c  8.21,61.57 88.3,
+000009e0: 3631 2e33 3920 3838 2e33 332c 3631 2e32  61.39 88.33,61.2
+000009f0: 3243 3838 2e34 332c 3630 2e37 3520 3838  2C88.43,60.75 88
+00000a00: 2e35 322c 3630 2e32 3220 3838 2e36 2c35  .52,60.22 88.6,5
+00000a10: 392e 3739 4338 382e 362c 3539 2e36 3420  9.79C88.6,59.64 
+00000a20: 3838 2e36 362c 3539 2e34 3920 3838 2e36  88.66,59.49 88.6
+00000a30: 382c 3539 2e33 3343 3838 2e37 372c 3538  8,59.33C88.77,58
+00000a40: 2e37 3120 3838 2e38 342c 3538 2e30 3820  .71 88.84,58.08 
+00000a50: 3838 2e38 382c 3537 2e34 354c 3838 2e38  88.88,57.45L88.8
+00000a60: 382c 3534 2e31 3743 3838 2e38 3137 2c35  8,54.17C88.817,5
+00000a70: 332e 3136 3420 3838 2e36 3933 2c35 322e  3.164 88.693,52.
+00000a80: 3136 3220 3838 2e35 312c 3531 2e31 3743  162 88.51,51.17C
+00000a90: 3838 2e33 382c 3530 2e35 2038 382e 3233  88.38,50.5 88.23
+00000aa0: 2c34 392e 3834 2038 382e 3035 2c34 392e  ,49.84 88.05,49.
+00000ab0: 3137 4c38 382c 3439 2e30 355a 4d38 352e  17L88,49.05ZM85.
+00000ac0: 3839 2c35 362e 3434 4c38 352e 3839 2c35  89,56.44L85.89,5
+00000ad0: 372e 3233 4338 352e 3839 2c35 372e 3738  7.23C85.89,57.78
+00000ae0: 2038 352e 3739 2c35 382e 3332 2038 352e   85.79,58.32 85.
+00000af0: 3732 2c35 382e 3836 4338 352e 3732 2c35  72,58.86C85.72,5
+00000b00: 392e 3031 2038 352e 3732 2c35 392e 3135  9.01 85.72,59.15
+00000b10: 2038 352e 3635 2c35 392e 3343 3835 2e35   85.65,59.3C85.5
+00000b20: 392c 3539 2e37 2038 352e 3531 2c36 302e  9,59.7 85.51,60.
+00000b30: 3131 2038 352e 3433 2c36 302e 3531 4c38  11 85.43,60.51L8
+00000b40: 352e 3332 2c36 302e 3939 4338 352e 3233  5.32,60.99C85.23
+00000b50: 2c36 312e 3338 2038 352e 3132 2c36 312e  ,61.38 85.12,61.
+00000b60: 3737 2038 352e 3031 2c36 322e 3136 4338  77 85.01,62.16C8
+00000b70: 352e 3031 2c36 322e 3331 2038 342e 3933  5.01,62.31 84.93
+00000b80: 2c36 322e 3436 2038 342e 3838 2c36 322e  ,62.46 84.88,62.
+00000b90: 3643 3834 2e37 342c 3633 2e30 3420 3834  6C84.74,63.04 84
+00000ba0: 2e35 392c 3633 2e34 3720 3834 2e34 322c  .59,63.47 84.42,
+00000bb0: 3633 2e39 4c38 342e 3237 2c36 342e 3238  63.9L84.27,64.28
+00000bc0: 4338 342e 312c 3634 2e37 3120 3833 2e39  C84.1,64.71 83.9
+00000bd0: 312c 3635 2e31 3420 3833 2e37 312c 3635  1,65.14 83.71,65
+00000be0: 2e35 3643 3833 2e35 312c 3635 2e39 3820  .56C83.51,65.98 
+00000bf0: 3833 2e34 332c 3636 2e31 3220 3833 2e32  83.43,66.12 83.2
+00000c00: 382c 3636 2e34 4c38 332e 3031 2c36 362e  8,66.4L83.01,66.
+00000c10: 3931 4338 322e 3833 2c36 372e 3232 3320  91C82.83,67.223 
+00000c20: 3832 2e36 3433 2c36 372e 3533 3720 3832  82.643,67.537 82
+00000c30: 2e34 352c 3637 2e38 354c 3832 2e33 352c  .45,67.85L82.35,
+00000c40: 3638 2e30 3143 3739 2e31 3231 2c36 382e  68.01C79.121,68.
+00000c50: 3034 3720 3735 2e39 3138 2c36 372e 3433  047 75.918,67.43
+00000c60: 3420 3732 2e39 332c 3636 2e32 3143 3634  4 72.93,66.21C64
+00000c70: 2e32 372c 3632 2e37 3420 3539 2c35 352e  .27,62.74 59,55.
+00000c80: 3532 2036 312e 3138 2c35 302e 3131 4336  52 61.18,50.11C6
+00000c90: 322e 3138 2c34 372e 3620 3634 2e37 2c34  2.18,47.6 64.7,4
+00000ca0: 352e 3832 2036 382e 3236 2c34 352e 3131  5.82 68.26,45.11
+00000cb0: 4337 322e 3438 392c 3434 2e33 3935 2037  C72.489,44.395 7
+00000cc0: 362e 3833 352c 3434 2e39 3038 2038 302e  6.835,44.908 80.
+00000cd0: 3738 2c34 362e 3539 4338 322e 3134 312c  78,46.59C82.141,
+00000ce0: 3437 2e31 3434 2038 332e 3435 332c 3437  47.144 83.453,47
+00000cf0: 2e38 3133 2038 342e 372c 3438 2e35 3943  .813 84.7,48.59C
+00000d00: 3834 2e37 362c 3438 2e37 3620 3834 2e38  84.76,48.76 84.8
+00000d10: 322c 3438 2e39 3320 3834 2e38 382c 3439  2,48.93 84.88,49
+00000d20: 2e31 4338 342e 3934 2c34 392e 3237 2038  .1C84.94,49.27 8
+00000d30: 352e 3035 2c34 392e 3633 2038 352e 3132  5.05,49.63 85.12
+00000d40: 2c34 392e 3943 3835 2e32 382c 3530 2e35  ,49.9C85.28,50.5
+00000d50: 2038 352e 3434 2c35 312e 3120 3835 2e35   85.44,51.1 85.5
+00000d60: 352c 3531 2e37 3343 3835 2e36 3931 2c35  5,51.73C85.691,5
+00000d70: 322e 3530 3720 3835 2e37 3932 2c35 332e  2.507 85.792,53.
+00000d80: 3239 3220 3835 2e38 352c 3534 2e30 384c  292 85.85,54.08L
+00000d90: 3835 2e38 352c 3535 2e38 3943 3835 2e38  85.85,55.89C85.8
+00000da0: 352c 3536 2e31 3220 3835 2e39 312c 3536  5,56.12 85.91,56
+00000db0: 2e32 3520 3835 2e39 312c 3536 2e34 354c  .25 85.91,56.45L
+00000dc0: 3835 2e38 392c 3536 2e34 345a 4d31 372e  85.89,56.44ZM17.
+00000dd0: 3636 2c36 3843 3136 2e36 3638 2c36 362e  66,68C16.668,66.
+00000de0: 3433 3520 3135 2e38 3639 2c36 342e 3735  435 15.869,64.75
+00000df0: 3620 3135 2e32 382c 3633 4c31 352e 3137  6 15.28,63L15.17
+00000e00: 2c36 322e 3638 4331 352e 3036 2c36 322e  ,62.68C15.06,62.
+00000e10: 3335 2031 342e 3936 2c36 322e 3031 2031  35 14.96,62.01 1
+00000e20: 342e 3837 2c36 312e 3638 4331 342e 3832  4.87,61.68C14.82
+00000e30: 332c 3631 2e34 3933 2031 342e 3737 372c  3,61.493 14.777,
+00000e40: 3631 2e33 3120 3134 2e37 332c 3631 2e31  61.31 14.73,61.1
+00000e50: 3343 3134 2e36 362c 3630 2e38 3420 3134  3C14.66,60.84 14
+00000e60: 2e35 392c 3630 2e35 3520 3134 2e35 332c  .59,60.55 14.53,
+00000e70: 3630 2e32 3743 3134 2e34 372c 3539 2e39  60.27C14.47,59.9
+00000e80: 3920 3134 2e34 332c 3539 2e37 3220 3134  9 14.43,59.72 14
+00000e90: 2e33 382c 3539 2e34 3443 3134 2e33 332c  .38,59.44C14.33,
+00000ea0: 3539 2e31 3620 3134 2e33 2c35 3920 3134  59.16 14.3,59 14
+00000eb0: 2e32 372c 3538 2e37 3843 3134 2e32 2c35  .27,58.78C14.2,5
+00000ec0: 382e 3237 2031 342e 3135 2c35 372e 3738  8.27 14.15,57.78
+00000ed0: 2031 342e 3131 2c35 372e 3233 4c31 342e   14.11,57.23L14.
+00000ee0: 3131 2c35 372e 3033 4331 342e 3030 382c  11,57.03C14.008,
+00000ef0: 3535 2e32 3336 2031 342e 3132 322c 3533  55.236 14.122,53
+00000f00: 2e34 3337 2031 342e 3435 2c35 312e 3637  .437 14.45,51.67
+00000f10: 4331 342e 3536 2c35 312e 3036 2031 342e  C14.56,51.06 14.
+00000f20: 3731 2c35 302e 3436 2031 342e 3838 2c34  71,50.46 14.88,4
+00000f30: 392e 3837 4331 342e 3936 2c34 392e 3539  9.87C14.96,49.59
+00000f40: 2031 352e 3034 2c34 392e 3332 2031 352e   15.04,49.32 15.
+00000f50: 3133 2c34 392e 3035 4331 352e 3232 2c34  13,49.05C15.22,4
+00000f60: 382e 3738 2031 352e 3234 2c34 382e 3732  8.78 15.24,48.72
+00000f70: 2031 352e 332c 3438 2e35 3543 3136 2e35   15.3,48.55C16.5
+00000f80: 3438 2c34 372e 3737 3420 3137 2e38 3539  48,47.774 17.859
+00000f90: 2c34 372e 3130 3520 3139 2e32 322c 3436  ,47.105 19.22,46
+00000fa0: 2e35 3543 3237 2e38 362c 3433 2e30 3920  .55C27.86,43.09 
+00000fb0: 3336 2e36 352c 3434 2e36 3720 3338 2e38  36.65,44.67 38.8
+00000fc0: 322c 3530 2e30 3843 3430 2e39 392c 3535  2,50.08C40.99,55
+00000fd0: 2e34 3920 3335 2e37 332c 3632 2e37 3420  .49 35.73,62.74 
+00000fe0: 3237 2e30 392c 3636 2e32 4332 342e 3130  27.09,66.2C24.10
+00000ff0: 312c 3637 2e34 3331 2032 302e 3839 332c  1,67.431 20.893,
+00001000: 3638 2e30 3433 2031 372e 3636 2c36 385a  68.043 17.66,68Z
+00001010: 4d36 382e 3537 2c37 372e 3638 4336 322e  M68.57,77.68C62.
+00001020: 3535 342c 3739 2e35 3038 2035 362e 3238  554,79.508 56.28
+00001030: 372c 3830 2e33 3736 2035 302c 3830 2e32  7,80.376 50,80.2
+00001040: 3543 3433 2e37 3337 2c38 302e 3337 2033  5C43.737,80.37 3
+00001050: 372e 3439 352c 3739 2e35 3036 2033 312e  7.495,79.506 31.
+00001060: 352c 3737 2e36 3943 3237 2e31 3835 2c37  5,77.69C27.185,7
+00001070: 362e 3338 2032 332e 3234 332c 3734 2e30  6.38 23.243,74.0
+00001080: 3632 2032 302c 3730 2e39 3343 3232 2e38  62 20,70.93C22.8
+00001090: 3135 2c37 302e 3730 3620 3235 2e35 382c  15,70.706 25.58,
+000010a0: 3730 2e30 3535 2032 382e 322c 3639 4333  70.055 28.2,69C3
+000010b0: 382e 3337 2c36 342e 3932 2034 342e 3339  8.37,64.92 44.39
+000010c0: 2c35 3620 3431 2e36 2c34 3943 3338 2e38  ,56 41.6,49C38.8
+000010d0: 312c 3432 2032 382e 3237 2c33 392e 3732  1,42 28.27,39.72
+000010e0: 2031 382e 312c 3433 2e38 4c31 372e 3433   18.1,43.8L17.43
+000010f0: 2c34 342e 3039 4331 382e 3937 332c 3431  ,44.09C18.973,41
+00001100: 2e36 3438 2032 312e 3031 392c 3339 2e35  .648 21.019,39.5
+00001110: 3631 2032 332e 3433 2c33 372e 3937 4332  61 23.43,37.97C2
+00001120: 362e 3637 312c 3335 2e38 3234 2033 302e  6.671,35.824 30.
+00001130: 3437 332c 3334 2e36 3820 3334 2e33 362c  473,34.68 34.36,
+00001140: 3334 2e36 3843 3335 2e38 3834 2c33 342e  34.68C35.884,34.
+00001150: 3638 3120 3337 2e34 3034 2c33 342e 3835  681 37.404,34.85
+00001160: 3220 3338 2e38 392c 3335 2e31 3943 3432  2 38.89,35.19C42
+00001170: 2e36 3934 2c33 362e 3034 3920 3436 2e31  .694,36.049 46.1
+00001180: 3931 2c33 372e 3933 3520 3439 2c34 302e  91,37.935 49,40.
+00001190: 3634 4c35 302c 3431 2e36 344c 3531 2c34  64L50,41.64L51,4
+000011a0: 302e 3634 4335 332e 3739 372c 3337 2e39  0.64C53.797,37.9
+000011b0: 3337 2035 372e 3237 392c 3336 2e30 3439  37 57.279,36.049
+000011c0: 2036 312e 3037 2c33 352e 3138 4336 362e   61.07,35.18C66.
+000011d0: 3430 322c 3333 2e39 3437 2037 322e 3031  402,33.947 72.01
+000011e0: 342c 3334 2e39 3638 2037 362e 3537 2c33  4,34.968 76.57,3
+000011f0: 3843 3738 2e39 382c 3339 2e35 3838 2038  8C78.98,39.588 8
+00001200: 312e 3032 362c 3431 2e36 3731 2038 322e  1.026,41.671 82.
+00001210: 3537 2c34 342e 3131 4c38 312e 392c 3433  57,44.11L81.9,43
+00001220: 2e38 3243 3737 2e34 3039 2c34 312e 3932  .82C77.409,41.92
+00001230: 3120 3732 2e34 3634 2c34 312e 3335 3520  1 72.464,41.355 
+00001240: 3637 2e36 362c 3432 2e31 3943 3633 2e30  67.66,42.19C63.0
+00001250: 382c 3433 2e31 3220 3539 2e37 392c 3435  8,43.12 59.79,45
+00001260: 2e35 3420 3538 2e33 392c 3439 2e30 3243  .54 58.39,49.02C
+00001270: 3535 2e36 2c35 352e 3937 2036 312e 3632  55.6,55.97 61.62
+00001280: 2c36 342e 3934 2037 312e 3739 2c36 392e  ,64.94 71.79,69.
+00001290: 3032 4337 342e 3431 342c 3730 2e30 3720  02C74.414,70.07 
+000012a0: 3737 2e31 3832 2c37 302e 3731 3420 3830  77.182,70.714 80
+000012b0: 2c37 302e 3933 4337 362e 3737 362c 3734  ,70.93C76.776,74
+000012c0: 2e30 3520 3732 2e38 3539 2c37 362e 3336  .05 72.859,76.36
+000012d0: 3320 3638 2e35 372c 3737 2e36 385a 2220  3 68.57,77.68Z" 
+000012e0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+000012f0: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
+00001300: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
+00001310: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
+00001320: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00001330: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
+00001340: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
+00001350: 3132 2c39 2e37 3032 3239 2c2d 312e 3738  12,9.70229,-1.78
+00001360: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
+00001370: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
+00001380: 312e 3333 2220 6379 3d22 3536 2220 723d  1.33" cy="56" r=
+00001390: 2235 2e31 3622 2073 7479 6c65 3d22 6669  "5.16" style="fi
+000013a0: 6c6c 3a72 6762 2832 3232 2c31 3230 2c31  ll:rgb(222,120,1
+000013b0: 3630 293b 222f 3e0a 2020 2020 2020 2020  60);"/>.        
+000013c0: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
+000013d0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+000013e0: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+000013f0: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00001400: 2d31 2e37 3835 3832 2922 3e0a 2020 2020  -1.78582)">.    
+00001410: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
+00001420: 6378 3d22 3238 2e36 3722 2063 793d 2235  cx="28.67" cy="5
+00001430: 3622 2072 3d22 352e 3136 2220 7374 796c  6" r="5.16" styl
+00001440: 653d 2266 696c 6c3a 7267 6228 3232 322c  e="fill:rgb(222,
+00001450: 3132 302c 3136 3029 3b22 2f3e 0a20 2020  120,160);"/>.   
+00001460: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00001470: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00001480: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+00001490: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+000014a0: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
+000014b0: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
+000014c0: 7468 2064 3d22 4d35 382c 3636 4335 352e  th d="M58,66C55.
+000014d0: 3931 322c 3638 2e31 3631 2035 332e 3030  912,68.161 53.00
+000014e0: 332c 3639 2e33 3339 2035 302c 3639 2e32  3,69.339 50,69.2
+000014f0: 3443 3436 2e39 3937 2c36 392e 3333 3920  4C46.997,69.339 
+00001500: 3434 2e30 3838 2c36 382e 3136 3120 3432  44.088,68.161 42
+00001510: 2c36 3643 3431 2e37 3134 2c36 352e 3637  ,66C41.714,65.67
+00001520: 3720 3431 2e33 3032 2c36 352e 3439 3120  7 41.302,65.491 
+00001530: 3430 2e38 372c 3635 2e34 3931 4334 302e  40.87,65.491C40.
+00001540: 3034 322c 3635 2e34 3931 2033 392e 3336  042,65.491 39.36
+00001550: 312c 3636 2e31 3732 2033 392e 3336 312c  1,66.172 39.361,
+00001560: 3637 4333 392e 3336 312c 3637 2e33 3638  67C39.361,67.368
+00001570: 2033 392e 3439 362c 3637 2e37 3234 2033   39.496,67.724 3
+00001580: 392e 3734 2c36 3843 3432 2e34 3033 2c37  9.74,68C42.403,7
+00001590: 302e 3830 3420 3436 2e31 3334 2c37 322e  0.804 46.134,72.
+000015a0: 3335 2035 302c 3732 2e32 3543 3533 2e38  35 50,72.25C53.8
+000015b0: 3632 2c37 322e 3334 3720 3537 2e35 392c  62,72.347 57.59,
+000015c0: 3730 2e38 3032 2036 302e 3235 2c36 3843  70.802 60.25,68C
+000015d0: 3630 2e34 3935 2c36 372e 3732 3520 3630  60.495,67.725 60
+000015e0: 2e36 332c 3637 2e33 3639 2036 302e 3633  .63,67.369 60.63
+000015f0: 2c36 3743 3630 2e36 332c 3636 2e31 3734  ,67C60.63,66.174
+00001600: 2035 392e 3935 312c 3635 2e34 3935 2035   59.951,65.495 5
+00001610: 392e 3132 352c 3635 2e34 3935 4335 382e  9.125,65.495C58.
+00001620: 3639 352c 3635 2e34 3935 2035 382e 3238  695,65.495 58.28
+00001630: 352c 3635 2e36 3739 2035 382c 3636 5a22  5,65.679 58,66Z"
+00001640: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
+00001650: 2832 3232 2c31 3230 2c31 3630 293b 6669  (222,120,160);fi
+00001660: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00001670: 222f 3e0a 2020 2020 2020 2020 3c2f 673e  "/>.        </g>
+00001680: 0a20 2020 203c 2f67 3e0a 3c2f 7376 673e  .    </g>.</svg>
+00001690: 0a                                       .
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/for-the-badge/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/45.svg`

 * *Files 5% similar despite different names*

```diff
@@ -1,362 +1,421 @@
 00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3230 3022 2068  k" width="200" h
-00000060: 6569 6768 743d 2232 3822 2072 6f6c 653d  eight="28" role=
+00000050: 6b22 2077 6964 7468 3d22 3133 3722 2068  k" width="137" h
+00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 494e 5445 5252 4f47 4154 453a 202d  ="INTERROGATE: -
-00000090: 312e 3025 223e 0a20 2020 203c 7469 746c  1.0%">.    <titl
-000000a0: 653e 494e 5445 5252 4f47 4154 453a 202d  e>INTERROGATE: -
-000000b0: 312e 3025 3c2f 7469 746c 653e 0a20 2020  1.0%</title>.   
-000000c0: 203c 6720 7368 6170 652d 7265 6e64 6572   <g shape-render
-000000d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000000e0: 3e0a 2020 2020 2020 2020 3c72 6563 7420  >.        <rect 
-000000f0: 7769 6474 683d 2231 3332 2e37 3522 2068  width="132.75" h
-00000100: 6569 6768 743d 2232 3822 2066 696c 6c3d  eight="28" fill=
-00000110: 2223 3535 3522 2f3e 0a20 2020 2020 2020  "#555"/>.       
-00000120: 203c 7265 6374 2078 3d22 3133 322e 3735   <rect x="132.75
-00000130: 2220 7769 6474 683d 2236 372e 3235 2220  " width="67.25" 
-00000140: 6865 6967 6874 3d22 3238 2220 6669 6c6c  height="28" fill
-00000150: 3d22 2339 6639 6639 6622 2f3e 0a20 2020  ="#9f9f9f"/>.   
-00000160: 203c 2f67 3e0a 2020 2020 3c67 2066 696c   </g>.    <g fil
-00000170: 6c3d 2223 6666 6622 2074 6578 742d 616e  l="#fff" text-an
-00000180: 6368 6f72 3d22 6d69 6464 6c65 2220 666f  chor="middle" fo
-00000190: 6e74 2d66 616d 696c 793d 2256 6572 6461  nt-family="Verda
-000001a0: 6e61 2c47 656e 6576 612c 4465 6a61 5675  na,Geneva,DejaVu
-000001b0: 2053 616e 732c 7361 6e73 2d73 6572 6966   Sans,sans-serif
-000001c0: 2220 7465 7874 2d72 656e 6465 7269 6e67  " text-rendering
-000001d0: 3d22 6765 6f6d 6574 7269 6350 7265 6369  ="geometricPreci
-000001e0: 7369 6f6e 2220 666f 6e74 2d73 697a 653d  sion" font-size=
-000001f0: 2231 3030 223e 0a20 2020 2020 2020 203c  "100">.        <
-00000200: 7465 7874 2074 7261 6e73 666f 726d 3d22  text transform="
-00000210: 7363 616c 6528 2e31 2922 2078 3d22 3737  scale(.1)" x="77
-00000220: 302e 3735 2220 793d 2231 3735 2220 7465  0.75" y="175" te
-00000230: 7874 4c65 6e67 7468 3d22 3836 372e 3522  xtLength="867.5"
-00000240: 2066 696c 6c3d 2223 6666 6622 3e49 4e54   fill="#fff">INT
-00000250: 4552 524f 4741 5445 3c2f 7465 7874 3e0a  ERROGATE</text>.
-00000260: 2020 2020 2020 2020 3c74 6578 7420 7472          <text tr
-00000270: 616e 7366 6f72 6d3d 2273 6361 6c65 282e  ansform="scale(.
-00000280: 3129 2220 783d 2231 3638 302e 3735 2220  1)" x="1680.75" 
-00000290: 793d 2231 3735 2220 7465 7874 4c65 6e67  y="175" textLeng
-000002a0: 7468 3d22 3335 3022 2066 696c 6c3d 2223  th="350" fill="#
-000002b0: 6666 6622 2066 6f6e 742d 7765 6967 6874  fff" font-weight
-000002c0: 3d22 626f 6c64 2220 6461 7461 2d69 6e74  ="bold" data-int
-000002d0: 6572 726f 6761 7465 3d22 7265 7375 6c74  errogate="result
-000002e0: 223e 2d31 2e30 253c 2f74 6578 743e 0a20  ">-1.0%</text>. 
-000002f0: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
-00000300: 643d 226c 6f67 6f2d 7069 6e6b 2220 7472  d="logo-pink" tr
-00000310: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00000320: 302e 3835 3438 3736 2c30 2c30 2c30 2e38  0.854876,0,0,0.8
-00000330: 3534 3837 362c 2d34 2e37 3335 3134 2c30  54876,-4.73514,0
-00000340: 2e38 3737 3132 3429 223e 0a20 2020 2020  .877124)">.     
-00000350: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00000360: 226d 6174 7269 7828 302e 3239 3930 3132  "matrix(0.299012
-00000370: 2c30 2c30 2c30 2e32 3939 3031 322c 392e  ,0,0,0.299012,9.
-00000380: 3730 3232 392c 2d31 2e37 3835 3832 2922  70229,-1.78582)"
-00000390: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
-000003a0: 6174 6820 643d 224d 3530 2c36 342e 3235  ath d="M50,64.25
-000003b0: 4335 322e 3736 2c36 342e 3235 2035 352c  C52.76,64.25 55,
-000003c0: 3631 2e31 3320 3535 2c35 392e 3735 4335  61.13 55,59.75C5
-000003d0: 352c 3538 2e33 3720 3532 2e37 362c 3537  5,58.37 52.76,57
-000003e0: 2e32 3520 3530 2c35 372e 3235 4334 372e  .25 50,57.25C47.
-000003f0: 3234 2c35 372e 3235 2034 352c 3538 2e33  24,57.25 45,58.3
-00000400: 3720 3435 2c35 392e 3735 4334 352c 3631  7 45,59.75C45,61
-00000410: 2e31 3320 3437 2e32 342c 3634 2e32 3520  .13 47.24,64.25 
-00000420: 3530 2c36 342e 3235 5a22 2073 7479 6c65  50,64.25Z" style
-00000430: 3d22 6669 6c6c 3a72 6762 2832 3232 2c31  ="fill:rgb(222,1
-00000440: 3230 2c31 3630 293b 6669 6c6c 2d72 756c  20,160);fill-rul
-00000450: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
-00000460: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
-00000470: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00000480: 226d 6174 7269 7828 302e 3239 3930 3132  "matrix(0.299012
-00000490: 2c30 2c30 2c30 2e32 3939 3031 322c 392e  ,0,0,0.299012,9.
-000004a0: 3730 3232 392c 2d31 2e37 3835 3832 2922  70229,-1.78582)"
-000004b0: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
-000004c0: 6174 6820 643d 224d 3838 2c34 392e 3035  ath d="M88,49.05
-000004d0: 4338 362e 3530 362c 3433 2e34 3735 2038  C86.506,43.475 8
-000004e0: 332e 3031 382c 3338 2e36 3338 2037 382e  3.018,38.638 78.
-000004f0: 322c 3335 2e34 3643 3732 2e39 3639 2c33  2,35.46C72.969,3
-00000500: 322e 3030 3220 3636 2e35 3339 2c33 302e  2.002 66.539,30.
-00000510: 3834 3420 3630 2e34 332c 3332 2e32 3643  844 60.43,32.26C
-00000520: 3536 2e35 3736 2c33 332e 3134 3520 3532  56.576,33.145 52
-00000530: 2e39 3935 2c33 342e 3935 3820 3530 2c33  .995,34.958 50,3
-00000540: 372e 3534 4334 362e 3939 382c 3334 2e39  7.54C46.998,34.9
-00000550: 3538 2034 332e 3431 312c 3333 2e31 3439  58 43.411,33.149
-00000560: 2033 392e 3535 2c33 322e 3237 4333 332e   39.55,32.27C33.
-00000570: 3434 312c 3330 2e38 3533 2032 372e 3031  441,30.853 27.01
-00000580: 312c 3332 2e30 3131 2032 312e 3738 2c33  1,32.011 21.78,3
-00000590: 352e 3437 4331 362e 3937 2c33 382e 3635  5.47C16.97,38.65
-000005a0: 3220 3133 2e34 3839 2c34 332e 3438 3920  2 13.489,43.489 
-000005b0: 3132 2c34 392e 3036 4c31 322c 3439 2e31  12,49.06L12,49.1
-000005c0: 3343 3131 2e38 322c 3439 2e37 3920 3131  3C11.82,49.79 11
-000005d0: 2e36 362c 3530 2e34 3620 3131 2e35 332c  .66,50.46 11.53,
-000005e0: 3531 2e31 3343 3131 2e31 3436 2c35 332e  51.13C11.146,53.
-000005f0: 3230 3720 3131 2e30 3231 2c35 352e 3332  207 11.021,55.32
-00000600: 3320 3131 2e31 362c 3537 2e34 3343 3131  3 11.16,57.43C11
-00000610: 2e31 362c 3538 2e30 3320 3131 2e32 362c  .16,58.03 11.26,
-00000620: 3538 2e36 3320 3131 2e33 342c 3539 2e32  58.63 11.34,59.2
-00000630: 3343 3131 2e33 342c 3539 2e35 3120 3131  3C11.34,59.51 11
-00000640: 2e34 332c 3539 2e37 3920 3131 2e34 382c  .43,59.79 11.48,
-00000650: 3630 2e30 3743 3131 2e35 332c 3630 2e33  60.07C11.53,60.3
-00000660: 3520 3131 2e35 382c 3630 2e36 3820 3131  5 11.58,60.68 11
-00000670: 2e36 342c 3630 2e39 3843 3131 2e37 2c36  .64,60.98C11.7,6
-00000680: 312e 3238 2031 312e 382c 3631 2e36 3920  1.28 11.8,61.69 
-00000690: 3131 2e38 392c 3632 2e30 3543 3131 2e39  11.89,62.05C11.9
-000006a0: 382c 3632 2e34 3120 3131 2e39 392c 3632  8,62.41 11.99,62
-000006b0: 2e34 3720 3132 2e30 352c 3632 2e36 3843  .47 12.05,62.68C
-000006c0: 3132 2e31 362c 3633 2e30 3720 3132 2e32  12.16,63.07 12.2
-000006d0: 382c 3633 2e34 3620 3132 2e34 312c 3633  8,63.46 12.41,63
-000006e0: 2e38 344c 3132 2e35 382c 3634 2e33 3443  .84L12.58,64.34C
-000006f0: 3132 2e37 322c 3634 2e37 3420 3132 2e38  12.72,64.74 12.8
-00000700: 382c 3635 2e31 3420 3133 2e30 342c 3635  8,65.14 13.04,65
-00000710: 2e35 334c 3133 2e32 332c 3635 2e39 3843  .53L13.23,65.98C
-00000720: 3133 2e34 3033 2c36 362e 3337 3320 3133  13.403,66.373 13
-00000730: 2e35 3833 2c36 362e 3736 3720 3133 2e37  .583,66.767 13.7
-00000740: 372c 3637 2e31 364c 3133 2e39 392c 3637  7,67.16L13.99,67
-00000750: 2e35 3943 3134 2e31 392c 3637 2e39 3720  .59C14.19,67.97 
-00000760: 3134 2e33 392c 3638 2e33 3520 3134 2e36  14.39,68.35 14.6
-00000770: 312c 3638 2e37 334c 3134 2e38 372c 3639  1,68.73L14.87,69
-00000780: 2e31 3543 3135 2e31 2c36 392e 3532 2031  .15C15.1,69.52 1
-00000790: 352e 3333 2c36 392e 3839 2031 352e 3538  5.33,69.89 15.58
-000007a0: 2c37 302e 3236 4c31 352e 3538 2c37 302e  ,70.26L15.58,70.
-000007b0: 3332 4c31 352e 3939 2c37 302e 3933 4331  32L15.99,70.93C1
-000007c0: 362e 3134 2c37 312e 3134 2031 362e 3239  6.14,71.14 16.29
-000007d0: 2c37 312e 3336 2031 362e 3435 2c37 312e  ,71.36 16.45,71.
-000007e0: 3537 4332 302e 3230 362c 3735 2e38 3320  57C20.206,75.83 
-000007f0: 3235 2e30 3836 2c37 382e 3935 2033 302e  25.086,78.95 30.
-00000800: 3533 2c38 302e 3537 4333 362e 3833 392c  53,80.57C36.839,
-00000810: 3832 2e34 3820 3433 2e34 312c 3833 2e33  82.48 43.41,83.3
-00000820: 3835 2035 302c 3833 2e32 3543 3536 2e35  85 50,83.25C56.5
-00000830: 3939 2c38 332e 3337 3420 3633 2e31 3737  99,83.374 63.177
-00000840: 2c38 322e 3435 3620 3639 2e34 392c 3830  ,82.456 69.49,80
-00000850: 2e35 3343 3734 2e36 3434 2c37 382e 3937  .53C74.644,78.97
-00000860: 3820 3739 2e33 3033 2c37 362e 3130 3220  8 79.303,76.102 
-00000870: 3833 2c37 322e 3139 4338 332e 3334 2c37  83,72.19C83.34,7
-00000880: 312e 3738 2038 332e 3635 2c37 312e 3335  1.78 83.65,71.35
-00000890: 2038 342c 3730 2e39 324c 3834 2e31 382c   84,70.92L84.18,
-000008a0: 3730 2e36 364c 3834 2e33 332c 3730 2e34  70.66L84.33,70.4
-000008b0: 344c 3834 2e34 312c 3730 2e33 3243 3834  4L84.41,70.32C84
-000008c0: 2e35 352c 3730 2e31 3220 3834 2e36 372c  .55,70.12 84.67,
-000008d0: 3639 2e39 2038 342e 3831 2c36 392e 3743  69.9 84.81,69.7C
-000008e0: 3835 2e30 372c 3639 2e33 2038 352e 3332  85.07,69.3 85.32
-000008f0: 2c36 382e 3839 2038 352e 3535 2c36 382e  ,68.89 85.55,68.
-00000900: 3438 4338 352e 3738 2c36 382e 3037 2038  48C85.78,68.07 8
-00000910: 362e 3032 2c36 372e 3635 2038 362e 3233  6.02,67.65 86.23
-00000920: 2c36 372e 3232 4338 362e 3331 2c36 372e  ,67.22C86.31,67.
-00000930: 3035 2038 362e 3339 2c36 362e 3838 2038  05 86.39,66.88 8
-00000940: 362e 3437 2c36 362e 3743 3836 2e36 372c  6.47,66.7C86.67,
-00000950: 3636 2e32 3820 3836 2e38 352c 3635 2e38  66.28 86.85,65.8
-00000960: 3720 3837 2e30 332c 3635 2e34 344c 3837  7 87.03,65.44L87
-00000970: 2e32 332c 3634 2e39 3243 3837 2e33 3937  .23,64.92C87.397
-00000980: 2c36 342e 3438 3720 3837 2e35 352c 3634  ,64.487 87.55,64
-00000990: 2e30 3520 3837 2e36 392c 3633 2e36 314c  .05 87.69,63.61L
-000009a0: 3837 2e38 352c 3633 2e30 3943 3837 2e39  87.85,63.09C87.9
-000009b0: 382c 3632 2e36 3420 3838 2e31 2c36 322e  8,62.64 88.1,62.
-000009c0: 3139 2038 382e 3231 2c36 312e 3734 4338  19 88.21,61.74C8
-000009d0: 382e 3231 2c36 312e 3537 2038 382e 332c  8.21,61.57 88.3,
-000009e0: 3631 2e33 3920 3838 2e33 332c 3631 2e32  61.39 88.33,61.2
-000009f0: 3243 3838 2e34 332c 3630 2e37 3520 3838  2C88.43,60.75 88
-00000a00: 2e35 322c 3630 2e32 3220 3838 2e36 2c35  .52,60.22 88.6,5
-00000a10: 392e 3739 4338 382e 362c 3539 2e36 3420  9.79C88.6,59.64 
-00000a20: 3838 2e36 362c 3539 2e34 3920 3838 2e36  88.66,59.49 88.6
-00000a30: 382c 3539 2e33 3343 3838 2e37 372c 3538  8,59.33C88.77,58
-00000a40: 2e37 3120 3838 2e38 342c 3538 2e30 3820  .71 88.84,58.08 
-00000a50: 3838 2e38 382c 3537 2e34 354c 3838 2e38  88.88,57.45L88.8
-00000a60: 382c 3534 2e31 3743 3838 2e38 3137 2c35  8,54.17C88.817,5
-00000a70: 332e 3136 3420 3838 2e36 3933 2c35 322e  3.164 88.693,52.
-00000a80: 3136 3220 3838 2e35 312c 3531 2e31 3743  162 88.51,51.17C
-00000a90: 3838 2e33 382c 3530 2e35 2038 382e 3233  88.38,50.5 88.23
-00000aa0: 2c34 392e 3834 2038 382e 3035 2c34 392e  ,49.84 88.05,49.
-00000ab0: 3137 4c38 382c 3439 2e30 355a 4d38 352e  17L88,49.05ZM85.
-00000ac0: 3839 2c35 362e 3434 4c38 352e 3839 2c35  89,56.44L85.89,5
-00000ad0: 372e 3233 4338 352e 3839 2c35 372e 3738  7.23C85.89,57.78
-00000ae0: 2038 352e 3739 2c35 382e 3332 2038 352e   85.79,58.32 85.
-00000af0: 3732 2c35 382e 3836 4338 352e 3732 2c35  72,58.86C85.72,5
-00000b00: 392e 3031 2038 352e 3732 2c35 392e 3135  9.01 85.72,59.15
-00000b10: 2038 352e 3635 2c35 392e 3343 3835 2e35   85.65,59.3C85.5
-00000b20: 392c 3539 2e37 2038 352e 3531 2c36 302e  9,59.7 85.51,60.
-00000b30: 3131 2038 352e 3433 2c36 302e 3531 4c38  11 85.43,60.51L8
-00000b40: 352e 3332 2c36 302e 3939 4338 352e 3233  5.32,60.99C85.23
-00000b50: 2c36 312e 3338 2038 352e 3132 2c36 312e  ,61.38 85.12,61.
-00000b60: 3737 2038 352e 3031 2c36 322e 3136 4338  77 85.01,62.16C8
-00000b70: 352e 3031 2c36 322e 3331 2038 342e 3933  5.01,62.31 84.93
-00000b80: 2c36 322e 3436 2038 342e 3838 2c36 322e  ,62.46 84.88,62.
-00000b90: 3643 3834 2e37 342c 3633 2e30 3420 3834  6C84.74,63.04 84
-00000ba0: 2e35 392c 3633 2e34 3720 3834 2e34 322c  .59,63.47 84.42,
-00000bb0: 3633 2e39 4c38 342e 3237 2c36 342e 3238  63.9L84.27,64.28
-00000bc0: 4338 342e 312c 3634 2e37 3120 3833 2e39  C84.1,64.71 83.9
-00000bd0: 312c 3635 2e31 3420 3833 2e37 312c 3635  1,65.14 83.71,65
-00000be0: 2e35 3643 3833 2e35 312c 3635 2e39 3820  .56C83.51,65.98 
-00000bf0: 3833 2e34 332c 3636 2e31 3220 3833 2e32  83.43,66.12 83.2
-00000c00: 382c 3636 2e34 4c38 332e 3031 2c36 362e  8,66.4L83.01,66.
-00000c10: 3931 4338 322e 3833 2c36 372e 3232 3320  91C82.83,67.223 
-00000c20: 3832 2e36 3433 2c36 372e 3533 3720 3832  82.643,67.537 82
-00000c30: 2e34 352c 3637 2e38 354c 3832 2e33 352c  .45,67.85L82.35,
-00000c40: 3638 2e30 3143 3739 2e31 3231 2c36 382e  68.01C79.121,68.
-00000c50: 3034 3720 3735 2e39 3138 2c36 372e 3433  047 75.918,67.43
-00000c60: 3420 3732 2e39 332c 3636 2e32 3143 3634  4 72.93,66.21C64
-00000c70: 2e32 372c 3632 2e37 3420 3539 2c35 352e  .27,62.74 59,55.
-00000c80: 3532 2036 312e 3138 2c35 302e 3131 4336  52 61.18,50.11C6
-00000c90: 322e 3138 2c34 372e 3620 3634 2e37 2c34  2.18,47.6 64.7,4
-00000ca0: 352e 3832 2036 382e 3236 2c34 352e 3131  5.82 68.26,45.11
-00000cb0: 4337 322e 3438 392c 3434 2e33 3935 2037  C72.489,44.395 7
-00000cc0: 362e 3833 352c 3434 2e39 3038 2038 302e  6.835,44.908 80.
-00000cd0: 3738 2c34 362e 3539 4338 322e 3134 312c  78,46.59C82.141,
-00000ce0: 3437 2e31 3434 2038 332e 3435 332c 3437  47.144 83.453,47
-00000cf0: 2e38 3133 2038 342e 372c 3438 2e35 3943  .813 84.7,48.59C
-00000d00: 3834 2e37 362c 3438 2e37 3620 3834 2e38  84.76,48.76 84.8
-00000d10: 322c 3438 2e39 3320 3834 2e38 382c 3439  2,48.93 84.88,49
-00000d20: 2e31 4338 342e 3934 2c34 392e 3237 2038  .1C84.94,49.27 8
-00000d30: 352e 3035 2c34 392e 3633 2038 352e 3132  5.05,49.63 85.12
-00000d40: 2c34 392e 3943 3835 2e32 382c 3530 2e35  ,49.9C85.28,50.5
-00000d50: 2038 352e 3434 2c35 312e 3120 3835 2e35   85.44,51.1 85.5
-00000d60: 352c 3531 2e37 3343 3835 2e36 3931 2c35  5,51.73C85.691,5
-00000d70: 322e 3530 3720 3835 2e37 3932 2c35 332e  2.507 85.792,53.
-00000d80: 3239 3220 3835 2e38 352c 3534 2e30 384c  292 85.85,54.08L
-00000d90: 3835 2e38 352c 3535 2e38 3943 3835 2e38  85.85,55.89C85.8
-00000da0: 352c 3536 2e31 3220 3835 2e39 312c 3536  5,56.12 85.91,56
-00000db0: 2e32 3520 3835 2e39 312c 3536 2e34 354c  .25 85.91,56.45L
-00000dc0: 3835 2e38 392c 3536 2e34 345a 4d31 372e  85.89,56.44ZM17.
-00000dd0: 3636 2c36 3843 3136 2e36 3638 2c36 362e  66,68C16.668,66.
-00000de0: 3433 3520 3135 2e38 3639 2c36 342e 3735  435 15.869,64.75
-00000df0: 3620 3135 2e32 382c 3633 4c31 352e 3137  6 15.28,63L15.17
-00000e00: 2c36 322e 3638 4331 352e 3036 2c36 322e  ,62.68C15.06,62.
-00000e10: 3335 2031 342e 3936 2c36 322e 3031 2031  35 14.96,62.01 1
-00000e20: 342e 3837 2c36 312e 3638 4331 342e 3832  4.87,61.68C14.82
-00000e30: 332c 3631 2e34 3933 2031 342e 3737 372c  3,61.493 14.777,
-00000e40: 3631 2e33 3120 3134 2e37 332c 3631 2e31  61.31 14.73,61.1
-00000e50: 3343 3134 2e36 362c 3630 2e38 3420 3134  3C14.66,60.84 14
-00000e60: 2e35 392c 3630 2e35 3520 3134 2e35 332c  .59,60.55 14.53,
-00000e70: 3630 2e32 3743 3134 2e34 372c 3539 2e39  60.27C14.47,59.9
-00000e80: 3920 3134 2e34 332c 3539 2e37 3220 3134  9 14.43,59.72 14
-00000e90: 2e33 382c 3539 2e34 3443 3134 2e33 332c  .38,59.44C14.33,
-00000ea0: 3539 2e31 3620 3134 2e33 2c35 3920 3134  59.16 14.3,59 14
-00000eb0: 2e32 372c 3538 2e37 3843 3134 2e32 2c35  .27,58.78C14.2,5
-00000ec0: 382e 3237 2031 342e 3135 2c35 372e 3738  8.27 14.15,57.78
-00000ed0: 2031 342e 3131 2c35 372e 3233 4c31 342e   14.11,57.23L14.
-00000ee0: 3131 2c35 372e 3033 4331 342e 3030 382c  11,57.03C14.008,
-00000ef0: 3535 2e32 3336 2031 342e 3132 322c 3533  55.236 14.122,53
-00000f00: 2e34 3337 2031 342e 3435 2c35 312e 3637  .437 14.45,51.67
-00000f10: 4331 342e 3536 2c35 312e 3036 2031 342e  C14.56,51.06 14.
-00000f20: 3731 2c35 302e 3436 2031 342e 3838 2c34  71,50.46 14.88,4
-00000f30: 392e 3837 4331 342e 3936 2c34 392e 3539  9.87C14.96,49.59
-00000f40: 2031 352e 3034 2c34 392e 3332 2031 352e   15.04,49.32 15.
-00000f50: 3133 2c34 392e 3035 4331 352e 3232 2c34  13,49.05C15.22,4
-00000f60: 382e 3738 2031 352e 3234 2c34 382e 3732  8.78 15.24,48.72
-00000f70: 2031 352e 332c 3438 2e35 3543 3136 2e35   15.3,48.55C16.5
-00000f80: 3438 2c34 372e 3737 3420 3137 2e38 3539  48,47.774 17.859
-00000f90: 2c34 372e 3130 3520 3139 2e32 322c 3436  ,47.105 19.22,46
-00000fa0: 2e35 3543 3237 2e38 362c 3433 2e30 3920  .55C27.86,43.09 
-00000fb0: 3336 2e36 352c 3434 2e36 3720 3338 2e38  36.65,44.67 38.8
-00000fc0: 322c 3530 2e30 3843 3430 2e39 392c 3535  2,50.08C40.99,55
-00000fd0: 2e34 3920 3335 2e37 332c 3632 2e37 3420  .49 35.73,62.74 
-00000fe0: 3237 2e30 392c 3636 2e32 4332 342e 3130  27.09,66.2C24.10
-00000ff0: 312c 3637 2e34 3331 2032 302e 3839 332c  1,67.431 20.893,
-00001000: 3638 2e30 3433 2031 372e 3636 2c36 385a  68.043 17.66,68Z
-00001010: 4d36 382e 3537 2c37 372e 3638 4336 322e  M68.57,77.68C62.
-00001020: 3535 342c 3739 2e35 3038 2035 362e 3238  554,79.508 56.28
-00001030: 372c 3830 2e33 3736 2035 302c 3830 2e32  7,80.376 50,80.2
-00001040: 3543 3433 2e37 3337 2c38 302e 3337 2033  5C43.737,80.37 3
-00001050: 372e 3439 352c 3739 2e35 3036 2033 312e  7.495,79.506 31.
-00001060: 352c 3737 2e36 3943 3237 2e31 3835 2c37  5,77.69C27.185,7
-00001070: 362e 3338 2032 332e 3234 332c 3734 2e30  6.38 23.243,74.0
-00001080: 3632 2032 302c 3730 2e39 3343 3232 2e38  62 20,70.93C22.8
-00001090: 3135 2c37 302e 3730 3620 3235 2e35 382c  15,70.706 25.58,
-000010a0: 3730 2e30 3535 2032 382e 322c 3639 4333  70.055 28.2,69C3
-000010b0: 382e 3337 2c36 342e 3932 2034 342e 3339  8.37,64.92 44.39
-000010c0: 2c35 3620 3431 2e36 2c34 3943 3338 2e38  ,56 41.6,49C38.8
-000010d0: 312c 3432 2032 382e 3237 2c33 392e 3732  1,42 28.27,39.72
-000010e0: 2031 382e 312c 3433 2e38 4c31 372e 3433   18.1,43.8L17.43
-000010f0: 2c34 342e 3039 4331 382e 3937 332c 3431  ,44.09C18.973,41
-00001100: 2e36 3438 2032 312e 3031 392c 3339 2e35  .648 21.019,39.5
-00001110: 3631 2032 332e 3433 2c33 372e 3937 4332  61 23.43,37.97C2
-00001120: 362e 3637 312c 3335 2e38 3234 2033 302e  6.671,35.824 30.
-00001130: 3437 332c 3334 2e36 3820 3334 2e33 362c  473,34.68 34.36,
-00001140: 3334 2e36 3843 3335 2e38 3834 2c33 342e  34.68C35.884,34.
-00001150: 3638 3120 3337 2e34 3034 2c33 342e 3835  681 37.404,34.85
-00001160: 3220 3338 2e38 392c 3335 2e31 3943 3432  2 38.89,35.19C42
-00001170: 2e36 3934 2c33 362e 3034 3920 3436 2e31  .694,36.049 46.1
-00001180: 3931 2c33 372e 3933 3520 3439 2c34 302e  91,37.935 49,40.
-00001190: 3634 4c35 302c 3431 2e36 344c 3531 2c34  64L50,41.64L51,4
-000011a0: 302e 3634 4335 332e 3739 372c 3337 2e39  0.64C53.797,37.9
-000011b0: 3337 2035 372e 3237 392c 3336 2e30 3439  37 57.279,36.049
-000011c0: 2036 312e 3037 2c33 352e 3138 4336 362e   61.07,35.18C66.
-000011d0: 3430 322c 3333 2e39 3437 2037 322e 3031  402,33.947 72.01
-000011e0: 342c 3334 2e39 3638 2037 362e 3537 2c33  4,34.968 76.57,3
-000011f0: 3843 3738 2e39 382c 3339 2e35 3838 2038  8C78.98,39.588 8
-00001200: 312e 3032 362c 3431 2e36 3731 2038 322e  1.026,41.671 82.
-00001210: 3537 2c34 342e 3131 4c38 312e 392c 3433  57,44.11L81.9,43
-00001220: 2e38 3243 3737 2e34 3039 2c34 312e 3932  .82C77.409,41.92
-00001230: 3120 3732 2e34 3634 2c34 312e 3335 3520  1 72.464,41.355 
-00001240: 3637 2e36 362c 3432 2e31 3943 3633 2e30  67.66,42.19C63.0
-00001250: 382c 3433 2e31 3220 3539 2e37 392c 3435  8,43.12 59.79,45
-00001260: 2e35 3420 3538 2e33 392c 3439 2e30 3243  .54 58.39,49.02C
-00001270: 3535 2e36 2c35 352e 3937 2036 312e 3632  55.6,55.97 61.62
-00001280: 2c36 342e 3934 2037 312e 3739 2c36 392e  ,64.94 71.79,69.
-00001290: 3032 4337 342e 3431 342c 3730 2e30 3720  02C74.414,70.07 
-000012a0: 3737 2e31 3832 2c37 302e 3731 3420 3830  77.182,70.714 80
-000012b0: 2c37 302e 3933 4337 362e 3737 362c 3734  ,70.93C76.776,74
-000012c0: 2e30 3520 3732 2e38 3539 2c37 362e 3336  .05 72.859,76.36
-000012d0: 3320 3638 2e35 372c 3737 2e36 385a 2220  3 68.57,77.68Z" 
-000012e0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
-000012f0: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
-00001300: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
-00001310: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
-00001320: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-00001330: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
-00001340: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
-00001350: 3132 2c39 2e37 3032 3239 2c2d 312e 3738  12,9.70229,-1.78
-00001360: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
-00001370: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-00001380: 312e 3333 2220 6379 3d22 3536 2220 723d  1.33" cy="56" r=
-00001390: 2235 2e31 3622 2073 7479 6c65 3d22 6669  "5.16" style="fi
-000013a0: 6c6c 3a72 6762 2832 3232 2c31 3230 2c31  ll:rgb(222,120,1
-000013b0: 3630 293b 222f 3e0a 2020 2020 2020 2020  60);"/>.        
-000013c0: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
-000013d0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-000013e0: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-000013f0: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00001400: 2d31 2e37 3835 3832 2922 3e0a 2020 2020  -1.78582)">.    
-00001410: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
-00001420: 6378 3d22 3238 2e36 3722 2063 793d 2235  cx="28.67" cy="5
-00001430: 3622 2072 3d22 352e 3136 2220 7374 796c  6" r="5.16" styl
-00001440: 653d 2266 696c 6c3a 7267 6228 3232 322c  e="fill:rgb(222,
-00001450: 3132 302c 3136 3029 3b22 2f3e 0a20 2020  120,160);"/>.   
-00001460: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00001470: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00001480: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-00001490: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-000014a0: 3032 3239 2c2d 312e 3738 3538 3229 223e  0229,-1.78582)">
-000014b0: 0a20 2020 2020 2020 2020 2020 203c 7061  .            <pa
-000014c0: 7468 2064 3d22 4d35 382c 3636 4335 352e  th d="M58,66C55.
-000014d0: 3931 322c 3638 2e31 3631 2035 332e 3030  912,68.161 53.00
-000014e0: 332c 3639 2e33 3339 2035 302c 3639 2e32  3,69.339 50,69.2
-000014f0: 3443 3436 2e39 3937 2c36 392e 3333 3920  4C46.997,69.339 
-00001500: 3434 2e30 3838 2c36 382e 3136 3120 3432  44.088,68.161 42
-00001510: 2c36 3643 3431 2e37 3134 2c36 352e 3637  ,66C41.714,65.67
-00001520: 3720 3431 2e33 3032 2c36 352e 3439 3120  7 41.302,65.491 
-00001530: 3430 2e38 372c 3635 2e34 3931 4334 302e  40.87,65.491C40.
-00001540: 3034 322c 3635 2e34 3931 2033 392e 3336  042,65.491 39.36
-00001550: 312c 3636 2e31 3732 2033 392e 3336 312c  1,66.172 39.361,
-00001560: 3637 4333 392e 3336 312c 3637 2e33 3638  67C39.361,67.368
-00001570: 2033 392e 3439 362c 3637 2e37 3234 2033   39.496,67.724 3
-00001580: 392e 3734 2c36 3843 3432 2e34 3033 2c37  9.74,68C42.403,7
-00001590: 302e 3830 3420 3436 2e31 3334 2c37 322e  0.804 46.134,72.
-000015a0: 3335 2035 302c 3732 2e32 3543 3533 2e38  35 50,72.25C53.8
-000015b0: 3632 2c37 322e 3334 3720 3537 2e35 392c  62,72.347 57.59,
-000015c0: 3730 2e38 3032 2036 302e 3235 2c36 3843  70.802 60.25,68C
-000015d0: 3630 2e34 3935 2c36 372e 3732 3520 3630  60.495,67.725 60
-000015e0: 2e36 332c 3637 2e33 3639 2036 302e 3633  .63,67.369 60.63
-000015f0: 2c36 3743 3630 2e36 332c 3636 2e31 3734  ,67C60.63,66.174
-00001600: 2035 392e 3935 312c 3635 2e34 3935 2035   59.951,65.495 5
-00001610: 392e 3132 352c 3635 2e34 3935 4335 382e  9.125,65.495C58.
-00001620: 3639 352c 3635 2e34 3935 2035 382e 3238  695,65.495 58.28
-00001630: 352c 3635 2e36 3739 2035 382c 3636 5a22  5,65.679 58,66Z"
-00001640: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
-00001650: 2832 3232 2c31 3230 2c31 3630 293b 6669  (222,120,160);fi
-00001660: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-00001670: 222f 3e0a 2020 2020 2020 2020 3c2f 673e  "/>.        </g>
-00001680: 0a20 2020 203c 2f67 3e0a 3c2f 7376 673e  .    </g>.</svg>
-00001690: 0a                                       .
+00000080: 3d22 496e 7465 7272 6f67 6174 653a 2031  ="Interrogate: 1
+00000090: 3030 2522 3e0a 2020 2020 3c74 6974 6c65  00%">.    <title
+000000a0: 3e49 6e74 6572 726f 6761 7465 3a20 3130  >Interrogate: 10
+000000b0: 3025 3c2f 7469 746c 653e 0a20 2020 203c  0%</title>.    <
+000000c0: 7374 796c 653e 613a 686f 7665 7220 236c  style>a:hover #l
+000000d0: 6c69 6e6b 7b66 696c 6c3a 7572 6c28 2362  link{fill:url(#b
+000000e0: 293b 7374 726f 6b65 3a23 6363 637d 613a  );stroke:#ccc}a:
+000000f0: 686f 7665 7220 2372 6c69 6e6b 7b66 696c  hover #rlink{fil
+00000100: 6c3a 2334 3138 3363 347d 3c2f 7374 796c  l:#4183c4}</styl
+00000110: 653e 0a20 2020 203c 6c69 6e65 6172 4772  e>.    <linearGr
+00000120: 6164 6965 6e74 2069 643d 2261 2220 7832  adient id="a" x2
+00000130: 3d22 3022 2079 323d 2231 3030 2522 3e0a  ="0" y2="100%">.
+00000140: 2020 2020 2020 2020 3c73 746f 7020 6f66          <stop of
+00000150: 6673 6574 3d22 3022 2073 746f 702d 636f  fset="0" stop-co
+00000160: 6c6f 723d 2223 6663 6663 6663 2220 7374  lor="#fcfcfc" st
+00000170: 6f70 2d6f 7061 6369 7479 3d22 3022 2f3e  op-opacity="0"/>
+00000180: 0a20 2020 2020 2020 203c 7374 6f70 206f  .        <stop o
+00000190: 6666 7365 743d 2231 2220 7374 6f70 2d6f  ffset="1" stop-o
+000001a0: 7061 6369 7479 3d22 2e31 222f 3e0a 2020  pacity=".1"/>.  
+000001b0: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
+000001c0: 6e74 3e0a 2020 2020 3c6c 696e 6561 7247  nt>.    <linearG
+000001d0: 7261 6469 656e 7420 6964 3d22 6222 2078  radient id="b" x
+000001e0: 323d 2230 2220 7932 3d22 3130 3025 223e  2="0" y2="100%">
+000001f0: 0a20 2020 2020 2020 203c 7374 6f70 206f  .        <stop o
+00000200: 6666 7365 743d 2230 2220 7374 6f70 2d63  ffset="0" stop-c
+00000210: 6f6c 6f72 3d22 2363 6363 2220 7374 6f70  olor="#ccc" stop
+00000220: 2d6f 7061 6369 7479 3d22 2e31 222f 3e0a  -opacity=".1"/>.
+00000230: 2020 2020 2020 2020 3c73 746f 7020 6f66          <stop of
+00000240: 6673 6574 3d22 3122 2073 746f 702d 6f70  fset="1" stop-op
+00000250: 6163 6974 793d 222e 3122 2f3e 0a20 2020  acity=".1"/>.   
+00000260: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
+00000270: 743e 0a20 2020 203c 6720 7374 726f 6b65  t>.    <g stroke
+00000280: 3d22 2364 3564 3564 3522 3e0a 2020 2020  ="#d5d5d5">.    
+00000290: 2020 2020 3c72 6563 7420 7374 726f 6b65      <rect stroke
+000002a0: 3d22 6e6f 6e65 2220 6669 6c6c 3d22 2366  ="none" fill="#f
+000002b0: 6366 6366 6322 2078 3d22 302e 3522 2079  cfcfc" x="0.5" y
+000002c0: 3d22 302e 3522 2077 6964 7468 3d22 3839  ="0.5" width="89
+000002d0: 2220 6865 6967 6874 3d22 3139 2220 7278  " height="19" rx
+000002e0: 3d22 3222 2f3e 0a20 2020 2020 2020 203c  ="2"/>.        <
+000002f0: 7265 6374 2078 3d22 3935 2e35 2220 793d  rect x="95.5" y=
+00000300: 2230 2e35 2220 7769 6474 683d 2234 3122  "0.5" width="41"
+00000310: 2068 6569 6768 743d 2231 3922 2072 783d   height="19" rx=
+00000320: 2232 2220 6669 6c6c 3d22 2366 6166 6166  "2" fill="#fafaf
+00000330: 6122 2f3e 0a20 2020 2020 2020 203c 7265  a"/>.        <re
+00000340: 6374 2078 3d22 3935 2220 793d 2237 2e35  ct x="95" y="7.5
+00000350: 2220 7769 6474 683d 2230 2e35 2220 6865  " width="0.5" he
+00000360: 6967 6874 3d22 3522 2073 7472 6f6b 653d  ight="5" stroke=
+00000370: 2223 6661 6661 6661 222f 3e0a 2020 2020  "#fafafa"/>.    
+00000380: 2020 2020 3c70 6174 6820 643d 224d 3935      <path d="M95
+00000390: 2e35 2036 2e35 206c 2d33 2033 7631 206c  .5 6.5 l-3 3v1 l
+000003a0: 3320 3322 2073 7472 6f6b 653d 2264 3564  3 3" stroke="d5d
+000003b0: 3564 3522 2066 696c 6c3d 2223 6661 6661  5d5" fill="#fafa
+000003c0: 6661 222f 3e0a 2020 2020 3c2f 673e 0a20  fa"/>.    </g>. 
+000003d0: 2020 203c 6720 6172 6961 2d68 6964 6465     <g aria-hidde
+000003e0: 6e3d 2274 7275 6522 2066 696c 6c3d 2223  n="true" fill="#
+000003f0: 3333 3322 2074 6578 742d 616e 6368 6f72  333" text-anchor
+00000400: 3d22 6d69 6464 6c65 2220 666f 6e74 2d66  ="middle" font-f
+00000410: 616d 696c 793d 2248 656c 7665 7469 6361  amily="Helvetica
+00000420: 204e 6575 652c 4865 6c76 6574 6963 612c   Neue,Helvetica,
+00000430: 4172 6961 6c2c 7361 6e73 2d73 6572 6966  Arial,sans-serif
+00000440: 2220 7465 7874 2d72 656e 6465 7269 6e67  " text-rendering
+00000450: 3d22 6765 6f6d 6574 7269 6350 7265 6369  ="geometricPreci
+00000460: 7369 6f6e 2220 666f 6e74 2d77 6569 6768  sion" font-weigh
+00000470: 743d 2237 3030 2220 666f 6e74 2d73 697a  t="700" font-siz
+00000480: 653d 2231 3130 7078 2220 6c69 6e65 2d68  e="110px" line-h
+00000490: 6569 6768 743d 2231 3470 7822 3e0a 2020  eight="14px">.  
+000004a0: 2020 2020 2020 3c72 6563 7420 6964 3d22        <rect id="
+000004b0: 6c6c 696e 6b22 2073 7472 6f6b 653d 2223  llink" stroke="#
+000004c0: 6435 6435 6435 2220 6669 6c6c 3d22 7572  d5d5d5" fill="ur
+000004d0: 6c28 2361 2922 2078 3d22 2e35 2220 793d  l(#a)" x=".5" y=
+000004e0: 222e 3522 2077 6964 7468 3d22 3839 2220  ".5" width="89" 
+000004f0: 6865 6967 6874 3d22 3139 2220 7278 3d22  height="19" rx="
+00000500: 3222 2f3e 0a20 2020 2020 2020 203c 7465  2"/>.        <te
+00000510: 7874 2061 7269 612d 6869 6464 656e 3d22  xt aria-hidden="
+00000520: 7472 7565 2220 783d 2235 3635 2220 793d  true" x="565" y=
+00000530: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
+00000540: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
+00000550: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
+00000560: 7468 3d22 3539 3022 3e49 6e74 6572 726f  th="590">Interro
+00000570: 6761 7465 3c2f 7465 7874 3e0a 2020 2020  gate</text>.    
+00000580: 2020 2020 3c74 6578 7420 783d 2235 3635      <text x="565
+00000590: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
+000005a0: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
+000005b0: 7465 7874 4c65 6e67 7468 3d22 3539 3022  textLength="590"
+000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
+000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
+000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
+000005f0: 7275 6522 2078 3d22 3131 3735 2220 793d  rue" x="1175" y=
+00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
+00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
+00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
+00000630: 7468 3d22 3333 3022 3e34 352e 3025 3c2f  th="330">45.0%</
+00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
+00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
+00000660: 3d22 3131 3735 2220 793d 2231 3430 2220  ="1175" y="140" 
+00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
+00000690: 3d22 3333 3022 3e34 352e 3025 3c2f 7465  ="330">45.0%</te
+000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
+000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
+000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
+000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
+000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
+000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
+00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00000710: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
+00000720: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
+00000730: 3132 2c39 2e37 3032 3239 2c2d 362e 3638  12,9.70229,-6.68
+00000740: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
+00000750: 2020 203c 7061 7468 2064 3d22 4d35 302c     <path d="M50,
+00000760: 3634 2e32 3543 3532 2e37 362c 3634 2e32  64.25C52.76,64.2
+00000770: 3520 3535 2c36 312e 3133 2035 352c 3539  5 55,61.13 55,59
+00000780: 2e37 3543 3535 2c35 382e 3337 2035 322e  .75C55,58.37 52.
+00000790: 3736 2c35 372e 3235 2035 302c 3537 2e32  76,57.25 50,57.2
+000007a0: 3543 3437 2e32 342c 3537 2e32 3520 3435  5C47.24,57.25 45
+000007b0: 2c35 382e 3337 2034 352c 3539 2e37 3543  ,58.37 45,59.75C
+000007c0: 3435 2c36 312e 3133 2034 372e 3234 2c36  45,61.13 47.24,6
+000007d0: 342e 3235 2035 302c 3634 2e32 355a 2220  4.25 50,64.25Z" 
+000007e0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+000007f0: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
+00000800: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
+00000810: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
+00000820: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00000830: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
+00000840: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
+00000850: 3132 2c39 2e37 3032 3239 2c2d 362e 3638  12,9.70229,-6.68
+00000860: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
+00000870: 2020 203c 7061 7468 2064 3d22 4d38 382c     <path d="M88,
+00000880: 3439 2e30 3543 3836 2e35 3036 2c34 332e  49.05C86.506,43.
+00000890: 3437 3520 3833 2e30 3138 2c33 382e 3633  475 83.018,38.63
+000008a0: 3820 3738 2e32 2c33 352e 3436 4337 322e  8 78.2,35.46C72.
+000008b0: 3936 392c 3332 2e30 3032 2036 362e 3533  969,32.002 66.53
+000008c0: 392c 3330 2e38 3434 2036 302e 3433 2c33  9,30.844 60.43,3
+000008d0: 322e 3236 4335 362e 3537 362c 3333 2e31  2.26C56.576,33.1
+000008e0: 3435 2035 322e 3939 352c 3334 2e39 3538  45 52.995,34.958
+000008f0: 2035 302c 3337 2e35 3443 3436 2e39 3938   50,37.54C46.998
+00000900: 2c33 342e 3935 3820 3433 2e34 3131 2c33  ,34.958 43.411,3
+00000910: 332e 3134 3920 3339 2e35 352c 3332 2e32  3.149 39.55,32.2
+00000920: 3743 3333 2e34 3431 2c33 302e 3835 3320  7C33.441,30.853 
+00000930: 3237 2e30 3131 2c33 322e 3031 3120 3231  27.011,32.011 21
+00000940: 2e37 382c 3335 2e34 3743 3136 2e39 372c  .78,35.47C16.97,
+00000950: 3338 2e36 3532 2031 332e 3438 392c 3433  38.652 13.489,43
+00000960: 2e34 3839 2031 322c 3439 2e30 364c 3132  .489 12,49.06L12
+00000970: 2c34 392e 3133 4331 312e 3832 2c34 392e  ,49.13C11.82,49.
+00000980: 3739 2031 312e 3636 2c35 302e 3436 2031  79 11.66,50.46 1
+00000990: 312e 3533 2c35 312e 3133 4331 312e 3134  1.53,51.13C11.14
+000009a0: 362c 3533 2e32 3037 2031 312e 3032 312c  6,53.207 11.021,
+000009b0: 3535 2e33 3233 2031 312e 3136 2c35 372e  55.323 11.16,57.
+000009c0: 3433 4331 312e 3136 2c35 382e 3033 2031  43C11.16,58.03 1
+000009d0: 312e 3236 2c35 382e 3633 2031 312e 3334  1.26,58.63 11.34
+000009e0: 2c35 392e 3233 4331 312e 3334 2c35 392e  ,59.23C11.34,59.
+000009f0: 3531 2031 312e 3433 2c35 392e 3739 2031  51 11.43,59.79 1
+00000a00: 312e 3438 2c36 302e 3037 4331 312e 3533  1.48,60.07C11.53
+00000a10: 2c36 302e 3335 2031 312e 3538 2c36 302e  ,60.35 11.58,60.
+00000a20: 3638 2031 312e 3634 2c36 302e 3938 4331  68 11.64,60.98C1
+00000a30: 312e 372c 3631 2e32 3820 3131 2e38 2c36  1.7,61.28 11.8,6
+00000a40: 312e 3639 2031 312e 3839 2c36 322e 3035  1.69 11.89,62.05
+00000a50: 4331 312e 3938 2c36 322e 3431 2031 312e  C11.98,62.41 11.
+00000a60: 3939 2c36 322e 3437 2031 322e 3035 2c36  99,62.47 12.05,6
+00000a70: 322e 3638 4331 322e 3136 2c36 332e 3037  2.68C12.16,63.07
+00000a80: 2031 322e 3238 2c36 332e 3436 2031 322e   12.28,63.46 12.
+00000a90: 3431 2c36 332e 3834 4c31 322e 3538 2c36  41,63.84L12.58,6
+00000aa0: 342e 3334 4331 322e 3732 2c36 342e 3734  4.34C12.72,64.74
+00000ab0: 2031 322e 3838 2c36 352e 3134 2031 332e   12.88,65.14 13.
+00000ac0: 3034 2c36 352e 3533 4c31 332e 3233 2c36  04,65.53L13.23,6
+00000ad0: 352e 3938 4331 332e 3430 332c 3636 2e33  5.98C13.403,66.3
+00000ae0: 3733 2031 332e 3538 332c 3636 2e37 3637  73 13.583,66.767
+00000af0: 2031 332e 3737 2c36 372e 3136 4c31 332e   13.77,67.16L13.
+00000b00: 3939 2c36 372e 3539 4331 342e 3139 2c36  99,67.59C14.19,6
+00000b10: 372e 3937 2031 342e 3339 2c36 382e 3335  7.97 14.39,68.35
+00000b20: 2031 342e 3631 2c36 382e 3733 4c31 342e   14.61,68.73L14.
+00000b30: 3837 2c36 392e 3135 4331 352e 312c 3639  87,69.15C15.1,69
+00000b40: 2e35 3220 3135 2e33 332c 3639 2e38 3920  .52 15.33,69.89 
+00000b50: 3135 2e35 382c 3730 2e32 364c 3135 2e35  15.58,70.26L15.5
+00000b60: 382c 3730 2e33 324c 3135 2e39 392c 3730  8,70.32L15.99,70
+00000b70: 2e39 3343 3136 2e31 342c 3731 2e31 3420  .93C16.14,71.14 
+00000b80: 3136 2e32 392c 3731 2e33 3620 3136 2e34  16.29,71.36 16.4
+00000b90: 352c 3731 2e35 3743 3230 2e32 3036 2c37  5,71.57C20.206,7
+00000ba0: 352e 3833 2032 352e 3038 362c 3738 2e39  5.83 25.086,78.9
+00000bb0: 3520 3330 2e35 332c 3830 2e35 3743 3336  5 30.53,80.57C36
+00000bc0: 2e38 3339 2c38 322e 3438 2034 332e 3431  .839,82.48 43.41
+00000bd0: 2c38 332e 3338 3520 3530 2c38 332e 3235  ,83.385 50,83.25
+00000be0: 4335 362e 3539 392c 3833 2e33 3734 2036  C56.599,83.374 6
+00000bf0: 332e 3137 372c 3832 2e34 3536 2036 392e  3.177,82.456 69.
+00000c00: 3439 2c38 302e 3533 4337 342e 3634 342c  49,80.53C74.644,
+00000c10: 3738 2e39 3738 2037 392e 3330 332c 3736  78.978 79.303,76
+00000c20: 2e31 3032 2038 332c 3732 2e31 3943 3833  .102 83,72.19C83
+00000c30: 2e33 342c 3731 2e37 3820 3833 2e36 352c  .34,71.78 83.65,
+00000c40: 3731 2e33 3520 3834 2c37 302e 3932 4c38  71.35 84,70.92L8
+00000c50: 342e 3138 2c37 302e 3636 4c38 342e 3333  4.18,70.66L84.33
+00000c60: 2c37 302e 3434 4c38 342e 3431 2c37 302e  ,70.44L84.41,70.
+00000c70: 3332 4338 342e 3535 2c37 302e 3132 2038  32C84.55,70.12 8
+00000c80: 342e 3637 2c36 392e 3920 3834 2e38 312c  4.67,69.9 84.81,
+00000c90: 3639 2e37 4338 352e 3037 2c36 392e 3320  69.7C85.07,69.3 
+00000ca0: 3835 2e33 322c 3638 2e38 3920 3835 2e35  85.32,68.89 85.5
+00000cb0: 352c 3638 2e34 3843 3835 2e37 382c 3638  5,68.48C85.78,68
+00000cc0: 2e30 3720 3836 2e30 322c 3637 2e36 3520  .07 86.02,67.65 
+00000cd0: 3836 2e32 332c 3637 2e32 3243 3836 2e33  86.23,67.22C86.3
+00000ce0: 312c 3637 2e30 3520 3836 2e33 392c 3636  1,67.05 86.39,66
+00000cf0: 2e38 3820 3836 2e34 372c 3636 2e37 4338  .88 86.47,66.7C8
+00000d00: 362e 3637 2c36 362e 3238 2038 362e 3835  6.67,66.28 86.85
+00000d10: 2c36 352e 3837 2038 372e 3033 2c36 352e  ,65.87 87.03,65.
+00000d20: 3434 4c38 372e 3233 2c36 342e 3932 4338  44L87.23,64.92C8
+00000d30: 372e 3339 372c 3634 2e34 3837 2038 372e  7.397,64.487 87.
+00000d40: 3535 2c36 342e 3035 2038 372e 3639 2c36  55,64.05 87.69,6
+00000d50: 332e 3631 4c38 372e 3835 2c36 332e 3039  3.61L87.85,63.09
+00000d60: 4338 372e 3938 2c36 322e 3634 2038 382e  C87.98,62.64 88.
+00000d70: 312c 3632 2e31 3920 3838 2e32 312c 3631  1,62.19 88.21,61
+00000d80: 2e37 3443 3838 2e32 312c 3631 2e35 3720  .74C88.21,61.57 
+00000d90: 3838 2e33 2c36 312e 3339 2038 382e 3333  88.3,61.39 88.33
+00000da0: 2c36 312e 3232 4338 382e 3433 2c36 302e  ,61.22C88.43,60.
+00000db0: 3735 2038 382e 3532 2c36 302e 3232 2038  75 88.52,60.22 8
+00000dc0: 382e 362c 3539 2e37 3943 3838 2e36 2c35  8.6,59.79C88.6,5
+00000dd0: 392e 3634 2038 382e 3636 2c35 392e 3439  9.64 88.66,59.49
+00000de0: 2038 382e 3638 2c35 392e 3333 4338 382e   88.68,59.33C88.
+00000df0: 3737 2c35 382e 3731 2038 382e 3834 2c35  77,58.71 88.84,5
+00000e00: 382e 3038 2038 382e 3838 2c35 372e 3435  8.08 88.88,57.45
+00000e10: 4c38 382e 3838 2c35 342e 3137 4338 382e  L88.88,54.17C88.
+00000e20: 3831 372c 3533 2e31 3634 2038 382e 3639  817,53.164 88.69
+00000e30: 332c 3532 2e31 3632 2038 382e 3531 2c35  3,52.162 88.51,5
+00000e40: 312e 3137 4338 382e 3338 2c35 302e 3520  1.17C88.38,50.5 
+00000e50: 3838 2e32 332c 3439 2e38 3420 3838 2e30  88.23,49.84 88.0
+00000e60: 352c 3439 2e31 374c 3838 2c34 392e 3035  5,49.17L88,49.05
+00000e70: 5a4d 3835 2e38 392c 3536 2e34 344c 3835  ZM85.89,56.44L85
+00000e80: 2e38 392c 3537 2e32 3343 3835 2e38 392c  .89,57.23C85.89,
+00000e90: 3537 2e37 3820 3835 2e37 392c 3538 2e33  57.78 85.79,58.3
+00000ea0: 3220 3835 2e37 322c 3538 2e38 3643 3835  2 85.72,58.86C85
+00000eb0: 2e37 322c 3539 2e30 3120 3835 2e37 322c  .72,59.01 85.72,
+00000ec0: 3539 2e31 3520 3835 2e36 352c 3539 2e33  59.15 85.65,59.3
+00000ed0: 4338 352e 3539 2c35 392e 3720 3835 2e35  C85.59,59.7 85.5
+00000ee0: 312c 3630 2e31 3120 3835 2e34 332c 3630  1,60.11 85.43,60
+00000ef0: 2e35 314c 3835 2e33 322c 3630 2e39 3943  .51L85.32,60.99C
+00000f00: 3835 2e32 332c 3631 2e33 3820 3835 2e31  85.23,61.38 85.1
+00000f10: 322c 3631 2e37 3720 3835 2e30 312c 3632  2,61.77 85.01,62
+00000f20: 2e31 3643 3835 2e30 312c 3632 2e33 3120  .16C85.01,62.31 
+00000f30: 3834 2e39 332c 3632 2e34 3620 3834 2e38  84.93,62.46 84.8
+00000f40: 382c 3632 2e36 4338 342e 3734 2c36 332e  8,62.6C84.74,63.
+00000f50: 3034 2038 342e 3539 2c36 332e 3437 2038  04 84.59,63.47 8
+00000f60: 342e 3432 2c36 332e 394c 3834 2e32 372c  4.42,63.9L84.27,
+00000f70: 3634 2e32 3843 3834 2e31 2c36 342e 3731  64.28C84.1,64.71
+00000f80: 2038 332e 3931 2c36 352e 3134 2038 332e   83.91,65.14 83.
+00000f90: 3731 2c36 352e 3536 4338 332e 3531 2c36  71,65.56C83.51,6
+00000fa0: 352e 3938 2038 332e 3433 2c36 362e 3132  5.98 83.43,66.12
+00000fb0: 2038 332e 3238 2c36 362e 344c 3833 2e30   83.28,66.4L83.0
+00000fc0: 312c 3636 2e39 3143 3832 2e38 332c 3637  1,66.91C82.83,67
+00000fd0: 2e32 3233 2038 322e 3634 332c 3637 2e35  .223 82.643,67.5
+00000fe0: 3337 2038 322e 3435 2c36 372e 3835 4c38  37 82.45,67.85L8
+00000ff0: 322e 3335 2c36 382e 3031 4337 392e 3132  2.35,68.01C79.12
+00001000: 312c 3638 2e30 3437 2037 352e 3931 382c  1,68.047 75.918,
+00001010: 3637 2e34 3334 2037 322e 3933 2c36 362e  67.434 72.93,66.
+00001020: 3231 4336 342e 3237 2c36 322e 3734 2035  21C64.27,62.74 5
+00001030: 392c 3535 2e35 3220 3631 2e31 382c 3530  9,55.52 61.18,50
+00001040: 2e31 3143 3632 2e31 382c 3437 2e36 2036  .11C62.18,47.6 6
+00001050: 342e 372c 3435 2e38 3220 3638 2e32 362c  4.7,45.82 68.26,
+00001060: 3435 2e31 3143 3732 2e34 3839 2c34 342e  45.11C72.489,44.
+00001070: 3339 3520 3736 2e38 3335 2c34 342e 3930  395 76.835,44.90
+00001080: 3820 3830 2e37 382c 3436 2e35 3943 3832  8 80.78,46.59C82
+00001090: 2e31 3431 2c34 372e 3134 3420 3833 2e34  .141,47.144 83.4
+000010a0: 3533 2c34 372e 3831 3320 3834 2e37 2c34  53,47.813 84.7,4
+000010b0: 382e 3539 4338 342e 3736 2c34 382e 3736  8.59C84.76,48.76
+000010c0: 2038 342e 3832 2c34 382e 3933 2038 342e   84.82,48.93 84.
+000010d0: 3838 2c34 392e 3143 3834 2e39 342c 3439  88,49.1C84.94,49
+000010e0: 2e32 3720 3835 2e30 352c 3439 2e36 3320  .27 85.05,49.63 
+000010f0: 3835 2e31 322c 3439 2e39 4338 352e 3238  85.12,49.9C85.28
+00001100: 2c35 302e 3520 3835 2e34 342c 3531 2e31  ,50.5 85.44,51.1
+00001110: 2038 352e 3535 2c35 312e 3733 4338 352e   85.55,51.73C85.
+00001120: 3639 312c 3532 2e35 3037 2038 352e 3739  691,52.507 85.79
+00001130: 322c 3533 2e32 3932 2038 352e 3835 2c35  2,53.292 85.85,5
+00001140: 342e 3038 4c38 352e 3835 2c35 352e 3839  4.08L85.85,55.89
+00001150: 4338 352e 3835 2c35 362e 3132 2038 352e  C85.85,56.12 85.
+00001160: 3931 2c35 362e 3235 2038 352e 3931 2c35  91,56.25 85.91,5
+00001170: 362e 3435 4c38 352e 3839 2c35 362e 3434  6.45L85.89,56.44
+00001180: 5a4d 3137 2e36 362c 3638 4331 362e 3636  ZM17.66,68C16.66
+00001190: 382c 3636 2e34 3335 2031 352e 3836 392c  8,66.435 15.869,
+000011a0: 3634 2e37 3536 2031 352e 3238 2c36 334c  64.756 15.28,63L
+000011b0: 3135 2e31 372c 3632 2e36 3843 3135 2e30  15.17,62.68C15.0
+000011c0: 362c 3632 2e33 3520 3134 2e39 362c 3632  6,62.35 14.96,62
+000011d0: 2e30 3120 3134 2e38 372c 3631 2e36 3843  .01 14.87,61.68C
+000011e0: 3134 2e38 3233 2c36 312e 3439 3320 3134  14.823,61.493 14
+000011f0: 2e37 3737 2c36 312e 3331 2031 342e 3733  .777,61.31 14.73
+00001200: 2c36 312e 3133 4331 342e 3636 2c36 302e  ,61.13C14.66,60.
+00001210: 3834 2031 342e 3539 2c36 302e 3535 2031  84 14.59,60.55 1
+00001220: 342e 3533 2c36 302e 3237 4331 342e 3437  4.53,60.27C14.47
+00001230: 2c35 392e 3939 2031 342e 3433 2c35 392e  ,59.99 14.43,59.
+00001240: 3732 2031 342e 3338 2c35 392e 3434 4331  72 14.38,59.44C1
+00001250: 342e 3333 2c35 392e 3136 2031 342e 332c  4.33,59.16 14.3,
+00001260: 3539 2031 342e 3237 2c35 382e 3738 4331  59 14.27,58.78C1
+00001270: 342e 322c 3538 2e32 3720 3134 2e31 352c  4.2,58.27 14.15,
+00001280: 3537 2e37 3820 3134 2e31 312c 3537 2e32  57.78 14.11,57.2
+00001290: 334c 3134 2e31 312c 3537 2e30 3343 3134  3L14.11,57.03C14
+000012a0: 2e30 3038 2c35 352e 3233 3620 3134 2e31  .008,55.236 14.1
+000012b0: 3232 2c35 332e 3433 3720 3134 2e34 352c  22,53.437 14.45,
+000012c0: 3531 2e36 3743 3134 2e35 362c 3531 2e30  51.67C14.56,51.0
+000012d0: 3620 3134 2e37 312c 3530 2e34 3620 3134  6 14.71,50.46 14
+000012e0: 2e38 382c 3439 2e38 3743 3134 2e39 362c  .88,49.87C14.96,
+000012f0: 3439 2e35 3920 3135 2e30 342c 3439 2e33  49.59 15.04,49.3
+00001300: 3220 3135 2e31 332c 3439 2e30 3543 3135  2 15.13,49.05C15
+00001310: 2e32 322c 3438 2e37 3820 3135 2e32 342c  .22,48.78 15.24,
+00001320: 3438 2e37 3220 3135 2e33 2c34 382e 3535  48.72 15.3,48.55
+00001330: 4331 362e 3534 382c 3437 2e37 3734 2031  C16.548,47.774 1
+00001340: 372e 3835 392c 3437 2e31 3035 2031 392e  7.859,47.105 19.
+00001350: 3232 2c34 362e 3535 4332 372e 3836 2c34  22,46.55C27.86,4
+00001360: 332e 3039 2033 362e 3635 2c34 342e 3637  3.09 36.65,44.67
+00001370: 2033 382e 3832 2c35 302e 3038 4334 302e   38.82,50.08C40.
+00001380: 3939 2c35 352e 3439 2033 352e 3733 2c36  99,55.49 35.73,6
+00001390: 322e 3734 2032 372e 3039 2c36 362e 3243  2.74 27.09,66.2C
+000013a0: 3234 2e31 3031 2c36 372e 3433 3120 3230  24.101,67.431 20
+000013b0: 2e38 3933 2c36 382e 3034 3320 3137 2e36  .893,68.043 17.6
+000013c0: 362c 3638 5a4d 3638 2e35 372c 3737 2e36  6,68ZM68.57,77.6
+000013d0: 3843 3632 2e35 3534 2c37 392e 3530 3820  8C62.554,79.508 
+000013e0: 3536 2e32 3837 2c38 302e 3337 3620 3530  56.287,80.376 50
+000013f0: 2c38 302e 3235 4334 332e 3733 372c 3830  ,80.25C43.737,80
+00001400: 2e33 3720 3337 2e34 3935 2c37 392e 3530  .37 37.495,79.50
+00001410: 3620 3331 2e35 2c37 372e 3639 4332 372e  6 31.5,77.69C27.
+00001420: 3138 352c 3736 2e33 3820 3233 2e32 3433  185,76.38 23.243
+00001430: 2c37 342e 3036 3220 3230 2c37 302e 3933  ,74.062 20,70.93
+00001440: 4332 322e 3831 352c 3730 2e37 3036 2032  C22.815,70.706 2
+00001450: 352e 3538 2c37 302e 3035 3520 3238 2e32  5.58,70.055 28.2
+00001460: 2c36 3943 3338 2e33 372c 3634 2e39 3220  ,69C38.37,64.92 
+00001470: 3434 2e33 392c 3536 2034 312e 362c 3439  44.39,56 41.6,49
+00001480: 4333 382e 3831 2c34 3220 3238 2e32 372c  C38.81,42 28.27,
+00001490: 3339 2e37 3220 3138 2e31 2c34 332e 384c  39.72 18.1,43.8L
+000014a0: 3137 2e34 332c 3434 2e30 3943 3138 2e39  17.43,44.09C18.9
+000014b0: 3733 2c34 312e 3634 3820 3231 2e30 3139  73,41.648 21.019
+000014c0: 2c33 392e 3536 3120 3233 2e34 332c 3337  ,39.561 23.43,37
+000014d0: 2e39 3743 3236 2e36 3731 2c33 352e 3832  .97C26.671,35.82
+000014e0: 3420 3330 2e34 3733 2c33 342e 3638 2033  4 30.473,34.68 3
+000014f0: 342e 3336 2c33 342e 3638 4333 352e 3838  4.36,34.68C35.88
+00001500: 342c 3334 2e36 3831 2033 372e 3430 342c  4,34.681 37.404,
+00001510: 3334 2e38 3532 2033 382e 3839 2c33 352e  34.852 38.89,35.
+00001520: 3139 4334 322e 3639 342c 3336 2e30 3439  19C42.694,36.049
+00001530: 2034 362e 3139 312c 3337 2e39 3335 2034   46.191,37.935 4
+00001540: 392c 3430 2e36 344c 3530 2c34 312e 3634  9,40.64L50,41.64
+00001550: 4c35 312c 3430 2e36 3443 3533 2e37 3937  L51,40.64C53.797
+00001560: 2c33 372e 3933 3720 3537 2e32 3739 2c33  ,37.937 57.279,3
+00001570: 362e 3034 3920 3631 2e30 372c 3335 2e31  6.049 61.07,35.1
+00001580: 3843 3636 2e34 3032 2c33 332e 3934 3720  8C66.402,33.947 
+00001590: 3732 2e30 3134 2c33 342e 3936 3820 3736  72.014,34.968 76
+000015a0: 2e35 372c 3338 4337 382e 3938 2c33 392e  .57,38C78.98,39.
+000015b0: 3538 3820 3831 2e30 3236 2c34 312e 3637  588 81.026,41.67
+000015c0: 3120 3832 2e35 372c 3434 2e31 314c 3831  1 82.57,44.11L81
+000015d0: 2e39 2c34 332e 3832 4337 372e 3430 392c  .9,43.82C77.409,
+000015e0: 3431 2e39 3231 2037 322e 3436 342c 3431  41.921 72.464,41
+000015f0: 2e33 3535 2036 372e 3636 2c34 322e 3139  .355 67.66,42.19
+00001600: 4336 332e 3038 2c34 332e 3132 2035 392e  C63.08,43.12 59.
+00001610: 3739 2c34 352e 3534 2035 382e 3339 2c34  79,45.54 58.39,4
+00001620: 392e 3032 4335 352e 362c 3535 2e39 3720  9.02C55.6,55.97 
+00001630: 3631 2e36 322c 3634 2e39 3420 3731 2e37  61.62,64.94 71.7
+00001640: 392c 3639 2e30 3243 3734 2e34 3134 2c37  9,69.02C74.414,7
+00001650: 302e 3037 2037 372e 3138 322c 3730 2e37  0.07 77.182,70.7
+00001660: 3134 2038 302c 3730 2e39 3343 3736 2e37  14 80,70.93C76.7
+00001670: 3736 2c37 342e 3035 2037 322e 3835 392c  76,74.05 72.859,
+00001680: 3736 2e33 3633 2036 382e 3537 2c37 372e  76.363 68.57,77.
+00001690: 3638 5a22 2073 7479 6c65 3d22 6669 6c6c  68Z" style="fill
+000016a0: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
+000016b0: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
+000016c0: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
+000016d0: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
+000016e0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+000016f0: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
+00001700: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
+00001710: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
+00001720: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
+00001730: 6378 3d22 3731 2e33 3322 2063 793d 2235  cx="71.33" cy="5
+00001740: 3622 2072 3d22 352e 3136 2220 7374 796c  6" r="5.16" styl
+00001750: 653d 2266 696c 6c3a 7267 6228 3232 322c  e="fill:rgb(222,
+00001760: 3132 302c 3136 3029 3b22 2f3e 0a20 2020  120,160);"/>.   
+00001770: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00001780: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
+00001790: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
+000017a0: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
+000017b0: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
+000017c0: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
+000017d0: 7263 6c65 2063 783d 2232 382e 3637 2220  rcle cx="28.67" 
+000017e0: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
+000017f0: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
+00001800: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
+00001810: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
+00001820: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
+00001830: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
+00001840: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
+00001850: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
+00001860: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
+00001870: 2020 3c70 6174 6820 643d 224d 3538 2c36    <path d="M58,6
+00001880: 3643 3535 2e39 3132 2c36 382e 3136 3120  6C55.912,68.161 
+00001890: 3533 2e30 3033 2c36 392e 3333 3920 3530  53.003,69.339 50
+000018a0: 2c36 392e 3234 4334 362e 3939 372c 3639  ,69.24C46.997,69
+000018b0: 2e33 3339 2034 342e 3038 382c 3638 2e31  .339 44.088,68.1
+000018c0: 3631 2034 322c 3636 4334 312e 3731 342c  61 42,66C41.714,
+000018d0: 3635 2e36 3737 2034 312e 3330 322c 3635  65.677 41.302,65
+000018e0: 2e34 3931 2034 302e 3837 2c36 352e 3439  .491 40.87,65.49
+000018f0: 3143 3430 2e30 3432 2c36 352e 3439 3120  1C40.042,65.491 
+00001900: 3339 2e33 3631 2c36 362e 3137 3220 3339  39.361,66.172 39
+00001910: 2e33 3631 2c36 3743 3339 2e33 3631 2c36  .361,67C39.361,6
+00001920: 372e 3336 3820 3339 2e34 3936 2c36 372e  7.368 39.496,67.
+00001930: 3732 3420 3339 2e37 342c 3638 4334 322e  724 39.74,68C42.
+00001940: 3430 332c 3730 2e38 3034 2034 362e 3133  403,70.804 46.13
+00001950: 342c 3732 2e33 3520 3530 2c37 322e 3235  4,72.35 50,72.25
+00001960: 4335 332e 3836 322c 3732 2e33 3437 2035  C53.862,72.347 5
+00001970: 372e 3539 2c37 302e 3830 3220 3630 2e32  7.59,70.802 60.2
+00001980: 352c 3638 4336 302e 3439 352c 3637 2e37  5,68C60.495,67.7
+00001990: 3235 2036 302e 3633 2c36 372e 3336 3920  25 60.63,67.369 
+000019a0: 3630 2e36 332c 3637 4336 302e 3633 2c36  60.63,67C60.63,6
+000019b0: 362e 3137 3420 3539 2e39 3531 2c36 352e  6.174 59.951,65.
+000019c0: 3439 3520 3539 2e31 3235 2c36 352e 3439  495 59.125,65.49
+000019d0: 3543 3538 2e36 3935 2c36 352e 3439 3520  5C58.695,65.495 
+000019e0: 3538 2e32 3835 2c36 352e 3637 3920 3538  58.285,65.679 58
+000019f0: 2c36 365a 2220 7374 796c 653d 2266 696c  ,66Z" style="fil
+00001a00: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
+00001a10: 3029 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  0);fill-rule:non
+00001a20: 7a65 726f 3b22 2f3e 0a20 2020 2020 2020  zero;"/>.       
+00001a30: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a3c   </g>.    </g>.<
+00001a40: 2f73 7667 3e0a                           /svg>.
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/45.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/60.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/90.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/99.png` & `interrogate-1.6.0/tests/unit/fixtures/plastic/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/99.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/plastic/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/plastic/default.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/0.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/0.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/100.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/100.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/45.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/60.svg`

 * *Files 1% similar despite different names*

```diff
@@ -93,21 +93,21 @@
 000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
 000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
 000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
 000005f0: 7275 6522 2078 3d22 3131 3735 2220 793d  rue" x="1175" y=
 00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
 00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
 00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000630: 7468 3d22 3333 3022 3e34 352e 3025 3c2f  th="330">45.0%</
+00000630: 7468 3d22 3333 3022 3e36 302e 3025 3c2f  th="330">60.0%</
 00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
 00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
 00000660: 3d22 3131 3735 2220 793d 2231 3430 2220  ="1175" y="140" 
 00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
 00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
-00000690: 3d22 3333 3022 3e34 352e 3025 3c2f 7465  ="330">45.0%</te
+00000690: 3d22 3333 3022 3e36 302e 3025 3c2f 7465  ="330">60.0%</te
 000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
 000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
 000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
 000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
 000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
 000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
 00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/60.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/90.svg`

 * *Files 0% similar despite different names*

```diff
@@ -93,21 +93,21 @@
 000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
 000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
 000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
 000005f0: 7275 6522 2078 3d22 3131 3735 2220 793d  rue" x="1175" y=
 00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
 00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
 00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000630: 7468 3d22 3333 3022 3e36 302e 3025 3c2f  th="330">60.0%</
+00000630: 7468 3d22 3333 3022 3e39 302e 3025 3c2f  th="330">90.0%</
 00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
 00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
 00000660: 3d22 3131 3735 2220 793d 2231 3430 2220  ="1175" y="140" 
 00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
 00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
-00000690: 3d22 3333 3022 3e36 302e 3025 3c2f 7465  ="330">60.0%</te
+00000690: 3d22 3333 3022 3e39 302e 3025 3c2f 7465  ="330">90.0%</te
 000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
 000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
 000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
 000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
 000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
 000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
 00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/89.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/89.svg`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/90.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/99.svg`

 * *Files 1% similar despite different names*

```diff
@@ -93,21 +93,21 @@
 000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
 000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
 000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
 000005f0: 7275 6522 2078 3d22 3131 3735 2220 793d  rue" x="1175" y=
 00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
 00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
 00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000630: 7468 3d22 3333 3022 3e39 302e 3025 3c2f  th="330">90.0%</
+00000630: 7468 3d22 3333 3022 3e39 392e 3925 3c2f  th="330">99.9%</
 00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
 00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
 00000660: 3d22 3131 3735 2220 793d 2231 3430 2220  ="1175" y="140" 
 00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
 00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
-00000690: 3d22 3333 3022 3e39 302e 3025 3c2f 7465  ="330">90.0%</te
+00000690: 3d22 3333 3022 3e39 392e 3925 3c2f 7465  ="330">99.9%</te
 000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
 000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
 000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
 000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
 000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
 000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
 00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/99.png` & `interrogate-1.6.0/tests/unit/fixtures/social/99.png`

 * *Files identical despite different names*

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/99.svg` & `interrogate-1.6.0/tests/unit/fixtures/social/default.svg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
 00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
 00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
 00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
 00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3133 3722 2068  k" width="137" h
+00000050: 6b22 2077 6964 7468 3d22 3133 3122 2068  k" width="131" h
 00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
 00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
 00000080: 3d22 496e 7465 7272 6f67 6174 653a 2031  ="Interrogate: 1
 00000090: 3030 2522 3e0a 2020 2020 3c74 6974 6c65  00%">.    <title
 000000a0: 3e49 6e74 6572 726f 6761 7465 3a20 3130  >Interrogate: 10
 000000b0: 3025 3c2f 7469 746c 653e 0a20 2020 203c  0%</title>.    <
 000000c0: 7374 796c 653e 613a 686f 7665 7220 236c  style>a:hover #l
@@ -42,15 +42,15 @@
 00000290: 2020 2020 3c72 6563 7420 7374 726f 6b65      <rect stroke
 000002a0: 3d22 6e6f 6e65 2220 6669 6c6c 3d22 2366  ="none" fill="#f
 000002b0: 6366 6366 6322 2078 3d22 302e 3522 2079  cfcfc" x="0.5" y
 000002c0: 3d22 302e 3522 2077 6964 7468 3d22 3839  ="0.5" width="89
 000002d0: 2220 6865 6967 6874 3d22 3139 2220 7278  " height="19" rx
 000002e0: 3d22 3222 2f3e 0a20 2020 2020 2020 203c  ="2"/>.        <
 000002f0: 7265 6374 2078 3d22 3935 2e35 2220 793d  rect x="95.5" y=
-00000300: 2230 2e35 2220 7769 6474 683d 2234 3122  "0.5" width="41"
+00000300: 2230 2e35 2220 7769 6474 683d 2233 3522  "0.5" width="35"
 00000310: 2068 6569 6768 743d 2231 3922 2072 783d   height="19" rx=
 00000320: 2232 2220 6669 6c6c 3d22 2366 6166 6166  "2" fill="#fafaf
 00000330: 6122 2f3e 0a20 2020 2020 2020 203c 7265  a"/>.        <re
 00000340: 6374 2078 3d22 3935 2220 793d 2237 2e35  ct x="95" y="7.5
 00000350: 2220 7769 6474 683d 2230 2e35 2220 6865  " width="0.5" he
 00000360: 6967 6874 3d22 3522 2073 7472 6f6b 653d  ight="5" stroke=
 00000370: 2223 6661 6661 6661 222f 3e0a 2020 2020  "#fafafa"/>.    
@@ -89,25 +89,25 @@
 00000580: 2020 2020 3c74 6578 7420 783d 2235 3635      <text x="565
 00000590: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
 000005a0: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
 000005b0: 7465 7874 4c65 6e67 7468 3d22 3539 3022  textLength="590"
 000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
 000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
 000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
-000005f0: 7275 6522 2078 3d22 3131 3735 2220 793d  rue" x="1175" y=
+000005f0: 7275 6522 2078 3d22 3131 3435 2220 793d  rue" x="1145" y=
 00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
 00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
 00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000630: 7468 3d22 3333 3022 3e39 392e 3925 3c2f  th="330">99.9%</
+00000630: 7468 3d22 3237 3022 3e2d 312e 3025 3c2f  th="270">-1.0%</
 00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
 00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
-00000660: 3d22 3131 3735 2220 793d 2231 3430 2220  ="1175" y="140" 
+00000660: 3d22 3131 3435 2220 793d 2231 3430 2220  ="1145" y="140" 
 00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
 00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
-00000690: 3d22 3333 3022 3e39 392e 3925 3c2f 7465  ="330">99.9%</te
+00000690: 3d22 3237 3022 3e2d 312e 3025 3c2f 7465  ="270">-1.0%</te
 000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
 000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
 000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
 000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
 000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
 000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
 00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
```

### Comparing `interrogate-1.5.0/tests/unit/fixtures/social/default.svg` & `interrogate-1.6.0/tests/unit/fixtures/flat-square-modified/100.svg`

 * *Files 24% similar despite different names*

```diff
@@ -1,421 +1,743 @@
-00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
-00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000020: 3030 2f73 7667 2220 786d 6c6e 733a 786c  00/svg" xmlns:xl
-00000030: 696e 6b3d 2268 7474 703a 2f2f 7777 772e  ink="http://www.
-00000040: 7733 2e6f 7267 2f31 3939 392f 786c 696e  w3.org/1999/xlin
-00000050: 6b22 2077 6964 7468 3d22 3133 3122 2068  k" width="131" h
-00000060: 6569 6768 743d 2232 3022 2072 6f6c 653d  eight="20" role=
-00000070: 2269 6d67 2220 6172 6961 2d6c 6162 656c  "img" aria-label
-00000080: 3d22 496e 7465 7272 6f67 6174 653a 2031  ="Interrogate: 1
-00000090: 3030 2522 3e0a 2020 2020 3c74 6974 6c65  00%">.    <title
-000000a0: 3e49 6e74 6572 726f 6761 7465 3a20 3130  >Interrogate: 10
-000000b0: 3025 3c2f 7469 746c 653e 0a20 2020 203c  0%</title>.    <
-000000c0: 7374 796c 653e 613a 686f 7665 7220 236c  style>a:hover #l
-000000d0: 6c69 6e6b 7b66 696c 6c3a 7572 6c28 2362  link{fill:url(#b
-000000e0: 293b 7374 726f 6b65 3a23 6363 637d 613a  );stroke:#ccc}a:
-000000f0: 686f 7665 7220 2372 6c69 6e6b 7b66 696c  hover #rlink{fil
-00000100: 6c3a 2334 3138 3363 347d 3c2f 7374 796c  l:#4183c4}</styl
-00000110: 653e 0a20 2020 203c 6c69 6e65 6172 4772  e>.    <linearGr
-00000120: 6164 6965 6e74 2069 643d 2261 2220 7832  adient id="a" x2
-00000130: 3d22 3022 2079 323d 2231 3030 2522 3e0a  ="0" y2="100%">.
-00000140: 2020 2020 2020 2020 3c73 746f 7020 6f66          <stop of
-00000150: 6673 6574 3d22 3022 2073 746f 702d 636f  fset="0" stop-co
-00000160: 6c6f 723d 2223 6663 6663 6663 2220 7374  lor="#fcfcfc" st
-00000170: 6f70 2d6f 7061 6369 7479 3d22 3022 2f3e  op-opacity="0"/>
-00000180: 0a20 2020 2020 2020 203c 7374 6f70 206f  .        <stop o
-00000190: 6666 7365 743d 2231 2220 7374 6f70 2d6f  ffset="1" stop-o
-000001a0: 7061 6369 7479 3d22 2e31 222f 3e0a 2020  pacity=".1"/>.  
-000001b0: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
-000001c0: 6e74 3e0a 2020 2020 3c6c 696e 6561 7247  nt>.    <linearG
-000001d0: 7261 6469 656e 7420 6964 3d22 6222 2078  radient id="b" x
-000001e0: 323d 2230 2220 7932 3d22 3130 3025 223e  2="0" y2="100%">
-000001f0: 0a20 2020 2020 2020 203c 7374 6f70 206f  .        <stop o
-00000200: 6666 7365 743d 2230 2220 7374 6f70 2d63  ffset="0" stop-c
-00000210: 6f6c 6f72 3d22 2363 6363 2220 7374 6f70  olor="#ccc" stop
-00000220: 2d6f 7061 6369 7479 3d22 2e31 222f 3e0a  -opacity=".1"/>.
-00000230: 2020 2020 2020 2020 3c73 746f 7020 6f66          <stop of
-00000240: 6673 6574 3d22 3122 2073 746f 702d 6f70  fset="1" stop-op
-00000250: 6163 6974 793d 222e 3122 2f3e 0a20 2020  acity=".1"/>.   
-00000260: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00000270: 743e 0a20 2020 203c 6720 7374 726f 6b65  t>.    <g stroke
-00000280: 3d22 2364 3564 3564 3522 3e0a 2020 2020  ="#d5d5d5">.    
-00000290: 2020 2020 3c72 6563 7420 7374 726f 6b65      <rect stroke
-000002a0: 3d22 6e6f 6e65 2220 6669 6c6c 3d22 2366  ="none" fill="#f
-000002b0: 6366 6366 6322 2078 3d22 302e 3522 2079  cfcfc" x="0.5" y
-000002c0: 3d22 302e 3522 2077 6964 7468 3d22 3839  ="0.5" width="89
-000002d0: 2220 6865 6967 6874 3d22 3139 2220 7278  " height="19" rx
-000002e0: 3d22 3222 2f3e 0a20 2020 2020 2020 203c  ="2"/>.        <
-000002f0: 7265 6374 2078 3d22 3935 2e35 2220 793d  rect x="95.5" y=
-00000300: 2230 2e35 2220 7769 6474 683d 2233 3522  "0.5" width="35"
-00000310: 2068 6569 6768 743d 2231 3922 2072 783d   height="19" rx=
-00000320: 2232 2220 6669 6c6c 3d22 2366 6166 6166  "2" fill="#fafaf
-00000330: 6122 2f3e 0a20 2020 2020 2020 203c 7265  a"/>.        <re
-00000340: 6374 2078 3d22 3935 2220 793d 2237 2e35  ct x="95" y="7.5
-00000350: 2220 7769 6474 683d 2230 2e35 2220 6865  " width="0.5" he
-00000360: 6967 6874 3d22 3522 2073 7472 6f6b 653d  ight="5" stroke=
-00000370: 2223 6661 6661 6661 222f 3e0a 2020 2020  "#fafafa"/>.    
-00000380: 2020 2020 3c70 6174 6820 643d 224d 3935      <path d="M95
-00000390: 2e35 2036 2e35 206c 2d33 2033 7631 206c  .5 6.5 l-3 3v1 l
-000003a0: 3320 3322 2073 7472 6f6b 653d 2264 3564  3 3" stroke="d5d
-000003b0: 3564 3522 2066 696c 6c3d 2223 6661 6661  5d5" fill="#fafa
-000003c0: 6661 222f 3e0a 2020 2020 3c2f 673e 0a20  fa"/>.    </g>. 
-000003d0: 2020 203c 6720 6172 6961 2d68 6964 6465     <g aria-hidde
-000003e0: 6e3d 2274 7275 6522 2066 696c 6c3d 2223  n="true" fill="#
-000003f0: 3333 3322 2074 6578 742d 616e 6368 6f72  333" text-anchor
-00000400: 3d22 6d69 6464 6c65 2220 666f 6e74 2d66  ="middle" font-f
-00000410: 616d 696c 793d 2248 656c 7665 7469 6361  amily="Helvetica
-00000420: 204e 6575 652c 4865 6c76 6574 6963 612c   Neue,Helvetica,
-00000430: 4172 6961 6c2c 7361 6e73 2d73 6572 6966  Arial,sans-serif
-00000440: 2220 7465 7874 2d72 656e 6465 7269 6e67  " text-rendering
-00000450: 3d22 6765 6f6d 6574 7269 6350 7265 6369  ="geometricPreci
-00000460: 7369 6f6e 2220 666f 6e74 2d77 6569 6768  sion" font-weigh
-00000470: 743d 2237 3030 2220 666f 6e74 2d73 697a  t="700" font-siz
-00000480: 653d 2231 3130 7078 2220 6c69 6e65 2d68  e="110px" line-h
-00000490: 6569 6768 743d 2231 3470 7822 3e0a 2020  eight="14px">.  
-000004a0: 2020 2020 2020 3c72 6563 7420 6964 3d22        <rect id="
-000004b0: 6c6c 696e 6b22 2073 7472 6f6b 653d 2223  llink" stroke="#
-000004c0: 6435 6435 6435 2220 6669 6c6c 3d22 7572  d5d5d5" fill="ur
-000004d0: 6c28 2361 2922 2078 3d22 2e35 2220 793d  l(#a)" x=".5" y=
-000004e0: 222e 3522 2077 6964 7468 3d22 3839 2220  ".5" width="89" 
-000004f0: 6865 6967 6874 3d22 3139 2220 7278 3d22  height="19" rx="
-00000500: 3222 2f3e 0a20 2020 2020 2020 203c 7465  2"/>.        <te
-00000510: 7874 2061 7269 612d 6869 6464 656e 3d22  xt aria-hidden="
-00000520: 7472 7565 2220 783d 2235 3635 2220 793d  true" x="565" y=
-00000530: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
-00000540: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
-00000550: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000560: 7468 3d22 3539 3022 3e49 6e74 6572 726f  th="590">Interro
-00000570: 6761 7465 3c2f 7465 7874 3e0a 2020 2020  gate</text>.    
-00000580: 2020 2020 3c74 6578 7420 783d 2235 3635      <text x="565
-00000590: 2220 793d 2231 3430 2220 7472 616e 7366  " y="140" transf
-000005a0: 6f72 6d3d 2273 6361 6c65 282e 3129 2220  orm="scale(.1)" 
-000005b0: 7465 7874 4c65 6e67 7468 3d22 3539 3022  textLength="590"
-000005c0: 3e49 6e74 6572 726f 6761 7465 3c2f 7465  >Interrogate</te
-000005d0: 7874 3e0a 2020 2020 2020 2020 3c74 6578  xt>.        <tex
-000005e0: 7420 6172 6961 2d68 6964 6465 6e3d 2274  t aria-hidden="t
-000005f0: 7275 6522 2078 3d22 3131 3435 2220 793d  rue" x="1145" y=
-00000600: 2231 3530 2220 6669 6c6c 3d22 2366 6666  "150" fill="#fff
-00000610: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
-00000620: 6c65 282e 3129 2220 7465 7874 4c65 6e67  le(.1)" textLeng
-00000630: 7468 3d22 3237 3022 3e2d 312e 3025 3c2f  th="270">-1.0%</
-00000640: 7465 7874 3e0a 2020 2020 2020 2020 3c74  text>.        <t
-00000650: 6578 7420 6964 3d22 726c 696e 6b22 2078  ext id="rlink" x
-00000660: 3d22 3131 3435 2220 793d 2231 3430 2220  ="1145" y="140" 
-00000670: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
-00000680: 282e 3129 2220 7465 7874 4c65 6e67 7468  (.1)" textLength
-00000690: 3d22 3237 3022 3e2d 312e 3025 3c2f 7465  ="270">-1.0%</te
-000006a0: 7874 3e0a 2020 2020 3c2f 673e 0a20 2020  xt>.    </g>.   
-000006b0: 203c 6720 6964 3d22 6c6f 676f 2d70 696e   <g id="logo-pin
-000006c0: 6b22 2074 7261 6e73 666f 726d 3d22 6d61  k" transform="ma
-000006d0: 7472 6978 2830 2e38 3534 3837 362c 302c  trix(0.854876,0,
-000006e0: 302c 302e 3835 3438 3736 2c2d 362e 3733  0,0.854876,-6.73
-000006f0: 3531 342c 312e 3237 3731 3234 2922 3e0a  514,1.277124)">.
-00000700: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-00000710: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
-00000720: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
-00000730: 3132 2c39 2e37 3032 3239 2c2d 362e 3638  12,9.70229,-6.68
-00000740: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
-00000750: 2020 203c 7061 7468 2064 3d22 4d35 302c     <path d="M50,
-00000760: 3634 2e32 3543 3532 2e37 362c 3634 2e32  64.25C52.76,64.2
-00000770: 3520 3535 2c36 312e 3133 2035 352c 3539  5 55,61.13 55,59
-00000780: 2e37 3543 3535 2c35 382e 3337 2035 322e  .75C55,58.37 52.
-00000790: 3736 2c35 372e 3235 2035 302c 3537 2e32  76,57.25 50,57.2
-000007a0: 3543 3437 2e32 342c 3537 2e32 3520 3435  5C47.24,57.25 45
-000007b0: 2c35 382e 3337 2034 352c 3539 2e37 3543  ,58.37 45,59.75C
-000007c0: 3435 2c36 312e 3133 2034 372e 3234 2c36  45,61.13 47.24,6
-000007d0: 342e 3235 2035 302c 3634 2e32 355a 2220  4.25 50,64.25Z" 
-000007e0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
-000007f0: 3232 322c 3132 302c 3136 3029 3b66 696c  222,120,160);fil
-00000800: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b22  l-rule:nonzero;"
-00000810: 2f3e 0a20 2020 2020 2020 203c 2f67 3e0a  />.        </g>.
-00000820: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-00000830: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
-00000840: 3939 3031 322c 302c 302c 302e 3239 3930  99012,0,0,0.2990
-00000850: 3132 2c39 2e37 3032 3239 2c2d 362e 3638  12,9.70229,-6.68
-00000860: 3538 3229 223e 0a20 2020 2020 2020 2020  582)">.         
-00000870: 2020 203c 7061 7468 2064 3d22 4d38 382c     <path d="M88,
-00000880: 3439 2e30 3543 3836 2e35 3036 2c34 332e  49.05C86.506,43.
-00000890: 3437 3520 3833 2e30 3138 2c33 382e 3633  475 83.018,38.63
-000008a0: 3820 3738 2e32 2c33 352e 3436 4337 322e  8 78.2,35.46C72.
-000008b0: 3936 392c 3332 2e30 3032 2036 362e 3533  969,32.002 66.53
-000008c0: 392c 3330 2e38 3434 2036 302e 3433 2c33  9,30.844 60.43,3
-000008d0: 322e 3236 4335 362e 3537 362c 3333 2e31  2.26C56.576,33.1
-000008e0: 3435 2035 322e 3939 352c 3334 2e39 3538  45 52.995,34.958
-000008f0: 2035 302c 3337 2e35 3443 3436 2e39 3938   50,37.54C46.998
-00000900: 2c33 342e 3935 3820 3433 2e34 3131 2c33  ,34.958 43.411,3
-00000910: 332e 3134 3920 3339 2e35 352c 3332 2e32  3.149 39.55,32.2
-00000920: 3743 3333 2e34 3431 2c33 302e 3835 3320  7C33.441,30.853 
-00000930: 3237 2e30 3131 2c33 322e 3031 3120 3231  27.011,32.011 21
-00000940: 2e37 382c 3335 2e34 3743 3136 2e39 372c  .78,35.47C16.97,
-00000950: 3338 2e36 3532 2031 332e 3438 392c 3433  38.652 13.489,43
-00000960: 2e34 3839 2031 322c 3439 2e30 364c 3132  .489 12,49.06L12
-00000970: 2c34 392e 3133 4331 312e 3832 2c34 392e  ,49.13C11.82,49.
-00000980: 3739 2031 312e 3636 2c35 302e 3436 2031  79 11.66,50.46 1
-00000990: 312e 3533 2c35 312e 3133 4331 312e 3134  1.53,51.13C11.14
-000009a0: 362c 3533 2e32 3037 2031 312e 3032 312c  6,53.207 11.021,
-000009b0: 3535 2e33 3233 2031 312e 3136 2c35 372e  55.323 11.16,57.
-000009c0: 3433 4331 312e 3136 2c35 382e 3033 2031  43C11.16,58.03 1
-000009d0: 312e 3236 2c35 382e 3633 2031 312e 3334  1.26,58.63 11.34
-000009e0: 2c35 392e 3233 4331 312e 3334 2c35 392e  ,59.23C11.34,59.
-000009f0: 3531 2031 312e 3433 2c35 392e 3739 2031  51 11.43,59.79 1
-00000a00: 312e 3438 2c36 302e 3037 4331 312e 3533  1.48,60.07C11.53
-00000a10: 2c36 302e 3335 2031 312e 3538 2c36 302e  ,60.35 11.58,60.
-00000a20: 3638 2031 312e 3634 2c36 302e 3938 4331  68 11.64,60.98C1
-00000a30: 312e 372c 3631 2e32 3820 3131 2e38 2c36  1.7,61.28 11.8,6
-00000a40: 312e 3639 2031 312e 3839 2c36 322e 3035  1.69 11.89,62.05
-00000a50: 4331 312e 3938 2c36 322e 3431 2031 312e  C11.98,62.41 11.
-00000a60: 3939 2c36 322e 3437 2031 322e 3035 2c36  99,62.47 12.05,6
-00000a70: 322e 3638 4331 322e 3136 2c36 332e 3037  2.68C12.16,63.07
-00000a80: 2031 322e 3238 2c36 332e 3436 2031 322e   12.28,63.46 12.
-00000a90: 3431 2c36 332e 3834 4c31 322e 3538 2c36  41,63.84L12.58,6
-00000aa0: 342e 3334 4331 322e 3732 2c36 342e 3734  4.34C12.72,64.74
-00000ab0: 2031 322e 3838 2c36 352e 3134 2031 332e   12.88,65.14 13.
-00000ac0: 3034 2c36 352e 3533 4c31 332e 3233 2c36  04,65.53L13.23,6
-00000ad0: 352e 3938 4331 332e 3430 332c 3636 2e33  5.98C13.403,66.3
-00000ae0: 3733 2031 332e 3538 332c 3636 2e37 3637  73 13.583,66.767
-00000af0: 2031 332e 3737 2c36 372e 3136 4c31 332e   13.77,67.16L13.
-00000b00: 3939 2c36 372e 3539 4331 342e 3139 2c36  99,67.59C14.19,6
-00000b10: 372e 3937 2031 342e 3339 2c36 382e 3335  7.97 14.39,68.35
-00000b20: 2031 342e 3631 2c36 382e 3733 4c31 342e   14.61,68.73L14.
-00000b30: 3837 2c36 392e 3135 4331 352e 312c 3639  87,69.15C15.1,69
-00000b40: 2e35 3220 3135 2e33 332c 3639 2e38 3920  .52 15.33,69.89 
-00000b50: 3135 2e35 382c 3730 2e32 364c 3135 2e35  15.58,70.26L15.5
-00000b60: 382c 3730 2e33 324c 3135 2e39 392c 3730  8,70.32L15.99,70
-00000b70: 2e39 3343 3136 2e31 342c 3731 2e31 3420  .93C16.14,71.14 
-00000b80: 3136 2e32 392c 3731 2e33 3620 3136 2e34  16.29,71.36 16.4
-00000b90: 352c 3731 2e35 3743 3230 2e32 3036 2c37  5,71.57C20.206,7
-00000ba0: 352e 3833 2032 352e 3038 362c 3738 2e39  5.83 25.086,78.9
-00000bb0: 3520 3330 2e35 332c 3830 2e35 3743 3336  5 30.53,80.57C36
-00000bc0: 2e38 3339 2c38 322e 3438 2034 332e 3431  .839,82.48 43.41
-00000bd0: 2c38 332e 3338 3520 3530 2c38 332e 3235  ,83.385 50,83.25
-00000be0: 4335 362e 3539 392c 3833 2e33 3734 2036  C56.599,83.374 6
-00000bf0: 332e 3137 372c 3832 2e34 3536 2036 392e  3.177,82.456 69.
-00000c00: 3439 2c38 302e 3533 4337 342e 3634 342c  49,80.53C74.644,
-00000c10: 3738 2e39 3738 2037 392e 3330 332c 3736  78.978 79.303,76
-00000c20: 2e31 3032 2038 332c 3732 2e31 3943 3833  .102 83,72.19C83
-00000c30: 2e33 342c 3731 2e37 3820 3833 2e36 352c  .34,71.78 83.65,
-00000c40: 3731 2e33 3520 3834 2c37 302e 3932 4c38  71.35 84,70.92L8
-00000c50: 342e 3138 2c37 302e 3636 4c38 342e 3333  4.18,70.66L84.33
-00000c60: 2c37 302e 3434 4c38 342e 3431 2c37 302e  ,70.44L84.41,70.
-00000c70: 3332 4338 342e 3535 2c37 302e 3132 2038  32C84.55,70.12 8
-00000c80: 342e 3637 2c36 392e 3920 3834 2e38 312c  4.67,69.9 84.81,
-00000c90: 3639 2e37 4338 352e 3037 2c36 392e 3320  69.7C85.07,69.3 
-00000ca0: 3835 2e33 322c 3638 2e38 3920 3835 2e35  85.32,68.89 85.5
-00000cb0: 352c 3638 2e34 3843 3835 2e37 382c 3638  5,68.48C85.78,68
-00000cc0: 2e30 3720 3836 2e30 322c 3637 2e36 3520  .07 86.02,67.65 
-00000cd0: 3836 2e32 332c 3637 2e32 3243 3836 2e33  86.23,67.22C86.3
-00000ce0: 312c 3637 2e30 3520 3836 2e33 392c 3636  1,67.05 86.39,66
-00000cf0: 2e38 3820 3836 2e34 372c 3636 2e37 4338  .88 86.47,66.7C8
-00000d00: 362e 3637 2c36 362e 3238 2038 362e 3835  6.67,66.28 86.85
-00000d10: 2c36 352e 3837 2038 372e 3033 2c36 352e  ,65.87 87.03,65.
-00000d20: 3434 4c38 372e 3233 2c36 342e 3932 4338  44L87.23,64.92C8
-00000d30: 372e 3339 372c 3634 2e34 3837 2038 372e  7.397,64.487 87.
-00000d40: 3535 2c36 342e 3035 2038 372e 3639 2c36  55,64.05 87.69,6
-00000d50: 332e 3631 4c38 372e 3835 2c36 332e 3039  3.61L87.85,63.09
-00000d60: 4338 372e 3938 2c36 322e 3634 2038 382e  C87.98,62.64 88.
-00000d70: 312c 3632 2e31 3920 3838 2e32 312c 3631  1,62.19 88.21,61
-00000d80: 2e37 3443 3838 2e32 312c 3631 2e35 3720  .74C88.21,61.57 
-00000d90: 3838 2e33 2c36 312e 3339 2038 382e 3333  88.3,61.39 88.33
-00000da0: 2c36 312e 3232 4338 382e 3433 2c36 302e  ,61.22C88.43,60.
-00000db0: 3735 2038 382e 3532 2c36 302e 3232 2038  75 88.52,60.22 8
-00000dc0: 382e 362c 3539 2e37 3943 3838 2e36 2c35  8.6,59.79C88.6,5
-00000dd0: 392e 3634 2038 382e 3636 2c35 392e 3439  9.64 88.66,59.49
-00000de0: 2038 382e 3638 2c35 392e 3333 4338 382e   88.68,59.33C88.
-00000df0: 3737 2c35 382e 3731 2038 382e 3834 2c35  77,58.71 88.84,5
-00000e00: 382e 3038 2038 382e 3838 2c35 372e 3435  8.08 88.88,57.45
-00000e10: 4c38 382e 3838 2c35 342e 3137 4338 382e  L88.88,54.17C88.
-00000e20: 3831 372c 3533 2e31 3634 2038 382e 3639  817,53.164 88.69
-00000e30: 332c 3532 2e31 3632 2038 382e 3531 2c35  3,52.162 88.51,5
-00000e40: 312e 3137 4338 382e 3338 2c35 302e 3520  1.17C88.38,50.5 
-00000e50: 3838 2e32 332c 3439 2e38 3420 3838 2e30  88.23,49.84 88.0
-00000e60: 352c 3439 2e31 374c 3838 2c34 392e 3035  5,49.17L88,49.05
-00000e70: 5a4d 3835 2e38 392c 3536 2e34 344c 3835  ZM85.89,56.44L85
-00000e80: 2e38 392c 3537 2e32 3343 3835 2e38 392c  .89,57.23C85.89,
-00000e90: 3537 2e37 3820 3835 2e37 392c 3538 2e33  57.78 85.79,58.3
-00000ea0: 3220 3835 2e37 322c 3538 2e38 3643 3835  2 85.72,58.86C85
-00000eb0: 2e37 322c 3539 2e30 3120 3835 2e37 322c  .72,59.01 85.72,
-00000ec0: 3539 2e31 3520 3835 2e36 352c 3539 2e33  59.15 85.65,59.3
-00000ed0: 4338 352e 3539 2c35 392e 3720 3835 2e35  C85.59,59.7 85.5
-00000ee0: 312c 3630 2e31 3120 3835 2e34 332c 3630  1,60.11 85.43,60
-00000ef0: 2e35 314c 3835 2e33 322c 3630 2e39 3943  .51L85.32,60.99C
-00000f00: 3835 2e32 332c 3631 2e33 3820 3835 2e31  85.23,61.38 85.1
-00000f10: 322c 3631 2e37 3720 3835 2e30 312c 3632  2,61.77 85.01,62
-00000f20: 2e31 3643 3835 2e30 312c 3632 2e33 3120  .16C85.01,62.31 
-00000f30: 3834 2e39 332c 3632 2e34 3620 3834 2e38  84.93,62.46 84.8
-00000f40: 382c 3632 2e36 4338 342e 3734 2c36 332e  8,62.6C84.74,63.
-00000f50: 3034 2038 342e 3539 2c36 332e 3437 2038  04 84.59,63.47 8
-00000f60: 342e 3432 2c36 332e 394c 3834 2e32 372c  4.42,63.9L84.27,
-00000f70: 3634 2e32 3843 3834 2e31 2c36 342e 3731  64.28C84.1,64.71
-00000f80: 2038 332e 3931 2c36 352e 3134 2038 332e   83.91,65.14 83.
-00000f90: 3731 2c36 352e 3536 4338 332e 3531 2c36  71,65.56C83.51,6
-00000fa0: 352e 3938 2038 332e 3433 2c36 362e 3132  5.98 83.43,66.12
-00000fb0: 2038 332e 3238 2c36 362e 344c 3833 2e30   83.28,66.4L83.0
-00000fc0: 312c 3636 2e39 3143 3832 2e38 332c 3637  1,66.91C82.83,67
-00000fd0: 2e32 3233 2038 322e 3634 332c 3637 2e35  .223 82.643,67.5
-00000fe0: 3337 2038 322e 3435 2c36 372e 3835 4c38  37 82.45,67.85L8
-00000ff0: 322e 3335 2c36 382e 3031 4337 392e 3132  2.35,68.01C79.12
-00001000: 312c 3638 2e30 3437 2037 352e 3931 382c  1,68.047 75.918,
-00001010: 3637 2e34 3334 2037 322e 3933 2c36 362e  67.434 72.93,66.
-00001020: 3231 4336 342e 3237 2c36 322e 3734 2035  21C64.27,62.74 5
-00001030: 392c 3535 2e35 3220 3631 2e31 382c 3530  9,55.52 61.18,50
-00001040: 2e31 3143 3632 2e31 382c 3437 2e36 2036  .11C62.18,47.6 6
-00001050: 342e 372c 3435 2e38 3220 3638 2e32 362c  4.7,45.82 68.26,
-00001060: 3435 2e31 3143 3732 2e34 3839 2c34 342e  45.11C72.489,44.
-00001070: 3339 3520 3736 2e38 3335 2c34 342e 3930  395 76.835,44.90
-00001080: 3820 3830 2e37 382c 3436 2e35 3943 3832  8 80.78,46.59C82
-00001090: 2e31 3431 2c34 372e 3134 3420 3833 2e34  .141,47.144 83.4
-000010a0: 3533 2c34 372e 3831 3320 3834 2e37 2c34  53,47.813 84.7,4
-000010b0: 382e 3539 4338 342e 3736 2c34 382e 3736  8.59C84.76,48.76
-000010c0: 2038 342e 3832 2c34 382e 3933 2038 342e   84.82,48.93 84.
-000010d0: 3838 2c34 392e 3143 3834 2e39 342c 3439  88,49.1C84.94,49
-000010e0: 2e32 3720 3835 2e30 352c 3439 2e36 3320  .27 85.05,49.63 
-000010f0: 3835 2e31 322c 3439 2e39 4338 352e 3238  85.12,49.9C85.28
-00001100: 2c35 302e 3520 3835 2e34 342c 3531 2e31  ,50.5 85.44,51.1
-00001110: 2038 352e 3535 2c35 312e 3733 4338 352e   85.55,51.73C85.
-00001120: 3639 312c 3532 2e35 3037 2038 352e 3739  691,52.507 85.79
-00001130: 322c 3533 2e32 3932 2038 352e 3835 2c35  2,53.292 85.85,5
-00001140: 342e 3038 4c38 352e 3835 2c35 352e 3839  4.08L85.85,55.89
-00001150: 4338 352e 3835 2c35 362e 3132 2038 352e  C85.85,56.12 85.
-00001160: 3931 2c35 362e 3235 2038 352e 3931 2c35  91,56.25 85.91,5
-00001170: 362e 3435 4c38 352e 3839 2c35 362e 3434  6.45L85.89,56.44
-00001180: 5a4d 3137 2e36 362c 3638 4331 362e 3636  ZM17.66,68C16.66
-00001190: 382c 3636 2e34 3335 2031 352e 3836 392c  8,66.435 15.869,
-000011a0: 3634 2e37 3536 2031 352e 3238 2c36 334c  64.756 15.28,63L
-000011b0: 3135 2e31 372c 3632 2e36 3843 3135 2e30  15.17,62.68C15.0
-000011c0: 362c 3632 2e33 3520 3134 2e39 362c 3632  6,62.35 14.96,62
-000011d0: 2e30 3120 3134 2e38 372c 3631 2e36 3843  .01 14.87,61.68C
-000011e0: 3134 2e38 3233 2c36 312e 3439 3320 3134  14.823,61.493 14
-000011f0: 2e37 3737 2c36 312e 3331 2031 342e 3733  .777,61.31 14.73
-00001200: 2c36 312e 3133 4331 342e 3636 2c36 302e  ,61.13C14.66,60.
-00001210: 3834 2031 342e 3539 2c36 302e 3535 2031  84 14.59,60.55 1
-00001220: 342e 3533 2c36 302e 3237 4331 342e 3437  4.53,60.27C14.47
-00001230: 2c35 392e 3939 2031 342e 3433 2c35 392e  ,59.99 14.43,59.
-00001240: 3732 2031 342e 3338 2c35 392e 3434 4331  72 14.38,59.44C1
-00001250: 342e 3333 2c35 392e 3136 2031 342e 332c  4.33,59.16 14.3,
-00001260: 3539 2031 342e 3237 2c35 382e 3738 4331  59 14.27,58.78C1
-00001270: 342e 322c 3538 2e32 3720 3134 2e31 352c  4.2,58.27 14.15,
-00001280: 3537 2e37 3820 3134 2e31 312c 3537 2e32  57.78 14.11,57.2
-00001290: 334c 3134 2e31 312c 3537 2e30 3343 3134  3L14.11,57.03C14
-000012a0: 2e30 3038 2c35 352e 3233 3620 3134 2e31  .008,55.236 14.1
-000012b0: 3232 2c35 332e 3433 3720 3134 2e34 352c  22,53.437 14.45,
-000012c0: 3531 2e36 3743 3134 2e35 362c 3531 2e30  51.67C14.56,51.0
-000012d0: 3620 3134 2e37 312c 3530 2e34 3620 3134  6 14.71,50.46 14
-000012e0: 2e38 382c 3439 2e38 3743 3134 2e39 362c  .88,49.87C14.96,
-000012f0: 3439 2e35 3920 3135 2e30 342c 3439 2e33  49.59 15.04,49.3
-00001300: 3220 3135 2e31 332c 3439 2e30 3543 3135  2 15.13,49.05C15
-00001310: 2e32 322c 3438 2e37 3820 3135 2e32 342c  .22,48.78 15.24,
-00001320: 3438 2e37 3220 3135 2e33 2c34 382e 3535  48.72 15.3,48.55
-00001330: 4331 362e 3534 382c 3437 2e37 3734 2031  C16.548,47.774 1
-00001340: 372e 3835 392c 3437 2e31 3035 2031 392e  7.859,47.105 19.
-00001350: 3232 2c34 362e 3535 4332 372e 3836 2c34  22,46.55C27.86,4
-00001360: 332e 3039 2033 362e 3635 2c34 342e 3637  3.09 36.65,44.67
-00001370: 2033 382e 3832 2c35 302e 3038 4334 302e   38.82,50.08C40.
-00001380: 3939 2c35 352e 3439 2033 352e 3733 2c36  99,55.49 35.73,6
-00001390: 322e 3734 2032 372e 3039 2c36 362e 3243  2.74 27.09,66.2C
-000013a0: 3234 2e31 3031 2c36 372e 3433 3120 3230  24.101,67.431 20
-000013b0: 2e38 3933 2c36 382e 3034 3320 3137 2e36  .893,68.043 17.6
-000013c0: 362c 3638 5a4d 3638 2e35 372c 3737 2e36  6,68ZM68.57,77.6
-000013d0: 3843 3632 2e35 3534 2c37 392e 3530 3820  8C62.554,79.508 
-000013e0: 3536 2e32 3837 2c38 302e 3337 3620 3530  56.287,80.376 50
-000013f0: 2c38 302e 3235 4334 332e 3733 372c 3830  ,80.25C43.737,80
-00001400: 2e33 3720 3337 2e34 3935 2c37 392e 3530  .37 37.495,79.50
-00001410: 3620 3331 2e35 2c37 372e 3639 4332 372e  6 31.5,77.69C27.
-00001420: 3138 352c 3736 2e33 3820 3233 2e32 3433  185,76.38 23.243
-00001430: 2c37 342e 3036 3220 3230 2c37 302e 3933  ,74.062 20,70.93
-00001440: 4332 322e 3831 352c 3730 2e37 3036 2032  C22.815,70.706 2
-00001450: 352e 3538 2c37 302e 3035 3520 3238 2e32  5.58,70.055 28.2
-00001460: 2c36 3943 3338 2e33 372c 3634 2e39 3220  ,69C38.37,64.92 
-00001470: 3434 2e33 392c 3536 2034 312e 362c 3439  44.39,56 41.6,49
-00001480: 4333 382e 3831 2c34 3220 3238 2e32 372c  C38.81,42 28.27,
-00001490: 3339 2e37 3220 3138 2e31 2c34 332e 384c  39.72 18.1,43.8L
-000014a0: 3137 2e34 332c 3434 2e30 3943 3138 2e39  17.43,44.09C18.9
-000014b0: 3733 2c34 312e 3634 3820 3231 2e30 3139  73,41.648 21.019
-000014c0: 2c33 392e 3536 3120 3233 2e34 332c 3337  ,39.561 23.43,37
-000014d0: 2e39 3743 3236 2e36 3731 2c33 352e 3832  .97C26.671,35.82
-000014e0: 3420 3330 2e34 3733 2c33 342e 3638 2033  4 30.473,34.68 3
-000014f0: 342e 3336 2c33 342e 3638 4333 352e 3838  4.36,34.68C35.88
-00001500: 342c 3334 2e36 3831 2033 372e 3430 342c  4,34.681 37.404,
-00001510: 3334 2e38 3532 2033 382e 3839 2c33 352e  34.852 38.89,35.
-00001520: 3139 4334 322e 3639 342c 3336 2e30 3439  19C42.694,36.049
-00001530: 2034 362e 3139 312c 3337 2e39 3335 2034   46.191,37.935 4
-00001540: 392c 3430 2e36 344c 3530 2c34 312e 3634  9,40.64L50,41.64
-00001550: 4c35 312c 3430 2e36 3443 3533 2e37 3937  L51,40.64C53.797
-00001560: 2c33 372e 3933 3720 3537 2e32 3739 2c33  ,37.937 57.279,3
-00001570: 362e 3034 3920 3631 2e30 372c 3335 2e31  6.049 61.07,35.1
-00001580: 3843 3636 2e34 3032 2c33 332e 3934 3720  8C66.402,33.947 
-00001590: 3732 2e30 3134 2c33 342e 3936 3820 3736  72.014,34.968 76
-000015a0: 2e35 372c 3338 4337 382e 3938 2c33 392e  .57,38C78.98,39.
-000015b0: 3538 3820 3831 2e30 3236 2c34 312e 3637  588 81.026,41.67
-000015c0: 3120 3832 2e35 372c 3434 2e31 314c 3831  1 82.57,44.11L81
-000015d0: 2e39 2c34 332e 3832 4337 372e 3430 392c  .9,43.82C77.409,
-000015e0: 3431 2e39 3231 2037 322e 3436 342c 3431  41.921 72.464,41
-000015f0: 2e33 3535 2036 372e 3636 2c34 322e 3139  .355 67.66,42.19
-00001600: 4336 332e 3038 2c34 332e 3132 2035 392e  C63.08,43.12 59.
-00001610: 3739 2c34 352e 3534 2035 382e 3339 2c34  79,45.54 58.39,4
-00001620: 392e 3032 4335 352e 362c 3535 2e39 3720  9.02C55.6,55.97 
-00001630: 3631 2e36 322c 3634 2e39 3420 3731 2e37  61.62,64.94 71.7
-00001640: 392c 3639 2e30 3243 3734 2e34 3134 2c37  9,69.02C74.414,7
-00001650: 302e 3037 2037 372e 3138 322c 3730 2e37  0.07 77.182,70.7
-00001660: 3134 2038 302c 3730 2e39 3343 3736 2e37  14 80,70.93C76.7
-00001670: 3736 2c37 342e 3035 2037 322e 3835 392c  76,74.05 72.859,
-00001680: 3736 2e33 3633 2036 382e 3537 2c37 372e  76.363 68.57,77.
-00001690: 3638 5a22 2073 7479 6c65 3d22 6669 6c6c  68Z" style="fill
-000016a0: 3a72 6762 2832 3232 2c31 3230 2c31 3630  :rgb(222,120,160
-000016b0: 293b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  );fill-rule:nonz
-000016c0: 6572 6f3b 222f 3e0a 2020 2020 2020 2020  ero;"/>.        
-000016d0: 3c2f 673e 0a20 2020 2020 2020 203c 6720  </g>.        <g 
-000016e0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-000016f0: 7828 302e 3239 3930 3132 2c30 2c30 2c30  x(0.299012,0,0,0
-00001700: 2e32 3939 3031 322c 392e 3730 3232 392c  .299012,9.70229,
-00001710: 2d36 2e36 3835 3832 2922 3e0a 2020 2020  -6.68582)">.    
-00001720: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
-00001730: 6378 3d22 3731 2e33 3322 2063 793d 2235  cx="71.33" cy="5
-00001740: 3622 2072 3d22 352e 3136 2220 7374 796c  6" r="5.16" styl
-00001750: 653d 2266 696c 6c3a 7267 6228 3232 322c  e="fill:rgb(222,
-00001760: 3132 302c 3136 3029 3b22 2f3e 0a20 2020  120,160);"/>.   
-00001770: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00001780: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00001790: 6d61 7472 6978 2830 2e32 3939 3031 322c  matrix(0.299012,
-000017a0: 302c 302c 302e 3239 3930 3132 2c39 2e37  0,0,0.299012,9.7
-000017b0: 3032 3239 2c2d 362e 3638 3538 3229 223e  0229,-6.68582)">
-000017c0: 0a20 2020 2020 2020 2020 2020 203c 6369  .            <ci
-000017d0: 7263 6c65 2063 783d 2232 382e 3637 2220  rcle cx="28.67" 
-000017e0: 6379 3d22 3536 2220 723d 2235 2e31 3622  cy="56" r="5.16"
-000017f0: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
-00001800: 2832 3232 2c31 3230 2c31 3630 293b 222f  (222,120,160);"/
-00001810: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-00001820: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00001830: 6f72 6d3d 226d 6174 7269 7828 302e 3239  orm="matrix(0.29
-00001840: 3930 3132 2c30 2c30 2c30 2e32 3939 3031  9012,0,0,0.29901
-00001850: 322c 392e 3730 3232 392c 2d36 2e36 3835  2,9.70229,-6.685
-00001860: 3832 2922 3e0a 2020 2020 2020 2020 2020  82)">.          
-00001870: 2020 3c70 6174 6820 643d 224d 3538 2c36    <path d="M58,6
-00001880: 3643 3535 2e39 3132 2c36 382e 3136 3120  6C55.912,68.161 
-00001890: 3533 2e30 3033 2c36 392e 3333 3920 3530  53.003,69.339 50
-000018a0: 2c36 392e 3234 4334 362e 3939 372c 3639  ,69.24C46.997,69
-000018b0: 2e33 3339 2034 342e 3038 382c 3638 2e31  .339 44.088,68.1
-000018c0: 3631 2034 322c 3636 4334 312e 3731 342c  61 42,66C41.714,
-000018d0: 3635 2e36 3737 2034 312e 3330 322c 3635  65.677 41.302,65
-000018e0: 2e34 3931 2034 302e 3837 2c36 352e 3439  .491 40.87,65.49
-000018f0: 3143 3430 2e30 3432 2c36 352e 3439 3120  1C40.042,65.491 
-00001900: 3339 2e33 3631 2c36 362e 3137 3220 3339  39.361,66.172 39
-00001910: 2e33 3631 2c36 3743 3339 2e33 3631 2c36  .361,67C39.361,6
-00001920: 372e 3336 3820 3339 2e34 3936 2c36 372e  7.368 39.496,67.
-00001930: 3732 3420 3339 2e37 342c 3638 4334 322e  724 39.74,68C42.
-00001940: 3430 332c 3730 2e38 3034 2034 362e 3133  403,70.804 46.13
-00001950: 342c 3732 2e33 3520 3530 2c37 322e 3235  4,72.35 50,72.25
-00001960: 4335 332e 3836 322c 3732 2e33 3437 2035  C53.862,72.347 5
-00001970: 372e 3539 2c37 302e 3830 3220 3630 2e32  7.59,70.802 60.2
-00001980: 352c 3638 4336 302e 3439 352c 3637 2e37  5,68C60.495,67.7
-00001990: 3235 2036 302e 3633 2c36 372e 3336 3920  25 60.63,67.369 
-000019a0: 3630 2e36 332c 3637 4336 302e 3633 2c36  60.63,67C60.63,6
-000019b0: 362e 3137 3420 3539 2e39 3531 2c36 352e  6.174 59.951,65.
-000019c0: 3439 3520 3539 2e31 3235 2c36 352e 3439  495 59.125,65.49
-000019d0: 3543 3538 2e36 3935 2c36 352e 3439 3520  5C58.695,65.495 
-000019e0: 3538 2e32 3835 2c36 352e 3637 3920 3538  58.285,65.679 58
-000019f0: 2c36 365a 2220 7374 796c 653d 2266 696c  ,66Z" style="fil
-00001a00: 6c3a 7267 6228 3232 322c 3132 302c 3136  l:rgb(222,120,16
-00001a10: 3029 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  0);fill-rule:non
-00001a20: 7a65 726f 3b22 2f3e 0a20 2020 2020 2020  zero;"/>.       
-00001a30: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a3c   </g>.    </g>.<
-00001a40: 2f73 7667 3e0a                           /svg>.
+00000000: 3c73 7667 2077 6964 7468 3d22 3134 3022  <svg width="140"
+00000010: 2068 6569 6768 743d 2232 3022 2076 6965   height="20" vie
+00000020: 7742 6f78 3d22 3020 3020 3134 3020 3230  wBox="0 0 140 20
+00000030: 2220 7665 7273 696f 6e3d 2231 2e31 2220  " version="1.1" 
+00000040: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00000050: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
+00000060: 6722 2078 6d6c 6e73 3a78 6c69 6e6b 3d22  g" xmlns:xlink="
+00000070: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000080: 672f 3139 3939 2f78 6c69 6e6b 2220 786d  g/1999/xlink" xm
+00000090: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
+000000a0: 6522 2078 6d6c 6e73 3a73 6572 6966 3d22  e" xmlns:serif="
+000000b0: 6874 7470 3a2f 2f77 7777 2e73 6572 6966  http://www.serif
+000000c0: 2e63 6f6d 2f22 2073 7479 6c65 3d22 6669  .com/" style="fi
+000000d0: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
+000000e0: 636c 6970 2d72 756c 653a 6576 656e 6f64  clip-rule:evenod
+000000f0: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00000100: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
+00000110: 6974 6572 6c69 6d69 743a 323b 223e 0a20  iterlimit:2;">. 
+00000120: 2020 203c 7469 746c 653e 696e 7465 7272     <title>interr
+00000130: 6f67 6174 653a 2031 3030 253c 2f74 6974  ogate: 100%</tit
+00000140: 6c65 3e0a 2020 2020 3c67 2074 7261 6e73  le>.    <g trans
+00000150: 666f 726d 3d22 6d61 7472 6978 2831 2c30  form="matrix(1,0
+00000160: 2c30 2c31 2c32 322c 3029 223e 0a20 2020  ,0,1,22,0)">.   
+00000170: 2020 2020 203c 6720 6964 3d22 6261 636b       <g id="back
+00000180: 6772 6f75 6e64 7322 2074 7261 6e73 666f  grounds" transfo
+00000190: 726d 3d22 6d61 7472 6978 2831 2e33 3237  rm="matrix(1.327
+000001a0: 3839 2c30 2c30 2c31 2c2d 3232 2e33 3839  89,0,0,1,-22.389
+000001b0: 322c 3029 223e 0a20 2020 2020 2020 2020  2,0)">.         
+000001c0: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
+000001d0: 3d22 3022 2077 6964 7468 3d22 3731 2220  ="0" width="71" 
+000001e0: 6865 6967 6874 3d22 3230 2220 7374 796c  height="20" styl
+000001f0: 653d 2266 696c 6c3a 7267 6228 3835 2c38  e="fill:rgb(85,8
+00000200: 352c 3835 293b 222f 3e0a 2020 2020 2020  5,85);"/>.      
+00000210: 2020 3c2f 673e 0a20 2020 2020 2020 203c    </g>.        <
+00000220: 7265 6374 2078 3d22 3731 2220 793d 2230  rect x="71" y="0
+00000230: 2220 7769 6474 683d 2234 3722 2068 6569  " width="47" hei
+00000240: 6768 743d 2232 3022 2064 6174 612d 696e  ght="20" data-in
+00000250: 7465 7272 6f67 6174 653d 2263 6f6c 6f72  terrogate="color
+00000260: 2220 7374 796c 653d 2266 696c 6c3a 2334  " style="fill:#4
+00000270: 6331 222f 3e0a 2020 2020 2020 2020 3c67  c1"/>.        <g
+00000280: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
+00000290: 6978 2831 2e31 3937 3436 2c30 2c30 2c31  ix(1.19746,0,0,1
+000002a0: 2c2d 3232 2e33 3734 342c 2d34 2e38 3537  ,-22.3744,-4.857
+000002b0: 3233 652d 3136 2922 3e0a 2020 2020 2020  23e-16)">.      
+000002c0: 2020 2020 2020 3c72 6563 7420 783d 2230        <rect x="0
+000002d0: 2220 793d 2230 2220 7769 6474 683d 2231  " y="0" width="1
+000002e0: 3138 2220 6865 6967 6874 3d22 3230 2220  18" height="20" 
+000002f0: 7374 796c 653d 2266 696c 6c3a 7572 6c28  style="fill:url(
+00000300: 235f 4c69 6e65 6172 3129 3b22 2f3e 0a20  #_Linear1);"/>. 
+00000310: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
+00000320: 3c2f 673e 0a20 2020 203c 6720 6669 6c6c  </g>.    <g fill
+00000330: 3d22 2366 6666 2220 7465 7874 2d61 6e63  ="#fff" text-anc
+00000340: 686f 723d 226d 6964 646c 6522 2066 6f6e  hor="middle" fon
+00000350: 742d 6661 6d69 6c79 3d22 4465 6a61 5675  t-family="DejaVu
+00000360: 2053 616e 732c 5665 7264 616e 612c 4765   Sans,Verdana,Ge
+00000370: 6e65 7661 2c73 616e 732d 7365 7269 6622  neva,sans-serif"
+00000380: 2066 6f6e 742d 7369 7a65 3d22 3131 3022   font-size="110"
+00000390: 3e0a 2020 2020 2020 2020 3c74 6578 7420  >.        <text 
+000003a0: 783d 2235 3930 2220 793d 2231 3530 2220  x="590" y="150" 
+000003b0: 6669 6c6c 3d22 2330 3130 3130 3122 2066  fill="#010101" f
+000003c0: 696c 6c2d 6f70 6163 6974 793d 222e 3322  ill-opacity=".3"
+000003d0: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
+000003e0: 6528 2e31 2922 2074 6578 744c 656e 6774  e(.1)" textLengt
+000003f0: 683d 2236 3130 223e 696e 7465 7272 6f67  h="610">interrog
+00000400: 6174 653c 2f74 6578 743e 0a20 2020 2020  ate</text>.     
+00000410: 2020 203c 7465 7874 2078 3d22 3539 3022     <text x="590"
+00000420: 2079 3d22 3134 3022 2074 7261 6e73 666f   y="140" transfo
+00000430: 726d 3d22 7363 616c 6528 2e31 2922 2074  rm="scale(.1)" t
+00000440: 6578 744c 656e 6774 683d 2236 3130 223e  extLength="610">
+00000450: 696e 7465 7272 6f67 6174 653c 2f74 6578  interrogate</tex
+00000460: 743e 0a20 2020 2020 2020 203c 7465 7874  t>.        <text
+00000470: 2078 3d22 3131 3630 2220 793d 2231 3530   x="1160" y="150
+00000480: 2220 6669 6c6c 3d22 2330 3130 3130 3122  " fill="#010101"
+00000490: 2066 696c 6c2d 6f70 6163 6974 793d 222e   fill-opacity=".
+000004a0: 3322 2074 7261 6e73 666f 726d 3d22 7363  3" transform="sc
+000004b0: 616c 6528 2e31 2922 2074 6578 744c 656e  ale(.1)" textLen
+000004c0: 6774 683d 2233 3330 2220 6461 7461 2d69  gth="330" data-i
+000004d0: 6e74 6572 726f 6761 7465 3d22 7265 7375  nterrogate="resu
+000004e0: 6c74 223e 3130 3025 3c2f 7465 7874 3e0a  lt">100%</text>.
+000004f0: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
+00000500: 2231 3136 3022 2079 3d22 3134 3022 2074  "1160" y="140" t
+00000510: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
+00000520: 2e31 2922 2074 6578 744c 656e 6774 683d  .1)" textLength=
+00000530: 2233 3330 2220 6461 7461 2d69 6e74 6572  "330" data-inter
+00000540: 726f 6761 7465 3d22 7265 7375 6c74 223e  rogate="result">
+00000550: 3130 3025 3c2f 7465 7874 3e0a 2020 2020  100%</text>.    
+00000560: 3c2f 673e 0a20 2020 203c 6720 6964 3d22  </g>.    <g id="
+00000570: 6c6f 676f 2d73 6861 646f 7722 2073 6572  logo-shadow" ser
+00000580: 6966 3a69 643d 226c 6f67 6f20 7368 6164  if:id="logo shad
+00000590: 6f77 2220 7472 616e 7366 6f72 6d3d 226d  ow" transform="m
+000005a0: 6174 7269 7828 302e 3835 3438 3736 2c30  atrix(0.854876,0
+000005b0: 2c30 2c30 2e38 3534 3837 362c 2d36 2e37  ,0,0.854876,-6.7
+000005c0: 3335 3134 2c31 2e37 3332 2922 3e0a 2020  3514,1.732)">.  
+000005d0: 2020 2020 2020 3c67 2074 7261 6e73 666f        <g transfo
+000005e0: 726d 3d22 6d61 7472 6978 2830 2e32 3939  rm="matrix(0.299
+000005f0: 3031 322c 302c 302c 302e 3239 3930 3132  012,0,0,0.299012
+00000600: 2c39 2e37 3032 3239 2c2d 362e 3638 3538  ,9.70229,-6.6858
+00000610: 3229 223e 0a20 2020 2020 2020 2020 2020  2)">.           
+00000620: 203c 7061 7468 2064 3d22 4d35 302c 3634   <path d="M50,64
+00000630: 2e32 3543 3532 2e37 362c 3634 2e32 3520  .25C52.76,64.25 
+00000640: 3535 2c36 312e 3133 2035 352c 3539 2e37  55,61.13 55,59.7
+00000650: 3543 3535 2c35 382e 3337 2035 322e 3736  5C55,58.37 52.76
+00000660: 2c35 372e 3235 2035 302c 3537 2e32 3543  ,57.25 50,57.25C
+00000670: 3437 2e32 342c 3537 2e32 3520 3435 2c35  47.24,57.25 45,5
+00000680: 382e 3337 2034 352c 3539 2e37 3543 3435  8.37 45,59.75C45
+00000690: 2c36 312e 3133 2034 372e 3234 2c36 342e  ,61.13 47.24,64.
+000006a0: 3235 2035 302c 3634 2e32 355a 2220 7374  25 50,64.25Z" st
+000006b0: 796c 653d 2266 696c 6c3a 7267 6228 312c  yle="fill:rgb(1,
+000006c0: 312c 3129 3b66 696c 6c2d 6f70 6163 6974  1,1);fill-opacit
+000006d0: 793a 302e 333b 6669 6c6c 2d72 756c 653a  y:0.3;fill-rule:
+000006e0: 6e6f 6e7a 6572 6f3b 222f 3e0a 2020 2020  nonzero;"/>.    
+000006f0: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+00000700: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
+00000710: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
+00000720: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
+00000730: 3232 392c 2d36 2e36 3835 3832 2922 3e0a  229,-6.68582)">.
+00000740: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+00000750: 6820 643d 224d 3838 2c34 392e 3035 4338  h d="M88,49.05C8
+00000760: 362e 3530 362c 3433 2e34 3735 2038 332e  6.506,43.475 83.
+00000770: 3031 382c 3338 2e36 3338 2037 382e 322c  018,38.638 78.2,
+00000780: 3335 2e34 3643 3732 2e39 3639 2c33 322e  35.46C72.969,32.
+00000790: 3030 3220 3636 2e35 3339 2c33 302e 3834  002 66.539,30.84
+000007a0: 3420 3630 2e34 332c 3332 2e32 3643 3536  4 60.43,32.26C56
+000007b0: 2e35 3736 2c33 332e 3134 3520 3532 2e39  .576,33.145 52.9
+000007c0: 3935 2c33 342e 3935 3820 3530 2c33 372e  95,34.958 50,37.
+000007d0: 3534 4334 362e 3939 382c 3334 2e39 3538  54C46.998,34.958
+000007e0: 2034 332e 3431 312c 3333 2e31 3439 2033   43.411,33.149 3
+000007f0: 392e 3535 2c33 322e 3237 4333 332e 3434  9.55,32.27C33.44
+00000800: 312c 3330 2e38 3533 2032 372e 3031 312c  1,30.853 27.011,
+00000810: 3332 2e30 3131 2032 312e 3738 2c33 352e  32.011 21.78,35.
+00000820: 3437 4331 362e 3937 2c33 382e 3635 3220  47C16.97,38.652 
+00000830: 3133 2e34 3839 2c34 332e 3438 3920 3132  13.489,43.489 12
+00000840: 2c34 392e 3036 4c31 322c 3439 2e31 3343  ,49.06L12,49.13C
+00000850: 3131 2e38 322c 3439 2e37 3920 3131 2e36  11.82,49.79 11.6
+00000860: 362c 3530 2e34 3620 3131 2e35 332c 3531  6,50.46 11.53,51
+00000870: 2e31 3343 3131 2e31 3436 2c35 332e 3230  .13C11.146,53.20
+00000880: 3720 3131 2e30 3231 2c35 352e 3332 3320  7 11.021,55.323 
+00000890: 3131 2e31 362c 3537 2e34 3343 3131 2e31  11.16,57.43C11.1
+000008a0: 362c 3538 2e30 3320 3131 2e32 362c 3538  6,58.03 11.26,58
+000008b0: 2e36 3320 3131 2e33 342c 3539 2e32 3343  .63 11.34,59.23C
+000008c0: 3131 2e33 342c 3539 2e35 3120 3131 2e34  11.34,59.51 11.4
+000008d0: 332c 3539 2e37 3920 3131 2e34 382c 3630  3,59.79 11.48,60
+000008e0: 2e30 3743 3131 2e35 332c 3630 2e33 3520  .07C11.53,60.35 
+000008f0: 3131 2e35 382c 3630 2e36 3820 3131 2e36  11.58,60.68 11.6
+00000900: 342c 3630 2e39 3843 3131 2e37 2c36 312e  4,60.98C11.7,61.
+00000910: 3238 2031 312e 382c 3631 2e36 3920 3131  28 11.8,61.69 11
+00000920: 2e38 392c 3632 2e30 3543 3131 2e39 382c  .89,62.05C11.98,
+00000930: 3632 2e34 3120 3131 2e39 392c 3632 2e34  62.41 11.99,62.4
+00000940: 3720 3132 2e30 352c 3632 2e36 3843 3132  7 12.05,62.68C12
+00000950: 2e31 362c 3633 2e30 3720 3132 2e32 382c  .16,63.07 12.28,
+00000960: 3633 2e34 3620 3132 2e34 312c 3633 2e38  63.46 12.41,63.8
+00000970: 344c 3132 2e35 382c 3634 2e33 3443 3132  4L12.58,64.34C12
+00000980: 2e37 322c 3634 2e37 3420 3132 2e38 382c  .72,64.74 12.88,
+00000990: 3635 2e31 3420 3133 2e30 342c 3635 2e35  65.14 13.04,65.5
+000009a0: 334c 3133 2e32 332c 3635 2e39 3843 3133  3L13.23,65.98C13
+000009b0: 2e34 3033 2c36 362e 3337 3320 3133 2e35  .403,66.373 13.5
+000009c0: 3833 2c36 362e 3736 3720 3133 2e37 372c  83,66.767 13.77,
+000009d0: 3637 2e31 364c 3133 2e39 392c 3637 2e35  67.16L13.99,67.5
+000009e0: 3943 3134 2e31 392c 3637 2e39 3720 3134  9C14.19,67.97 14
+000009f0: 2e33 392c 3638 2e33 3520 3134 2e36 312c  .39,68.35 14.61,
+00000a00: 3638 2e37 334c 3134 2e38 372c 3639 2e31  68.73L14.87,69.1
+00000a10: 3543 3135 2e31 2c36 392e 3532 2031 352e  5C15.1,69.52 15.
+00000a20: 3333 2c36 392e 3839 2031 352e 3538 2c37  33,69.89 15.58,7
+00000a30: 302e 3236 4c31 352e 3538 2c37 302e 3332  0.26L15.58,70.32
+00000a40: 4c31 352e 3939 2c37 302e 3933 4331 362e  L15.99,70.93C16.
+00000a50: 3134 2c37 312e 3134 2031 362e 3239 2c37  14,71.14 16.29,7
+00000a60: 312e 3336 2031 362e 3435 2c37 312e 3537  1.36 16.45,71.57
+00000a70: 4332 302e 3230 362c 3735 2e38 3320 3235  C20.206,75.83 25
+00000a80: 2e30 3836 2c37 382e 3935 2033 302e 3533  .086,78.95 30.53
+00000a90: 2c38 302e 3537 4333 362e 3833 392c 3832  ,80.57C36.839,82
+00000aa0: 2e34 3820 3433 2e34 312c 3833 2e33 3835  .48 43.41,83.385
+00000ab0: 2035 302c 3833 2e32 3543 3536 2e35 3939   50,83.25C56.599
+00000ac0: 2c38 332e 3337 3420 3633 2e31 3737 2c38  ,83.374 63.177,8
+00000ad0: 322e 3435 3620 3639 2e34 392c 3830 2e35  2.456 69.49,80.5
+00000ae0: 3343 3734 2e36 3434 2c37 382e 3937 3820  3C74.644,78.978 
+00000af0: 3739 2e33 3033 2c37 362e 3130 3220 3833  79.303,76.102 83
+00000b00: 2c37 322e 3139 4338 332e 3334 2c37 312e  ,72.19C83.34,71.
+00000b10: 3738 2038 332e 3635 2c37 312e 3335 2038  78 83.65,71.35 8
+00000b20: 342c 3730 2e39 324c 3834 2e31 382c 3730  4,70.92L84.18,70
+00000b30: 2e36 364c 3834 2e33 332c 3730 2e34 344c  .66L84.33,70.44L
+00000b40: 3834 2e34 312c 3730 2e33 3243 3834 2e35  84.41,70.32C84.5
+00000b50: 352c 3730 2e31 3220 3834 2e36 372c 3639  5,70.12 84.67,69
+00000b60: 2e39 2038 342e 3831 2c36 392e 3743 3835  .9 84.81,69.7C85
+00000b70: 2e30 372c 3639 2e33 2038 352e 3332 2c36  .07,69.3 85.32,6
+00000b80: 382e 3839 2038 352e 3535 2c36 382e 3438  8.89 85.55,68.48
+00000b90: 4338 352e 3738 2c36 382e 3037 2038 362e  C85.78,68.07 86.
+00000ba0: 3032 2c36 372e 3635 2038 362e 3233 2c36  02,67.65 86.23,6
+00000bb0: 372e 3232 4338 362e 3331 2c36 372e 3035  7.22C86.31,67.05
+00000bc0: 2038 362e 3339 2c36 362e 3838 2038 362e   86.39,66.88 86.
+00000bd0: 3437 2c36 362e 3743 3836 2e36 372c 3636  47,66.7C86.67,66
+00000be0: 2e32 3820 3836 2e38 352c 3635 2e38 3720  .28 86.85,65.87 
+00000bf0: 3837 2e30 332c 3635 2e34 344c 3837 2e32  87.03,65.44L87.2
+00000c00: 332c 3634 2e39 3243 3837 2e33 3937 2c36  3,64.92C87.397,6
+00000c10: 342e 3438 3720 3837 2e35 352c 3634 2e30  4.487 87.55,64.0
+00000c20: 3520 3837 2e36 392c 3633 2e36 314c 3837  5 87.69,63.61L87
+00000c30: 2e38 352c 3633 2e30 3943 3837 2e39 382c  .85,63.09C87.98,
+00000c40: 3632 2e36 3420 3838 2e31 2c36 322e 3139  62.64 88.1,62.19
+00000c50: 2038 382e 3231 2c36 312e 3734 4338 382e   88.21,61.74C88.
+00000c60: 3231 2c36 312e 3537 2038 382e 332c 3631  21,61.57 88.3,61
+00000c70: 2e33 3920 3838 2e33 332c 3631 2e32 3243  .39 88.33,61.22C
+00000c80: 3838 2e34 332c 3630 2e37 3520 3838 2e35  88.43,60.75 88.5
+00000c90: 322c 3630 2e32 3220 3838 2e36 2c35 392e  2,60.22 88.6,59.
+00000ca0: 3739 4338 382e 362c 3539 2e36 3420 3838  79C88.6,59.64 88
+00000cb0: 2e36 362c 3539 2e34 3920 3838 2e36 382c  .66,59.49 88.68,
+00000cc0: 3539 2e33 3343 3838 2e37 372c 3538 2e37  59.33C88.77,58.7
+00000cd0: 3120 3838 2e38 342c 3538 2e30 3820 3838  1 88.84,58.08 88
+00000ce0: 2e38 382c 3537 2e34 354c 3838 2e38 382c  .88,57.45L88.88,
+00000cf0: 3534 2e31 3743 3838 2e38 3137 2c35 332e  54.17C88.817,53.
+00000d00: 3136 3420 3838 2e36 3933 2c35 322e 3136  164 88.693,52.16
+00000d10: 3220 3838 2e35 312c 3531 2e31 3743 3838  2 88.51,51.17C88
+00000d20: 2e33 382c 3530 2e35 2038 382e 3233 2c34  .38,50.5 88.23,4
+00000d30: 392e 3834 2038 382e 3035 2c34 392e 3137  9.84 88.05,49.17
+00000d40: 4c38 382c 3439 2e30 355a 4d38 352e 3839  L88,49.05ZM85.89
+00000d50: 2c35 362e 3434 4c38 352e 3839 2c35 372e  ,56.44L85.89,57.
+00000d60: 3233 4338 352e 3839 2c35 372e 3738 2038  23C85.89,57.78 8
+00000d70: 352e 3739 2c35 382e 3332 2038 352e 3732  5.79,58.32 85.72
+00000d80: 2c35 382e 3836 4338 352e 3732 2c35 392e  ,58.86C85.72,59.
+00000d90: 3031 2038 352e 3732 2c35 392e 3135 2038  01 85.72,59.15 8
+00000da0: 352e 3635 2c35 392e 3343 3835 2e35 392c  5.65,59.3C85.59,
+00000db0: 3539 2e37 2038 352e 3531 2c36 302e 3131  59.7 85.51,60.11
+00000dc0: 2038 352e 3433 2c36 302e 3531 4c38 352e   85.43,60.51L85.
+00000dd0: 3332 2c36 302e 3939 4338 352e 3233 2c36  32,60.99C85.23,6
+00000de0: 312e 3338 2038 352e 3132 2c36 312e 3737  1.38 85.12,61.77
+00000df0: 2038 352e 3031 2c36 322e 3136 4338 352e   85.01,62.16C85.
+00000e00: 3031 2c36 322e 3331 2038 342e 3933 2c36  01,62.31 84.93,6
+00000e10: 322e 3436 2038 342e 3838 2c36 322e 3643  2.46 84.88,62.6C
+00000e20: 3834 2e37 342c 3633 2e30 3420 3834 2e35  84.74,63.04 84.5
+00000e30: 392c 3633 2e34 3720 3834 2e34 322c 3633  9,63.47 84.42,63
+00000e40: 2e39 4c38 342e 3237 2c36 342e 3238 4338  .9L84.27,64.28C8
+00000e50: 342e 312c 3634 2e37 3120 3833 2e39 312c  4.1,64.71 83.91,
+00000e60: 3635 2e31 3420 3833 2e37 312c 3635 2e35  65.14 83.71,65.5
+00000e70: 3643 3833 2e35 312c 3635 2e39 3820 3833  6C83.51,65.98 83
+00000e80: 2e34 332c 3636 2e31 3220 3833 2e32 382c  .43,66.12 83.28,
+00000e90: 3636 2e34 4c38 332e 3031 2c36 362e 3931  66.4L83.01,66.91
+00000ea0: 4338 322e 3833 2c36 372e 3232 3320 3832  C82.83,67.223 82
+00000eb0: 2e36 3433 2c36 372e 3533 3720 3832 2e34  .643,67.537 82.4
+00000ec0: 352c 3637 2e38 354c 3832 2e33 352c 3638  5,67.85L82.35,68
+00000ed0: 2e30 3143 3739 2e31 3231 2c36 382e 3034  .01C79.121,68.04
+00000ee0: 3720 3735 2e39 3138 2c36 372e 3433 3420  7 75.918,67.434 
+00000ef0: 3732 2e39 332c 3636 2e32 3143 3634 2e32  72.93,66.21C64.2
+00000f00: 372c 3632 2e37 3420 3539 2c35 352e 3532  7,62.74 59,55.52
+00000f10: 2036 312e 3138 2c35 302e 3131 4336 322e   61.18,50.11C62.
+00000f20: 3138 2c34 372e 3620 3634 2e37 2c34 352e  18,47.6 64.7,45.
+00000f30: 3832 2036 382e 3236 2c34 352e 3131 4337  82 68.26,45.11C7
+00000f40: 322e 3438 392c 3434 2e33 3935 2037 362e  2.489,44.395 76.
+00000f50: 3833 352c 3434 2e39 3038 2038 302e 3738  835,44.908 80.78
+00000f60: 2c34 362e 3539 4338 322e 3134 312c 3437  ,46.59C82.141,47
+00000f70: 2e31 3434 2038 332e 3435 332c 3437 2e38  .144 83.453,47.8
+00000f80: 3133 2038 342e 372c 3438 2e35 3943 3834  13 84.7,48.59C84
+00000f90: 2e37 362c 3438 2e37 3620 3834 2e38 322c  .76,48.76 84.82,
+00000fa0: 3438 2e39 3320 3834 2e38 382c 3439 2e31  48.93 84.88,49.1
+00000fb0: 4338 342e 3934 2c34 392e 3237 2038 352e  C84.94,49.27 85.
+00000fc0: 3035 2c34 392e 3633 2038 352e 3132 2c34  05,49.63 85.12,4
+00000fd0: 392e 3943 3835 2e32 382c 3530 2e35 2038  9.9C85.28,50.5 8
+00000fe0: 352e 3434 2c35 312e 3120 3835 2e35 352c  5.44,51.1 85.55,
+00000ff0: 3531 2e37 3343 3835 2e36 3931 2c35 322e  51.73C85.691,52.
+00001000: 3530 3720 3835 2e37 3932 2c35 332e 3239  507 85.792,53.29
+00001010: 3220 3835 2e38 352c 3534 2e30 384c 3835  2 85.85,54.08L85
+00001020: 2e38 352c 3535 2e38 3943 3835 2e38 352c  .85,55.89C85.85,
+00001030: 3536 2e31 3220 3835 2e39 312c 3536 2e32  56.12 85.91,56.2
+00001040: 3520 3835 2e39 312c 3536 2e34 354c 3835  5 85.91,56.45L85
+00001050: 2e38 392c 3536 2e34 345a 4d31 372e 3636  .89,56.44ZM17.66
+00001060: 2c36 3843 3136 2e36 3638 2c36 362e 3433  ,68C16.668,66.43
+00001070: 3520 3135 2e38 3639 2c36 342e 3735 3620  5 15.869,64.756 
+00001080: 3135 2e32 382c 3633 4c31 352e 3137 2c36  15.28,63L15.17,6
+00001090: 322e 3638 4331 352e 3036 2c36 322e 3335  2.68C15.06,62.35
+000010a0: 2031 342e 3936 2c36 322e 3031 2031 342e   14.96,62.01 14.
+000010b0: 3837 2c36 312e 3638 4331 342e 3832 332c  87,61.68C14.823,
+000010c0: 3631 2e34 3933 2031 342e 3737 372c 3631  61.493 14.777,61
+000010d0: 2e33 3120 3134 2e37 332c 3631 2e31 3343  .31 14.73,61.13C
+000010e0: 3134 2e36 362c 3630 2e38 3420 3134 2e35  14.66,60.84 14.5
+000010f0: 392c 3630 2e35 3520 3134 2e35 332c 3630  9,60.55 14.53,60
+00001100: 2e32 3743 3134 2e34 372c 3539 2e39 3920  .27C14.47,59.99 
+00001110: 3134 2e34 332c 3539 2e37 3220 3134 2e33  14.43,59.72 14.3
+00001120: 382c 3539 2e34 3443 3134 2e33 332c 3539  8,59.44C14.33,59
+00001130: 2e31 3620 3134 2e33 2c35 3920 3134 2e32  .16 14.3,59 14.2
+00001140: 372c 3538 2e37 3843 3134 2e32 2c35 382e  7,58.78C14.2,58.
+00001150: 3237 2031 342e 3135 2c35 372e 3738 2031  27 14.15,57.78 1
+00001160: 342e 3131 2c35 372e 3233 4c31 342e 3131  4.11,57.23L14.11
+00001170: 2c35 372e 3033 4331 342e 3030 382c 3535  ,57.03C14.008,55
+00001180: 2e32 3336 2031 342e 3132 322c 3533 2e34  .236 14.122,53.4
+00001190: 3337 2031 342e 3435 2c35 312e 3637 4331  37 14.45,51.67C1
+000011a0: 342e 3536 2c35 312e 3036 2031 342e 3731  4.56,51.06 14.71
+000011b0: 2c35 302e 3436 2031 342e 3838 2c34 392e  ,50.46 14.88,49.
+000011c0: 3837 4331 342e 3936 2c34 392e 3539 2031  87C14.96,49.59 1
+000011d0: 352e 3034 2c34 392e 3332 2031 352e 3133  5.04,49.32 15.13
+000011e0: 2c34 392e 3035 4331 352e 3232 2c34 382e  ,49.05C15.22,48.
+000011f0: 3738 2031 352e 3234 2c34 382e 3732 2031  78 15.24,48.72 1
+00001200: 352e 332c 3438 2e35 3543 3136 2e35 3438  5.3,48.55C16.548
+00001210: 2c34 372e 3737 3420 3137 2e38 3539 2c34  ,47.774 17.859,4
+00001220: 372e 3130 3520 3139 2e32 322c 3436 2e35  7.105 19.22,46.5
+00001230: 3543 3237 2e38 362c 3433 2e30 3920 3336  5C27.86,43.09 36
+00001240: 2e36 352c 3434 2e36 3720 3338 2e38 322c  .65,44.67 38.82,
+00001250: 3530 2e30 3843 3430 2e39 392c 3535 2e34  50.08C40.99,55.4
+00001260: 3920 3335 2e37 332c 3632 2e37 3420 3237  9 35.73,62.74 27
+00001270: 2e30 392c 3636 2e32 4332 342e 3130 312c  .09,66.2C24.101,
+00001280: 3637 2e34 3331 2032 302e 3839 332c 3638  67.431 20.893,68
+00001290: 2e30 3433 2031 372e 3636 2c36 385a 4d36  .043 17.66,68ZM6
+000012a0: 382e 3537 2c37 372e 3638 4336 322e 3535  8.57,77.68C62.55
+000012b0: 342c 3739 2e35 3038 2035 362e 3238 372c  4,79.508 56.287,
+000012c0: 3830 2e33 3736 2035 302c 3830 2e32 3543  80.376 50,80.25C
+000012d0: 3433 2e37 3337 2c38 302e 3337 2033 372e  43.737,80.37 37.
+000012e0: 3439 352c 3739 2e35 3036 2033 312e 352c  495,79.506 31.5,
+000012f0: 3737 2e36 3943 3237 2e31 3835 2c37 362e  77.69C27.185,76.
+00001300: 3338 2032 332e 3234 332c 3734 2e30 3632  38 23.243,74.062
+00001310: 2032 302c 3730 2e39 3343 3232 2e38 3135   20,70.93C22.815
+00001320: 2c37 302e 3730 3620 3235 2e35 382c 3730  ,70.706 25.58,70
+00001330: 2e30 3535 2032 382e 322c 3639 4333 382e  .055 28.2,69C38.
+00001340: 3337 2c36 342e 3932 2034 342e 3339 2c35  37,64.92 44.39,5
+00001350: 3620 3431 2e36 2c34 3943 3338 2e38 312c  6 41.6,49C38.81,
+00001360: 3432 2032 382e 3237 2c33 392e 3732 2031  42 28.27,39.72 1
+00001370: 382e 312c 3433 2e38 4c31 372e 3433 2c34  8.1,43.8L17.43,4
+00001380: 342e 3039 4331 382e 3937 332c 3431 2e36  4.09C18.973,41.6
+00001390: 3438 2032 312e 3031 392c 3339 2e35 3631  48 21.019,39.561
+000013a0: 2032 332e 3433 2c33 372e 3937 4332 362e   23.43,37.97C26.
+000013b0: 3637 312c 3335 2e38 3234 2033 302e 3437  671,35.824 30.47
+000013c0: 332c 3334 2e36 3820 3334 2e33 362c 3334  3,34.68 34.36,34
+000013d0: 2e36 3843 3335 2e38 3834 2c33 342e 3638  .68C35.884,34.68
+000013e0: 3120 3337 2e34 3034 2c33 342e 3835 3220  1 37.404,34.852 
+000013f0: 3338 2e38 392c 3335 2e31 3943 3432 2e36  38.89,35.19C42.6
+00001400: 3934 2c33 362e 3034 3920 3436 2e31 3931  94,36.049 46.191
+00001410: 2c33 372e 3933 3520 3439 2c34 302e 3634  ,37.935 49,40.64
+00001420: 4c35 302c 3431 2e36 344c 3531 2c34 302e  L50,41.64L51,40.
+00001430: 3634 4335 332e 3739 372c 3337 2e39 3337  64C53.797,37.937
+00001440: 2035 372e 3237 392c 3336 2e30 3439 2036   57.279,36.049 6
+00001450: 312e 3037 2c33 352e 3138 4336 362e 3430  1.07,35.18C66.40
+00001460: 322c 3333 2e39 3437 2037 322e 3031 342c  2,33.947 72.014,
+00001470: 3334 2e39 3638 2037 362e 3537 2c33 3843  34.968 76.57,38C
+00001480: 3738 2e39 382c 3339 2e35 3838 2038 312e  78.98,39.588 81.
+00001490: 3032 362c 3431 2e36 3731 2038 322e 3537  026,41.671 82.57
+000014a0: 2c34 342e 3131 4c38 312e 392c 3433 2e38  ,44.11L81.9,43.8
+000014b0: 3243 3737 2e34 3039 2c34 312e 3932 3120  2C77.409,41.921 
+000014c0: 3732 2e34 3634 2c34 312e 3335 3520 3637  72.464,41.355 67
+000014d0: 2e36 362c 3432 2e31 3943 3633 2e30 382c  .66,42.19C63.08,
+000014e0: 3433 2e31 3220 3539 2e37 392c 3435 2e35  43.12 59.79,45.5
+000014f0: 3420 3538 2e33 392c 3439 2e30 3243 3535  4 58.39,49.02C55
+00001500: 2e36 2c35 352e 3937 2036 312e 3632 2c36  .6,55.97 61.62,6
+00001510: 342e 3934 2037 312e 3739 2c36 392e 3032  4.94 71.79,69.02
+00001520: 4337 342e 3431 342c 3730 2e30 3720 3737  C74.414,70.07 77
+00001530: 2e31 3832 2c37 302e 3731 3420 3830 2c37  .182,70.714 80,7
+00001540: 302e 3933 4337 362e 3737 362c 3734 2e30  0.93C76.776,74.0
+00001550: 3520 3732 2e38 3539 2c37 362e 3336 3320  5 72.859,76.363 
+00001560: 3638 2e35 372c 3737 2e36 385a 2220 7374  68.57,77.68Z" st
+00001570: 796c 653d 2266 696c 6c3a 7267 6228 312c  yle="fill:rgb(1,
+00001580: 312c 3129 3b66 696c 6c2d 6f70 6163 6974  1,1);fill-opacit
+00001590: 793a 302e 333b 6669 6c6c 2d72 756c 653a  y:0.3;fill-rule:
+000015a0: 6e6f 6e7a 6572 6f3b 222f 3e0a 2020 2020  nonzero;"/>.    
+000015b0: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+000015c0: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
+000015d0: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
+000015e0: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
+000015f0: 3232 392c 2d36 2e36 3835 3832 2922 3e0a  229,-6.68582)">.
+00001600: 2020 2020 2020 2020 2020 2020 3c63 6972              <cir
+00001610: 636c 6520 6378 3d22 3731 2e33 3322 2063  cle cx="71.33" c
+00001620: 793d 2235 3622 2072 3d22 352e 3136 2220  y="56" r="5.16" 
+00001630: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+00001640: 312c 312c 3129 3b66 696c 6c2d 6f70 6163  1,1,1);fill-opac
+00001650: 6974 793a 302e 333b 222f 3e0a 2020 2020  ity:0.3;"/>.    
+00001660: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+00001670: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
+00001680: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
+00001690: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
+000016a0: 3232 392c 2d36 2e36 3835 3832 2922 3e0a  229,-6.68582)">.
+000016b0: 2020 2020 2020 2020 2020 2020 3c63 6972              <cir
+000016c0: 636c 6520 6378 3d22 3238 2e36 3722 2063  cle cx="28.67" c
+000016d0: 793d 2235 3622 2072 3d22 352e 3136 2220  y="56" r="5.16" 
+000016e0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+000016f0: 312c 312c 3129 3b66 696c 6c2d 6f70 6163  1,1,1);fill-opac
+00001700: 6974 793a 302e 333b 222f 3e0a 2020 2020  ity:0.3;"/>.    
+00001710: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+00001720: 203c 6720 7472 616e 7366 6f72 6d3d 226d   <g transform="m
+00001730: 6174 7269 7828 302e 3239 3930 3132 2c30  atrix(0.299012,0
+00001740: 2c30 2c30 2e32 3939 3031 322c 392e 3730  ,0,0.299012,9.70
+00001750: 3232 392c 2d36 2e36 3835 3832 2922 3e0a  229,-6.68582)">.
+00001760: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+00001770: 6820 643d 224d 3538 2c36 3643 3535 2e39  h d="M58,66C55.9
+00001780: 3132 2c36 382e 3136 3120 3533 2e30 3033  12,68.161 53.003
+00001790: 2c36 392e 3333 3920 3530 2c36 392e 3234  ,69.339 50,69.24
+000017a0: 4334 362e 3939 372c 3639 2e33 3339 2034  C46.997,69.339 4
+000017b0: 342e 3038 382c 3638 2e31 3631 2034 322c  4.088,68.161 42,
+000017c0: 3636 4334 312e 3731 342c 3635 2e36 3737  66C41.714,65.677
+000017d0: 2034 312e 3330 322c 3635 2e34 3931 2034   41.302,65.491 4
+000017e0: 302e 3837 2c36 352e 3439 3143 3430 2e30  0.87,65.491C40.0
+000017f0: 3432 2c36 352e 3439 3120 3339 2e33 3631  42,65.491 39.361
+00001800: 2c36 362e 3137 3220 3339 2e33 3631 2c36  ,66.172 39.361,6
+00001810: 3743 3339 2e33 3631 2c36 372e 3336 3820  7C39.361,67.368 
+00001820: 3339 2e34 3936 2c36 372e 3732 3420 3339  39.496,67.724 39
+00001830: 2e37 342c 3638 4334 322e 3430 332c 3730  .74,68C42.403,70
+00001840: 2e38 3034 2034 362e 3133 342c 3732 2e33  .804 46.134,72.3
+00001850: 3520 3530 2c37 322e 3235 4335 332e 3836  5 50,72.25C53.86
+00001860: 322c 3732 2e33 3437 2035 372e 3539 2c37  2,72.347 57.59,7
+00001870: 302e 3830 3220 3630 2e32 352c 3638 4336  0.802 60.25,68C6
+00001880: 302e 3439 352c 3637 2e37 3235 2036 302e  0.495,67.725 60.
+00001890: 3633 2c36 372e 3336 3920 3630 2e36 332c  63,67.369 60.63,
+000018a0: 3637 4336 302e 3633 2c36 362e 3137 3420  67C60.63,66.174 
+000018b0: 3539 2e39 3531 2c36 352e 3439 3520 3539  59.951,65.495 59
+000018c0: 2e31 3235 2c36 352e 3439 3543 3538 2e36  .125,65.495C58.6
+000018d0: 3935 2c36 352e 3439 3520 3538 2e32 3835  95,65.495 58.285
+000018e0: 2c36 352e 3637 3920 3538 2c36 365a 2220  ,65.679 58,66Z" 
+000018f0: 7374 796c 653d 2266 696c 6c3a 7267 6228  style="fill:rgb(
+00001900: 312c 312c 3129 3b66 696c 6c2d 6f70 6163  1,1,1);fill-opac
+00001910: 6974 793a 302e 333b 6669 6c6c 2d72 756c  ity:0.3;fill-rul
+00001920: 653a 6e6f 6e7a 6572 6f3b 222f 3e0a 2020  e:nonzero;"/>.  
+00001930: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
+00001940: 2f67 3e0a 2020 2020 3c67 2069 643d 226c  /g>.    <g id="l
+00001950: 6f67 6f2d 7069 6e6b 2220 7365 7269 663a  ogo-pink" serif:
+00001960: 6964 3d22 6c6f 676f 2070 696e 6b22 2074  id="logo pink" t
+00001970: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00001980: 2830 2e38 3534 3837 362c 302c 302c 302e  (0.854876,0,0,0.
+00001990: 3835 3438 3736 2c2d 362e 3733 3531 342c  854876,-6.73514,
+000019a0: 302e 3837 3731 3234 2922 3e0a 2020 2020  0.877124)">.    
+000019b0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+000019c0: 3d22 6d61 7472 6978 2830 2e32 3939 3031  ="matrix(0.29901
+000019d0: 322c 302c 302c 302e 3239 3930 3132 2c39  2,0,0,0.299012,9
+000019e0: 2e37 3032 3239 2c2d 362e 3638 3538 3229  .70229,-6.68582)
+000019f0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00001a00: 7061 7468 2064 3d22 4d35 302c 3634 2e32  path d="M50,64.2
+00001a10: 3543 3532 2e37 362c 3634 2e32 3520 3535  5C52.76,64.25 55
+00001a20: 2c36 312e 3133 2035 352c 3539 2e37 3543  ,61.13 55,59.75C
+00001a30: 3535 2c35 382e 3337 2035 322e 3736 2c35  55,58.37 52.76,5
+00001a40: 372e 3235 2035 302c 3537 2e32 3543 3437  7.25 50,57.25C47
+00001a50: 2e32 342c 3537 2e32 3520 3435 2c35 382e  .24,57.25 45,58.
+00001a60: 3337 2034 352c 3539 2e37 3543 3435 2c36  37 45,59.75C45,6
+00001a70: 312e 3133 2034 372e 3234 2c36 342e 3235  1.13 47.24,64.25
+00001a80: 2035 302c 3634 2e32 355a 2220 7374 796c   50,64.25Z" styl
+00001a90: 653d 2266 696c 6c3a 7267 6228 3232 322c  e="fill:rgb(222,
+00001aa0: 3132 302c 3136 3029 3b66 696c 6c2d 7275  120,160);fill-ru
+00001ab0: 6c65 3a6e 6f6e 7a65 726f 3b22 2f3e 0a20  le:nonzero;"/>. 
+00001ac0: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
+00001ad0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+00001ae0: 3d22 6d61 7472 6978 2830 2e32 3939 3031  ="matrix(0.29901
+00001af0: 322c 302c 302c 302e 3239 3930 3132 2c39  2,0,0,0.299012,9
+00001b00: 2e37 3032 3239 2c2d 362e 3638 3538 3229  .70229,-6.68582)
+00001b10: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00001b20: 7061 7468 2064 3d22 4d38 382c 3439 2e30  path d="M88,49.0
+00001b30: 3543 3836 2e35 3036 2c34 332e 3437 3520  5C86.506,43.475 
+00001b40: 3833 2e30 3138 2c33 382e 3633 3820 3738  83.018,38.638 78
+00001b50: 2e32 2c33 352e 3436 4337 322e 3936 392c  .2,35.46C72.969,
+00001b60: 3332 2e30 3032 2036 362e 3533 392c 3330  32.002 66.539,30
+00001b70: 2e38 3434 2036 302e 3433 2c33 322e 3236  .844 60.43,32.26
+00001b80: 4335 362e 3537 362c 3333 2e31 3435 2035  C56.576,33.145 5
+00001b90: 322e 3939 352c 3334 2e39 3538 2035 302c  2.995,34.958 50,
+00001ba0: 3337 2e35 3443 3436 2e39 3938 2c33 342e  37.54C46.998,34.
+00001bb0: 3935 3820 3433 2e34 3131 2c33 332e 3134  958 43.411,33.14
+00001bc0: 3920 3339 2e35 352c 3332 2e32 3743 3333  9 39.55,32.27C33
+00001bd0: 2e34 3431 2c33 302e 3835 3320 3237 2e30  .441,30.853 27.0
+00001be0: 3131 2c33 322e 3031 3120 3231 2e37 382c  11,32.011 21.78,
+00001bf0: 3335 2e34 3743 3136 2e39 372c 3338 2e36  35.47C16.97,38.6
+00001c00: 3532 2031 332e 3438 392c 3433 2e34 3839  52 13.489,43.489
+00001c10: 2031 322c 3439 2e30 364c 3132 2c34 392e   12,49.06L12,49.
+00001c20: 3133 4331 312e 3832 2c34 392e 3739 2031  13C11.82,49.79 1
+00001c30: 312e 3636 2c35 302e 3436 2031 312e 3533  1.66,50.46 11.53
+00001c40: 2c35 312e 3133 4331 312e 3134 362c 3533  ,51.13C11.146,53
+00001c50: 2e32 3037 2031 312e 3032 312c 3535 2e33  .207 11.021,55.3
+00001c60: 3233 2031 312e 3136 2c35 372e 3433 4331  23 11.16,57.43C1
+00001c70: 312e 3136 2c35 382e 3033 2031 312e 3236  1.16,58.03 11.26
+00001c80: 2c35 382e 3633 2031 312e 3334 2c35 392e  ,58.63 11.34,59.
+00001c90: 3233 4331 312e 3334 2c35 392e 3531 2031  23C11.34,59.51 1
+00001ca0: 312e 3433 2c35 392e 3739 2031 312e 3438  1.43,59.79 11.48
+00001cb0: 2c36 302e 3037 4331 312e 3533 2c36 302e  ,60.07C11.53,60.
+00001cc0: 3335 2031 312e 3538 2c36 302e 3638 2031  35 11.58,60.68 1
+00001cd0: 312e 3634 2c36 302e 3938 4331 312e 372c  1.64,60.98C11.7,
+00001ce0: 3631 2e32 3820 3131 2e38 2c36 312e 3639  61.28 11.8,61.69
+00001cf0: 2031 312e 3839 2c36 322e 3035 4331 312e   11.89,62.05C11.
+00001d00: 3938 2c36 322e 3431 2031 312e 3939 2c36  98,62.41 11.99,6
+00001d10: 322e 3437 2031 322e 3035 2c36 322e 3638  2.47 12.05,62.68
+00001d20: 4331 322e 3136 2c36 332e 3037 2031 322e  C12.16,63.07 12.
+00001d30: 3238 2c36 332e 3436 2031 322e 3431 2c36  28,63.46 12.41,6
+00001d40: 332e 3834 4c31 322e 3538 2c36 342e 3334  3.84L12.58,64.34
+00001d50: 4331 322e 3732 2c36 342e 3734 2031 322e  C12.72,64.74 12.
+00001d60: 3838 2c36 352e 3134 2031 332e 3034 2c36  88,65.14 13.04,6
+00001d70: 352e 3533 4c31 332e 3233 2c36 352e 3938  5.53L13.23,65.98
+00001d80: 4331 332e 3430 332c 3636 2e33 3733 2031  C13.403,66.373 1
+00001d90: 332e 3538 332c 3636 2e37 3637 2031 332e  3.583,66.767 13.
+00001da0: 3737 2c36 372e 3136 4c31 332e 3939 2c36  77,67.16L13.99,6
+00001db0: 372e 3539 4331 342e 3139 2c36 372e 3937  7.59C14.19,67.97
+00001dc0: 2031 342e 3339 2c36 382e 3335 2031 342e   14.39,68.35 14.
+00001dd0: 3631 2c36 382e 3733 4c31 342e 3837 2c36  61,68.73L14.87,6
+00001de0: 392e 3135 4331 352e 312c 3639 2e35 3220  9.15C15.1,69.52 
+00001df0: 3135 2e33 332c 3639 2e38 3920 3135 2e35  15.33,69.89 15.5
+00001e00: 382c 3730 2e32 364c 3135 2e35 382c 3730  8,70.26L15.58,70
+00001e10: 2e33 324c 3135 2e39 392c 3730 2e39 3343  .32L15.99,70.93C
+00001e20: 3136 2e31 342c 3731 2e31 3420 3136 2e32  16.14,71.14 16.2
+00001e30: 392c 3731 2e33 3620 3136 2e34 352c 3731  9,71.36 16.45,71
+00001e40: 2e35 3743 3230 2e32 3036 2c37 352e 3833  .57C20.206,75.83
+00001e50: 2032 352e 3038 362c 3738 2e39 3520 3330   25.086,78.95 30
+00001e60: 2e35 332c 3830 2e35 3743 3336 2e38 3339  .53,80.57C36.839
+00001e70: 2c38 322e 3438 2034 332e 3431 2c38 332e  ,82.48 43.41,83.
+00001e80: 3338 3520 3530 2c38 332e 3235 4335 362e  385 50,83.25C56.
+00001e90: 3539 392c 3833 2e33 3734 2036 332e 3137  599,83.374 63.17
+00001ea0: 372c 3832 2e34 3536 2036 392e 3439 2c38  7,82.456 69.49,8
+00001eb0: 302e 3533 4337 342e 3634 342c 3738 2e39  0.53C74.644,78.9
+00001ec0: 3738 2037 392e 3330 332c 3736 2e31 3032  78 79.303,76.102
+00001ed0: 2038 332c 3732 2e31 3943 3833 2e33 342c   83,72.19C83.34,
+00001ee0: 3731 2e37 3820 3833 2e36 352c 3731 2e33  71.78 83.65,71.3
+00001ef0: 3520 3834 2c37 302e 3932 4c38 342e 3138  5 84,70.92L84.18
+00001f00: 2c37 302e 3636 4c38 342e 3333 2c37 302e  ,70.66L84.33,70.
+00001f10: 3434 4c38 342e 3431 2c37 302e 3332 4338  44L84.41,70.32C8
+00001f20: 342e 3535 2c37 302e 3132 2038 342e 3637  4.55,70.12 84.67
+00001f30: 2c36 392e 3920 3834 2e38 312c 3639 2e37  ,69.9 84.81,69.7
+00001f40: 4338 352e 3037 2c36 392e 3320 3835 2e33  C85.07,69.3 85.3
+00001f50: 322c 3638 2e38 3920 3835 2e35 352c 3638  2,68.89 85.55,68
+00001f60: 2e34 3843 3835 2e37 382c 3638 2e30 3720  .48C85.78,68.07 
+00001f70: 3836 2e30 322c 3637 2e36 3520 3836 2e32  86.02,67.65 86.2
+00001f80: 332c 3637 2e32 3243 3836 2e33 312c 3637  3,67.22C86.31,67
+00001f90: 2e30 3520 3836 2e33 392c 3636 2e38 3820  .05 86.39,66.88 
+00001fa0: 3836 2e34 372c 3636 2e37 4338 362e 3637  86.47,66.7C86.67
+00001fb0: 2c36 362e 3238 2038 362e 3835 2c36 352e  ,66.28 86.85,65.
+00001fc0: 3837 2038 372e 3033 2c36 352e 3434 4c38  87 87.03,65.44L8
+00001fd0: 372e 3233 2c36 342e 3932 4338 372e 3339  7.23,64.92C87.39
+00001fe0: 372c 3634 2e34 3837 2038 372e 3535 2c36  7,64.487 87.55,6
+00001ff0: 342e 3035 2038 372e 3639 2c36 332e 3631  4.05 87.69,63.61
+00002000: 4c38 372e 3835 2c36 332e 3039 4338 372e  L87.85,63.09C87.
+00002010: 3938 2c36 322e 3634 2038 382e 312c 3632  98,62.64 88.1,62
+00002020: 2e31 3920 3838 2e32 312c 3631 2e37 3443  .19 88.21,61.74C
+00002030: 3838 2e32 312c 3631 2e35 3720 3838 2e33  88.21,61.57 88.3
+00002040: 2c36 312e 3339 2038 382e 3333 2c36 312e  ,61.39 88.33,61.
+00002050: 3232 4338 382e 3433 2c36 302e 3735 2038  22C88.43,60.75 8
+00002060: 382e 3532 2c36 302e 3232 2038 382e 362c  8.52,60.22 88.6,
+00002070: 3539 2e37 3943 3838 2e36 2c35 392e 3634  59.79C88.6,59.64
+00002080: 2038 382e 3636 2c35 392e 3439 2038 382e   88.66,59.49 88.
+00002090: 3638 2c35 392e 3333 4338 382e 3737 2c35  68,59.33C88.77,5
+000020a0: 382e 3731 2038 382e 3834 2c35 382e 3038  8.71 88.84,58.08
+000020b0: 2038 382e 3838 2c35 372e 3435 4c38 382e   88.88,57.45L88.
+000020c0: 3838 2c35 342e 3137 4338 382e 3831 372c  88,54.17C88.817,
+000020d0: 3533 2e31 3634 2038 382e 3639 332c 3532  53.164 88.693,52
+000020e0: 2e31 3632 2038 382e 3531 2c35 312e 3137  .162 88.51,51.17
+000020f0: 4338 382e 3338 2c35 302e 3520 3838 2e32  C88.38,50.5 88.2
+00002100: 332c 3439 2e38 3420 3838 2e30 352c 3439  3,49.84 88.05,49
+00002110: 2e31 374c 3838 2c34 392e 3035 5a4d 3835  .17L88,49.05ZM85
+00002120: 2e38 392c 3536 2e34 344c 3835 2e38 392c  .89,56.44L85.89,
+00002130: 3537 2e32 3343 3835 2e38 392c 3537 2e37  57.23C85.89,57.7
+00002140: 3820 3835 2e37 392c 3538 2e33 3220 3835  8 85.79,58.32 85
+00002150: 2e37 322c 3538 2e38 3643 3835 2e37 322c  .72,58.86C85.72,
+00002160: 3539 2e30 3120 3835 2e37 322c 3539 2e31  59.01 85.72,59.1
+00002170: 3520 3835 2e36 352c 3539 2e33 4338 352e  5 85.65,59.3C85.
+00002180: 3539 2c35 392e 3720 3835 2e35 312c 3630  59,59.7 85.51,60
+00002190: 2e31 3120 3835 2e34 332c 3630 2e35 314c  .11 85.43,60.51L
+000021a0: 3835 2e33 322c 3630 2e39 3943 3835 2e32  85.32,60.99C85.2
+000021b0: 332c 3631 2e33 3820 3835 2e31 322c 3631  3,61.38 85.12,61
+000021c0: 2e37 3720 3835 2e30 312c 3632 2e31 3643  .77 85.01,62.16C
+000021d0: 3835 2e30 312c 3632 2e33 3120 3834 2e39  85.01,62.31 84.9
+000021e0: 332c 3632 2e34 3620 3834 2e38 382c 3632  3,62.46 84.88,62
+000021f0: 2e36 4338 342e 3734 2c36 332e 3034 2038  .6C84.74,63.04 8
+00002200: 342e 3539 2c36 332e 3437 2038 342e 3432  4.59,63.47 84.42
+00002210: 2c36 332e 394c 3834 2e32 372c 3634 2e32  ,63.9L84.27,64.2
+00002220: 3843 3834 2e31 2c36 342e 3731 2038 332e  8C84.1,64.71 83.
+00002230: 3931 2c36 352e 3134 2038 332e 3731 2c36  91,65.14 83.71,6
+00002240: 352e 3536 4338 332e 3531 2c36 352e 3938  5.56C83.51,65.98
+00002250: 2038 332e 3433 2c36 362e 3132 2038 332e   83.43,66.12 83.
+00002260: 3238 2c36 362e 344c 3833 2e30 312c 3636  28,66.4L83.01,66
+00002270: 2e39 3143 3832 2e38 332c 3637 2e32 3233  .91C82.83,67.223
+00002280: 2038 322e 3634 332c 3637 2e35 3337 2038   82.643,67.537 8
+00002290: 322e 3435 2c36 372e 3835 4c38 322e 3335  2.45,67.85L82.35
+000022a0: 2c36 382e 3031 4337 392e 3132 312c 3638  ,68.01C79.121,68
+000022b0: 2e30 3437 2037 352e 3931 382c 3637 2e34  .047 75.918,67.4
+000022c0: 3334 2037 322e 3933 2c36 362e 3231 4336  34 72.93,66.21C6
+000022d0: 342e 3237 2c36 322e 3734 2035 392c 3535  4.27,62.74 59,55
+000022e0: 2e35 3220 3631 2e31 382c 3530 2e31 3143  .52 61.18,50.11C
+000022f0: 3632 2e31 382c 3437 2e36 2036 342e 372c  62.18,47.6 64.7,
+00002300: 3435 2e38 3220 3638 2e32 362c 3435 2e31  45.82 68.26,45.1
+00002310: 3143 3732 2e34 3839 2c34 342e 3339 3520  1C72.489,44.395 
+00002320: 3736 2e38 3335 2c34 342e 3930 3820 3830  76.835,44.908 80
+00002330: 2e37 382c 3436 2e35 3943 3832 2e31 3431  .78,46.59C82.141
+00002340: 2c34 372e 3134 3420 3833 2e34 3533 2c34  ,47.144 83.453,4
+00002350: 372e 3831 3320 3834 2e37 2c34 382e 3539  7.813 84.7,48.59
+00002360: 4338 342e 3736 2c34 382e 3736 2038 342e  C84.76,48.76 84.
+00002370: 3832 2c34 382e 3933 2038 342e 3838 2c34  82,48.93 84.88,4
+00002380: 392e 3143 3834 2e39 342c 3439 2e32 3720  9.1C84.94,49.27 
+00002390: 3835 2e30 352c 3439 2e36 3320 3835 2e31  85.05,49.63 85.1
+000023a0: 322c 3439 2e39 4338 352e 3238 2c35 302e  2,49.9C85.28,50.
+000023b0: 3520 3835 2e34 342c 3531 2e31 2038 352e  5 85.44,51.1 85.
+000023c0: 3535 2c35 312e 3733 4338 352e 3639 312c  55,51.73C85.691,
+000023d0: 3532 2e35 3037 2038 352e 3739 322c 3533  52.507 85.792,53
+000023e0: 2e32 3932 2038 352e 3835 2c35 342e 3038  .292 85.85,54.08
+000023f0: 4c38 352e 3835 2c35 352e 3839 4338 352e  L85.85,55.89C85.
+00002400: 3835 2c35 362e 3132 2038 352e 3931 2c35  85,56.12 85.91,5
+00002410: 362e 3235 2038 352e 3931 2c35 362e 3435  6.25 85.91,56.45
+00002420: 4c38 352e 3839 2c35 362e 3434 5a4d 3137  L85.89,56.44ZM17
+00002430: 2e36 362c 3638 4331 362e 3636 382c 3636  .66,68C16.668,66
+00002440: 2e34 3335 2031 352e 3836 392c 3634 2e37  .435 15.869,64.7
+00002450: 3536 2031 352e 3238 2c36 334c 3135 2e31  56 15.28,63L15.1
+00002460: 372c 3632 2e36 3843 3135 2e30 362c 3632  7,62.68C15.06,62
+00002470: 2e33 3520 3134 2e39 362c 3632 2e30 3120  .35 14.96,62.01 
+00002480: 3134 2e38 372c 3631 2e36 3843 3134 2e38  14.87,61.68C14.8
+00002490: 3233 2c36 312e 3439 3320 3134 2e37 3737  23,61.493 14.777
+000024a0: 2c36 312e 3331 2031 342e 3733 2c36 312e  ,61.31 14.73,61.
+000024b0: 3133 4331 342e 3636 2c36 302e 3834 2031  13C14.66,60.84 1
+000024c0: 342e 3539 2c36 302e 3535 2031 342e 3533  4.59,60.55 14.53
+000024d0: 2c36 302e 3237 4331 342e 3437 2c35 392e  ,60.27C14.47,59.
+000024e0: 3939 2031 342e 3433 2c35 392e 3732 2031  99 14.43,59.72 1
+000024f0: 342e 3338 2c35 392e 3434 4331 342e 3333  4.38,59.44C14.33
+00002500: 2c35 392e 3136 2031 342e 332c 3539 2031  ,59.16 14.3,59 1
+00002510: 342e 3237 2c35 382e 3738 4331 342e 322c  4.27,58.78C14.2,
+00002520: 3538 2e32 3720 3134 2e31 352c 3537 2e37  58.27 14.15,57.7
+00002530: 3820 3134 2e31 312c 3537 2e32 334c 3134  8 14.11,57.23L14
+00002540: 2e31 312c 3537 2e30 3343 3134 2e30 3038  .11,57.03C14.008
+00002550: 2c35 352e 3233 3620 3134 2e31 3232 2c35  ,55.236 14.122,5
+00002560: 332e 3433 3720 3134 2e34 352c 3531 2e36  3.437 14.45,51.6
+00002570: 3743 3134 2e35 362c 3531 2e30 3620 3134  7C14.56,51.06 14
+00002580: 2e37 312c 3530 2e34 3620 3134 2e38 382c  .71,50.46 14.88,
+00002590: 3439 2e38 3743 3134 2e39 362c 3439 2e35  49.87C14.96,49.5
+000025a0: 3920 3135 2e30 342c 3439 2e33 3220 3135  9 15.04,49.32 15
+000025b0: 2e31 332c 3439 2e30 3543 3135 2e32 322c  .13,49.05C15.22,
+000025c0: 3438 2e37 3820 3135 2e32 342c 3438 2e37  48.78 15.24,48.7
+000025d0: 3220 3135 2e33 2c34 382e 3535 4331 362e  2 15.3,48.55C16.
+000025e0: 3534 382c 3437 2e37 3734 2031 372e 3835  548,47.774 17.85
+000025f0: 392c 3437 2e31 3035 2031 392e 3232 2c34  9,47.105 19.22,4
+00002600: 362e 3535 4332 372e 3836 2c34 332e 3039  6.55C27.86,43.09
+00002610: 2033 362e 3635 2c34 342e 3637 2033 382e   36.65,44.67 38.
+00002620: 3832 2c35 302e 3038 4334 302e 3939 2c35  82,50.08C40.99,5
+00002630: 352e 3439 2033 352e 3733 2c36 322e 3734  5.49 35.73,62.74
+00002640: 2032 372e 3039 2c36 362e 3243 3234 2e31   27.09,66.2C24.1
+00002650: 3031 2c36 372e 3433 3120 3230 2e38 3933  01,67.431 20.893
+00002660: 2c36 382e 3034 3320 3137 2e36 362c 3638  ,68.043 17.66,68
+00002670: 5a4d 3638 2e35 372c 3737 2e36 3843 3632  ZM68.57,77.68C62
+00002680: 2e35 3534 2c37 392e 3530 3820 3536 2e32  .554,79.508 56.2
+00002690: 3837 2c38 302e 3337 3620 3530 2c38 302e  87,80.376 50,80.
+000026a0: 3235 4334 332e 3733 372c 3830 2e33 3720  25C43.737,80.37 
+000026b0: 3337 2e34 3935 2c37 392e 3530 3620 3331  37.495,79.506 31
+000026c0: 2e35 2c37 372e 3639 4332 372e 3138 352c  .5,77.69C27.185,
+000026d0: 3736 2e33 3820 3233 2e32 3433 2c37 342e  76.38 23.243,74.
+000026e0: 3036 3220 3230 2c37 302e 3933 4332 322e  062 20,70.93C22.
+000026f0: 3831 352c 3730 2e37 3036 2032 352e 3538  815,70.706 25.58
+00002700: 2c37 302e 3035 3520 3238 2e32 2c36 3943  ,70.055 28.2,69C
+00002710: 3338 2e33 372c 3634 2e39 3220 3434 2e33  38.37,64.92 44.3
+00002720: 392c 3536 2034 312e 362c 3439 4333 382e  9,56 41.6,49C38.
+00002730: 3831 2c34 3220 3238 2e32 372c 3339 2e37  81,42 28.27,39.7
+00002740: 3220 3138 2e31 2c34 332e 384c 3137 2e34  2 18.1,43.8L17.4
+00002750: 332c 3434 2e30 3943 3138 2e39 3733 2c34  3,44.09C18.973,4
+00002760: 312e 3634 3820 3231 2e30 3139 2c33 392e  1.648 21.019,39.
+00002770: 3536 3120 3233 2e34 332c 3337 2e39 3743  561 23.43,37.97C
+00002780: 3236 2e36 3731 2c33 352e 3832 3420 3330  26.671,35.824 30
+00002790: 2e34 3733 2c33 342e 3638 2033 342e 3336  .473,34.68 34.36
+000027a0: 2c33 342e 3638 4333 352e 3838 342c 3334  ,34.68C35.884,34
+000027b0: 2e36 3831 2033 372e 3430 342c 3334 2e38  .681 37.404,34.8
+000027c0: 3532 2033 382e 3839 2c33 352e 3139 4334  52 38.89,35.19C4
+000027d0: 322e 3639 342c 3336 2e30 3439 2034 362e  2.694,36.049 46.
+000027e0: 3139 312c 3337 2e39 3335 2034 392c 3430  191,37.935 49,40
+000027f0: 2e36 344c 3530 2c34 312e 3634 4c35 312c  .64L50,41.64L51,
+00002800: 3430 2e36 3443 3533 2e37 3937 2c33 372e  40.64C53.797,37.
+00002810: 3933 3720 3537 2e32 3739 2c33 362e 3034  937 57.279,36.04
+00002820: 3920 3631 2e30 372c 3335 2e31 3843 3636  9 61.07,35.18C66
+00002830: 2e34 3032 2c33 332e 3934 3720 3732 2e30  .402,33.947 72.0
+00002840: 3134 2c33 342e 3936 3820 3736 2e35 372c  14,34.968 76.57,
+00002850: 3338 4337 382e 3938 2c33 392e 3538 3820  38C78.98,39.588 
+00002860: 3831 2e30 3236 2c34 312e 3637 3120 3832  81.026,41.671 82
+00002870: 2e35 372c 3434 2e31 314c 3831 2e39 2c34  .57,44.11L81.9,4
+00002880: 332e 3832 4337 372e 3430 392c 3431 2e39  3.82C77.409,41.9
+00002890: 3231 2037 322e 3436 342c 3431 2e33 3535  21 72.464,41.355
+000028a0: 2036 372e 3636 2c34 322e 3139 4336 332e   67.66,42.19C63.
+000028b0: 3038 2c34 332e 3132 2035 392e 3739 2c34  08,43.12 59.79,4
+000028c0: 352e 3534 2035 382e 3339 2c34 392e 3032  5.54 58.39,49.02
+000028d0: 4335 352e 362c 3535 2e39 3720 3631 2e36  C55.6,55.97 61.6
+000028e0: 322c 3634 2e39 3420 3731 2e37 392c 3639  2,64.94 71.79,69
+000028f0: 2e30 3243 3734 2e34 3134 2c37 302e 3037  .02C74.414,70.07
+00002900: 2037 372e 3138 322c 3730 2e37 3134 2038   77.182,70.714 8
+00002910: 302c 3730 2e39 3343 3736 2e37 3736 2c37  0,70.93C76.776,7
+00002920: 342e 3035 2037 322e 3835 392c 3736 2e33  4.05 72.859,76.3
+00002930: 3633 2036 382e 3537 2c37 372e 3638 5a22  63 68.57,77.68Z"
+00002940: 2073 7479 6c65 3d22 6669 6c6c 3a72 6762   style="fill:rgb
+00002950: 2832 3232 2c31 3230 2c31 3630 293b 6669  (222,120,160);fi
+00002960: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
+00002970: 222f 3e0a 2020 2020 2020 2020 3c2f 673e  "/>.        </g>
+00002980: 0a20 2020 2020 2020 203c 6720 7472 616e  .        <g tran
+00002990: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
+000029a0: 3239 3930 3132 2c30 2c30 2c30 2e32 3939  299012,0,0,0.299
+000029b0: 3031 322c 392e 3730 3232 392c 2d36 2e36  012,9.70229,-6.6
+000029c0: 3835 3832 2922 3e0a 2020 2020 2020 2020  8582)">.        
+000029d0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000029e0: 3731 2e33 3322 2063 793d 2235 3622 2072  71.33" cy="56" r
+000029f0: 3d22 352e 3136 2220 7374 796c 653d 2266  ="5.16" style="f
+00002a00: 696c 6c3a 7267 6228 3232 322c 3132 302c  ill:rgb(222,120,
+00002a10: 3136 3029 3b22 2f3e 0a20 2020 2020 2020  160);"/>.       
+00002a20: 203c 2f67 3e0a 2020 2020 2020 2020 3c67   </g>.        <g
+00002a30: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
+00002a40: 6978 2830 2e32 3939 3031 322c 302c 302c  ix(0.299012,0,0,
+00002a50: 302e 3239 3930 3132 2c39 2e37 3032 3239  0.299012,9.70229
+00002a60: 2c2d 362e 3638 3538 3229 223e 0a20 2020  ,-6.68582)">.   
+00002a70: 2020 2020 2020 2020 203c 6369 7263 6c65           <circle
+00002a80: 2063 783d 2232 382e 3637 2220 6379 3d22   cx="28.67" cy="
+00002a90: 3536 2220 723d 2235 2e31 3622 2073 7479  56" r="5.16" sty
+00002aa0: 6c65 3d22 6669 6c6c 3a72 6762 2832 3232  le="fill:rgb(222
+00002ab0: 2c31 3230 2c31 3630 293b 222f 3e0a 2020  ,120,160);"/>.  
+00002ac0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
+00002ad0: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00002ae0: 226d 6174 7269 7828 302e 3239 3930 3132  "matrix(0.299012
+00002af0: 2c30 2c30 2c30 2e32 3939 3031 322c 392e  ,0,0,0.299012,9.
+00002b00: 3730 3232 392c 2d36 2e36 3835 3832 2922  70229,-6.68582)"
+00002b10: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+00002b20: 6174 6820 643d 224d 3538 2c36 3643 3535  ath d="M58,66C55
+00002b30: 2e39 3132 2c36 382e 3136 3120 3533 2e30  .912,68.161 53.0
+00002b40: 3033 2c36 392e 3333 3920 3530 2c36 392e  03,69.339 50,69.
+00002b50: 3234 4334 362e 3939 372c 3639 2e33 3339  24C46.997,69.339
+00002b60: 2034 342e 3038 382c 3638 2e31 3631 2034   44.088,68.161 4
+00002b70: 322c 3636 4334 312e 3731 342c 3635 2e36  2,66C41.714,65.6
+00002b80: 3737 2034 312e 3330 322c 3635 2e34 3931  77 41.302,65.491
+00002b90: 2034 302e 3837 2c36 352e 3439 3143 3430   40.87,65.491C40
+00002ba0: 2e30 3432 2c36 352e 3439 3120 3339 2e33  .042,65.491 39.3
+00002bb0: 3631 2c36 362e 3137 3220 3339 2e33 3631  61,66.172 39.361
+00002bc0: 2c36 3743 3339 2e33 3631 2c36 372e 3336  ,67C39.361,67.36
+00002bd0: 3820 3339 2e34 3936 2c36 372e 3732 3420  8 39.496,67.724 
+00002be0: 3339 2e37 342c 3638 4334 322e 3430 332c  39.74,68C42.403,
+00002bf0: 3730 2e38 3034 2034 362e 3133 342c 3732  70.804 46.134,72
+00002c00: 2e33 3520 3530 2c37 322e 3235 4335 332e  .35 50,72.25C53.
+00002c10: 3836 322c 3732 2e33 3437 2035 372e 3539  862,72.347 57.59
+00002c20: 2c37 302e 3830 3220 3630 2e32 352c 3638  ,70.802 60.25,68
+00002c30: 4336 302e 3439 352c 3637 2e37 3235 2036  C60.495,67.725 6
+00002c40: 302e 3633 2c36 372e 3336 3920 3630 2e36  0.63,67.369 60.6
+00002c50: 332c 3637 4336 302e 3633 2c36 362e 3137  3,67C60.63,66.17
+00002c60: 3420 3539 2e39 3531 2c36 352e 3439 3520  4 59.951,65.495 
+00002c70: 3539 2e31 3235 2c36 352e 3439 3543 3538  59.125,65.495C58
+00002c80: 2e36 3935 2c36 352e 3439 3520 3538 2e32  .695,65.495 58.2
+00002c90: 3835 2c36 352e 3637 3920 3538 2c36 365a  85,65.679 58,66Z
+00002ca0: 2220 7374 796c 653d 2266 696c 6c3a 7267  " style="fill:rg
+00002cb0: 6228 3232 322c 3132 302c 3136 3029 3b66  b(222,120,160);f
+00002cc0: 696c 6c2d 7275 6c65 3a6e 6f6e 7a65 726f  ill-rule:nonzero
+00002cd0: 3b22 2f3e 0a20 2020 2020 2020 203c 2f67  ;"/>.        </g
+00002ce0: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
+00002cf0: 6465 6673 3e0a 2020 2020 2020 2020 3c6c  defs>.        <l
+00002d00: 696e 6561 7247 7261 6469 656e 7420 6964  inearGradient id
+00002d10: 3d22 5f4c 696e 6561 7231 2220 7831 3d22  ="_Linear1" x1="
+00002d20: 3022 2079 313d 2230 2220 7832 3d22 3122  0" y1="0" x2="1"
+00002d30: 2079 323d 2230 2220 6772 6164 6965 6e74   y2="0" gradient
+00002d40: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00002d50: 4f6e 5573 6522 2067 7261 6469 656e 7454  OnUse" gradientT
+00002d60: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00002d70: 2831 2e32 3234 3635 652d 3135 2c32 302c  (1.22465e-15,20,
+00002d80: 2d32 302c 312e 3232 3436 3565 2d31 352c  -20,1.22465e-15,
+00002d90: 302c 3029 223e 0a20 2020 2020 2020 2020  0,0)">.         
+00002da0: 2020 203c 7374 6f70 206f 6666 7365 743d     <stop offset=
+00002db0: 2230 2220 7374 796c 653d 2273 746f 702d  "0" style="stop-
+00002dc0: 636f 6c6f 723a 7267 6228 3138 372c 3138  color:rgb(187,18
+00002dd0: 372c 3138 3729 3b73 746f 702d 6f70 6163  7,187);stop-opac
+00002de0: 6974 793a 302e 3122 2f3e 0a20 2020 2020  ity:0.1"/>.     
+00002df0: 2020 2020 2020 203c 7374 6f70 206f 6666         <stop off
+00002e00: 7365 743d 2231 2220 7374 796c 653d 2273  set="1" style="s
+00002e10: 746f 702d 636f 6c6f 723a 626c 6163 6b3b  top-color:black;
+00002e20: 7374 6f70 2d6f 7061 6369 7479 3a30 2e31  stop-opacity:0.1
+00002e30: 222f 3e0a 2020 2020 2020 2020 3c2f 6c69  "/>.        </li
+00002e40: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
+00002e50: 2020 3c2f 6465 6673 3e0a 3c2f 7376 673e    </defs>.</svg>
+00002e60: 0a                                       .
```

### Comparing `interrogate-1.5.0/tests/unit/test_badge_gen.py` & `interrogate-1.6.0/tests/unit/test_badge_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 def test_get_badge():
     """SVG badge is templated as expected."""
     actual = badge_gen.get_badge(99.9, "#4c1")
     actual = actual.replace("\n", "").replace("\r", "")
     expected_fixture = os.path.join(FIXTURES, "default-style", "99.svg")
-    with open(expected_fixture, "r") as f:
+    with open(expected_fixture) as f:
         expected = f.read()
         expected = expected.replace("\n", "").replace("\r", "")
 
     assert expected == actual
 
 
 @pytest.mark.parametrize(
```

### Comparing `interrogate-1.5.0/tests/unit/test_config.py` & `interrogate-1.6.0/tests/unit/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,38 +24,40 @@
         (("/usr/src/app/pyproject.toml",), "is_file", "/usr/src/app"),
         # return root if nothing matches
         (("/usr/src/app", "/usr/src/test"), None, "/"),
     ),
 )
 def test_find_project_root(srcs, patch_func, expected, monkeypatch):
     """Return expected directory of project root."""
-    expected = pathlib.Path(expected)
-    if patch_func:
-        monkeypatch.setattr(config.pathlib.Path, patch_func, lambda x: True)
-    monkeypatch.setattr(config.pathlib.Path, "resolve", lambda x: x)
+    with monkeypatch.context() as mp:
+        expected = pathlib.Path(expected)
+        if patch_func:
+            mp.setattr(config.pathlib.Path, patch_func, lambda x: True)
+        mp.setattr(config.pathlib.Path, "resolve", lambda x: x)
 
-    actual = config.find_project_root(srcs)
+        actual = config.find_project_root(srcs)
 
-    assert expected == actual
+        assert expected == actual
 
 
 @pytest.mark.parametrize(
     "is_file,expected",
     (
         (True, str(pathlib.Path("/usr/src/pyproject.toml"))),
         (False, None),
     ),
 )
 def test_find_project_config(is_file, expected, mocker, monkeypatch):
     """Return absolute path if pyproject.toml or setup.cfg is detected."""
-    monkeypatch.setattr(config.pathlib.Path, "is_file", lambda x: is_file)
-    monkeypatch.setattr(config.pathlib.Path, "resolve", lambda x: x)
+    with monkeypatch.context() as mp:
+        mp.setattr(config.pathlib.Path, "is_file", lambda x: is_file)
+        mp.setattr(config.pathlib.Path, "resolve", lambda x: x)
 
-    actual = config.find_project_config(("/usr/src/app",))
-    assert expected == actual
+        actual = config.find_project_config(("/usr/src/app",))
+        assert expected == actual
 
 
 def test_parse_pyproject_toml(tmpdir):
     """Return expected config data from a pyproject.toml file."""
     toml_data = (
         "[tool.foo]\n"
         'foo = "bar"\n'
```

### Comparing `interrogate-1.5.0/tests/unit/test_utils.py` & `interrogate-1.6.0/tests/unit/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pytest
 
 from interrogate import config
 from interrogate import utils
 
 
 IS_WINDOWS = sys.platform in ("cygwin", "win32")
-IS_PY38 = sys.version_info >= (3, 8)
 
 
 @pytest.mark.parametrize(
     "value,exp",
     (
         # no regex given
         (None, None),
@@ -334,60 +333,19 @@
         padded_cells, colwidths, colaligns, table_type=table_type
     )
 
     assert width - 1 == len(actual)
     assert expected == actual
 
 
-@pytest.mark.skipif(IS_PY38, reason="monkeypatching functools fails on 3.8")
 @pytest.mark.parametrize("table_type", ("detailed", "summary"))
 def test_output_formatter_get_table_formatter(table_type, mocker, monkeypatch):
     """The returned table formatter uses the correct table type."""
     mock_table_format = mocker.Mock()
     monkeypatch.setattr(utils.tabulate, "TableFormat", mock_table_format)
-    mock_functools_partial = mocker.Mock()
-
-    # functools.partial does not have an __eq__ method so any comparison
-    # between two partial functions will use id() and not actual equality.
-    # To work around this, we mock functools.partial. But it isn't as
-    # easy as it is with other monkeypatching:
-    # https://github.com/pytest-dev/pytest/pull/3382
-    # However, this fails on py3.8
-    with monkeypatch.context() as m:
-        m.setattr(utils.functools, "partial", mock_functools_partial)
-
-        conf = config.InterrogateConfig()
-        formatter = utils.OutputFormatter(conf)
-        formatter.get_table_formatter(table_type=table_type)
-
-    mock_table_format.assert_called_once_with(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=mock_functools_partial.return_value,
-        datarow=mock_functools_partial.return_value,
-        padding=1,
-        with_header_hide=None,
-    )
-    mock_functools_partial.assert_called_once_with(
-        formatter._interrogate_line_formatter, table_type=table_type
-    )
-
-
-@pytest.mark.skipif(
-    not IS_PY38, reason="monkeypatching functools fails on 3.8"
-)
-@pytest.mark.parametrize("table_type", ("detailed", "summary"))
-def test_output_formatter_get_table_formatter_py38(
-    table_type, mocker, monkeypatch
-):
-    """The returned table formatter uses the correct table type."""
-    mock_table_format = mocker.Mock()
-    monkeypatch.setattr(utils.tabulate, "TableFormat", mock_table_format)
 
     conf = config.InterrogateConfig()
     formatter = utils.OutputFormatter(conf)
     formatter.get_table_formatter(table_type=table_type)
 
     mock_table_format.assert_called_once()
```

