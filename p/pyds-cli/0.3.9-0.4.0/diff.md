# Comparing `tmp/pyds-cli-0.3.9.tar.gz` & `tmp/pyds-cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyds-cli-0.3.9.tar", last modified: Sat Oct 21 01:00:51 2023, max compression
+gzip compressed data, was "pyds-cli-0.4.0.tar", last modified: Sun Apr  7 16:23:46 2024, max compression
```

## Comparing `pyds-cli-0.3.9.tar` & `pyds-cli-0.4.0.tar`

### file list

```diff
@@ -1,74 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.035168 pyds-cli-0.3.9/pyds/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.039168 pyds-cli-0.3.9/pyds/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.043168 pyds-cli-0.3.9/pyds/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.bumpversion.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.darglint.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.043168 pyds-cli-0.3.9/pyds/cli/templates/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.devcontainer/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.devcontainer/devcontainer.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.env.j2
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.flake8.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.031168 pyds-cli-0.3.9/pyds/cli/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.043168 pyds-cli-0.3.9/pyds/cli/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.github/workflows/code-style.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.github/workflows/docs.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.github/workflows/release-pypi-package.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/MANIFEST.in.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.047168 pyds-cli-0.3.9/pyds/cli/templates/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/docs/api.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/docs/apidocs.css.j2
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/docs/config.js.j2
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/docs/index.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/environment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/mkdocs.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.047168 pyds-cli-0.3.9/pyds/cli/templates/src/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/cli.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/models.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/preprocessing.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/schemas.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/src/utils.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/pyds/cli/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/tests/test___init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/tests/test_cli.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/cli/templates/tests/test_models.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/pyds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/pyds/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-21 00:58:40.000000 pyds-cli-0.3.9/pyds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/pyds_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-21 01:00:51.000000 pyds-cli-0.3.9/pyds_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-10-21 00:58:40.000000 pyds-cli-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.035168 pyds-cli-0.3.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 01:00:51.051168 pyds-cli-0.3.9/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-21 00:58:32.000000 pyds-cli-0.3.9/tests/cli/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.920358 pyds-cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-07 16:23:46.916358 pyds-cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.912358 pyds-cli-0.4.0/pyds/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.916358 pyds-cli-0.4.0/pyds/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/cli/talk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.916358 pyds-cli-0.4.0/pyds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/pyds/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 16:19:27.000000 pyds-cli-0.4.0/pyds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.916358 pyds-cli-0.4.0/pyds_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 16:23:46.000000 pyds-cli-0.4.0/pyds_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 16:19:27.000000 pyds-cli-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:23:46.920358 pyds-cli-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.912358 pyds-cli-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:23:46.916358 pyds-cli-0.4.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-07 16:19:24.000000 pyds-cli-0.4.0/tests/cli/test_talk.py
```

### Comparing `pyds-cli-0.3.9/PKG-INFO` & `pyds-cli-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pyds-cli
-Version: 0.3.9
+Version: 0.4.0
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: jinja2>=3.0.2
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1
 Requires-Dist: rich>=10.12.0
 Requires-Dist: ruamel.yaml>=0.17.17
 Requires-Dist: case-converter>=1.0.2
 Requires-Dist: jinja2-strcase>=0.0.2
+Requires-Dist: cookiecutter
+Requires-Dist: sh
 
 # PyDS CLI
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Helping you manage your data science projects _sanely_.
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: pyds-cli Version: 0.3.9 Description-Content-Type:
+Metadata-Version: 2.1 Name: pyds-cli Version: 0.4.0 Description-Content-Type:
 text/markdown Requires-Dist: typer>=0.3.8 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: jinja2>=3.0.2 Requires-Dist: loguru>=0.5.3 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1 Requires-Dist: rich>=10.12.0 Requires-
 Dist: ruamel.yaml>=0.17.17 Requires-Dist: case-converter>=1.0.2 Requires-Dist:
