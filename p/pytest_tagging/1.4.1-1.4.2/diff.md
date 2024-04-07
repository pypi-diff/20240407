# Comparing `tmp/pytest_tagging-1.4.1.tar.gz` & `tmp/pytest_tagging-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_tagging-1.4.1.tar", max compression
+gzip compressed data, was "pytest_tagging-1.4.2.tar", max compression
```

## Comparing `pytest_tagging-1.4.1.tar` & `pytest_tagging-1.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-02-15 19:44:58.879028 pytest_tagging-1.4.1/LICENSE
--rw-r--r--   0        0        0     1917 2024-02-15 19:44:58.879028 pytest_tagging-1.4.1/README.md
--rw-r--r--   0        0        0     1571 2024-02-15 19:44:58.879028 pytest_tagging-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       68 2024-02-15 19:44:58.879028 pytest_tagging-1.4.1/pytest_tagging/__init__.py
--rw-r--r--   0        0        0     5177 2024-02-15 19:44:58.879028 pytest_tagging-1.4.1/pytest_tagging/plugin.py
--rw-r--r--   0        0        0     1160 2024-02-15 19:44:58.883028 pytest_tagging-1.4.1/pytest_tagging/utils.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 pytest_tagging-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1919 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/README.md
+-rw-r--r--   0        0        0     1518 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/__init__.py
+-rw-r--r--   0        0        0     5147 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/plugin.py
+-rw-r--r--   0        0        0      833 2024-04-07 10:13:40.916855 pytest_tagging-1.4.2/pytest_tagging/utils.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 pytest_tagging-1.4.2/PKG-INFO
```

### Comparing `pytest_tagging-1.4.1/LICENSE` & `pytest_tagging-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_tagging-1.4.1/README.md` & `pytest_tagging-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,26 +34,27 @@
 By default, all tests that match at least one tag will be collected. To only select
 tests that have all the provided tags, use the option --tags-operand=AND, like so:
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME --tags-operand AND
 ```
 
-You can also display all available tags by specifyin `--tags` empty:
+You can also display all available tags by specifying `--tags` empty:
 
 ```sh
 pytest --tags
 >>Available tags:
 >>foo
 >>bar
 ```
 
 Tags can be combined using `pytest_tagging.combine_tags`:
 
 ```sh
 from pytest_tagging import combine_tags
 combine_tags("all", "foo", "bar")
 ```
+
 Then you can execute `pytest --tags all` and it will run all tests with `foo` and `bar` tags
 
 ## Extra
 - It is thread-safe, so it can be used with [pytest-parallel](https://github.com/browsertron/pytest-parallel).
```

