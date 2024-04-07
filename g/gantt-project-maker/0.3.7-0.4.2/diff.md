# Comparing `tmp/gantt-project-maker-0.3.7.tar.gz` & `tmp/gantt-project-maker-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantt-project-maker-0.3.7.tar", last modified: Tue Feb 13 09:07:50 2024, max compression
+gzip compressed data, was "gantt-project-maker-0.4.2.tar", last modified: Sun Apr  7 11:47:05 2024, max compression
```

## Comparing `gantt-project-maker-0.3.7.tar` & `gantt-project-maker-0.4.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.564672 gantt-project-maker-0.3.7/
--rw-rw-rw-   0        0        0      630 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/.coveragerc
--rw-rw-rw-   0        0        0      660 2024-01-26 08:30:03.000000 gantt-project-maker-0.3.7/.gitignore
--rw-rw-rw-   0        0        0      557 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/.readthedocs.yml
--rw-rw-rw-   0        0        0       83 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     1749 2024-02-13 09:06:27.000000 gantt-project-maker-0.3.7/CHANGELOG.rst
--rw-rw-rw-   0        0        0    12616 2024-01-22 07:42:49.000000 gantt-project-maker-0.3.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1103 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1544 2024-02-13 09:07:50.562670 gantt-project-maker-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      855 2024-01-22 07:40:49.000000 gantt-project-maker-0.3.7/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.284153 gantt-project-maker-0.3.7/docs/
--rw-rw-rw-   0        0        0     1183 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.292682 gantt-project-maker-0.3.7/docs/_static/
--rw-rw-rw-   0        0        0       19 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/changelog.rst
--rw-rw-rw-   0        0        0    10086 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/contributing.rst
--rw-rw-rw-   0        0        0     2422 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/index.rst
--rw-rw-rw-   0        0        0       74 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/license.rst
--rw-rw-rw-   0        0        0       41 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.343807 gantt-project-maker-0.3.7/examples/
--rw-rw-rw-   0        0        0     3500 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/examples/Makefile
--rw-rw-rw-   0        0        0     1155 2024-02-06 13:08:12.000000 gantt-project-maker-0.3.7/examples/employees.yml
--rw-rw-rw-   0        0        0     2999 2024-01-30 13:20:35.000000 gantt-project-maker-0.3.7/examples/projects.yml
--rw-rw-rw-   0        0        0    14028 2024-02-10 09:57:18.000000 gantt-project-maker-0.3.7/examples/projects_emp1.yml
--rw-rw-rw-   0        0        0     7854 2024-02-06 08:12:09.000000 gantt-project-maker-0.3.7/examples/projects_emp2.yml
--rw-rw-rw-   0        0        0     1978 2024-02-06 15:14:03.000000 gantt-project-maker-0.3.7/examples/projects_emp3.yml
--rw-rw-rw-   0        0        0      247 2024-01-24 10:35:34.000000 gantt-project-maker-0.3.7/examples/vacations.yml
--rw-rw-rw-   0        0        0      355 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0      824 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/readme.md
--rw-rw-rw-   0        0        0      235 2024-01-26 08:13:44.000000 gantt-project-maker-0.3.7/requirements.txt
--rw-rw-rw-   0        0        0     1277 2024-02-13 09:07:50.570202 gantt-project-maker-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.125044 gantt-project-maker-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.437688 gantt-project-maker-0.3.7/src/gantt_project_maker/
--rw-rw-rw-   0        0        0      606 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/__init__.py
--rw-rw-rw-   0        0        0     2150 2024-02-01 10:53:32.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/colors.py
--rw-rw-rw-   0        0        0    14726 2024-02-10 10:38:55.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/excelwriter.py
--rw-rw-rw-   0        0        0   106824 2024-02-05 11:25:42.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/gantt.py
--rw-rw-rw-   0        0        0    19481 2024-02-10 10:05:25.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/main.py
--rw-rw-rw-   0        0        0    43543 2024-02-13 09:04:18.000000 gantt-project-maker-0.3.7/src/gantt_project_maker/project_classes.py
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.556467 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/
--rw-rw-rw-   0        0        0     1544 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1155 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-13 09:07:47.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-13 09:07:49.000000 gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-13 09:07:50.543427 gantt-project-maker-0.3.7/tests/
--rw-rw-rw-   0        0        0      297 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/tests/conftest.py
--rw-rw-rw-   0        0        0      930 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/tests/test_colors.py
--rw-rw-rw-   0        0        0      844 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/tests/test_main.py
--rw-rw-rw-   0        0        0      843 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/tests/test_project_classes.py
--rw-rw-rw-   0        0        0     2944 2024-01-19 20:20:41.000000 gantt-project-maker-0.3.7/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.948590 gantt-project-maker-0.4.2/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      602 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      602 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2270 2024-04-07 11:46:29.000000 gantt-project-maker-0.4.2/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12750 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1895 2024-04-07 11:47:05.948590 gantt-project-maker-0.4.2/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      824 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.936590 gantt-project-maker-0.4.2/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.936590 gantt-project-maker-0.4.2/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9772 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1445 2024-04-07 11:41:20.000000 gantt-project-maker-0.4.2/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      341 2024-03-20 15:23:39.000000 gantt-project-maker-0.4.2/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.940590 gantt-project-maker-0.4.2/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     3396 2023-10-20 05:17:33.000000 gantt-project-maker-0.4.2/examples/Makefile
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1097 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/examples/employees.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     4936 2024-04-06 09:18:31.000000 gantt-project-maker-0.4.2/examples/projects.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    13653 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/examples/projects_emp1.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7551 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/examples/projects_emp2.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2498 2024-03-20 13:30:50.000000 gantt-project-maker-0.4.2/examples/projects_emp3.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      233 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/examples/vacations.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      803 2023-10-20 05:21:11.000000 gantt-project-maker-0.4.2/readme.md
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      116 2024-03-20 15:26:55.000000 gantt-project-maker-0.4.2/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1376 2024-04-07 11:47:05.948590 gantt-project-maker-0.4.2/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      714 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.928590 gantt-project-maker-0.4.2/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.944590 gantt-project-maker-0.4.2/src/gantt_project_maker/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      590 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2085 2024-02-26 15:43:00.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/colors.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    26645 2024-04-06 06:35:29.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/excelwriter.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   104839 2024-04-05 07:05:22.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/gantt.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    21340 2024-04-07 10:57:32.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/main.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    61849 2024-04-07 11:03:13.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/project_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     3054 2024-04-06 09:16:53.000000 gantt-project-maker-0.4.2/src/gantt_project_maker/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.944590 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1895 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1212 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       69 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      210 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       20 2024-04-07 11:47:05.000000 gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-07 11:47:05.944590 gantt-project-maker-0.4.2/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      287 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      897 2023-09-25 08:35:47.000000 gantt-project-maker-0.4.2/tests/test_colors.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      815 2023-09-21 18:35:30.000000 gantt-project-maker-0.4.2/tests/test_main.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      816 2023-09-25 08:35:47.000000 gantt-project-maker-0.4.2/tests/test_project_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2023-09-21 12:19:05.000000 gantt-project-maker-0.4.2/tox.ini
```

### Comparing `gantt-project-maker-0.3.7/.coveragerc` & `gantt-project-maker-0.4.2/.coveragerc`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# .coveragerc to control coverage.py
-[run]
-branch = True
-source = gantt_project_maker
-# omit = bad_file.py
-
-[paths]
-source =
-    src/
-    */site-packages/
-
-[report]
-# Regexes for lines to exclude from consideration
-exclude_lines =
-    # Have to re-enable the standard pragma
-    pragma: no cover
-
-    # Don't complain about missing debug-only code:
-    def __repr__
-    if self\.debug
-
-    # Don't complain if tests don't hit defensive assertion code:
-    raise AssertionError
-    raise NotImplementedError
-
-    # Don't complain if non-runnable code isn't run:
-    if 0:
-    if __name__ == .__main__.:
+# .coveragerc to control coverage.py
+[run]
+branch = True
+source = gantt_project_maker
+# omit = bad_file.py
+
+[paths]
+source =
+    src/
+    */site-packages/
+
+[report]
+# Regexes for lines to exclude from consideration
+exclude_lines =
+    # Have to re-enable the standard pragma
+    pragma: no cover
+
+    # Don't complain about missing debug-only code:
+    def __repr__
+    if self\.debug
+
+    # Don't complain if tests don't hit defensive assertion code:
+    raise AssertionError
+    raise NotImplementedError
+
+    # Don't complain if non-runnable code isn't run:
+    if 0:
+    if __name__ == .__main__.:
```

