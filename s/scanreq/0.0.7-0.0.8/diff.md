# Comparing `tmp/scanreq-0.0.7.tar.gz` & `tmp/scanreq-0.0.8.tar.gz`

## Comparing `scanreq-0.0.7.tar` & `scanreq-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.7/requirements-dev.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.7/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.7/setup.cfg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__main__.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 scanreq-0.0.7/tests/test_scanner.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.7/LICENSE
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 scanreq-0.0.7/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 scanreq-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 scanreq-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.8/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.8/src/scanreq/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.8/src/scanreq/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 scanreq-0.0.8/src/scanreq/__main__.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 scanreq-0.0.8/src/scanreq/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 scanreq-0.0.8/tests/test_scanner.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 scanreq-0.0.8/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 scanreq-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 scanreq-0.0.8/PKG-INFO
```

### Comparing `scanreq-0.0.7/.pre-commit-config.yaml` & `scanreq-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.7/tests/test_scanner.py` & `scanreq-0.0.8/tests/test_scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from unittest import mock
 
 import pytest
 
 from src.scanreq.scanner import (
+    clean_package_name,
     get_main_packages,
     read_requirements,
     search_string_in_file,
     search_string_in_python_files,
 )
 
 
@@ -84,14 +85,30 @@
     expected_file = os.path.join(directory, "test2.py")
 
     found_files = search_string_in_python_files(directory, search_string)
     assert expected_file in found_files
     assert len(found_files) == 1
 
 
+@pytest.mark.parametrize(
+    "package_name, expected",
+    [
+        ("django==3.2", "django"),
+        (" Django==3.2 ", "django"),
+        ("Flask>=1.0", "flask"),
+        ("requests", "requests"),
+        (" NumPy ", "numpy"),
+        ("django-cookie-cutter>2.0", "django-cookie-cutter"),
+        ("django-cookie-cutter<2.0", "django-cookie-cutter"),
+    ],
+)
+def test_clean_package_name(package_name, expected):
+    assert clean_package_name(package_name) == expected
+
+
 def test_read_requirements_valid_file(tmp_path):
     # Create a temporary requirements file
     requirements_content = """
     Django==3.0.5
     requests==2.23.0 # A comment
     numpy
     """
```

### Comparing `scanreq-0.0.7/.gitignore` & `scanreq-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.7/LICENSE` & `scanreq-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.7/README.md` & `scanreq-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 ```console
 pip3 install scanreq
 ```
 
 
 ## Usage
 
-> **Note:** Ensure you're working on python environment.
+> **Note:** Ensure you're working on python environment & already installed all your project requirements.txt
 
 ```console
-scanreq -r requirements.txt -p . -o unused-requirements.txt
+scanreq -r requirements.txt -p . -o unused-requirements.txt -i black,flake8
 ```
 
 ```
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
  1.  Module: rcssmin                       -> Package: rcssmin
  2.  Module: model_utils                   -> Package: django-model-utils
@@ -66,39 +66,41 @@
 Cool right? 😎
 
 ```console
 scanreq --help
 ```
 
 ```
-usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT]
+usage: scanreq [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT] [-i IGNORED_PACKAGES]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
                         Path to the requirements.txt file to read packages from.
   -p PATH, --path PATH  Project path to scan for unused packages (default: current directory).
   -o OUTPUT, --output OUTPUT
                         Path to the output file where unused packages will be saved.
+  -i IGNORED_PACKAGES, --ignored-packages IGNORED_PACKAGES
+                        Comma separated list of package names to be ignored.
 ```
 
 > **Note:** Don't forget to cross-check the unused packages after finding them,
 > because sometimes they are used in different cases without being imported in the code.
 > For example: `argon2-cffi` used in `settings.PASSWORD_HASHERS = ["django.contrib.auth.hashers.Argon2PasswordHasher", ...]` for Django.
 
 
 ## ToDo List
 
 - [x] Support argument parser (command arguments)
    - [x] Directory to scan
    - [x] Requirement file to scan
    - [x] Option to write the output of unused packages
+   - [x] Option to exclude or ignore some packages
    - [ ] Option to auto replace the package from requirements.txt file
-   - [ ] Option to exclude or ignore some packages
 - [x] Support CLI - make it as a command
 - [x] Write some tests
 - [x] Publish to PyPi
 - [x] Support multiple python versions
 - [ ] Support scan the `pyproject.toml`
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
```

### Comparing `scanreq-0.0.7/pyproject.toml` & `scanreq-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.7/PKG-INFO` & `scanreq-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scanreq
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python tool to scan all unused packages in requirements.txt file for your project.
 Project-URL: Changelog, https://github.com/agusmakmun/scan-unused-requirements/releases
 Project-URL: Documentation, https://github.com/agusmakmun/scan-unused-requirements
 Project-URL: Issues, https://github.com/agusmakmun/scan-unused-requirements/issues
 Project-URL: Source, https://github.com/agusmakmun/scan-unused-requirements
 Author-email: agusmakmun <summon.agus@gmail.com>
 License-Expression: MIT
@@ -61,18 +61,18 @@
 ```console
 pip3 install scanreq
 ```
 
 
 ## Usage
 
-> **Note:** Ensure you're working on python environment.
+> **Note:** Ensure you're working on python environment & already installed all your project requirements.txt
 
 ```console
-scanreq -r requirements.txt -p . -o unused-requirements.txt
+scanreq -r requirements.txt -p . -o unused-requirements.txt -i black,flake8
 ```
 
 ```
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
  1.  Module: rcssmin                       -> Package: rcssmin
  2.  Module: model_utils                   -> Package: django-model-utils
@@ -94,39 +94,41 @@
 Cool right? 😎
 
 ```console
 scanreq --help
 ```
 
 ```
-usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT]
+usage: scanreq [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT] [-i IGNORED_PACKAGES]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
                         Path to the requirements.txt file to read packages from.
   -p PATH, --path PATH  Project path to scan for unused packages (default: current directory).
   -o OUTPUT, --output OUTPUT
                         Path to the output file where unused packages will be saved.
+  -i IGNORED_PACKAGES, --ignored-packages IGNORED_PACKAGES
+                        Comma separated list of package names to be ignored.
 ```
 
 > **Note:** Don't forget to cross-check the unused packages after finding them,
 > because sometimes they are used in different cases without being imported in the code.
 > For example: `argon2-cffi` used in `settings.PASSWORD_HASHERS = ["django.contrib.auth.hashers.Argon2PasswordHasher", ...]` for Django.
 
 
 ## ToDo List
 
 - [x] Support argument parser (command arguments)
    - [x] Directory to scan
    - [x] Requirement file to scan
    - [x] Option to write the output of unused packages
+   - [x] Option to exclude or ignore some packages
    - [ ] Option to auto replace the package from requirements.txt file
-   - [ ] Option to exclude or ignore some packages
 - [x] Support CLI - make it as a command
 - [x] Write some tests
 - [x] Publish to PyPi
 - [x] Support multiple python versions
 - [ ] Support scan the `pyproject.toml`
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
```