### Comparing `pytest_tagging-1.4.1/pyproject.toml` & `pytest_tagging-1.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_tagging"
-version = "1.4.1"
+version = "1.4.2"
 description = "a pytest plugin to tag tests"
 authors = ["Sergio Castillo <s.cast.lara@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/scastlara/pytest-tagging"
 repository = "https://github.com/scastlara/pytest-tagging"
 
@@ -19,58 +19,53 @@
 pytest-parallel = "*"
 pytest-cov = "*"
 ruff = "*"
 
 [tool.poetry.group.dev.dependencies]
 py = "^1.11.0"
 
-[tool.black]
-line-length = 120
-target_version = ["py311"]
-
 [tool.ruff]
 target-version = "py311"
 line-length = 120
+
+[tool.ruff.lint]
 select = [
     "C9",  # mccabe
     "E",   # pycodestyle error
     "W",   # pycodestyle warning
     "F",   # pyflakes
     "B",   # bugbear
     "I",   # isort
     "C4",  # comprehensions
     "SIM", # simplify
     "N",   # pep8-naming
 ]
 ignore = [
-    "E501",   # line length (black handles it)
+    "E501", # line length (black handles it)
 ]
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:tagging
     --cov
     --cov-report term-missing
     --cov-report=xml:./tests/coverage.xml
     --junitxml=./tests/junit.xml
 """
 
 [tool.coverage.run]
-omit = [
-    "tests/*",
-    "/tmp/*"
-]
+omit = ["tests/*", "/tmp/*"]
 
 [tool.coverage.report]
 source = "pytest_tagging"
 fail_under = 90
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 [tool.commitizen]
-version = "1.4.1"
+version = "1.4.2"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_tagging-1.4.1/pytest_tagging/plugin.py` & `pytest_tagging-1.4.2/pytest_tagging/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from collections import Counter
+from dataclasses import dataclass
 from enum import Enum
 
 import pytest
 
-from .utils import TagCounterThreadSafe, get_run_tags, get_tags_from_item
+from .utils import TagCounterThreadSafe, get_tags_from_item
 
 
 class OperandChoices(Enum):
     OR = "OR"
     AND = "AND"
 
 
+@dataclass(frozen=True, slots=True)
+class TaggingOptions:
+    tags: list[str] | None = None
+    operand: OperandChoices = OperandChoices.OR
+
+
 # Allows you to combine tags
 _combined_tags = {}
 
 
 def combine_tags(tag_name: str, *args):
     """Combine all tags in `args` into `new_tag`"""
     _combined_tags[tag_name] = args
@@ -23,113 +30,106 @@
 def select_counter_class(config) -> type[Counter] | type[TagCounterThreadSafe]:
     must_be_threadsafe = getattr(config.option, "workers", None) or getattr(config.option, "tests_per_worker", None)
     return TagCounterThreadSafe if must_be_threadsafe else Counter
 
 
 def pytest_configure(config) -> None:
     config.addinivalue_line("markers", "tags('tag1', 'tag2'): add tags to a given test")
+    config_opts = TaggingOptions(
+        tags=config.getoption("--tags"),
+        operand=config.getoption("--tags-operand"),
+    )
     counter_class = select_counter_class(config)
-    config.pluginmanager.register(TaggerRunner(counter_class), "taggerrunner")
+    config.pluginmanager.register(TaggerRunner(counter_class, config=config_opts), "taggerrunner")
 
 
 def pytest_addoption(parser, pluginmanager) -> None:
     group = parser.getgroup("tagging")
 
-    # --tags can be in 3 states
-    # []] if not specified
-    # [[]] if specified but empty
-    # [["my_tag"]] if specified with an tag
-    # That means with multiple --tags it becomes [["my_tag1"], ["my_tag2"]]
-    # With action="extend" it cannot become [[]]
     group.addoption(
         "--tags",
-        default=[],
+        default=None,  # it can be none because we have to distinguish between provided empty and not provided
         nargs="*",
-        action="append",
-        help="Run the tests that contain the given tags, separated by commas",
+        action="extend",
+        help="Run the tests that contain the given tags.",
     )
     group.addoption(
         "--tags-operand",
         type=OperandChoices,
         default=OperandChoices.OR,
         choices=list(OperandChoices),
     )
-    parser.addini(
-        "tags",
-        help="Run the tests that contain the given tags, separated by commas",
-    )
 
 
 class TaggerRunner:
-    def __init__(self, counter_class: type[Counter] | type[TagCounterThreadSafe]) -> None:
+    def __init__(
+        self,
+        counter_class: type[Counter] | type[TagCounterThreadSafe],
+        config: TaggingOptions,
+    ) -> None:
         self.counter = counter_class()
+        self.config = config
         self._available_tags: list[str] = []
 
-    def get_available_tags(self, items) -> list:
+    def get_available_tags(self, items) -> list[str]:
         """
         Returns all available tags
         :param items: Items from pytest_collection_modifyitems
         """
-        available_tags = []
+        available_tags = set()
         for item in items:
             test_tags = set(get_tags_from_item(item))
-            for tag in test_tags:
-                if tag not in available_tags:
-                    available_tags.append(tag)
+            available_tags.update(test_tags)
+        return list(available_tags)
 
-        return available_tags
+    def get_tags_to_run(self, tags: list[str] | None, available_tags: list[str], operand: OperandChoices) -> set[str]:
+        if tags is None:
+            return set(available_tags)
+        found_combined_tags = set(tags) & set(_combined_tags)
+        for tag_name in found_combined_tags:
+            tags += _combined_tags[tag_name]
+        return set(tags) or set()
 
     def pytest_report_header(self, config) -> list[str]:
         """Add tagging config to pytest header."""
-        tags = config.getoption("--tags")
-        return [f"tagging: tags={tags}"]
+        return [f"tagging: tags={self.config.tags}"]
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_collection_modifyitems(self, session, config, items):
         selected_items = []
         deselected_items = []
+        self._available_tags = self.get_available_tags(items)
 
-        all_run_tags = get_run_tags(config.getoption("--tags"))
-        if all_run_tags is not None:
-            # --tags was provided
-            if len(all_run_tags) == 0:
-                # If no items in --tags
-                self._available_tags = self.get_available_tags(items)
-                for item in items:
+        all_run_tags = self.get_tags_to_run(
+            tags=self.config.tags,
+            available_tags=self._available_tags,
+            operand=self.config.operand,
+        )
+        if self.config.tags == [] or (self.config.tags is not None and not all_run_tags):
+            # No tags match the conditions to run
+            # or we just passed an empty `--tags` options to see them all.
+            for item in items:
+                deselected_items.append(item)
+        else:
+            # Some tags were selected
+            for item in items:
+                test_tags = get_tags_from_item(item)
+                if (self.config.operand is OperandChoices.OR and test_tags & all_run_tags) or (
+                    self.config.operand is OperandChoices.AND and all_run_tags <= test_tags
+                ):
+                    selected_items.append(item)
+                else:
                     deselected_items.append(item)
-            else:
-                # If items in --tags
-                operand = config.getoption("--tags-operand")
-
-                # Allows you to combine tags
-                found_combined_tags = set(all_run_tags) & set(_combined_tags)
-                for tag_name in found_combined_tags:
-                    all_run_tags += _combined_tags[tag_name]
-
-                for item in items:
-                    run_tags = set(all_run_tags)
-                    test_tags = get_tags_from_item(item)
-                    if (
-                        not run_tags
-                        or (operand is OperandChoices.OR and test_tags & run_tags)
-                        or (operand is OperandChoices.AND and run_tags <= test_tags)
-                    ):
-                        selected_items.append(item)
-                    else:
-                        deselected_items.append(item)
             config.hook.pytest_deselected(items=deselected_items)
-        else:
-            # --tags was not provided. Run all tests as normal
-            selected_items = items
         items[:] = selected_items
         yield
 
     @pytest.hookimpl(hookwrapper=True, trylast=True)
     def pytest_terminal_summary(self, terminalreporter, exitstatus, config):
-        tags = get_run_tags(config.getoption("--tags"))
+        tags = self.config.tags
         if tags is not None and len(tags) == 0:
             terminalreporter.write_line("=" * 6 + " Available tags " + "=" * 6)
             for tag in self._available_tags:
                 terminalreporter.write_line(f"- '{tag}'")
 
         if self.counter:
             terminalreporter.write_sep("=", "failing tags", yellow=True, bold=True)
```

### Comparing `pytest_tagging-1.4.1/PKG-INFO` & `pytest_tagging-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_tagging
-Version: 1.4.1
+Version: 1.4.2
 Summary: a pytest plugin to tag tests
 Home-page: https://github.com/scastlara/pytest-tagging
 License: MIT
 Author: Sergio Castillo
 Author-email: s.cast.lara@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,27 +52,28 @@
 By default, all tests that match at least one tag will be collected. To only select
 tests that have all the provided tags, use the option --tags-operand=AND, like so:
 
 ```sh
 pytest --tags integration --tags MY_COMPONENT_NAME --tags-operand AND
 ```
 
-You can also display all available tags by specifyin `--tags` empty:
+You can also display all available tags by specifying `--tags` empty:
 
 ```sh
 pytest --tags
 >>Available tags:
 >>foo
 >>bar
 ```
 
 Tags can be combined using `pytest_tagging.combine_tags`:
 
 ```sh
 from pytest_tagging import combine_tags
 combine_tags("all", "foo", "bar")
 ```
+
 Then you can execute `pytest --tags all` and it will run all tests with `foo` and `bar` tags
 
 ## Extra
 - It is thread-safe, so it can be used with [pytest-parallel](https://github.com/browsertron/pytest-parallel).
```