### Comparing `gantt-project-maker-0.3.7/CHANGELOG.rst` & `gantt-project-maker-0.4.2/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,65 @@
-=========
-Changelog
-=========
-
-Version 0.3.7
-=============
-- Added option --vacations in order to export a gantt chart of the vacations per employer
-- Added option --collaps_tasks in order to collaps the tasks per project to one task in order to simplify the output
-- Improved some feedback at errors with missing employees
-- if --output_filename is given on the command line, do not add employees to the base
-- bug fix on quarter label in excel output
-- bug fix on pdf output of resources
-
-Version 0.2.4
-=============
-- Added --pdf option in order to convert svg file into pdf as well
-
-Version 0.2.3
-=============
-- Added possibility to add margin_left and margin_right property to project to prevent cluttering of labels
-- Added possibility to filter on one or more employees to only display the project of the selected employees
-- Change default font size for level 0 and 1 in project plan
-- Add name of employee to title if a filter was used
-
-Version 0.1.9
-=============
-- In resources overview, task colors now match the colors in the project overview
-- The task color can now explicitly be given. Default task color matches the project color.
-- Started to update the documentation. Still needs to be finished
-
-
-Version 0.1.7
-=============
-- Improved colouring of resources schema
-
-Version 0.1.6
-=============
-- Added some basic checks on the tasks start and end dates to be more specifics on errors
-
-Version 0.1.5
-=============
-- Bug today reference fixed
-- Vacation now correctly added
-- Font properties can be specified in setting file
-- dayfist can be set to false
-
-Version 0.1.3
-=============
-
-- Dynamic columns added
-- First version of Gantt Project maker
-- First bug fixes established
+=========
+Changelog
+=========
+
+Version 0.4.2
+=============
+- Added new Excel format output to collect all the projects per contributor
+- Added possibility to assign number of hours to each contributor's task
+- Added summations of hours per contributor
+
+Version 0.4.0
+=============
+- Added option --suffix in order add a extra suffix to the filename
+- Added option --project in order to filter on the main projects which are going to be included
+- Added replacement variable for both titles and date/time. Now a variable 'my_variable'
+  can be defined which replaces all occurrences of {{ my_variable }}
+
+Version 0.3.7
+=============
+- Added option --vacations in order to export a gantt chart of the vacations per employer
+- Added option --collaps_tasks in order to collaps the tasks per project to one task in order to simplify the output
+- Improved some feedback at errors with missing employees
+- if --output_filename is given on the command line, do not add employees to the base
+- bug fix on quarter label in excel output
+- bug fix on pdf output of resources
+
+Version 0.2.4
+=============
+- Added --pdf option in order to convert svg file into pdf as well
+
+Version 0.2.3
+=============
+- Added possibility to add margin_left and margin_right property to project to prevent cluttering of labels
+- Added possibility to filter on one or more employees to only display the project of the selected employees
+- Change default font size for level 0 and 1 in project plan
+- Add name of employee to title if a filter was used
+
+Version 0.1.9
+=============
+- In resources overview, task colors now match the colors in the project overview
+- The task color can now explicitly be given. Default task color matches the project color.
+- Started to update the documentation. Still needs to be finished
+
+
+Version 0.1.7
+=============
+- Improved colouring of resources schema
+
+Version 0.1.6
+=============
+- Added some basic checks on the tasks start and end dates to be more specifics on errors
+
+Version 0.1.5
+=============
+- Bug today reference fixed
+- Vacation now correctly added
+- Font properties can be specified in setting file
+- dayfist can be set to false
+
+Version 0.1.3
+=============
+
+- Dynamic columns added
+- First version of Gantt Project maker
+- First bug fixes established
```

### Comparing `gantt-project-maker-0.3.7/CONTRIBUTING.rst` & `gantt-project-maker-0.4.2/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,310 +1,323 @@
-============
-Contributing
-============
-
-Welcome to ``gantt-project-maker`` contributor's guide.
-
-This document focuses on getting any potential contributor familiarized
-with the development processes, but `other kinds of contributions`_ are also
-appreciated.
-
-If you are new to using git_ or have never collaborated in a project previously,
-please have a look at `contribution-guide.org`_. Other resources are also
-listed in the excellent `guide created by FreeCodeCamp`_ [#contrib1]_.
-
-Please notice, all users and contributors are expected to be **open,
-considerate, reasonable, and respectful**. When in doubt, `Python Software
-Foundation's Code of Conduct`_ is a good reference in terms of behavior
-guidelines.
-
-
-Issue Reports
-=============
-
-If you experience bugs or general issues with ``gantt-project-maker``, please have a look
-on the `issue tracker`_. If you don't see anything useful there, please feel
-free to fire an issue report.
-
-.. tip::
-   Please don't forget to include the closed issues in your search.
-   Sometimes a solution was already reported, and the problem is considered
-   **solved**.
-
-New issue reports should include information about your programming environment
-(e.g., operating system, Python version) and steps to reproduce the problem.
-Please try also to simplify the reproduction steps to a very minimal example
-that still illustrates the problem you are facing. By removing other factors,
-you help us to identify the root cause of the issue.
-
-
-Documentation Improvements
-==========================
-
-You can help improve ``gantt-project-maker`` docs by making them more readable and coherent, or
-by adding missing information and correcting mistakes.
-
-``gantt-project-maker`` documentation uses Sphinx_ as its main documentation compiler.
-This means that the docs are kept in the same repository as the project code, and
-that any documentation update is done in the same way was a code contribution.
-The documentation is written in reStructuredText_.
-
-   .. tip::
-      Please notice that the `GitHub web interface`_ provides a quick way of
-      propose changes in ``gantt-project-maker``'s files. While this mechanism can
-      be tricky for normal code contributions, it works perfectly fine for
-      contributing to the docs, and can be quite handy.
-
-      If you are interested in trying this method out, please navigate to
-      the ``docs`` folder in the source repository_, find which file you
-      would like to propose changes and click in the little pencil icon at the
-      top, to open `GitHub's code editor`_. Once you finish editing the file,
-      please write a message in the form at the bottom of the page describing
-      which changes have you made and what are the motivations behind them and
-      submit your proposal.
-
-When working on documentation changes in your local machine, you can
-compile them using |tox|_::
-
-    tox -e docs
-
-and use Python's built-in web server for a preview in your web browser
-(``http://localhost:8000``)::
-
-    python3 -m http.server --directory 'docs/_build/html'
-
-
-Code Contributions
-==================
-
-* The code is a front end to python-gantt_ project developed `Alexandre Norman`_, but as this project is not maintained
-  anymore.
-* The front end was written by `Eelco van Vliet`_
-* The gantt module has been included into this project and adapted where required.
-* A yaml file settings file is used to defined all the project and other properties
-* Task are added per project. See the User manual for more details
-
-
-Submit an issue
----------------
-
-Before you work on any non-trivial code contribution it's best to first create
-a report in the `issue tracker`_ to start a discussion on the subject.
-This often provides additional considerations and avoids unnecessary work.
-
-Create an environment
----------------------
-
-Before you start coding, we recommend creating an isolated `virtual
-environment`_ to avoid any problems with your installed Python packages.
-This can easily be done via either |virtualenv|_::
-
-    virtualenv <PATH TO VENV>
-    source <PATH TO VENV>/bin/activate
-
-or Miniconda_::
-
-    conda create -n gantt-project-maker python=3 six virtualenv pytest pytest-cov
-    conda activate gantt-project-maker
-
-Clone the repository
---------------------
-
-#. Create an user account on |the repository service| if you do not already have one.
-#. Fork the project repository_: click on the *Fork* button near the top of the
-   page. This creates a copy of the code under your account on |the repository service|.
-#. Clone this copy to your local disk::
-
-    git clone git@github.com:eelcovv/gantt-project-maker.git
-    cd gantt-project-maker
-
-#. You should run::
-
-    pip install -U pip setuptools -e .
-
-   to be able to import the package under development in the Python REPL.
-
-Implement your changes
-----------------------
-
-#. Create a branch to hold your changes::
-
-    git checkout -b my-feature
-
-   and start making changes. Never work on the main branch!
-
-#. Start your work on this branch. Don't forget to add docstrings_ to new
-   functions, modules and classes, especially if they are part of public APIs.
-
-#. Add yourself to the list of contributors in ``AUTHORS.rst``.
-
-#. When you’re done editing, do::
-
-    git add <MODIFIED FILES>
-    git commit
-
-   to record your changes in git_.
-
-   .. important:: Don't forget to add unit tests and documentation in case your
-      contribution adds an additional feature and is not just a bugfix.
-
-      Moreover, writing a `descriptive commit message`_ is highly recommended.
-      In case of doubt, you can check the commit history with::
-
-         git log --graph --decorate --pretty=oneline --abbrev-commit --all
-
-      to look for recurring communication patterns.
-
-#. Please check that your changes don't break any unit tests with::
-
-    tox
-
-   (after having installed |tox|_ with ``pip install tox`` or ``pipx``).
-
-   You can also use |tox|_ to run several other pre-configured tasks in the
-   repository. Try ``tox -av`` to see a list of the available checks.
-
-Submit your contribution
-------------------------
-
-#. If everything works fine, push your local branch to |the repository service| with::
-
-    git push -u origin my-feature
-
-#. Go to the web page of your fork and click |contribute button|
-   to send your changes for review.
-
-   .. todo:: if you are using GitHub, you can uncomment the following paragraph
-
-      Find more detailed information in `creating a PR`_. You might also want to open
-      the PR as a draft first and mark it as ready for review after the feedbacks
-      from the continuous integration (CI) system or any required fixes.
-
-
-Troubleshooting
----------------
-
-The following tips can be used when facing problems to build or test the
-package:
-
-#. Make sure to fetch all the tags from the upstream repository_.
-   The command ``git describe --abbrev=0 --tags`` should return the version you
-   are expecting. If you are trying to run CI scripts in a fork repository,
-   make sure to push all the tags.
-   You can also try to remove all the egg files or the complete egg folder, i.e.,
-   ``.eggs``, as well as the ``*.egg-info`` folders in the ``src`` folder or
-   potentially in the root of your project.
-
-#. Sometimes |tox|_ misses out when new dependencies are added, especially to
-   ``setup.cfg`` and ``docs/requirements.txt``. If you find any problems with
-   missing dependencies when running a command with |tox|_, try to recreate the
-   ``tox`` environment using the ``-r`` flag. For example, instead of::
-
-    tox -e docs
-
-   Try running::
-
-    tox -r -e docs
-
-#. Make sure to have a reliable |tox|_ installation that uses the correct
-   Python version (e.g., 3.7+). When in doubt you can run::
-
-    tox --version
-    # OR
-    which tox
-
-   If you have trouble and are seeing weird errors upon running |tox|_, you can
-   also try to create a dedicated `virtual environment`_ with a |tox|_ binary
-   freshly installed. For example::
-
-    virtualenv .venv
-    source .venv/bin/activate
-    .venv/bin/pip install tox
-    .venv/bin/tox -e all
-
-#. `Pytest can drop you`_ in an interactive session in the case an error occurs.
-   In order to do that you need to pass a ``--pdb`` option (for example by
-   running ``tox -- -k <NAME OF THE FALLING TEST> --pdb``).
-   You can also setup breakpoints manually instead of using the ``--pdb`` option.
-
-
-Maintainer tasks
-================
-
-Releases
---------
-
-.. todo:: This section assumes you are using PyPI to publicly release your package.
-
-   If instead you are using a different/private package index, please update
-   the instructions accordingly.
-
-If you are part of the group of maintainers and have correct user permissions
-on PyPI_, the following steps can be used to release a new version for
-``gantt-project-maker``:
-
-#. Make sure all unit tests are successful.
-#. Tag the current commit on the main branch with a release tag, e.g., ``v1.2.3``.
-#. Push the new tag to the upstream repository_, e.g., ``git push upstream v1.2.3``
-#. Clean up the ``dist`` and ``build`` folders with ``tox -e clean``
-   (or ``rm -rf dist build``)
-   to avoid confusion with old builds and Sphinx docs.
-#. Run ``tox -e build`` and check that the files in ``dist`` have
-   the correct version (no ``.dirty`` or git_ hash) according to the git_ tag.
-   Also check the sizes of the distributions, if they are too big (e.g., >
-   500KB), unwanted clutter may have been accidentally included.
-#. Run ``tox -e publish -- --repository pypi`` and check that everything was
-   uploaded to PyPI_ correctly.
-
-
-
-.. [#contrib1] Even though, these resources focus on open source projects and
-   communities, the general ideas behind collaborating with other developers
-   to collectively create software are general and can be applied to all sorts
-   of environments, including private companies and proprietary code bases.
-
-
-.. <-- start -->
-
-.. |the repository service| replace:: GitHub
-.. |contribute button| replace:: "Create pull request"
-
-.. _repository: https://github.com/eelcovv/gantt-project-maker
-.. _issue tracker: https://github.com/eelcovv/gantt-project-maker/issues
-.. _python-gantt: https://pypi.org/project/python-gantt
-.. _Alexandre Norman: norman@xael.org
-.. _Eelco van Vliet: eelcovv@gmail.org
-.. <-- end -->
-
-
-.. |virtualenv| replace:: ``virtualenv``
-.. |pre-commit| replace:: ``pre-commit``
-.. |tox| replace:: ``tox``
-
-
-.. _black: https://pypi.org/project/black/
-.. _CommonMark: https://commonmark.org/
-.. _contribution-guide.org: https://www.contribution-guide.org/
-.. _creating a PR: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
-.. _descriptive commit message: https://chris.beams.io/posts/git-commit
-.. _docstrings: https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
-.. _first-contributions tutorial: https://github.com/firstcontributions/first-contributions
-.. _flake8: https://flake8.pycqa.org/en/stable/
-.. _git: https://git-scm.com
-.. _GitHub's fork and pull request workflow: https://guides.github.com/activities/forking/
-.. _guide created by FreeCodeCamp: https://github.com/FreeCodeCamp/how-to-contribute-to-open-source
-.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-.. _MyST: https://myst-parser.readthedocs.io/en/latest/syntax/syntax.html
-.. _other kinds of contributions: https://opensource.guide/how-to-contribute
-.. _pre-commit: https://pre-commit.com/
-.. _PyPI: https://pypi.org/
-.. _PyScaffold's contributor's guide: https://pyscaffold.org/en/stable/contributing.html
-.. _Pytest can drop you: https://docs.pytest.org/en/stable/how-to/failures.html#using-python-library-pdb-with-pytest
-.. _Python Software Foundation's Code of Conduct: https://www.python.org/psf/conduct/
-.. _reStructuredText: https://www.sphinx-doc.org/en/master/usage/restructuredtext/
-.. _Sphinx: https://www.sphinx-doc.org/en/master/
-.. _tox: https://tox.wiki/en/stable/
-.. _virtual environment: https://realpython.com/python-virtual-environments-a-primer/
-.. _virtualenv: https://virtualenv.pypa.io/en/stable/
-
-.. _GitHub web interface: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
-.. _GitHub's code editor: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
+============
+Contributing
+============
+
+Welcome to ``gantt-project-maker`` contributor's guide.
+
+This document focuses on getting any potential contributor familiarized
+with the development processes, but `other kinds of contributions`_ are also
+appreciated.
+
+If you are new to using git_ or have never collaborated in a project previously,
+please have a look at `contribution-guide.org`_. Other resources are also
+listed in the excellent `guide created by FreeCodeCamp`_ [#contrib1]_.
+
+Please notice, all users and contributors are expected to be **open,
+considerate, reasonable, and respectful**. When in doubt, `Python Software
+Foundation's Code of Conduct`_ is a good reference in terms of behavior
+guidelines.
+
+
+Issue Reports
+=============
+
+If you experience bugs or general issues with ``gantt-project-maker``, please have a look
+on the `issue tracker`_. If you don't see anything useful there, please feel
+free to fire an issue report.
+
+.. tip::
+   Please don't forget to include the closed issues in your search.
+   Sometimes a solution was already reported, and the problem is considered
+   **solved**.
+
+New issue reports should include information about your programming environment
+(e.g., operating system, Python version) and steps to reproduce the problem.
+Please try also to simplify the reproduction steps to a very minimal example
+that still illustrates the problem you are facing. By removing other factors,
+you help us to identify the root cause of the issue.
+
+
+Documentation Improvements
+==========================
+
+You can help improve ``gantt-project-maker`` docs by making them more readable and coherent, or
+by adding missing information and correcting mistakes.
+
+``gantt-project-maker`` documentation uses Sphinx_ as its main documentation compiler.
+This means that the docs are kept in the same repository as the project code, and
+that any documentation update is done in the same way was a code contribution.
+The documentation is written in reStructuredText_.
+
+   .. tip::
+      Please notice that the `GitHub web interface`_ provides a quick way of
+      propose changes in ``gantt-project-maker``'s files. While this mechanism can
+      be tricky for normal code contributions, it works perfectly fine for
+      contributing to the docs, and can be quite handy.
+
+      If you are interested in trying this method out, please navigate to
+      the ``docs`` folder in the source repository_, find which file you
+      would like to propose changes and click in the little pencil icon at the
+      top, to open `GitHub's code editor`_. Once you finish editing the file,
+      please write a message in the form at the bottom of the page describing
+      which changes have you made and what are the motivations behind them and
+      submit your proposal.
+
+When working on documentation changes in your local machine, you can
+compile them using |tox|_::
+
+    tox -e docs
+
+and use Python's built-in web server for a preview in your web browser
+(``http://localhost:8000``)::
+
+    python3 -m http.server --directory 'docs/_build/html'
+
+
+Code Contributions
+==================
+
+* The code is a front end to python-gantt_ project developed `Alexandre Norman`_, but as this project is not maintained
+  anymore.
+* The front end was written by `Eelco van Vliet`_
+* The gantt module has been included into this project and adapted where required.
+* A yaml file settings file is used to defined all the project and other properties
+* Task are added per project. See the User manual for more details
+
+
+Submit an issue
+---------------
+
+Before you work on any non-trivial code contribution it's best to first create
+a report in the `issue tracker`_ to start a discussion on the subject.
+This often provides additional considerations and avoids unnecessary work.
+
+Create an environment
+---------------------
+
+Before you start coding, we recommend creating an isolated `virtual
+environment`_ to avoid any problems with your installed Python packages.
+This can easily be done via either |virtualenv|_::
+
+    virtualenv <PATH TO VENV>
+    source <PATH TO VENV>/bin/activate
+
+or Miniconda_::
+
+    conda create -n gantt-project-maker python=3 six virtualenv pytest pytest-cov
+    conda activate gantt-project-maker
+
+Clone the repository
+--------------------
+
+#. Create an user account on |the repository service| if you do not already have one.
+#. Fork the project repository_: click on the *Fork* button near the top of the
+   page. This creates a copy of the code under your account on |the repository service|.
+#. Clone this copy to your local disk::
+
+    git clone git@github.com:eelcovv/gantt-project-maker.git
+    cd gantt-project-maker
+
+#. You should run::
+
+    pip install -U pip setuptools -e .
+
+   to be able to import the package under development in the Python REPL.
+
+#. Install |pre-commit|_::
+
+    pip install pre-commit
+    pre-commit install
+
+   ``gantt-project-maker`` comes with a lot of hooks configured to automatically help the
+   developer to check the code being written.
+
+Implement your changes
+----------------------
+
+#. Create a branch to hold your changes::
+
+    git checkout -b my-feature
+
+   and start making changes. Never work on the main branch!
+
+#. Start your work on this branch. Don't forget to add docstrings_ to new
+   functions, modules and classes, especially if they are part of public APIs.
+
+#. Add yourself to the list of contributors in ``AUTHORS.rst``.
+
+#. When you’re done editing, do::
+
+    git add <MODIFIED FILES>
+    git commit
+
+   to record your changes in git_.
+
+   Please make sure to see the validation messages from |pre-commit|_ and fix
+   any eventual issues.
+   This should automatically use flake8_/black_ to check/fix the code style
+   in a way that is compatible with the project.
+
+   .. important:: Don't forget to add unit tests and documentation in case your
+      contribution adds an additional feature and is not just a bugfix.
+
+      Moreover, writing a `descriptive commit message`_ is highly recommended.
+      In case of doubt, you can check the commit history with::
+
+         git log --graph --decorate --pretty=oneline --abbrev-commit --all
+
+      to look for recurring communication patterns.
+
+#. Please check that your changes don't break any unit tests with::
+
+    tox
+
+   (after having installed |tox|_ with ``pip install tox`` or ``pipx``).
+
+   You can also use |tox|_ to run several other pre-configured tasks in the
+   repository. Try ``tox -av`` to see a list of the available checks.
+
+Submit your contribution
+------------------------
+
+#. If everything works fine, push your local branch to |the repository service| with::
+
+    git push -u origin my-feature
+
+#. Go to the web page of your fork and click |contribute button|
+   to send your changes for review.
+
+   .. todo:: if you are using GitHub, you can uncomment the following paragraph
+
+      Find more detailed information in `creating a PR`_. You might also want to open
+      the PR as a draft first and mark it as ready for review after the feedbacks
+      from the continuous integration (CI) system or any required fixes.
+
+
+Troubleshooting
+---------------
+
+The following tips can be used when facing problems to build or test the
+package:
+
+#. Make sure to fetch all the tags from the upstream repository_.
+   The command ``git describe --abbrev=0 --tags`` should return the version you
+   are expecting. If you are trying to run CI scripts in a fork repository,
+   make sure to push all the tags.
+   You can also try to remove all the egg files or the complete egg folder, i.e.,
+   ``.eggs``, as well as the ``*.egg-info`` folders in the ``src`` folder or
+   potentially in the root of your project.
+
+#. Sometimes |tox|_ misses out when new dependencies are added, especially to
+   ``setup.cfg`` and ``docs/requirements.txt``. If you find any problems with
+   missing dependencies when running a command with |tox|_, try to recreate the
+   ``tox`` environment using the ``-r`` flag. For example, instead of::
+
+    tox -e docs
+
+   Try running::
+
+    tox -r -e docs
+
+#. Make sure to have a reliable |tox|_ installation that uses the correct
+   Python version (e.g., 3.7+). When in doubt you can run::
+
+    tox --version
+    # OR
+    which tox
+
+   If you have trouble and are seeing weird errors upon running |tox|_, you can
+   also try to create a dedicated `virtual environment`_ with a |tox|_ binary
+   freshly installed. For example::
+
+    virtualenv .venv
+    source .venv/bin/activate
+    .venv/bin/pip install tox
+    .venv/bin/tox -e all
+
+#. `Pytest can drop you`_ in an interactive session in the case an error occurs.
+   In order to do that you need to pass a ``--pdb`` option (for example by
+   running ``tox -- -k <NAME OF THE FALLING TEST> --pdb``).
+   You can also setup breakpoints manually instead of using the ``--pdb`` option.
+
+
+Maintainer tasks
+================
+
+Releases
+--------
+
+.. todo:: This section assumes you are using PyPI to publicly release your package.
+
+   If instead you are using a different/private package index, please update
+   the instructions accordingly.
+
+If you are part of the group of maintainers and have correct user permissions
+on PyPI_, the following steps can be used to release a new version for
+``gantt-project-maker``:
+
+#. Make sure all unit tests are successful.
+#. Tag the current commit on the main branch with a release tag, e.g., ``v1.2.3``.
+#. Push the new tag to the upstream repository_, e.g., ``git push upstream v1.2.3``
+#. Clean up the ``dist`` and ``build`` folders with ``tox -e clean``
+   (or ``rm -rf dist build``)
+   to avoid confusion with old builds and Sphinx docs.
+#. Run ``tox -e build`` and check that the files in ``dist`` have
+   the correct version (no ``.dirty`` or git_ hash) according to the git_ tag.
+   Also check the sizes of the distributions, if they are too big (e.g., >
+   500KB), unwanted clutter may have been accidentally included.
+#. Run ``tox -e publish -- --repository pypi`` and check that everything was
+   uploaded to PyPI_ correctly.
+
+
+
+.. [#contrib1] Even though, these resources focus on open source projects and
+   communities, the general ideas behind collaborating with other developers
+   to collectively create software are general and can be applied to all sorts
+   of environments, including private companies and proprietary code bases.
+
+
+.. <-- start -->
+
+.. |the repository service| replace:: GitHub
+.. |contribute button| replace:: "Create pull request"
+
+.. _repository: https://github.com/eelcovv/gantt-project-maker
+.. _issue tracker: https://github.com/eelcovv/gantt-project-maker/issues
+.. _python-gantt: https://pypi.org/project/python-gantt
+.. _Alexandre Norman: norman@xael.org
+.. _Eelco van Vliet: eelcovv@gmail.org
+.. <-- end -->
+
+
+.. |virtualenv| replace:: ``virtualenv``
+.. |pre-commit| replace:: ``pre-commit``
+.. |tox| replace:: ``tox``
+
+
+.. _black: https://pypi.org/project/black/
+.. _CommonMark: https://commonmark.org/
+.. _contribution-guide.org: https://www.contribution-guide.org/
+.. _creating a PR: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
+.. _descriptive commit message: https://chris.beams.io/posts/git-commit
+.. _docstrings: https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
+.. _first-contributions tutorial: https://github.com/firstcontributions/first-contributions
+.. _flake8: https://flake8.pycqa.org/en/stable/
+.. _git: https://git-scm.com
+.. _GitHub's fork and pull request workflow: https://guides.github.com/activities/forking/
+.. _guide created by FreeCodeCamp: https://github.com/FreeCodeCamp/how-to-contribute-to-open-source
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _MyST: https://myst-parser.readthedocs.io/en/latest/syntax/syntax.html
+.. _other kinds of contributions: https://opensource.guide/how-to-contribute
+.. _pre-commit: https://pre-commit.com/
+.. _PyPI: https://pypi.org/
+.. _PyScaffold's contributor's guide: https://pyscaffold.org/en/stable/contributing.html
+.. _Pytest can drop you: https://docs.pytest.org/en/stable/how-to/failures.html#using-python-library-pdb-with-pytest
+.. _Python Software Foundation's Code of Conduct: https://www.python.org/psf/conduct/
+.. _reStructuredText: https://www.sphinx-doc.org/en/master/usage/restructuredtext/
+.. _Sphinx: https://www.sphinx-doc.org/en/master/
+.. _tox: https://tox.wiki/en/stable/
+.. _virtual environment: https://realpython.com/python-virtual-environments-a-primer/
+.. _virtualenv: https://virtualenv.pypa.io/en/stable/
+
+.. _GitHub web interface: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
+.. _GitHub's code editor: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
```

### Comparing `gantt-project-maker-0.3.7/LICENSE.txt` & `gantt-project-maker-0.4.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Eelco van Vliet
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023 Eelco van Vliet
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `gantt-project-maker-0.3.7/PKG-INFO` & `gantt-project-maker-0.4.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,63 @@
-Metadata-Version: 2.1
-Name: gantt-project-maker
-Version: 0.3.7
-Summary: Create Gantt project charts
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: Eelco van Vliet
-Author-email: eelcovv@gmail.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE.txt
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-
-.. These are examples of badges you might want to add to your README:
-   please update the URLs accordingly
-
-    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://gantt-project-maker.readthedocs.io/en/stable/
-
-.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
-    :alt: Project generated with PyScaffold
-    :target: https://pyscaffold.org/
-
-|
-
-===================
-gantt-project-maker
-===================
-
-
-    A tool to make Gantt Project charts
-
-
-This tool is a front end to the Python module python-gantt in order to easily set up your projects
-
-
-.. _pyscaffold-notes:
-
-Note
-====
-
-This project has been set up using PyScaffold 4.5. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
+Metadata-Version: 2.1
+Name: gantt-project-maker
+Version: 0.4.2
+Summary: Create Gantt project charts
+Home-page: https://github.com/eelcovv/gantt-project-maker/
+Author: Eelco van Vliet
+Author-email: eelcovv@gmail.com
+License: MIT
+Project-URL: Documentation, https://gantt-project-maker.readthedocs.io/en/latest/
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: pandas
+Requires-Dist: python-dateutil
+Requires-Dist: PyYAML
+Requires-Dist: SVG42PDF
+Requires-Dist: svgwrite
+Requires-Dist: webcolors
+Requires-Dist: xlsxWriter
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: setuptools<=69.2.0; extra == "dev"
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+.. These are examples of badges you might want to add to your README:
+   please update the URLs accordingly
+
+    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
+        :alt: ReadTheDocs
+        :target: https://gantt-project-maker.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
+    :alt: Project generated with PyScaffold
+    :target: https://pyscaffold.org/
+
+|
+
+===================
+gantt-project-maker
+===================
+
+
+    A tool to make Gantt Project charts
+
+
+This tool is a front end to the Python module python-gantt in order to easily set up your projects
+
+
+.. _pyscaffold-notes:
+
+Note
+====
+
+This project has been set up using PyScaffold 4.5. For details and usage
+information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `gantt-project-maker-0.3.7/README.rst` & `gantt-project-maker-0.4.2/README.rst`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-.. These are examples of badges you might want to add to your README:
-   please update the URLs accordingly
-
-    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://gantt-project-maker.readthedocs.io/en/stable/
-
-.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
-    :alt: Project generated with PyScaffold
-    :target: https://pyscaffold.org/
-
-|
-
-===================
-gantt-project-maker
-===================
-
-
-    A tool to make Gantt Project charts
-
-
-This tool is a front end to the Python module python-gantt in order to easily set up your projects
-
-
-.. _pyscaffold-notes:
-
-Note
-====
-
-This project has been set up using PyScaffold 4.5. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
+.. These are examples of badges you might want to add to your README:
+   please update the URLs accordingly
+
+    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
+        :alt: ReadTheDocs
+        :target: https://gantt-project-maker.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
+    :alt: Project generated with PyScaffold
+    :target: https://pyscaffold.org/
+
+|
+
+===================
+gantt-project-maker
+===================
+
+
+    A tool to make Gantt Project charts
+
+
+This tool is a front end to the Python module python-gantt in order to easily set up your projects
+
+
+.. _pyscaffold-notes:
+
+Note
+====
+
+This project has been set up using PyScaffold 4.5. For details and usage
+information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `gantt-project-maker-0.3.7/docs/conf.py` & `gantt-project-maker-0.4.2/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,286 +1,288 @@
-# This file is execfile()d with the current directory set to its containing dir.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-import os
-import sys
-import shutil
-
-# -- Path setup --------------------------------------------------------------
-
-__location__ = os.path.dirname(__file__)
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.join(__location__, "../src"))
-
-# -- Run sphinx-apidoc -------------------------------------------------------
-# This hack is necessary since RTD does not issue `sphinx-apidoc` before running
-# `sphinx-build -b html . _build/html`. See Issue:
-# https://github.com/readthedocs/readthedocs.org/issues/1139
-# DON'T FORGET: Check the box "Install your project inside a virtualenv using
-# setup.py install" in the RTD Advanced Settings.
-# Additionally it helps us to avoid running apidoc manually
-
-try:  # for Sphinx >= 1.7
-    from sphinx.ext import apidoc
-except ImportError:
-    from sphinx import apidoc
-
-output_dir = os.path.join(__location__, "api")
-module_dir = os.path.join(__location__, "../src/gantt_project_maker")
-try:
-    shutil.rmtree(output_dir)
-except FileNotFoundError:
-    pass
-
-try:
-    import sphinx
-
-    cmd_line = f"sphinx-apidoc --implicit-namespaces -f -o {output_dir} {module_dir}"
-
-    args = cmd_line.split(" ")
-    if tuple(sphinx.__version__.split(".")) >= ("1", "7"):
-        # This is a rudimentary parse_version to avoid external dependencies
-        args = args[1:]
-
-    apidoc.main(args)
-except Exception as e:
-    print("Running `sphinx-apidoc` failed!\n{}".format(e))
-
-# -- General configuration ---------------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be extensions
-# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.todo",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.viewcode",
-    "sphinx.ext.coverage",
-    "sphinx.ext.doctest",
-    "sphinx.ext.ifconfig",
-    "sphinx.ext.mathjax",
-    "sphinx.ext.napoleon",
-]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix of source filenames.
-source_suffix = ".rst"
-
-# The encoding of source files.
-# source_encoding = 'utf-8-sig'
-
-# The master toctree document.
-master_doc = "index"
-
-# General information about the project.
-project = "gantt-project-maker"
-copyright = "2023, Eelco van Vliet"
-
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# version: The short X.Y version.
-# release: The full version, including alpha/beta/rc tags.
-# If you don’t need the separation provided between version and release,
-# just set them both to the same value.
-try:
-    from gantt_project_maker import __version__ as version
-except ImportError:
-    version = ""
-
-if not version or version.lower() == "unknown":
-    version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
-
-release = version
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-# language = None
-
-# There are two options for replacing |today|: either, you set today to some
-# non-false value, then it is used:
-# today = ''
-# Else, today_fmt is used as the format for a strftime call.
-# today_fmt = '%B %d, %Y'
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv"]
-
-# The reST default role (used for this markup: `text`) to use for all documents.
-# default_role = None
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-# add_function_parentheses = True
-
-# If true, the current module name will be prepended to all description
-# unit titles (such as .. function::).
-# add_module_names = True
-
-# If true, sectionauthor and moduleauthor directives will be shown in the
-# output. They are ignored by default.
-# show_authors = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# A list of ignored prefixes for module index sorting.
-# modindex_common_prefix = []
-
-# If true, keep warnings as "system message" paragraphs in the built documents.
-# keep_warnings = False
-
-# If this is True, todo emits a warning for each TODO entries. The default is False.
-todo_emit_warnings = True
-
-
-# -- Options for HTML output -------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-html_theme = "alabaster"
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
-
-# Add any paths that contain custom themes here, relative to this directory.
-# html_theme_path = []
-
-# The name for this set of Sphinx documents.  If None, it defaults to
-# "<project> v<release> documentation".
-# html_title = None
-
-# A shorter title for the navigation bar.  Default is the same as html_title.
-# html_short_title = None
-
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-# html_logo = ""
-
-# The name of an image file (within the static path) to use as favicon of the
-# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
-# pixels large.
-# html_favicon = None
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
-# using the given strftime format.
-# html_last_updated_fmt = '%b %d, %Y'
-
-# If true, SmartyPants will be used to convert quotes and dashes to
-# typographically correct entities.
-# html_use_smartypants = True
-
-# Custom sidebar templates, maps document names to template names.
-# html_sidebars = {}
-
-# Additional templates that should be rendered to pages, maps page names to
-# template names.
-# html_additional_pages = {}
-
-# If false, no module index is generated.
-# html_domain_indices = True
-
-# If false, no index is generated.
-# html_use_index = True
-
-# If true, the index is split into individual pages for each letter.
-# html_split_index = False
-
-# If true, links to the reST sources are added to the pages.
-# html_show_sourcelink = True
-
-# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-# html_show_sphinx = True
-
-# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-# html_show_copyright = True
-
-# If true, an OpenSearch description file will be output, and all pages will
-# contain a <link> tag referring to it.  The value of this option must be the
-# base URL from which the finished HTML is served.
-# html_use_opensearch = ''
-
-# This is the file name suffix for HTML files (e.g. ".xhtml").
-# html_file_suffix = None
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "gantt-project-maker-doc"
-
-
-# -- Options for LaTeX output ------------------------------------------------
-
-latex_elements = {
-    # The paper size ("letterpaper" or "a4paper").
-    # "papersize": "letterpaper",
-    # The font size ("10pt", "11pt" or "12pt").
-    # "pointsize": "10pt",
-    # Additional stuff for the LaTeX preamble.
-    # "preamble": "",
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [
-    ("index", "user_guide.tex", "gantt-project-maker Documentation", "Eelco van Vliet", "manual")
-]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-# latex_logo = ""
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-# latex_use_parts = False
-
-# If true, show page references after internal links.
-# latex_show_pagerefs = False
-
-# If true, show URL addresses after external links.
-# latex_show_urls = False
-
-# Documents to append as an appendix to all manuals.
-# latex_appendices = []
-
-# If false, no module index is generated.
-# latex_domain_indices = True
-
-# -- External mapping --------------------------------------------------------
-python_version = ".".join(map(str, sys.version_info[0:2]))
-intersphinx_mapping = {
-    "sphinx": ("https://www.sphinx-doc.org/en/master", None),
-    "python": ("https://docs.python.org/" + python_version, None),
-    "matplotlib": ("https://matplotlib.org", None),
-    "numpy": ("https://numpy.org/doc/stable", None),
-    "sklearn": ("https://scikit-learn.org/stable", None),
-    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
-    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
-    "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
-    "pyscaffold": ("https://pyscaffold.org/en/stable", None),
-}
-
-print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+# This file is execfile()d with the current directory set to its containing dir.
+#
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+import os
+import sys
+import shutil
+
+# -- Path setup --------------------------------------------------------------
+
+__location__ = os.path.dirname(__file__)
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+sys.path.insert(0, os.path.join(__location__, "../src"))
+
+# -- Run sphinx-apidoc -------------------------------------------------------
+# This hack is necessary since RTD does not issue `sphinx-apidoc` before running
+# `sphinx-build -b html . _build/html`. See Issue:
+# https://github.com/readthedocs/readthedocs.org/issues/1139
+# DON'T FORGET: Check the box "Install your project inside a virtualenv using
+# setup.py install" in the RTD Advanced Settings.
+# Additionally it helps us to avoid running apidoc manually
+
+try:  # for Sphinx >= 1.7
+    from sphinx.ext import apidoc
+except ImportError:
+    from sphinx import apidoc
+
+output_dir = os.path.join(__location__, "api")
+module_dir = os.path.join(__location__, "../src/gantt_project_maker")
+try:
+    shutil.rmtree(output_dir)
+except FileNotFoundError:
+    pass
+
+try:
+    import sphinx
+
+    cmd_line = f"sphinx-apidoc --implicit-namespaces -f -o {output_dir} {module_dir}"
+
+    args = cmd_line.split(" ")
+    if tuple(sphinx.__version__.split(".")) >= ("1", "7"):
+        # This is a rudimentary parse_version to avoid external dependencies
+        args = args[1:]
+
+    apidoc.main(args)
+except Exception as e:
+    print("Running `sphinx-apidoc` failed!\n{}".format(e))
+
+# -- General configuration ---------------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be extensions
+# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix of source filenames.
+source_suffix = ".rst"
+
+# The encoding of source files.
+# source_encoding = 'utf-8-sig'
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "gantt-project-maker"
+copyright = "2024, Eelco van Vliet"
+
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+#
+# version: The short X.Y version.
+# release: The full version, including alpha/beta/rc tags.
+# If you don’t need the separation provided between version and release,
+# just set them both to the same value.
+try:
+    from gantt_project_maker import __version__ as version
+except ImportError:
+    version = ""
+
+if not version or version.lower() == "unknown":
+    version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
+
+release = version
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+# language = None
+
+# There are two options for replacing |today|: either, you set today to some
+# non-false value, then it is used:
+# today = ''
+# Else, today_fmt is used as the format for a strftime call.
+# today_fmt = '%B %d, %Y'
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv"]
+
+# The reST default role (used for this markup: `text`) to use for all documents.
+# default_role = None
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+# add_function_parentheses = True
+
+# If true, the current module name will be prepended to all description
+# unit titles (such as .. function::).
+# add_module_names = True
+
+# If true, sectionauthor and moduleauthor directives will be shown in the
+# output. They are ignored by default.
+# show_authors = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# A list of ignored prefixes for module index sorting.
+# modindex_common_prefix = []
+
+# If true, keep warnings as "system message" paragraphs in the built documents.
+# keep_warnings = False
+
+# If this is True, todo emits a warning for each TODO entries. The default is False.
+todo_emit_warnings = True
+
+
+# -- Options for HTML output -------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+html_theme = "sphinx_rtd_theme"
+
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
+# documentation.
+
+# Add any paths that contain custom themes here, relative to this directory.
+# html_theme_path = []
+
+# The name for this set of Sphinx documents.  If None, it defaults to
+# "<project> v<release> documentation".
+# html_title = None
+
+# A shorter title for the navigation bar.  Default is the same as html_title.
+# html_short_title = None
+
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
+# html_logo = ""
+
+# The name of an image file (within the static path) to use as favicon of the
+# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
+# pixels large.
+# html_favicon = None
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
+# using the given strftime format.
+# html_last_updated_fmt = '%b %d, %Y'
+
+# If true, SmartyPants will be used to convert quotes and dashes to
+# typographically correct entities.
+# html_use_smartypants = True
+
+# Custom sidebar templates, maps document names to template names.
+# html_sidebars = {}
+
+# Additional templates that should be rendered to pages, maps page names to
+# template names.
+# html_additional_pages = {}
+
+# If false, no module index is generated.
+# html_domain_indices = True
+
+# If false, no index is generated.
+# html_use_index = True
+
+# If true, the index is split into individual pages for each letter.
+# html_split_index = False
+
+# If true, links to the reST sources are added to the pages.
+# html_show_sourcelink = True
+
+# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
+# html_show_sphinx = True
+
+# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
+# html_show_copyright = True
+
+# If true, an OpenSearch description file will be output, and all pages will
+# contain a <link> tag referring to it.  The value of this option must be the
+# base URL from which the finished HTML is served.
+# html_use_opensearch = ''
+
+# This is the file name suffix for HTML files (e.g. ".xhtml").
+# html_file_suffix = None
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "gantt-project-maker-doc"
+
+
+# -- Options for LaTeX output ------------------------------------------------
+
+latex_elements = {
+    # The paper size ("letterpaper" or "a4paper").
+    # "papersize": "letterpaper",
+    # The font size ("10pt", "11pt" or "12pt").
+    # "pointsize": "10pt",
+    # Additional stuff for the LaTeX preamble.
+    # "preamble": "",
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass [howto/manual]).
+latex_documents = [
+    (
+        "index",
+        "user_guide.tex",
+        "gantt-project-maker Documentation",
+        "Eelco van Vliet",
+        "manual",
+    )
+]
+
+# The name of an image file (relative to this directory) to place at the top of
+# the title page.
+# latex_logo = ""
+
+# For "manual" documents, if this is true, then toplevel headings are parts,
+# not chapters.
+# latex_use_parts = False
+
+# If true, show page references after internal links.
+# latex_show_pagerefs = False
+
+# If true, show URL addresses after external links.
+# latex_show_urls = False
+
+# Documents to append as an appendix to all manuals.
+# latex_appendices = []
+
+# If false, no module index is generated.
+# latex_domain_indices = True
+
+# -- External mapping --------------------------------------------------------
+python_version = ".".join(map(str, sys.version_info[0:2]))
+intersphinx_mapping = {
+    "sphinx": ("https://www.sphinx-doc.org/en/master", None),
+    "python": ("https://docs.python.org/" + python_version, None),
+    "matplotlib": ("https://matplotlib.org", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "sklearn": ("https://scikit-learn.org/stable", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
+    "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
+    "pyscaffold": ("https://pyscaffold.org/en/stable", None),
+}
+
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `gantt-project-maker-0.3.7/examples/Makefile` & `gantt-project-maker-0.4.2/examples/Makefile`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-resources_dir = output_resources
-planning_dir = output_planning
-excel_dir = output_excel
-
-# define targets
-target_global = $(planning_dir)/projects_all_tasks.svg
-target_excel = $(excel_dir)/projects.xlsx
-target_resources = $(resources_dir)/projects_all_resources.svg
-targets_emp1 = $(planning_dir)/projects_emp1_all_tasks.svg
-targets_emp2 = $(planning_dir)/projects_emp2_all_tasks.svg
-targets_emp3 = $(planning_dir)/projects_emp3_all_tasks.svg
-
-targets_emp1_resources = $(resources_dir)/projects_emp1_all_resources.svg
-targets_emp2_resources = $(resources_dir)/projects_emp2_all_resources.svg
-targets_emp3_resources = $(resources_dir)/projects_emp3_all_resources.svg
-
-all_targets_tasks = $(target_global) \
-					$(targets_emp1) \
-					$(targets_emp2) \
-					$(targets_emp3) \
-all_targets_resources = $(target_resources) \
-						$(targets_emp1_resources) \
-						$(targets_emp2_resources) \
-						$(targets_emp3_resources) \
-
-targets = $(all_targets_resources) $(all_targets_tasks) $(target_excel)
-
-settings_file_global = projects.yml
-settings_file_emp1 = projects_emp1.yml
-settings_file_emp2 = projects_emp2.yml
-settings_file_emp3 = projects_emp3.yml
-
-settings_files = $(settings_file_global) \
-				 $(settings_file_emp1) \
-				 $(settings_file_emp2) \
-				 $(settings_file_emp3)
-
-executable = gantt_project_maker
-
-# default wordt alleen de volledige tijdsperiode gemaakt. Wil je ook 'einde_jaar' hebben, geef dan
-# OPTIONS="--period einde_jaar"
-# mee op de command line
-default_options = --period all
-
-ifdef OPTIONS
-	options=$(default_options) $(OPTIONS)
-else
-	options=$(default_options)
-endif
-
-default: all
-
-all_tasks: global emp1 emp2 emp3 xlsx
-all_resources: resources emp1_resources emp2_resources emp3_resources
-
-all: all_tasks all_resources
-
-resources: $(target_resources)
-$(target_resources): $(settings_files)
-	$(executable)  $(settings_file_global)  $(options) --resources
-
-
-xlsx: $(target_excel)
-$(target_excel): $(settings_files)
-	$(executable)  $(settings_file_global)  $(options) --export
-
-global: $(target_global)
-$(target_global): $(settings_files)
-	$(executable)  $(settings_file_global)  $(options)
-
-emp1: $(targets_emp1)
-$(targets_emp1): $(settings_file_emp1)
-	$(executable)  $(settings_file_global)  $(options) --employee emp1
-
-emp1_resources: $(targets_emp1_resources)
-$(targets_emp1_resources): $(settings_file_emp1)
-	$(executable)  $(settings_file_global)  $(options) --employee emp1 --resources
-
-emp2: $(targets_emp2)
-$(targets_emp2): $(settings_file_emp2)
-	$(executable)  $(settings_file_global)  $(options) --employee emp2
-
-emp2_resources: $(targets_emp2_resources)
-$(targets_emp2_resources): $(settings_file_emp2)
-	$(executable)  $(settings_file_global)  $(options) --employee emp2 --resources
-
-emp3: $(targets_emp3)
-$(targets_emp3): $(settings_file_emp3)
-	$(executable)  $(settings_file_global)  $(options) --employee emp3
-
-emp3_resources: $(targets_emp3_resources)
-$(targets_emp3_resources): $(settings_file_emp3)
-	$(executable)  $(settings_file_global)  $(options) --employee emp3 --resources
-
-clean_task:
-	@$(foreach file, $(all_targets_tasks), test -f $(file) && rm -v $(file) || echo No $(file);)
-
-clean_resources:
-	@$(foreach file, $(all_targets_resources), test -f $(file) && rm -v $(file) || echo No $(file);)
-
-clean_excel:
-	@$(foreach file, $(target_excel), test -f $(file) && rm -v $(file) || echo No $(file);)
-
-clean: clean_resources clean_task clean_excel
+resources_dir = output_resources
+planning_dir = output_planning
+excel_dir = output_excel
+
+# define targets
+target_global = $(planning_dir)/projects_all_tasks.svg
+target_excel = $(excel_dir)/projects.xlsx
+target_resources = $(resources_dir)/projects_all_resources.svg
+targets_emp1 = $(planning_dir)/projects_emp1_all_tasks.svg
+targets_emp2 = $(planning_dir)/projects_emp2_all_tasks.svg
+targets_emp3 = $(planning_dir)/projects_emp3_all_tasks.svg
+
+targets_emp1_resources = $(resources_dir)/projects_emp1_all_resources.svg
+targets_emp2_resources = $(resources_dir)/projects_emp2_all_resources.svg
+targets_emp3_resources = $(resources_dir)/projects_emp3_all_resources.svg
+
+all_targets_tasks = $(target_global) \
+					$(targets_emp1) \
+					$(targets_emp2) \
+					$(targets_emp3) \
+all_targets_resources = $(target_resources) \
+						$(targets_emp1_resources) \
+						$(targets_emp2_resources) \
+						$(targets_emp3_resources) \
+
+targets = $(all_targets_resources) $(all_targets_tasks) $(target_excel)
+
+settings_file_global = projects.yml
+settings_file_emp1 = projects_emp1.yml
+settings_file_emp2 = projects_emp2.yml
+settings_file_emp3 = projects_emp3.yml
+
+settings_files = $(settings_file_global) \
+				 $(settings_file_emp1) \
+				 $(settings_file_emp2) \
+				 $(settings_file_emp3)
+
+executable = gantt_project_maker
+
+# default wordt alleen de volledige tijdsperiode gemaakt. Wil je ook 'einde_jaar' hebben, geef dan
+# OPTIONS="--period einde_jaar"
+# mee op de command line
+default_options = --period all
+
+ifdef OPTIONS
+	options=$(default_options) $(OPTIONS)
+else
+	options=$(default_options)
+endif
+
+default: all
+
+all_tasks: global emp1 emp2 emp3 xlsx
+all_resources: resources emp1_resources emp2_resources emp3_resources
+
+all: all_tasks all_resources
+
+resources: $(target_resources)
+$(target_resources): $(settings_files)
+	$(executable)  $(settings_file_global)  $(options) --resources
+
+
+xlsx: $(target_excel)
+$(target_excel): $(settings_files)
+	$(executable)  $(settings_file_global)  $(options) --export
+
+global: $(target_global)
+$(target_global): $(settings_files)
+	$(executable)  $(settings_file_global)  $(options)
+
+emp1: $(targets_emp1)
+$(targets_emp1): $(settings_file_emp1)
+	$(executable)  $(settings_file_global)  $(options) --employee emp1
+
+emp1_resources: $(targets_emp1_resources)
+$(targets_emp1_resources): $(settings_file_emp1)
+	$(executable)  $(settings_file_global)  $(options) --employee emp1 --resources
+
+emp2: $(targets_emp2)
+$(targets_emp2): $(settings_file_emp2)
+	$(executable)  $(settings_file_global)  $(options) --employee emp2
+
+emp2_resources: $(targets_emp2_resources)
+$(targets_emp2_resources): $(settings_file_emp2)
+	$(executable)  $(settings_file_global)  $(options) --employee emp2 --resources
+
+emp3: $(targets_emp3)
+$(targets_emp3): $(settings_file_emp3)
+	$(executable)  $(settings_file_global)  $(options) --employee emp3
+
+emp3_resources: $(targets_emp3_resources)
+$(targets_emp3_resources): $(settings_file_emp3)
+	$(executable)  $(settings_file_global)  $(options) --employee emp3 --resources
+
+clean_task:
+	@$(foreach file, $(all_targets_tasks), test -f $(file) && rm -v $(file) || echo No $(file);)
+
+clean_resources:
+	@$(foreach file, $(all_targets_resources), test -f $(file) && rm -v $(file) || echo No $(file);)
+
+clean_excel:
+	@$(foreach file, $(target_excel), test -f $(file) && rm -v $(file) || echo No $(file);)
+
+clean: clean_resources clean_task clean_excel
```

### Comparing `gantt-project-maker-0.3.7/examples/employees.yml` & `gantt-project-maker-0.4.2/examples/employees.yml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-emp1:
-  name: Employee One
-  color: cyan
-  vacations:
-    spring_holiday_23:
-      label: Spring vacation '23
-      start: 2-2-2023
-      end: 23-2-2023
-    summer_holiday_23:
-      label: Summer holiday '23
-      start: 18-7-2023
-      end: 13-8-2023
-emp2:
-  name: Employee Two
-  color: khaki
-  vacations:
-    summer_holiday_23:
-      label: Summer holiday '23
-      start: 10-7-2023
-      end: 28-7-2023
-emp3:
-  name: Employee Three
-  color: plum
-  vacations:
-    summer_holiday_23:
-      label: Summer holiday '23
-      start: 31-7-2023
-      end: 4-8-2023
-emp4:
-  name: Employee Four
-  color: bisque
-  vacations:
-    summer_holiday_23:
-      label: Summer holiday '23
-      start: 1-8-2023
-      end: 16-8-2023
-emp5:
-  name: Employee Five
-  color: mistyrose
-  vacations:
-    summer_holiday_23:
-      label: Summer holiday '23
-      start: 1-8-2023
-      end: 16-8-2023
-emp6:
-  name: Employee Six
-  color: lavender
-emp7:
-  name: Employee Seven
-  color: dodgerblue
-emp8:
-  name: Employee Eight
-department1:
-  name: Department One
-  color: wheat
-default:
-  name: Default employee
-  color: orange
+emp1:
+  name: Employee One
+  color: cyan
+  vacations:
+    spring_holiday_23:
+      label: Spring vacation '23
+      start: 2-2-2023
+      end: 23-2-2023
+    summer_holiday_23:
+      label: Summer holiday '23
+      start: 18-7-2023
+      end: 13-8-2023
+emp2:
+  name: Employee Two
+  color: khaki
+  vacations:
+    summer_holiday_23:
+      label: Summer holiday '23
+      start: 10-7-2023
+      end: 28-7-2023
+emp3:
+  name: Employee Three
+  color: plum
+  vacations:
+    summer_holiday_23:
+      label: Summer holiday '23
+      start: 31-7-2023
+      end: 4-8-2023
+emp4:
+  name: Employee Four
+  color: bisque
+  vacations:
+    summer_holiday_23:
+      label: Summer holiday '23
+      start: 1-8-2023
+      end: 16-8-2023
+emp5:
+  name: Employee Five
+  color: mistyrose
+  vacations:
+    summer_holiday_23:
+      label: Summer holiday '23
+      start: 1-8-2023
+      end: 16-8-2023
+emp6:
+  name: Employee Six
+  color: lavender
+emp7:
+  name: Employee Seven
+  color: dodgerblue
+emp8:
+  name: Employee Eight
+department1:
+  name: Department One
+  color: wheat
+default:
+  name: Default employee
+  color: orange
```

### Comparing `gantt-project-maker-0.3.7/examples/projects_emp3.yml` & `gantt-project-maker-0.4.2/examples/projects_emp3.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,109 @@
-general:
-  title: Project Leader Three
-  color: blue
-  projects:
-    - all_project
-projects:
-  project_1:
-    title: Project One 2022
-    color: corporatelichtblauw
-    project_leader: PL1
-    department1: "Yes"
-    cci: "No"
-    remark: "Check with Bob"
-    tasks:
-      request_documents:
-        label: Request documents
-        start: 7-8-2023
-        end: 1-9-2023
-        project_leader: emp3
-        department1: "Yes"
-        cci: "No"
-        remark: Priority
-        employees:
-          - emp3
-      prepare_request:
-        label: Prepare request
-        start: 1-7-2023
-        end: 21-7-2023
-        project_leader: emp3
-        remark: Priority
-        employees:
-          - emp3
-      finish_project:
-        label: Finish project
-        start: 1-9-2023
-        end: 17-9-2023
-        project_leader: emp3
-        remark: Priority
-        employees:
-          - emp3
-  project_2:
-    title: Project Two 2022
-    title_collapsed: Long description of project two 2022
-    employees_collapsed: "default"
-    color: yellow
-    project_leader: PL1
-    department1: "Yes"
-    cci: "No"
-    remark: "Check with Bob"
-    tasks:
-      do_something:
-        label: Do something
-        start: 4-5-2023
-        end: 20-5-2023
-        project_leader: emp3
-        department1: "Yes"
-        cci: "No"
-        remark: Priority
-        employees:
-          - emp3
-      another_thing:
-        label: Do something else
-        start: 5-6-2023
-        end: 21-7-2023
-        project_leader: emp3
-        remark: Priority
-        employees:
-          - emp3
-      last_thing:
-        label: Final thing of project 2
-        start: 1-7-2023
-        end: 1-8-2023
-        project_leader: emp3
-        remark: Priority
-        employees:
-          - emp3
-  all_project:
-    title: All projects of major project
-    color: red
-    project_leader: PL3
-    tasks:
-      - project_1
-      - project_2
+general:
+  title: Project Leader Three
+  color: blue
+  projects:
+    - all_project
+    - side_project
+variables:
+  year: 2023
+  year_plus_one: 2024
+projects:
+  project_1:
+    title: Project One {{ year }}
+    color: corporatelichtblauw
+    project_leader: PL1
+    department1: "Yes"
+    cci: "No"
+    remark: "Check with Bob"
+    tasks:
+      request_documents:
+        label: Request documents
+        start: 7-8-2023
+        end: 1-9-2023
+        project_leader: emp3
+        department1: "Yes"
+        cci: "No"
+        remark: Priority
+        employees:
+          - emp3
+      prepare_request:
+        label: Prepare request
+        start: 1-7-2023
+        end: 21-7-2023
+        project_leader: emp3
+        remark: Priority
+        employees:
+          - emp3
+      finish_project:
+        label: Finish project
+        start: 1-9-2023
+        end: 17-9-2023
+        project_leader: emp3
+        remark: Priority
+        employees:
+          - emp3
+  project_2:
+    title: Project Two 2022
+    title_collapsed: Long description of project two 2022
+    employees_collapsed: "default"
+    color: yellow
+    project_leader: PL1
+    department1: "Yes"
+    cci: "No"
+    remark: "Check with Bob"
+    tasks:
+      do_something:
+        label: Do something
+        start: 4-5-2023
+        end: 20-5-2023
+        project_leader: emp3
+        department1: "Yes"
+        cci: "No"
+        remark: Priority
+        employees:
+          - emp3
+      another_thing:
+        label: Do something else
+        start: 5-6-2023
+        end: 21-7-2023
+        project_leader: emp3
+        remark: Priority
+        employees:
+          - emp3
+      last_thing:
+        label: Final thing of project 2
+        start: 1-7-2023
+        end: 1-8-2023
+        project_leader: emp3
+        remark: Priority
+        employees:
+          - emp3
+  all_project:
+    title: All projects of major project
+    color: red
+    project_leader: PL3
+    tasks:
+      - project_1
+      - project_2
+  side_project:
+    title:  A long side project in {{ year }}
+    color: green
+    project_leader: PL4
+    tasks:
+      short_task:
+        label: A short task for {{ year }}
+        start: 1-8-2023
+        end: 10-8-2023
+        remark: Priority
+        employees:
+          emp4: 30
+      long_task:
+        label: A long task for {{ year_plus_one }}
+        start: 1-9-2023
+        end: 10-11-2023
+        project_leader: emp3
+        remark: Priority
+        employees:
+          emp3: 30
+          emp4: 100
+          emp5: 50
```

### Comparing `gantt-project-maker-0.3.7/setup.py` & `gantt-project-maker-0.4.2/setup.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-    Setup file for gantt-project-maker.
-    Use setup.cfg to configure your project.
-
-    This file was generated with PyScaffold 4.5.
-    PyScaffold helps you to put up the scaffold of your new Python project.
-    Learn more under: https://pyscaffold.org/
-"""
-from setuptools import setup
-
-if __name__ == "__main__":
-    try:
-        setup(use_scm_version={"version_scheme": "no-guess-dev"})
-    except:  # noqa
-        print(
-            "\n\nAn error occurred while building the project, "
-            "please ensure you have the most updated version of setuptools, "
-            "setuptools_scm and wheel with:\n"
-            "   pip install -U setuptools setuptools_scm wheel\n\n"
-        )
-        raise
+"""
+    Setup file for gantt-project-maker.
+    Use setup.cfg to configure your project.
+
+    This file was generated with PyScaffold 4.5.
+    PyScaffold helps you to put up the scaffold of your new Python project.
+    Learn more under: https://pyscaffold.org/
+"""
+from setuptools import setup
+
+if __name__ == "__main__":
+    try:
+        setup(use_scm_version={"version_scheme": "no-guess-dev"})
+    except:  # noqa
+        print(
+            "\n\nAn error occurred while building the project, "
+            "please ensure you have the most updated version of setuptools, "
+            "setuptools_scm and wheel with:\n"
+            "   pip install -U setuptools setuptools_scm wheel\n\n"
+        )
+        raise
```

### Comparing `gantt-project-maker-0.3.7/src/gantt_project_maker/__init__.py` & `gantt-project-maker-0.4.2/src/gantt_project_maker/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import sys
-
-if sys.version_info[:2] >= (3, 8):
-    # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
-    from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
-else:
-    from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
-
-try:
-    # Change here if project is renamed and does not equal the package name
-    dist_name = "gantt-project-maker"
-    __version__ = version(dist_name)
-except PackageNotFoundError:  # pragma: no cover
-    __version__ = "unknown"
-finally:
-    del version, PackageNotFoundError
+import sys
+
+if sys.version_info[:2] >= (3, 8):
+    # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
+    from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
+else:
+    from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
+
+try:
+    # Change here if project is renamed and does not equal the package name
+    dist_name = "gantt-project-maker"
+    __version__ = version(dist_name)
+except PackageNotFoundError:  # pragma: no cover
+    __version__ = "unknown"
+finally:
+    del version, PackageNotFoundError
```

### Comparing `gantt-project-maker-0.3.7/src/gantt_project_maker/colors.py` & `gantt-project-maker-0.4.2/src/gantt_project_maker/colors.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-Definition of CBS rbg colors. Based on the color rgb definitions from the cbs LaTeX template
-"""
-
-import logging
-
-import webcolors
-
-_logger = logging.getLogger(__name__)
-
-
-# A bit tricky, but we use it to store the custom colors
-CUSTOM_COLORS_HEX = {}
-
-
-def hex_number_to_hex_hash(hex_number):
-    """
-    Args:
-        hex_number: int or str
-            Hexadecimal representation of a color, with or without a leading #
-
-    Returns: str
-        Hexadecimal color with a leading #
-    """
-    hex_code = str(hex_number)
-    if set(list(hex_code.upper())).difference(set(list("1234567890ABCDEF#"))):
-        raise ValueError(
-            f"Hex color {hex_code} is not valid as it contains characters out of the valid range"
-        )
-    if not hex_code.startswith("#"):
-        if "#" in hex_code:
-            raise ValueError(
-                f"Hex color {hex_code} is not valid as the # is not at the start"
-            )
-        hex_code = f"#{hex_code}"
-    if len(hex_code) != 7:
-        raise ValueError(
-            f"Hex color {hex_code} is not valid as is has an invalid amount of digit "
-        )
-    return hex_code
-
-
-def set_custom_colors(custom_colors):
-    """Set the hex colors defined in the dictionary to the global variable CUSTOM_COLORS_HEX"""
-    for color_name, color_hex in custom_colors.items():
-        CUSTOM_COLORS_HEX[color_name] = hex_number_to_hex_hash(color_hex)
-
-
-def color_to_hex(color: str):
-    """Convert a named color into a hex code with a leading #"""
-    color_hex_code = None
-    if color is not None:
-        try:
-            color_hex_code = CUSTOM_COLORS_HEX[color]
-            _logger.debug(f"color {color} met cbs colors omgezet naar {color_hex_code}")
-        except KeyError:
-            try:
-                color_hex_code = webcolors.name_to_hex(color)
-                _logger.debug(
-                    f"color {color} met webcolors omgezet naar {color_hex_code}"
-                )
-            except (AttributeError, ValueError) as err:
-                color_hex_code = hex_number_to_hex_hash(color)
-
-    return color_hex_code
+"""
+Definition of CBS rbg colors. Based on the color rgb definitions from the cbs LaTeX template
+"""
+
+import logging
+
+import webcolors
+
+_logger = logging.getLogger(__name__)
+
+
+# A bit tricky, but we use it to store the custom colors
+CUSTOM_COLORS_HEX = {}
+
+
+def hex_number_to_hex_hash(hex_number):
+    """
+    Args:
+        hex_number: int or str
+            Hexadecimal representation of a color, with or without a leading #
+
+    Returns: str
+        Hexadecimal color with a leading #
+    """
+    hex_code = str(hex_number)
+    if set(list(hex_code.upper())).difference(set(list("1234567890ABCDEF#"))):
+        raise ValueError(
+            f"Hex color {hex_code} is not valid as it contains characters out of the valid range"
+        )
+    if not hex_code.startswith("#"):
+        if "#" in hex_code:
+            raise ValueError(
+                f"Hex color {hex_code} is not valid as the # is not at the start"
+            )
+        hex_code = f"#{hex_code}"
+    if len(hex_code) != 7:
+        raise ValueError(
+            f"Hex color {hex_code} is not valid as is has an invalid amount of digit "
+        )
+    return hex_code
+
+
+def set_custom_colors(custom_colors):
+    """Set the hex colors defined in the dictionary to the global variable CUSTOM_COLORS_HEX"""
+    for color_name, color_hex in custom_colors.items():
+        CUSTOM_COLORS_HEX[color_name] = hex_number_to_hex_hash(color_hex)
+
+
+def color_to_hex(color: str):
+    """Convert a named color into a hex code with a leading #"""
+    color_hex_code = None
+    if color is not None:
+        try:
+            color_hex_code = CUSTOM_COLORS_HEX[color]
+            _logger.debug(f"color {color} met cbs colors omgezet naar {color_hex_code}")
+        except KeyError:
+            try:
+                color_hex_code = webcolors.name_to_hex(color)
+                _logger.debug(
+                    f"color {color} met webcolors omgezet naar {color_hex_code}"
+                )
+            except (AttributeError, ValueError) as err:
+                color_hex_code = hex_number_to_hex_hash(color)
+
+    return color_hex_code
```

### Comparing `gantt-project-maker-0.3.7/src/gantt_project_maker/main.py` & `gantt-project-maker-0.4.2/src/gantt_project_maker/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,569 +1,624 @@
-"""
-This is the main start up file of the project planner
-"""
-
-import argparse
-import codecs
-import locale
-import logging
-import sys
-from datetime import datetime
-from pathlib import Path
-
-import dateutil.parser as dparse
-import yaml
-
-from gantt_project_maker import __version__
-from gantt_project_maker.colors import set_custom_colors
-from gantt_project_maker.project_classes import (
-    ProjectPlanner,
-    SCALES,
-    parse_date,
-    extend_suffix,
-)
-
-__author__ = "Eelco van Vliet"
-__copyright__ = "Eelco van Vliet"
-__license__ = "MIT"
-
-_logger = logging.getLogger(__name__)
-
-
-############################################################################
-
-
-def get_info_from_file_or_settings(settings, key):
-    """
-    Get the information directly from the settings or from a separate file if a filename is given
-    Parameters
-    ----------
-    settings: dict
-        Settings file
-    key: str
-        Key of the settings file we want to read
-
-    Returns
-    -------
-    dict:
-        Structure with information from the settings or separate file
-
-    """
-    information = settings[key]
-
-    if isinstance(information, str):
-        with codecs.open(information, "r", encoding="UTF-8") as stream:
-            information = yaml.load(stream=stream, Loader=yaml.Loader)
-
-    return information
-
-
-def get_pasted_employees(args_employee, employees_info):
-    """get the list of full names or requested employees and return as a comma separated string"""
-    all_employees = []
-    for employee in args_employee:
-        employee_name = get_employee_name(employees_info, employee)
-        all_employees.append(employee_name)
-    all_employees = ", ".join(all_employees)
-    return all_employees
-
-
-def get_employee_name(employees_info, employee):
-    """get the full name of the employee from the settings file"""
-    try:
-        request_employee = employees_info[employee]
-    except KeyError as err:
-        _logger.warning(err)
-        raise KeyError(
-            f"Employee {employee} given via argument is not find in section 'employees' "
-            f"in settings file. Please add this employee to your settings"
-        )
-    else:
-        try:
-            request_name = request_employee["name"]
-        except KeyError as err:
-            _logger.warning(err)
-            raise KeyError("'name' not given for employee {request_employee} ")
-
-    return request_name
-
-
-def check_if_date(value):
-    """check if an argument is a valid date. Return the original string value"""
-    try:
-        date = dparse.parse(value).date()
-    except ValueError:
-        raise argparse.ArgumentTypeError(f"Date {value} is not a valid date")
-    return value
-
-
-def parse_args(args):
-    """Parse command line parameters
-
-    Args:
-      args (List[str]): command line parameters as list of strings
-          (for example  ``["--help"]``).
-
-    Returns:
-      :obj:`argparse.Namespace`: command line parameters namespace
-    """
-
-    parser = argparse.ArgumentParser(
-        description="A front end to the python-gantt project planning"
-    )
-    parser.add_argument("settings_filename", help="Name of the configuration file")
-    parser.add_argument("--output_filename", help="Name of the text output file")
-    parser.add_argument(
-        "--version",
-        action="version",
-        version=f"gantt_project_maker {__version__}",
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        dest="loglevel",
-        help="set loglevel to INFO",
-        action="store_const",
-        const=logging.INFO,
-        default=logging.INFO,
-    )
-    parser.add_argument(
-        "-vv",
-        "--debug",
-        dest="loglevel",
-        help="set loglevel to DEBUG",
-        action="store_const",
-        const=logging.DEBUG,
-    )
-    parser.add_argument(
-        "-q",
-        "--quiet",
-        dest="loglevel",
-        help="set loglevel to WARNING",
-        action="store_const",
-        const=logging.WARNING,
-    )
-    parser.add_argument(
-        "-vvv",
-        "--very_verbose",
-        help="Also show the logging of the gantt module",
-        action="store_true",
-    )
-    parser.add_argument(
-        "-s",
-        "--scale",
-        help="The scale of the grid of the project scheme",
-        choices=set(SCALES.keys()),
-    )
-    parser.add_argument(
-        "--details",
-        help="Add all the tasks with the detail attribute",
-        action="store_true",
-        default=True,
-    )
-    parser.add_argument(
-        "--no_details",
-        help="Suppress all the tasks with the detail attribute.",
-        action="store_false",
-        dest="details",
-    )
-    parser.add_argument(
-        "-e",
-        "--export_to_xlsx",
-        help="Export the project plan to Excel",
-        action="store_true",
-    )
-    parser.add_argument(
-        "-c",
-        "--collaps_tasks",
-        help="Collaps the tasks per project to one task to remove details",
-        action="store_true",
-    )
-    parser.add_argument(
-        "-b",
-        "--resources",
-        help="Write the resources file of the planning",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--vacations",
-        help="Write the vacations file of all the  employees",
-        action="store_true",
-    )
-    parser.add_argument(
-        "-m",
-        "--employee",
-        help="Only use the projects of this employee. Can be given multiple times for multiple "
-        "employees.",
-        action="append",
-    )
-    parser.add_argument(
-        "-f",
-        "--filter_employees",
-        help="Only include tasks to which this employee contributes. Can be given multiple times for multiple "
-        "employees.",
-        action="append",
-    )
-    parser.add_argument(
-        "-p",
-        "--period",
-        help="On export this period from the list of periods as given in the settings file. If "
-        "not given, all the periods are writen to file",
-        action="append",
-    )
-    parser.add_argument(
-        "--start_planning",
-        type=check_if_date,
-        help="Start of the planning. If not given, the value given in de settings file is taken",
-    )
-    parser.add_argument(
-        "--end_planning",
-        type=check_if_date,
-        help="End of the planning. If not given, the value given in de settings file is taken",
-    )
-    parser.add_argument(
-        "--weeks_margin_left",
-        type=int,
-        help="Shifts start of planning with this number of weeks left without adding projects. Default is read "
-        "from the settings file. This value overrides the default",
-    )
-    parser.add_argument(
-        "--weeks_margin_right",
-        type=int,
-        help="Shifts start of planning with this number of weeks right without adding projects. Default is read "
-        "from the settings file. This value overrides the default.",
-    )
-    parser.add_argument("--pdf", help="Save the svg also as pdf ", action="store_true")
-
-    return parser.parse_args(args)
-
-
-def setup_logging(loglevel):
-    """Setup basic logging
-
-    Args:
-      loglevel (int): minimum loglevel for emitting messages
-    """
-    if loglevel == logging.DEBUG:
-        log_format = "[%(levelname)5s]:%(filename)s/%(lineno)d: %(message)s"
-    else:
-        log_format = "[%(levelname)s] %(message)s"
-    logging.basicConfig(
-        level=loglevel,
-        stream=sys.stdout,
-        format=log_format,
-        datefmt="%Y-%m-%d %H:%M:%S",
-    )
-
-
-def check_if_items_are_available(requested_items, available_items, label=""):
-    """
-    Check is the passed items in the list are available in the keys of the dictionary
-
-    Parameters
-    ----------
-    requested_items: list
-        All requested items  in the list
-    available_items: dict
-        The dictionary with the keys
-    label: str
-        Used for information to the screen
-
-    """
-    unique_available_items = set(list(available_items.keys()))
-    if missing_items := set(requested_items).difference(unique_available_items):
-        raise ValueError(
-            f"The {label} {missing_items} are not defined in the settings file.\n"
-            f"The following keys are available: {unique_available_items}"
-        )
-    return True
-
-
-def make_banner(width=80) -> None:
-    """
-    Make a banner with the start time
-    Args:
-        width:  int
-            With of the banner
-
-    Returns:
-    """
-    print("-" * 80)
-    exe = Path(sys.argv[0]).stem
-    now = datetime.now()
-    print(
-        f"Start '{exe} {' '.join(sys.argv[1:])}'\nat {now.date()} {now.time().strftime('%H:%M')} "
-    )
-    print("-" * 80)
-
-
-def main(args):
-    args = parse_args(args)
-
-    if args.loglevel < logging.WARNING:
-        make_banner()
-
-    setup_logging(args.loglevel)
-    if args.very_verbose:
-        gantt_logger = logging.getLogger("Gantt")
-        gantt_logger.setLevel(args.loglevel)
-
-    _logger.info("Reading settings file {}".format(args.settings_filename))
-    with codecs.open(args.settings_filename, "r", encoding="UTF-8") as stream:
-        settings = yaml.load(stream=stream, Loader=yaml.Loader)
-
-    general_settings = settings["general"]
-    try:
-        project_settings_per_project_leader = settings[
-            "project_settings_file_per_employee"
-        ]
-    except KeyError as err:
-        _logger.warning(err)
-        raise KeyError(
-            "Entry project_settings_file_per_employee not found. Are you sure this"
-            "is the main settingsfile and not the settings file of an employee?"
-        )
-    period_info = settings["periods"]
-    dayfirst = general_settings["dayfirst"]
-
-    if args.scale is not None:
-        scale_key = args.scale
-    else:
-        scale_key = general_settings.get("scale", "daily")
-    scale = SCALES[scale_key]
-
-    if args.start_planning is None:
-        start = parse_date(general_settings["planning_start"], dayfirst=dayfirst)
-    else:
-        start = parse_date(args.start_planning, dayfirst=dayfirst)
-    if args.end_planning is None:
-        end = parse_date(general_settings["planning_end"], dayfirst=dayfirst)
-    else:
-        end = parse_date(args.end_planning, dayfirst=dayfirst)
-
-    if args.weeks_margin_left is None:
-        weeks_margin_left = general_settings.get("weeks_margin_left")
-    else:
-        weeks_margin_left = args.weeks_margin_left
-
-    if args.weeks_margin_right is None:
-        weeks_margin_right = general_settings.get("weeks_margin_right")
-    else:
-        weeks_margin_right = args.weeks_margin_right
-
-    programma_title = general_settings["title"]
-    programma_color = general_settings.get("color")
-    vacation_color = general_settings.get("vacation_color", programma_color)
-    output_directories = general_settings.get("output_directories")
-    excel_info = settings.get("excel")
-    employees_info = get_info_from_file_or_settings(settings=settings, key="employees")
-    vacations_info = get_info_from_file_or_settings(settings=settings, key="vacations")
-
-    if args.employee:
-        all_employees = get_pasted_employees(
-            args.employee, employees_info=employees_info
-        )
-        programma_title += f"/{all_employees}"
-
-    if args.filter_employees:
-        all_filter_employees = get_pasted_employees(
-            args.filter_employees, employees_info=employees_info
-        )
-        programma_title += f": {all_filter_employees}"
-
-    fill = "black"
-    stroke = "black"
-    stroke_width = 0
-    font_family = "Verdana"
-    if font_info := general_settings.get("font_info"):
-        fill = font_info.get("fill", fill)
-        stroke = font_info.get("stroke", stroke)
-        stroke_width = font_info.get("stroke_width", stroke_width)
-        font_family = font_info.get("font_family", font_family)
-
-    if custom_colors := general_settings.get("custom_colors"):
-        set_custom_colors(custom_colors=custom_colors)
-
-    vacations_title_default = "Vacations"
-    if country_code := general_settings.get("country_code"):
-        locale.setlocale(locale.LC_TIME, country_code)
-        if country_code.startswith("nl"):
-            vacations_title_default = "Vakanties"
-    vacations_title = general_settings.get("vacations_title", vacations_title_default)
-
-    if output_directories is not None:
-        planning_directory = Path(output_directories.get("planning", "."))
-        resources_directory = Path(output_directories.get("resources", "."))
-        excel_directory = Path(output_directories.get("excel", "."))
-        vacations_directory = Path(output_directories.get("vacations", "."))
-    else:
-        planning_directory = Path(".")
-        resources_directory = Path(".")
-        excel_directory = Path(".")
-        vacations_directory = Path(".")
-
-    if args.employee is not None:
-        check_if_items_are_available(
-            requested_items=args.employee,
-            available_items=project_settings_per_project_leader,
-            label="employee project",
-        )
-    if args.filter_employees is not None:
-        check_if_items_are_available(
-            requested_items=args.filter_employees,
-            available_items=employees_info,
-            label="employee task",
-        )
-
-    if args.period is not None:
-        check_if_items_are_available(
-            requested_items=args.period, available_items=period_info, label="period"
-        )
-
-    # read the settings file per employee
-    settings_per_project_leader = {}
-    for (
-        project_leader_key,
-        employee_settings_file,
-    ) in project_settings_per_project_leader.items():
-        _logger.info(
-            f"Reading settings file {employee_settings_file} of  employee {project_leader_key}"
-        )
-        with codecs.open(employee_settings_file, "r", encoding="UTF-8") as stream:
-            settings_per_project_leader[project_leader_key] = yaml.load(
-                stream=stream, Loader=yaml.Loader
-            )
-
-    if args.output_filename is None:
-        output_filename = Path(args.settings_filename).with_suffix(".svg")
-        # add employees from input arguments to output file name
-        if args.employee is not None:
-            output_filename = extend_suffix(
-                output_filename=output_filename, extensions=args.employee
-            )
-
-        # add filtered employees from input arguments to output file name
-        if args.filter_employees is not None:
-            extensions = ["contributors"] + sorted(args.filter_employees)
-            output_filename = extend_suffix(
-                output_filename=output_filename, extensions=extensions
-            )
-    else:
-        # just use the output filename as defined on the command line
-        output_filename = Path(args.output_filename).with_suffix(".svg")
-
-    today = None
-    try:
-        today_reference = general_settings["reference_date"]
-    except KeyError:
-        _logger.debug("No date found")
-    else:
-        if today_reference is not None:
-            if today_reference == "today":
-                today = datetime.today().date()
-                _logger.debug("Setting date to today {}".format(today))
-            else:
-                today = parse_date(today_reference, dayfirst=dayfirst)
-                _logger.debug("Setting date to {}".format(today))
-        else:
-            _logger.debug("today key found be no date defined")
-
-    # Begin de planning
-    planning = ProjectPlanner(
-        programma_title=programma_title,
-        vacations_title=vacations_title,
-        programma_color=programma_color,
-        vacation_color=vacation_color,
-        output_file_name=output_filename,
-        planning_start=start,
-        planning_end=end,
-        weeks_margin_left=weeks_margin_left,
-        weeks_margin_right=weeks_margin_right,
-        today=today,
-        dayfirst=dayfirst,
-        scale=scale,
-        period_info=period_info,
-        excel_info=excel_info,
-        details=args.details,
-        filter_employees=args.filter_employees,
-        save_svg_as_pdf=args.pdf,
-        collaps_tasks=args.collaps_tasks,
-        periods=args.period,
-    )
-
-    # add global information, vacations and employees
-    planning.add_global_information(
-        fill=fill, stroke=stroke, stroke_width=stroke_width, font_family=font_family
-    )
-    planning.add_vacations(vacations_info=vacations_info)
-    planning.add_employees(employees_info=employees_info)
-
-    # Add the general tasks per employee. It is not mandatory to add tasks_and_milestones,
-    # however, you may. The advantage is that multiply tasks can share the same milestone
-    for (
-        project_leader_key,
-        project_leader_settings,
-    ) in settings_per_project_leader.items():
-        if tasks_and_milestones_info := project_leader_settings.get(
-            "tasks_and_milestones"
-        ):
-            _logger.info(f"Adding global tasks en milestones of {project_leader_key} ")
-            planning.add_tasks_and_milestones(
-                tasks_and_milestones_info=tasks_and_milestones_info
-            )
-
-    # Voeg nu de projecten per employee toe.
-    for (
-        project_leader_key,
-        project_leader_settings,
-    ) in settings_per_project_leader.items():
-        if args.employee is not None and project_leader_key not in args.employee:
-            _logger.debug(f"Skip employee {project_leader_key}")
-            continue
-
-        project_employee_info = project_leader_settings["general"]
-        subprojects_info = project_leader_settings["projects"]
-
-        subprojects_selection = project_employee_info["projects"]
-        subprojects_title = project_employee_info["title"]
-        subprojects_color = project_employee_info.get("color")
-        planning.make_projects(
-            subprojects_info=subprojects_info,
-            subprojects_selection=subprojects_selection,
-            subprojects_title=subprojects_title,
-            subprojects_color=subprojects_color,
-        )
-
-    # Everything has been added to the planning. Write it to file
-    planning.write_planning(
-        write_resources=args.resources,
-        write_vacations=args.vacations,
-        planning_output_directory=planning_directory,
-        resource_output_directory=resources_directory,
-        vacations_output_directory=vacations_directory,
-        periods=args.period,
-    )
-
-    if args.export_to_xlsx:
-        planning.export_to_excel(excel_output_directory=excel_directory)
-
-
-def run():
-    """Calls :func:`main` passing the CLI arguments extracted from :obj:`sys.argv`
-
-    This function can be used as entry point to create console scripts with setuptools.
-    """
-    main(sys.argv[1:])
-
-
-if __name__ == "__main__":
-    # ^  This is a guard statement that will prevent the following code from
-    #    being executed in the case someone imports this file instead of
-    #    executing it as a script.
-    #    https://docs.python.org/3/library/__main__.html
-
-    # After installing your project with pip, users can also run your Python
-    # modules as scripts via the ``-m`` flag, as defined in PEP 338::
-    #
-    #     python -m gantt_projectplanner.skeleton 42
-    #
-    run()
+"""
+This is the main start-up file of the project planner
+"""
+
+import argparse
+import codecs
+import locale
+import logging
+import sys
+from datetime import datetime
+from pathlib import Path
+
+import yaml
+
+from gantt_project_maker import __version__
+from gantt_project_maker.colors import set_custom_colors
+from gantt_project_maker.project_classes import (
+    ProjectPlanner,
+    SCALES,
+    parse_date,
+    extend_suffix,
+)
+from gantt_project_maker.utils import check_if_date
+
+__author__ = "Eelco van Vliet"
+__copyright__ = "Eelco van Vliet"
+__license__ = "MIT"
+
+_logger = logging.getLogger(__name__)
+
+
+############################################################################
+
+
+def get_info_from_file_or_settings(settings, key):
+    """
+    Get the information directly from the settings or from a separate file if a filename is given
+    Parameters
+    ----------
+    settings: dict
+        Settings file
+    key: str
+        Key of the settings file we want to read
+
+    Returns
+    -------
+    dict:
+        Structure with information from the settings or separate file
+
+    """
+    information = settings[key]
+
+    if isinstance(information, str):
+        with codecs.open(information, "r", encoding="UTF-8") as stream:
+            information = yaml.load(stream=stream, Loader=yaml.Loader)
+
+    return information
+
+
+def get_pasted_employees(args_employee, employees_info):
+    """get the list of full names or requested employees and return as a comma separated string"""
+    all_employees = []
+    for employee in args_employee:
+        employee_name = get_employee_name(employees_info, employee)
+        all_employees.append(employee_name)
+    all_employees = ", ".join(all_employees)
+    return all_employees
+
+
+def get_employee_name(employees_info, employee):
+    """get the full name of the employee from the settings file"""
+    try:
+        request_employee = employees_info[employee]
+    except KeyError as err:
+        _logger.warning(err)
+        raise KeyError(
+            f"Employee {employee} given via argument is not find in section 'employees' "
+            f"in settings file. Please add this employee to your settings"
+        )
+    else:
+        try:
+            request_name = request_employee["name"]
+        except KeyError as err:
+            _logger.warning(err)
+            raise KeyError("'name' not given for employee {request_employee} ")
+
+    return request_name
+
+
+def parse_args(args):
+    """Parse command line parameters
+
+    Args:
+      args (List[str]): command line parameters as a list of strings
+          (for example, ``["--help"]``).
+
+    Returns:
+      obj:`argparse.Namespace`: command line parameters namespace
+    """
+
+    parser = argparse.ArgumentParser(
+        description="A front end to the python-gantt project planning"
+    )
+    parser.add_argument("settings_filename", help="Name of the configuration file")
+    parser.add_argument("--output_filename", help="Name of the text output file")
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=f"gantt_project_maker {__version__}",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        dest="loglevel",
+        help="set loglevel to INFO",
+        action="store_const",
+        const=logging.INFO,
+        default=logging.INFO,
+    )
+    parser.add_argument(
+        "-vv",
+        "--debug",
+        dest="loglevel",
+        help="set loglevel to DEBUG",
+        action="store_const",
+        const=logging.DEBUG,
+    )
+    parser.add_argument(
+        "-q",
+        "--quiet",
+        dest="loglevel",
+        help="set loglevel to WARNING",
+        action="store_const",
+        const=logging.WARNING,
+    )
+    parser.add_argument(
+        "-vvv",
+        "--very_verbose",
+        help="Also show the logging of the gantt module",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-s",
+        "--scale",
+        help="The scale of the grid of the project scheme",
+        choices=set(SCALES.keys()),
+    )
+    parser.add_argument(
+        "--details",
+        help="Add all the tasks with the detail attribute",
+        action="store_true",
+        default=True,
+    )
+    parser.add_argument(
+        "--no_details",
+        help="Suppress all the tasks with the detail attribute.",
+        action="store_false",
+        dest="details",
+    )
+    parser.add_argument(
+        "-e",
+        "--export_to_xlsx",
+        help="Export the project plan to Excel",
+        action="append",
+        nargs="*",
+    )
+    parser.add_argument(
+        "-c",
+        "--collaps_tasks",
+        help="Collaps the tasks per project to one task to remove details",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-b",
+        "--resources",
+        help="Write the resources file of the planning",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--vacations",
+        help="Write the vacations file of all the  employees",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-m",
+        "--employee",
+        help="Only use the projects of this employee. Can be given multiple times for multiple "
+        "employees.",
+        action="append",
+    )
+    parser.add_argument(
+        "-f",
+        "--filter_employees",
+        help="Only include tasks to which this employee contributes. Can be given multiple times for multiple "
+        "employees.",
+        action="append",
+    )
+    parser.add_argument(
+        "--projects",
+        help="Only include the main project given in this list. Argument can be given multiple times for multiple "
+        "projects to include. Alternatively, a comma-separated list of projects may be given. If not given, "
+        "all projects defined under 'projects' will be included.",
+        action="append",
+    )
+    parser.add_argument(
+        "-p",
+        "--period",
+        help="On export this period from the list of periods as given in the settings file. If "
+        "not given, all the periods are writen to file",
+        action="append",
+    )
+    parser.add_argument(
+        "--start_planning",
+        type=check_if_date,
+        help="Start of the planning. If not given, the value given in de settings file is taken",
+    )
+    parser.add_argument(
+        "--end_planning",
+        type=check_if_date,
+        help="End of the planning. If not given, the value given in de settings file is taken",
+    )
+    parser.add_argument(
+        "--weeks_margin_left",
+        type=int,
+        help="Shifts start of planning with this number of weeks left without adding projects. Default is read "
+        "from the settings file. This value overrides the default",
+    )
+    parser.add_argument(
+        "--weeks_margin_right",
+        type=int,
+        help="Shifts start of planning with this number of weeks right without adding projects. Default is read "
+        "from the settings file. This value overrides the default.",
+    )
+    parser.add_argument("--suffix", help="Add a suffix to the final output filename ")
+    parser.add_argument("--pdf", help="Save the svg also as pdf ", action="store_true")
+
+    return parser.parse_args(args)
+
+
+def setup_logging(loglevel: int):
+    """Setup basic logging
+
+    Args:
+      loglevel (int): minimum loglevel for emitting messages
+    """
+    if loglevel == logging.DEBUG:
+        log_format = "[%(levelname)5s]:%(filename)s/%(lineno)d: %(message)s"
+    else:
+        log_format = "[%(levelname)s] %(message)s"
+    logging.basicConfig(
+        level=loglevel,
+        stream=sys.stdout,
+        format=log_format,
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
+
+
+def check_if_items_are_available(
+    requested_items: list, available_items: dict, label: str = ""
+):
+    """
+    Check is the passed items in the list are available in the keys of the dictionary
+
+    Args:
+    requested_items (list): All requested items in the list
+    available_items (dict): The dictionary with the keys for which the check is performed
+    label (str, optional): Used for information to the screen
+
+    """
+    unique_available_items = set(list(available_items.keys()))
+    if missing_items := set(requested_items).difference(unique_available_items):
+        raise ValueError(
+            f"The {label} {missing_items} are not defined in the settings file.\n"
+            f"The following keys are available: {unique_available_items}"
+        )
+    return True
+
+
+def get_projects_from_arguments(projects_args) -> list or None:
+    """
+    Get the projects from the command line arguments and return a list
+
+    Args:
+        projects_args (list or None): The list of projects may contain comma-separated values
+
+    Returns:
+        list or None: The list of projects
+    """
+
+    projects = None
+    if projects_args is not None:
+        projects = list()
+        for project in projects_args:
+            all_projects = project.split(",")
+            projects.extend(all_projects)
+    return projects
+
+
+def make_banner(width=80) -> None:
+    """
+    Make a banner with the start time
+    Args:
+        width (int, optional): Width of the banner.
+        Defaults to 80
+    """
+    print("-" * width)
+    exe = Path(sys.argv[0]).stem
+    now = datetime.now()
+    print(
+        f"Start '{exe} {' '.join(sys.argv[1:])}'\nat {now.date()} {now.time().strftime('%H:%M')} "
+    )
+    print("-" * width)
+
+
+def main(args):
+    """Wrapper allowing: func:`postal_code2nuts` to be called with string arguments in a CLI fashion
+
+    Instead of returning the value from: func:`postal_code2nuts`, it prints the result to the
+    ``stdout`` in a nicely formatted message.
+
+    Args:
+      args (List[str]): command line parameters as a list of strings
+          (for example, ``["--verbose", "42"]``).
+    """
+
+    args = parse_args(args)
+
+    if args.loglevel < logging.WARNING:
+        make_banner()
+
+    setup_logging(args.loglevel)
+    if args.very_verbose:
+        gantt_logger = logging.getLogger("Gantt")
+        gantt_logger.setLevel(args.loglevel)
+
+    _logger.info("Reading settings file {}".format(args.settings_filename))
+    with codecs.open(args.settings_filename, "r", encoding="UTF-8") as stream:
+        settings = yaml.load(stream=stream, Loader=yaml.Loader)
+
+    general_settings = settings["general"]
+    try:
+        project_settings_per_project_leader = settings[
+            "project_settings_file_per_employee"
+        ]
+    except KeyError as err:
+        _logger.warning(err)
+        raise KeyError(
+            "Entry project_settings_file_per_employee not found. Are you sure this"
+            "is the main settingsfile and not the settings file of an employee?"
+        )
+    period_info = settings["periods"]
+    dayfirst = general_settings["dayfirst"]
+
+    if args.scale is not None:
+        scale_key = args.scale
+    else:
+        scale_key = general_settings.get("scale", "daily")
+    scale = SCALES[scale_key]
+
+    if args.start_planning is None:
+        start = parse_date(general_settings["planning_start"], dayfirst=dayfirst)
+    else:
+        start = parse_date(args.start_planning, dayfirst=dayfirst)
+    if args.end_planning is None:
+        end = parse_date(general_settings["planning_end"], dayfirst=dayfirst)
+    else:
+        end = parse_date(args.end_planning, dayfirst=dayfirst)
+
+    if args.weeks_margin_left is None:
+        weeks_margin_left = general_settings.get("weeks_margin_left")
+    else:
+        weeks_margin_left = args.weeks_margin_left
+
+    if args.weeks_margin_right is None:
+        weeks_margin_right = general_settings.get("weeks_margin_right")
+    else:
+        weeks_margin_right = args.weeks_margin_right
+
+    programma_title = general_settings["title"]
+    programma_color = general_settings.get("color")
+    vacation_color = general_settings.get("vacation_color", programma_color)
+    output_directories = general_settings.get("output_directories")
+    excel_info = settings.get("excel")
+    employees_info = get_info_from_file_or_settings(settings=settings, key="employees")
+    vacations_info = get_info_from_file_or_settings(settings=settings, key="vacations")
+
+    if args.employee:
+        all_employees = get_pasted_employees(
+            args.employee, employees_info=employees_info
+        )
+        programma_title += f"/{all_employees}"
+
+    if args.filter_employees:
+        all_filter_employees = get_pasted_employees(
+            args.filter_employees, employees_info=employees_info
+        )
+        programma_title += f": {all_filter_employees}"
+
+    filter_projects = get_projects_from_arguments(args.projects)
+
+    fill = "black"
+    stroke = "black"
+    stroke_width = 0
+    font_family = "Verdana"
+    if font_info := general_settings.get("font_info"):
+        fill = font_info.get("fill", fill)
+        stroke = font_info.get("stroke", stroke)
+        stroke_width = font_info.get("stroke_width", stroke_width)
+        font_family = font_info.get("font_family", font_family)
+
+    if custom_colors := general_settings.get("custom_colors"):
+        set_custom_colors(custom_colors=custom_colors)
+
+    vacations_title_default = "Vacations"
+    if country_code := general_settings.get("country_code"):
+        locale.setlocale(locale.LC_TIME, country_code)
+        if country_code.startswith("nl"):
+            vacations_title_default = "Vakanties"
+    vacations_title = general_settings.get("vacations_title", vacations_title_default)
+
+    if output_directories is not None:
+        planning_directory = Path(output_directories.get("planning", "."))
+        resources_directory = Path(output_directories.get("resources", "."))
+        excel_directory = Path(output_directories.get("excel", "."))
+        vacations_directory = Path(output_directories.get("vacations", "."))
+    else:
+        planning_directory = Path(".")
+        resources_directory = Path(".")
+        excel_directory = Path(".")
+        vacations_directory = Path(".")
+
+    if args.employee is not None:
+        check_if_items_are_available(
+            requested_items=args.employee,
+            available_items=project_settings_per_project_leader,
+            label="employee project",
+        )
+    if args.filter_employees is not None:
+        check_if_items_are_available(
+            requested_items=args.filter_employees,
+            available_items=employees_info,
+            label="employee task",
+        )
+
+    if args.period is not None:
+        check_if_items_are_available(
+            requested_items=args.period, available_items=period_info, label="period"
+        )
+
+    # read the settings file per employee
+    settings_per_project_leader = {}
+    for (
+        project_leader_key,
+        employee_settings_file,
+    ) in project_settings_per_project_leader.items():
+        if args.employee is not None and project_leader_key not in args.employee:
+            _logger.debug(
+                f"Skip reading settings file for employee {project_leader_key}"
+            )
+            continue
+
+        _logger.info(
+            f"Reading settings file {employee_settings_file} of  employee {project_leader_key}"
+        )
+        with codecs.open(employee_settings_file, encoding="UTF-8") as stream:
+            settings_per_project_leader[project_leader_key] = yaml.load(
+                stream=stream, Loader=yaml.Loader
+            )
+
+    if args.output_filename is None:
+        output_filename = Path(args.settings_filename).with_suffix(".svg")
+        # add employees from input arguments to output file name
+        if args.employee is not None:
+            output_filename = extend_suffix(
+                output_filename=output_filename, extensions=args.employee
+            )
+
+        # add filtered employees from input arguments to output file name
+        if args.filter_employees is not None:
+            extensions = ["contributors"] + sorted(args.filter_employees)
+            output_filename = extend_suffix(
+                output_filename=output_filename, extensions=extensions
+            )
+    else:
+        # Treat the output filename as defined on the command line
+        output_filename = Path(args.output_filename).with_suffix(".svg")
+
+    today = None
+    try:
+        today_reference = general_settings["reference_date"]
+    except KeyError:
+        _logger.debug("No date found")
+    else:
+        if today_reference is not None:
+            if today_reference == "today":
+                today = datetime.today().date()
+                _logger.debug("Setting date to today {}".format(today))
+            else:
+                today = parse_date(today_reference, dayfirst=dayfirst)
+                _logger.debug("Setting date to {}".format(today))
+        else:
+            _logger.debug("today key found be no date defined")
+
+    # Begin de planning
+    planning = ProjectPlanner(
+        programma_title=programma_title,
+        vacations_title=vacations_title,
+        programma_color=programma_color,
+        vacation_color=vacation_color,
+        output_file_name=output_filename,
+        planning_start=start,
+        planning_end=end,
+        weeks_margin_left=weeks_margin_left,
+        weeks_margin_right=weeks_margin_right,
+        today=today,
+        dayfirst=dayfirst,
+        scale=scale,
+        period_info=period_info,
+        excel_info=excel_info,
+        details=args.details,
+        filter_employees=args.filter_employees,
+        save_svg_as_pdf=args.pdf,
+        collaps_tasks=args.collaps_tasks,
+        periods=args.period,
+    )
+
+    # add global information, vacations and employees
+    planning.add_global_information(
+        fill=fill, stroke=stroke, stroke_width=stroke_width, font_family=font_family
+    )
+    planning.add_vacations(vacations_info=vacations_info)
+    planning.add_employees(employees_info=employees_info)
+
+    # Add the general tasks per employee. It is not mandatory to add tasks_and_milestones,
+    # however, you may. The advantage is that multiply tasks can share the same milestone
+    for (
+        project_leader_key,
+        project_leader_settings,
+    ) in settings_per_project_leader.items():
+        if tasks_and_milestones_info := project_leader_settings.get(
+            "tasks_and_milestones"
+        ):
+            _logger.info(f"Adding global tasks en milestones of {project_leader_key} ")
+            variables_info = project_leader_settings.get("variables")
+            planning.add_tasks_and_milestones(
+                tasks_and_milestones_info=tasks_and_milestones_info,
+                variables_info=variables_info,
+            )
+
+    # Voeg nu de projecten per employee toe.
+    for (
+        project_leader_key,
+        project_leader_settings,
+    ) in settings_per_project_leader.items():
+        if args.employee is not None and project_leader_key not in args.employee:
+            _logger.debug(f"Skip employee {project_leader_key}")
+            continue
+
+        project_employee_info = project_leader_settings["general"]
+        subprojects_info = project_leader_settings["projects"]
+        variables_info = project_leader_settings.get("variables")
+
+        subprojects_selection = project_employee_info["projects"]
+        subprojects_title = project_employee_info["title"]
+        subprojects_color = project_employee_info.get("color")
+        if filter_projects is not None:
+            # in case a project is given on the command line argument, only allow projects given on the filter.
+            subprojects_selection = list(
+                set(subprojects_selection).intersection(set(filter_projects))
+            )
+        if subprojects_selection:
+            planning.make_projects(
+                project_leader_key=project_leader_key,
+                subprojects_info=subprojects_info,
+                subprojects_selection=subprojects_selection,
+                subprojects_title=subprojects_title,
+                subprojects_color=subprojects_color,
+                variables_info=variables_info,
+            )
+
+    # Everything has been added to the planning. Write it to file
+    planning.write_planning(
+        write_resources=args.resources,
+        write_vacations=args.vacations,
+        planning_output_directory=planning_directory,
+        resource_output_directory=resources_directory,
+        vacations_output_directory=vacations_directory,
+        periods=args.period,
+        suffix=args.suffix,
+    )
+
+    planning.make_resource_dataframe()
+
+    if args.export_to_xlsx is not None:
+        if args.export_to_xlsx[0]:
+            excel_output_formats = [out for out in args.export_to_xlsx[0]]
+        else:
+            excel_output_formats = ["all"]
+        planning.export_to_excel(
+            excel_output_directory=excel_directory,
+            excel_output_formats=excel_output_formats,
+        )
+
+
+def run():
+    """Calls: func:`main` passing the CLI arguments extracted from: obj:`sys.argv`
+
+    This function can be used as an entry point to create console scripts with setuptools.
+    """
+    main(sys.argv[1:])
+
+
+if __name__ == "__main__":
+    # ^ This is a guard statement that will prevent the following code from
+    #    being executed in the case someone imports this file instead of
+    #    executing it as a script.
+    #    https://docs.python.org/3/library/__main__.html
+
+    # After installing your project with pip, users can also run your Python
+    # modules as scripts via the ``-m`` flag, as defined in PEP 338::
+    #
+    #     python -m gantt_projectplanner.skeleton 42
+    #
+    run()
```

### Comparing `gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/PKG-INFO` & `gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,63 @@
-Metadata-Version: 2.1
-Name: gantt-project-maker
-Version: 0.3.7
-Summary: Create Gantt project charts
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: Eelco van Vliet
-Author-email: eelcovv@gmail.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE.txt
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-
-.. These are examples of badges you might want to add to your README:
-   please update the URLs accordingly
-
-    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
-        :alt: ReadTheDocs
-        :target: https://gantt-project-maker.readthedocs.io/en/stable/
-
-.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
-    :alt: Project generated with PyScaffold
-    :target: https://pyscaffold.org/
-
-|
-
-===================
-gantt-project-maker
-===================
-
-
-    A tool to make Gantt Project charts
-
-
-This tool is a front end to the Python module python-gantt in order to easily set up your projects
-
-
-.. _pyscaffold-notes:
-
-Note
-====
-
-This project has been set up using PyScaffold 4.5. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
+Metadata-Version: 2.1
+Name: gantt-project-maker
+Version: 0.4.2
+Summary: Create Gantt project charts
+Home-page: https://github.com/eelcovv/gantt-project-maker/
+Author: Eelco van Vliet
+Author-email: eelcovv@gmail.com
+License: MIT
+Project-URL: Documentation, https://gantt-project-maker.readthedocs.io/en/latest/
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: pandas
+Requires-Dist: python-dateutil
+Requires-Dist: PyYAML
+Requires-Dist: SVG42PDF
+Requires-Dist: svgwrite
+Requires-Dist: webcolors
+Requires-Dist: xlsxWriter
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: setuptools<=69.2.0; extra == "dev"
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+.. These are examples of badges you might want to add to your README:
+   please update the URLs accordingly
+
+    .. image:: https://readthedocs.org/projects/gantt-project-maker/badge/?version=latest
+        :alt: ReadTheDocs
+        :target: https://gantt-project-maker.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
+    :alt: Project generated with PyScaffold
+    :target: https://pyscaffold.org/
+
+|
+
+===================
+gantt-project-maker
+===================
+
+
+    A tool to make Gantt Project charts
+
+
+This tool is a front end to the Python module python-gantt in order to easily set up your projects
+
+
+.. _pyscaffold-notes:
+
+Note
+====
+
+This project has been set up using PyScaffold 4.5. For details and usage
+information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `gantt-project-maker-0.3.7/src/gantt_project_maker.egg-info/SOURCES.txt` & `gantt-project-maker-0.4.2/src/gantt_project_maker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 pyproject.toml
@@ -31,14 +32,15 @@
 examples/vacations.yml
 src/gantt_project_maker/__init__.py
 src/gantt_project_maker/colors.py
 src/gantt_project_maker/excelwriter.py
 src/gantt_project_maker/gantt.py
 src/gantt_project_maker/main.py
 src/gantt_project_maker/project_classes.py
+src/gantt_project_maker/utils.py
 src/gantt_project_maker.egg-info/PKG-INFO
 src/gantt_project_maker.egg-info/SOURCES.txt
 src/gantt_project_maker.egg-info/dependency_links.txt
 src/gantt_project_maker.egg-info/entry_points.txt
 src/gantt_project_maker.egg-info/not-zip-safe
 src/gantt_project_maker.egg-info/requires.txt
 src/gantt_project_maker.egg-info/top_level.txt
```

### Comparing `gantt-project-maker-0.3.7/tests/test_main.py` & `gantt-project-maker-0.4.2/tests/test_main.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import pytest
-
-from gantt_project_maker.main import check_if_items_are_available
-
-__author__ = "Eelco van Vliet"
-__copyright__ = "Eelco van Vliet"
-__license__ = "MIT"
-
-
-def test_check_if_items_are_available():
-    """API Tests if check succeeds"""
-
-    input_list = ["A", "B"]
-    available_dict = {"A": 0, "B": 1, "C": 2}
-
-    assert check_if_items_are_available(
-        requested_items=input_list, available_items=available_dict, label="test1"
-    )
-
-
-def test_check_if_items_are_available_error():
-    """API Tests if check files. Should raise a value error"""
-
-    input_list = ["A", "B", "D"]
-    available_dict = {"A": 0, "B": 1, "C": 2}
-    with pytest.raises(ValueError):
-        check_if_items_are_available(
-            requested_items=input_list, available_items=available_dict, label="test2"
-        )
+import pytest
+
+from gantt_project_maker.main import check_if_items_are_available
+
+__author__ = "Eelco van Vliet"
+__copyright__ = "Eelco van Vliet"
+__license__ = "MIT"
+
+
+def test_check_if_items_are_available():
+    """API Tests if check succeeds"""
+
+    input_list = ["A", "B"]
+    available_dict = {"A": 0, "B": 1, "C": 2}
+
+    assert check_if_items_are_available(
+        requested_items=input_list, available_items=available_dict, label="test1"
+    )
+
+
+def test_check_if_items_are_available_error():
+    """API Tests if check files. Should raise a value error"""
+
+    input_list = ["A", "B", "D"]
+    available_dict = {"A": 0, "B": 1, "C": 2}
+    with pytest.raises(ValueError):
+        check_if_items_are_available(
+            requested_items=input_list, available_items=available_dict, label="test2"
+        )
```

### Comparing `gantt-project-maker-0.3.7/tests/test_project_classes.py` & `gantt-project-maker-0.4.2/tests/test_project_classes.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pytest
-import dateutil.parser as dparse
-
-from gantt_project_maker.project_classes import get_nearest_saturday, parse_date
-
-__author__ = "Eelco van Vliet"
-__copyright__ = "Eelco van Vliet"
-__license__ = "MIT"
-
-
-def test_parse_date():
-    date = "25-12-2023"
-    assert parse_date(date, dayfirst=True) == dparse.parse(date, dayfirst=True).date()
-    assert (
-        parse_date(None, date_default=date, dayfirst=True)
-        == dparse.parse(date, dayfirst=True).date()
-    )
-
-
-def test_nearest_saturday():
-    """API Tests if check succeeds"""
-
-    date = parse_date("25-12-2023", dayfirst=True)
-    assert get_nearest_saturday(date) == parse_date("23-12-2023", dayfirst=True)
-
-    date = parse_date("28-12-2023", dayfirst=True)
-    assert get_nearest_saturday(date) == parse_date("30-12-2023", dayfirst=True)
+import pytest
+import dateutil.parser as dparse
+
+from gantt_project_maker.project_classes import get_nearest_saturday, parse_date
+
+__author__ = "Eelco van Vliet"
+__copyright__ = "Eelco van Vliet"
+__license__ = "MIT"
+
+
+def test_parse_date():
+    date = "25-12-2023"
+    assert parse_date(date, dayfirst=True) == dparse.parse(date, dayfirst=True).date()
+    assert (
+        parse_date(None, date_default=date, dayfirst=True)
+        == dparse.parse(date, dayfirst=True).date()
+    )
+
+
+def test_nearest_saturday():
+    """API Tests if check succeeds"""
+
+    date = parse_date("25-12-2023", dayfirst=True)
+    assert get_nearest_saturday(date) == parse_date("23-12-2023", dayfirst=True)
+
+    date = parse_date("28-12-2023", dayfirst=True)
+    assert get_nearest_saturday(date) == parse_date("30-12-2023", dayfirst=True)
```

### Comparing `gantt-project-maker-0.3.7/tox.ini` & `gantt-project-maker-0.4.2/tox.ini`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# Tox configuration file
-# Read more under https://tox.wiki/
-# THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
-
-[tox]
-minversion = 3.24
-envlist = default
-isolated_build = True
-
-
-[testenv]
-description = Invoke pytest to run automated tests
-setenv =
-    TOXINIDIR = {toxinidir}
-passenv =
-    HOME
-    SETUPTOOLS_*
-extras =
-    testing
-commands =
-    pytest {posargs}
-
-
-# # To run `tox -e lint` you need to make sure you have a
-# # `.pre-commit-config.yaml` file. See https://pre-commit.com
-# [testenv:lint]
-# description = Perform static analysis and style checks
-# skip_install = True
-# deps = pre-commit
-# passenv =
-#     HOMEPATH
-#     PROGRAMDATA
-#     SETUPTOOLS_*
-# commands =
-#     pre-commit run --all-files {posargs:--show-diff-on-failure}
-
-
-[testenv:{build,clean}]
-description =
-    build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
-    clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
-# https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
-skip_install = True
-changedir = {toxinidir}
-deps =
-    build: build[virtualenv]
-passenv =
-    SETUPTOOLS_*
-commands =
-    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
-    clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
-    build: python -m build {posargs}
-# By default, both `sdist` and `wheel` are built. If your sdist is too big or you don't want
-# to make it available, consider running: `tox -e build -- --wheel`
-
-
-[testenv:{docs,doctests,linkcheck}]
-description =
-    docs: Invoke sphinx-build to build the docs
-    doctests: Invoke sphinx-build to run doctests
-    linkcheck: Check for broken links in the documentation
-passenv =
-    SETUPTOOLS_*
-setenv =
-    DOCSDIR = {toxinidir}/docs
-    BUILDDIR = {toxinidir}/docs/_build
-    docs: BUILD = html
-    doctests: BUILD = doctest
-    linkcheck: BUILD = linkcheck
-deps =
-    -r {toxinidir}/docs/requirements.txt
-    # ^  requirements.txt shared with Read The Docs
-commands =
-    sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
-
-
-[testenv:publish]
-description =
-    Publish the package you have been developing to a package index server.
-    By default, it uses testpypi. If you really want to publish your package
-    to be publicly accessible in PyPI, use the `-- --repository pypi` option.
-skip_install = True
-changedir = {toxinidir}
-passenv =
-    # See: https://twine.readthedocs.io/en/latest/
-    TWINE_USERNAME
-    TWINE_PASSWORD
-    TWINE_REPOSITORY
-    TWINE_REPOSITORY_URL
-deps = twine
-commands =
-    python -m twine check dist/*
-    python -m twine upload {posargs:--repository {env:TWINE_REPOSITORY:testpypi}} dist/*
+# Tox configuration file
+# Read more under https://tox.wiki/
+# THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
+
+[tox]
+minversion = 3.24
+envlist = default
+isolated_build = True
+
+
+[testenv]
+description = Invoke pytest to run automated tests
+setenv =
+    TOXINIDIR = {toxinidir}
+passenv =
+    HOME
+    SETUPTOOLS_*
+extras =
+    testing
+commands =
+    pytest {posargs}
+
+
+# # To run `tox -e lint` you need to make sure you have a
+# # `.pre-commit-config.yaml` file. See https://pre-commit.com
+# [testenv:lint]
+# description = Perform static analysis and style checks
+# skip_install = True
+# deps = pre-commit
+# passenv =
+#     HOMEPATH
+#     PROGRAMDATA
+#     SETUPTOOLS_*
+# commands =
+#     pre-commit run --all-files {posargs:--show-diff-on-failure}
+
+
+[testenv:{build,clean}]
+description =
+    build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
+    clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
+# https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
+skip_install = True
+changedir = {toxinidir}
+deps =
+    build: build[virtualenv]
+passenv =
+    SETUPTOOLS_*
+commands =
+    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
+    clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
+    build: python -m build {posargs}
+# By default, both `sdist` and `wheel` are built. If your sdist is too big or you don't want
+# to make it available, consider running: `tox -e build -- --wheel`
+
+
+[testenv:{docs,doctests,linkcheck}]
+description =
+    docs: Invoke sphinx-build to build the docs
+    doctests: Invoke sphinx-build to run doctests
+    linkcheck: Check for broken links in the documentation
+passenv =
+    SETUPTOOLS_*
+setenv =
+    DOCSDIR = {toxinidir}/docs
+    BUILDDIR = {toxinidir}/docs/_build
+    docs: BUILD = html
+    doctests: BUILD = doctest
+    linkcheck: BUILD = linkcheck
+deps =
+    -r {toxinidir}/docs/requirements.txt
+    # ^  requirements.txt shared with Read The Docs
+commands =
+    sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
+
+
+[testenv:publish]
+description =
+    Publish the package you have been developing to a package index server.
+    By default, it uses testpypi. If you really want to publish your package
+    to be publicly accessible in PyPI, use the `-- --repository pypi` option.
+skip_install = True
+changedir = {toxinidir}
+passenv =
+    # See: https://twine.readthedocs.io/en/latest/
+    TWINE_USERNAME
+    TWINE_PASSWORD
+    TWINE_REPOSITORY
+    TWINE_REPOSITORY_URL
+deps = twine
+commands =
+    python -m twine check dist/*
+    python -m twine upload {posargs:--repository {env:TWINE_REPOSITORY:testpypi}} dist/*
```

