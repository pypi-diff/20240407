# Comparing `tmp/pytest_tagging-1.4.2.tar.gz` & `tmp/pytest_tagging-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_tagging-1.4.2.tar", max compression
+gzip compressed data, was "pytest_tagging-1.5.0.tar", max compression
```

## Comparing `pytest_tagging-1.4.2.tar` & `pytest_tagging-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/LICENSE
--rw-r--r--   0        0        0     1919 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/README.md
--rw-r--r--   0        0        0     1518 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pyproject.toml
--rw-r--r--   0        0        0       68 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/__init__.py
--rw-r--r--   0        0        0     5147 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/plugin.py
--rw-r--r--   0        0        0      833 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/utils.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 pytest_tagging-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2275 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/README.md
+-rw-r--r--   0        0        0     1518 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pytest_tagging/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pytest_tagging/choices.py
+-rw-r--r--   0        0        0     4259 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pytest_tagging/plugin.py
+-rw-r--r--   0        0        0     2483 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pytest_tagging/selector.py
+-rw-r--r--   0        0        0      959 2024-04-07 20:03:34.002165 pytest_tagging-1.5.0/pytest_tagging/utils.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 pytest_tagging-1.5.0/PKG-INFO
```

### Comparing `pytest_tagging-1.4.2/LICENSE` & `pytest_tagging-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.4.2/README.md` & `pytest_tagging-1.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 It supports selecting only tests with a specific tag, and displays a counter of how many tests failed
 for each specific tag.
 
 This package exists because doing all of this with `pytest.mark` is painful, since it requires registering marks, 
 and you cannot use variables defined elsewhere easily.
 
-
 ## Usage
 
 ```python
 @pytest.mark.tags("JIRA-XX", "integration", constants.COMPONENT_X)
 def test_foo():
     assert False
 ```
@@ -26,15 +25,14 @@
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME
 ```
 
 ![pytest-tagging-screenshot](/media/screenshot-1.png)
 
-
 By default, all tests that match at least one tag will be collected. To only select
 tests that have all the provided tags, use the option --tags-operand=AND, like so:
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME --tags-operand AND
 ```
 
@@ -43,18 +41,31 @@
 ```sh
 pytest --tags
 >>Available tags:
 >>foo
 >>bar
 ```
 
+### Combining tags
+
 Tags can be combined using `pytest_tagging.combine_tags`:
 
-```sh
+```python
 from pytest_tagging import combine_tags
 combine_tags("all", "foo", "bar")
 ```
 
 Then you can execute `pytest --tags all` and it will run all tests with `foo` and `bar` tags
 
+### Excluding tags
+
+You can exclude tags for a particular test run by using the option `--exclude-tags` in a similar
+way to the `--tags` option. Notice tests with tags that are excluded will not be executed, even if
+they contain a tag that was selected with `--tags`.
+
+```sh
+pytest --tags mobile --tags web --exclude-tags flaky
+```
+
 ## Extra
+
 - It is thread-safe, so it can be used with [pytest-parallel](https://github.com/browsertron/pytest-parallel).
```

### Comparing `pytest_tagging-1.4.2/pyproject.toml` & `pytest_tagging-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_tagging"
-version = "1.4.2"
+version = "1.5.0"
 description = "a pytest plugin to tag tests"
 authors = ["Sergio Castillo <s.cast.lara@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/scastlara/pytest-tagging"
 repository = "https://github.com/scastlara/pytest-tagging"
 
@@ -57,15 +57,15 @@
 
 [tool.coverage.report]
 source = "pytest_tagging"
 fail_under = 90
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 [tool.commitizen]
-version = "1.4.2"
+version = "1.5.0"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_tagging-1.4.2/PKG-INFO` & `pytest_tagging-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_tagging
-Version: 1.4.2
+Version: 1.5.0
 Summary: a pytest plugin to tag tests
 Home-page: https://github.com/scastlara/pytest-tagging
 License: MIT
 Author: Sergio Castillo
 Author-email: s.cast.lara@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,14 @@
 
 It supports selecting only tests with a specific tag, and displays a counter of how many tests failed
 for each specific tag.
 
 This package exists because doing all of this with `pytest.mark` is painful, since it requires registering marks, 
 and you cannot use variables defined elsewhere easily.
 
-
 ## Usage
 
 ```python
 @pytest.mark.tags("JIRA-XX", "integration", constants.COMPONENT_X)
 def test_foo():
     assert False
 ```
@@ -44,15 +43,14 @@
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME
 ```
 
 ![pytest-tagging-screenshot](/media/screenshot-1.png)
 
-
 By default, all tests that match at least one tag will be collected. To only select
 tests that have all the provided tags, use the option --tags-operand=AND, like so:
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME --tags-operand AND
 ```
 
@@ -61,19 +59,32 @@
 ```sh
 pytest --tags
 >>Available tags:
 >>foo
 >>bar
 ```
 
+### Combining tags
+
 Tags can be combined using `pytest_tagging.combine_tags`:
 
-```sh
+```python
 from pytest_tagging import combine_tags
 combine_tags("all", "foo", "bar")
 ```
 
 Then you can execute `pytest --tags all` and it will run all tests with `foo` and `bar` tags
 
+### Excluding tags
+
+You can exclude tags for a particular test run by using the option `--exclude-tags` in a similar
+way to the `--tags` option. Notice tests with tags that are excluded will not be executed, even if
+they contain a tag that was selected with `--tags`.
+
+```sh
+pytest --tags mobile --tags web --exclude-tags flaky
+```
+
 ## Extra
+
 - It is thread-safe, so it can be used with [pytest-parallel](https://github.com/browsertron/pytest-parallel).
```