-jinja2-strcase>=0.0.2 # PyDS CLI [![All Contributors](https://img.shields.io/
-badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-) Helping
-you manage your data science projects _sanely_. [![asciicast](https://
-asciinema.org/a/quuvL2LCafmRfpFAbQLREwpke.svg)](https://asciinema.org/a/
+jinja2-strcase>=0.0.2 Requires-Dist: cookiecutter Requires-Dist: sh # PyDS CLI
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-
+orange.svg?style=flat-square)](#contributors-) Helping you manage your data
+science projects _sanely_. [![asciicast](https://asciinema.org/a/
+quuvL2LCafmRfpFAbQLREwpke.svg)](https://asciinema.org/a/
 quuvL2LCafmRfpFAbQLREwpke) ## Requirements - [Anaconda]/[Miniconda]/
 [Miniforge]/[Mambaforge] (Mambaforge recommended!) - `git` on your PATH
 [Anaconda]: https://www.anaconda.com [Miniconda]: https://docs.conda.io/en/
 latest/miniconda.html [Miniforge]: https://github.com/conda-forge/miniforge
 [Mambaforge]: https://github.com/conda-forge/miniforge#mambaforge ## Quickstart
 We're in development! Install directly from `git` into your base Anaconda
 environment. ```python pip install git+https://github.com/ericmjl/pyds-cli ```
```

### Comparing `pyds-cli-0.3.9/README.md` & `pyds-cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.3.9/pyds/cli/__init__.py` & `pyds-cli-0.4.0/pyds/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 from .conda import app as conda_app
 from .docs import app as docs_app
 from .environment import app as env_app
 from .package import app as package_app
 from .project import app as project_app
 from .system import app as system_app
+from .talk import app as talk_app
 
 app = typer.Typer()
 app.add_typer(conda_app, name="conda")
 app.add_typer(docs_app, name="docs")
 app.add_typer(env_app, name="env")
 app.add_typer(package_app, name="package")
 app.add_typer(project_app, name="project")
 app.add_typer(system_app, name="system")
+app.add_typer(talk_app, name="talk")
 
 
 @app.command()
 def configure(
     name: str = typer.Option(..., help="Your name", prompt=True),
     email: str = typer.Option(..., help="Your email address", prompt=True),
     github_username: str = typer.Option("", help="Your GitHub username", prompt=True),
```

### Comparing `pyds-cli-0.3.9/pyds/cli/conda.py` & `pyds-cli-0.4.0/pyds/cli/conda.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,12 +40,12 @@
     run("python -m pip install -e .", show_out=True, activate_env=True)
 
 
 @app.command()
 def update():
     """Update the conda environment associated with the project."""
     ensure_base_env()
-    run(f"source activate base && {CONDA_EXE} env update -f environment.yml")
+    run(f"{CONDA_EXE} env update -f environment.yml")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pyds-cli-0.3.9/pyds/cli/environment.py` & `pyds-cli-0.4.0/pyds/cli/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 
 # from ..utils import read_conda_env
 
 app = Typer()
 
 
 @app.command()
-def set_env_var(key: str, value: str):
+def set(key: str, value: str):
     """Set a key-value pair in the `.env` file.
 
     :param key: The name of the environment variable.
     :param value: The value to set the environment variable to.
     """
     env_vars = read_env_vars()
     env_vars[key] = value
     write(env_vars)
     print(f"✅ Successfully set environment variable for {key}! 🎉")
 
 
 @app.command()
-def delete_env_var(key: str):
+def delete(key: str):
     """Remove an environment variable from the `.env` file.
 
     :param key: The name of the environment variable.
     """
     env_vars = read_env_vars()
     env_vars.pop(key, None)
     write(env_vars)
 
 
 @app.command()
-def show_env_vars(keys: bool = True, values: bool = False):
+def show(keys: bool = True, values: bool = False):
     """Show all environment variables.
 
     :param keys: Whether to show the keys or not.
     :param values: Whether to show the values or not.
     """
     env_vars = read_env_vars()
     if keys and values:
```

### Comparing `pyds-cli-0.3.9/pyds/cli/package.py` & `pyds-cli-0.4.0/pyds/cli/package.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.3.9/pyds/cli/system.py` & `pyds-cli-0.4.0/pyds/cli/system.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.3.9/pyds/cli/templates/pyproject.toml.j2` & `pyds-cli-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # https://setuptools.pypa.io/en/latest/userguide/quickstart.html
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 88
 target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
@@ -56,32 +56,37 @@
 # See https://docs.astral.sh/ruff/rules/ for a list of rules.
 # See https://docs.astral.sh/ruff/configuration/#using-pyprojecttoml for configuration documentation
 select = ["E", "F", "I"]
 
 [tool.setuptools]
 include-package-data = true
 
-[tool.setuptools.packages.find]
-where = ["{{ project_name | replace('-', '_') }}"]
+[tool.setuptools.packages]
+find = {}  # Scanning implicit namespaces is active by default
 
 [project]
-name = "{{ project_name }}"
-version = "0.0.1"
+name = "pyds-cli"
+version = "0.4.0"
 dependencies = [
-    "matplotlib",
-    "pandas",
-    "scikit-learn",
-    "numpy",
+    "typer >=0.3.8",
+    "pyyaml >=6.0",
+    "jinja2 >=3.0.2",
+    "loguru >=0.5.3",
+    "pyprojroot",
+    "python-dotenv >=0.19.1",
+    "rich >=10.12.0",
+    "ruamel.yaml >=0.17.17",
+    "case-converter >=1.0.2",
+    "jinja2-strcase >= 0.0.2",
+    "cookiecutter",
+    "sh",
 ]
 readme = "README.md"
 
-[project.optional-dependencies]
-tests = [
-    "pytest"
-]
-docs = [
-    "mkdocs-material",
-    "mkdocs"
-]
-
 [project.scripts]
-{{ project_name }} = "{{ project_name | replace('-', '_') }}.cli:app"
+pyds = "pyds.cli:app"
+
+[tool.coverage.run]
+omit = [
+    "*/templates/*",
+    "tests/*",
+]
```

### Comparing `pyds-cli-0.3.9/pyds/utils/__init__.py` & `pyds-cli-0.4.0/pyds/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import subprocess
 from pathlib import Path
 from typing import Dict
 
 import ruamel.yaml
 from loguru import logger
 from pyprojroot import here
+from sh import which
 
 ANACONDA = os.getenv("anaconda", os.getenv("CONDA_PREFIX"))
 
 
 def read_config():
     """Read PyDS configuration file.
 
@@ -56,28 +57,27 @@
         env = get_conda_env_name()
         cmd = f"bash -c 'source activate {env} && {cmd}'"
     else:
         cmd = f"bash -c 'source activate base && {cmd}'"
     if log:
         logger.info(f"+ {cmd}")
 
+    run_kwargs = {
+        "cwd": cwd,
+        "shell": shell,
+    }
+
     if show_out:
-        out = subprocess.run(
-            cmd,
-            cwd=cwd,
-            shell=shell,
-            stdout=subprocess.PIPE,
-        )
+        run_kwargs["stdout"] = subprocess.PIPE
     else:
-        out = subprocess.run(
-            cmd,
-            cwd=cwd,
-            shell=shell,
-            capture_output=capture_output,
-        )
+        run_kwargs["capture_output"] = capture_output
+    out = subprocess.run(
+        cmd,
+        **run_kwargs,
+    )
     return out
 
 
 def read_conda_env(env_file="environment.yml", cwd: Path = Path(".")) -> Dict:
     """Load `environment.yml` as a dictionary.
 
     We try loading from the specified working directory first.
@@ -144,22 +144,28 @@
     I intend to expand this function
     with other ways of getting the `conda_exe` programmatically.
 
     :raises Exception: If we cannot find a path to a conda executable.
     :returns: Path to the conda or mamba executable.
     """
     # First, try mamba
-    res = run("which mamba", log=False)
-    if res.returncode == 0:
-        return Path(res.stdout.decode("utf-8").strip("\n"))
-
-    # If mamba isn't available, try conda by using the `which conda` command.
-    res = run("which conda")
-    if res.returncode == 0:
-        return Path(res.stdout.decode("utf-8").strip("\n"))
+    try:
+        return which("mamba").strip("\n")
+    except Exception:
+        pass
+
+    try:
+        return which("micromamba").strip("\n")
+    except Exception:
+        pass
+
+    try:
+        return which("conda").strip("\n")
+    except Exception:
+        pass
 
     # If `which conda` fails, try using environmenet variables.
     conda_exe = os.getenv("CONDA_EXE")
     if conda_exe is not None:
         return Path(conda_exe)
 
     raise Exception("Could not find conda executable! Do you have `conda` installed?")
```

### Comparing `pyds-cli-0.3.9/pyds_cli.egg-info/PKG-INFO` & `pyds-cli-0.4.0/pyds_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pyds-cli
-Version: 0.3.9
+Version: 0.4.0
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: jinja2>=3.0.2
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1
 Requires-Dist: rich>=10.12.0
 Requires-Dist: ruamel.yaml>=0.17.17
 Requires-Dist: case-converter>=1.0.2
 Requires-Dist: jinja2-strcase>=0.0.2
+Requires-Dist: cookiecutter
+Requires-Dist: sh
 
 # PyDS CLI
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Helping you manage your data science projects _sanely_.
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: pyds-cli Version: 0.3.9 Description-Content-Type:
+Metadata-Version: 2.1 Name: pyds-cli Version: 0.4.0 Description-Content-Type:
 text/markdown Requires-Dist: typer>=0.3.8 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: jinja2>=3.0.2 Requires-Dist: loguru>=0.5.3 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1 Requires-Dist: rich>=10.12.0 Requires-
 Dist: ruamel.yaml>=0.17.17 Requires-Dist: case-converter>=1.0.2 Requires-Dist:
-jinja2-strcase>=0.0.2 # PyDS CLI [![All Contributors](https://img.shields.io/
-badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-) Helping
-you manage your data science projects _sanely_. [![asciicast](https://
-asciinema.org/a/quuvL2LCafmRfpFAbQLREwpke.svg)](https://asciinema.org/a/
+jinja2-strcase>=0.0.2 Requires-Dist: cookiecutter Requires-Dist: sh # PyDS CLI
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-
+orange.svg?style=flat-square)](#contributors-) Helping you manage your data
+science projects _sanely_. [![asciicast](https://asciinema.org/a/
+quuvL2LCafmRfpFAbQLREwpke.svg)](https://asciinema.org/a/
 quuvL2LCafmRfpFAbQLREwpke) ## Requirements - [Anaconda]/[Miniconda]/
 [Miniforge]/[Mambaforge] (Mambaforge recommended!) - `git` on your PATH
 [Anaconda]: https://www.anaconda.com [Miniconda]: https://docs.conda.io/en/
 latest/miniconda.html [Miniforge]: https://github.com/conda-forge/miniforge
 [Mambaforge]: https://github.com/conda-forge/miniforge#mambaforge ## Quickstart
 We're in development! Install directly from `git` into your base Anaconda
 environment. ```python pip install git+https://github.com/ericmjl/pyds-cli ```
```

### Comparing `pyds-cli-0.3.9/tests/cli/conftest.py` & `pyds-cli-0.4.0/tests/cli/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 
 @pytest.fixture(scope="session", autouse=True)
 def initialized_project() -> Tuple[Path, Path]:
     """Initialize a project.
 
     :yields: A two-tuple of temp dir path and project directory path.
     """
-    runner = CliRunner()
+    runner = CliRunner(mix_stderr=False)
 
     # Run `pyds configure` only if the config file is not found.
     # This prevents local configurations from being overwritten by the test.
     try:
         read_config()
     except FileNotFoundError:
         runner.invoke(
             app, ["configure"], input="GitHub Bot\nbot@github.com\nbot\nbot\nbot"
         )
-    project_name = str(uuid4())
     tmp_path = Path("/tmp/pyds-cli")
-    project_dir = tmp_path / project_name
-    project_dir.mkdir(parents=True)
-    os.chdir(project_dir)
-
+    tmp_path.mkdir(exist_ok=True, parents=True)
+    os.chdir(tmp_path)
+    project_name = str(uuid4())
     result = runner.invoke(
         app,
-        ["project", "initialize"],
-        input=".\nblah\nMIT\nY\nY\nY\n",
+        ["project", "init"],
+        input=f"{project_name}\nTest Project\nericmjl\nEric Ma\ne@ma\n",
     )
+    project_dir = tmp_path / project_name
+    os.chdir(project_dir)
+
     assert result.exit_code == 0, result.stderr
     yield tmp_path, project_name
     run(f"conda env remove -n {project_name}")
     run(f"rm -rf {tmp_path}")
```

### Comparing `pyds-cli-0.3.9/tests/cli/test___init__.py` & `pyds-cli-0.4.0/tests/cli/test___init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.3.9/tests/cli/test_conda.py` & `pyds-cli-0.4.0/tests/cli/test_conda.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.3.9/tests/cli/test_environment.py` & `pyds-cli-0.4.0/tests/cli/test_environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 from typer.testing import CliRunner
 
 from pyds.cli import app
 
 runner = CliRunner()
 
 
-def test_set_env_var(initialized_project):
+def test_set(initialized_project):
     """Execution test for setting environment variables.
 
     :param initialized_project: conftest.py fixture for our initialized project.
     """
-    result = runner.invoke(app, ["env", "set-env-var", "key", "value"])
+    result = runner.invoke(app, ["env", "set", "key", "value"])
     assert result.exit_code == 0
 
 
-def test_delete_env_var(initialized_project):
+def test_delete(initialized_project):
     """Execution test for setting environment variables.
 
     :param initialized_project: conftest.py fixture for our initialized project.
     """
-    result = runner.invoke(app, ["env", "delete-env-var", "key"])
+    result = runner.invoke(app, ["env", "delete", "key"])
     assert result.exit_code == 0
 
 
 @pytest.mark.parametrize("keys", [True, False])
 @pytest.mark.parametrize("values", [True, False])
-def test_show_env_vars(initialized_project, keys: bool, values: bool):
+def test_show(initialized_project, keys: bool, values: bool):
     """Execution test for displaying environment variables.
 
     :param initialized_project: conftest.py fixture for our initialized project.
     :param keys: Whether or not to show keys.
     :param values: Whether or not to show values.
     """
-    cmd = ["env", "show-env-vars"]
+    cmd = ["env", "show"]
     if keys:
         cmd.append("--keys")
     elif not keys:
         cmd.append("--no-keys")
 
     if values:
         cmd.append("--values")
```

