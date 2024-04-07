# Comparing `tmp/pillory-1.0.0.tar.gz` & `tmp/pillory-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.0.0.tar` & `pillory-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       18 2024-04-07 01:15:23.936487 pillory-1.0.0/.gitignore
--rw-r--r--   0        0        0     9161 2024-04-07 00:53:05.664564 pillory-1.0.0/LICENSE
--rw-r--r--   0        0        0     3603 2024-04-07 00:28:31.480671 pillory-1.0.0/README.md
--rwxr-xr-x   0        0        0     2933 2024-04-07 01:12:22.932496 pillory-1.0.0/pillory.py
--rw-r--r--   0        0        0      409 2024-04-07 00:53:05.672564 pillory-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 pillory-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-04-07 02:49:31.399297 pillory-1.0.1/.circleci/config.yml
+-rw-r--r--   0        0        0       18 2024-04-07 02:49:31.399297 pillory-1.0.1/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-07 02:49:31.399297 pillory-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-04-07 02:49:31.399297 pillory-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3465 2024-04-07 02:49:31.399297 pillory-1.0.1/README.md
+-rw-r--r--   0        0        0     1321 2024-04-07 02:49:31.399297 pillory-1.0.1/dev-requirements.txt
+-rwxr-xr-x   0        0        0     2932 2024-04-07 02:49:31.399297 pillory-1.0.1/pillory.py
+-rw-r--r--   0        0        0      587 2024-04-07 02:49:31.399297 pillory-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 pillory-1.0.1/PKG-INFO
```

### Comparing `pillory-1.0.0/LICENSE` & `pillory-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.0.0/README.md` & `pillory-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pillory
+Version: 1.0.1
+Summary: A linter to scrutinize how you are using mocks in Python.
+Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: flit~=3.9 ; extra == "dev"
+Requires-Dist: pip-tools~=7.4 ; extra == "dev"
+Requires-Dist: pre-commit~=3.7 ; extra == "dev"
+Requires-Dist: ruff~=0.3 ; extra == "dev"
+Project-URL: Home, https://github.com/fffergal/pillory
+Provides-Extra: dev
+
 # Pillory
 
 A linter to scrutinize how you are using mocks in Python.
 
 If you often hear or make the comment "patch the import not the definition" or
 spend a lot of time explaining or helping people debug mocks, this linter could
 help you.
@@ -24,39 +38,39 @@
 
 ```
 python -m pillory 'tests/**/test_*.py'
 ```
 
 ### Rules
 
-PM101 patched implementation
-    You patched the implementation of a class or function instead of where it is
-    imported to in the module under test. e.g. "parsers.Parser" where Parser is
-    defined instead of "__main__.Parser" where it is used. This means you may
-    not have affected the module under test at all, or you have replaced the
-    target in a way which will affect other code that uses it, which is bad for
-    test isolation (making sure tests don't affect other tests, and that each
-    test tests what is intended and don't change how other parts of the code
-    work). There is a warning about not affecting the right module in the
-    [Python Standard Library docs][stdlibdocs], but there is an [even better
-    article by Ned Batchelder][nedbat] explaining how it works and the
-    additional problems with test isolation.
-
-PM102 patched is not a top level module attribute
-    You patched something like a method on a class. Because class methods can't
-    be imported by themselves, this means all uses of the class will be
-    affected, not just the module under test.
-
-PM103 patched builtins
-    You patched the builtins module instead of the built-in function in the
-    module under test. Built-ins are actually added to every module and that's
-    where they should be patched, to avoid similar issues to patching the
-    implementation. There is a CPython detail that means the builtins module may
-    be added to the lookup of each module, so patching the builtins module _can_
-    work, but it's not guaranteed and it still has problems with test isolation.
+*PM101 patched implementation*
+: You patched the implementation of a class or function instead of where it is
+imported to in the module under test. e.g. "parsers.Parser" where Parser is
+defined instead of "__main__.Parser" where it is used. This means you may not
+have affected the module under test at all, or you have replaced the target in a
+way which will affect other code that uses it, which is bad for test isolation
+(making sure tests don't affect other tests, and that each test tests what is
+intended and don't change how other parts of the code work). There is a warning
+about not affecting the right module in the [Python Standard Library
+docs][stdlibdocs], but there is an [even better article by Ned
+Batchelder][nedbat] explaining how it works and the additional problems with
+test isolation.
+
+*PM102 patched is not a top level module attribute*
+: You patched something like a method on a class. Because class methods can't be
+imported by themselves, this means all uses of the class will be affected, not
+just the module under test.
+
+*PM103 patched builtins*
+: You patched the builtins module instead of the built-in function in the module
+under test. Built-ins are actually added to every module and that's where they
+should be patched, to avoid similar issues to patching the implementation. There
+is a CPython detail that means the builtins module may be added to the lookup of
+each module, so patching the builtins module _can_ work, but it's not guaranteed
+and it still has problems with test isolation.
 
 [stdlibdocs]: https://docs.python.org/3/library/unittest.mock.html#where-to-patch
 [nedbat]: https://nedbatchelder.com/blog/201908/why_your_mock_doesnt_work.html
 
 ## Known issues
 
 * No --help text.
@@ -68,15 +82,14 @@
   require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
   "OK".
 * No pre-commit integration.
-* No strong, written justification for the reasons behind the errors.
 
 ## What's with the name?
 
 I thought it was funny that mock can also mean "make fun of" as well as the
 meaning of "mimic" that we use in testing. I imagined the linter cruelly calling
 out how you are using mocks incorrectly. Except I couldn't call it "mock", or
 "mock mocker", that would be confusing! So I picked a name with a similar
@@ -87,7 +100,8 @@
 Thank you for your interest in making a contribution.
 
 Please talk to the maintainer before making a pull request to make sure what you
 are adding is wanted.
 
 This project uses the Apache License 2.0. You will be credited in the git
 history, but for ease of maintenance copyright stays with the maintainer.
+
```

### Comparing `pillory-1.0.0/pillory.py` & `pillory-1.0.1/pillory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 A linter to scrutinize how you are using mocks in Python.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 import ast
 import importlib
 import pathlib
 import sys
 from collections.abc import Iterator
 
-
 # Excludes taken from ruff.
 EXCLUDE = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".git-rewrite",
```

### Comparing `pillory-1.0.0/PKG-INFO` & `pillory-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pillory
-Version: 1.0.0
-Summary: A linter to scrutinize how you are using mocks in Python.
-Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: Apache Software License
-Project-URL: Home, https://github.com/fffergal/pillory
-
 # Pillory
 
 A linter to scrutinize how you are using mocks in Python.
 
 If you often hear or make the comment "patch the import not the definition" or
 spend a lot of time explaining or helping people debug mocks, this linter could
 help you.
@@ -33,39 +24,39 @@
 
 ```
 python -m pillory 'tests/**/test_*.py'
 ```
 
 ### Rules
 
-PM101 patched implementation
-    You patched the implementation of a class or function instead of where it is
-    imported to in the module under test. e.g. "parsers.Parser" where Parser is
-    defined instead of "__main__.Parser" where it is used. This means you may
-    not have affected the module under test at all, or you have replaced the
-    target in a way which will affect other code that uses it, which is bad for
-    test isolation (making sure tests don't affect other tests, and that each
-    test tests what is intended and don't change how other parts of the code
-    work). There is a warning about not affecting the right module in the
-    [Python Standard Library docs][stdlibdocs], but there is an [even better
-    article by Ned Batchelder][nedbat] explaining how it works and the
-    additional problems with test isolation.
-
-PM102 patched is not a top level module attribute
-    You patched something like a method on a class. Because class methods can't
-    be imported by themselves, this means all uses of the class will be
-    affected, not just the module under test.
-
-PM103 patched builtins
-    You patched the builtins module instead of the built-in function in the
-    module under test. Built-ins are actually added to every module and that's
-    where they should be patched, to avoid similar issues to patching the
-    implementation. There is a CPython detail that means the builtins module may
-    be added to the lookup of each module, so patching the builtins module _can_
-    work, but it's not guaranteed and it still has problems with test isolation.
+*PM101 patched implementation*
+: You patched the implementation of a class or function instead of where it is
+imported to in the module under test. e.g. "parsers.Parser" where Parser is
+defined instead of "__main__.Parser" where it is used. This means you may not
+have affected the module under test at all, or you have replaced the target in a
+way which will affect other code that uses it, which is bad for test isolation
+(making sure tests don't affect other tests, and that each test tests what is
+intended and don't change how other parts of the code work). There is a warning
+about not affecting the right module in the [Python Standard Library
+docs][stdlibdocs], but there is an [even better article by Ned
+Batchelder][nedbat] explaining how it works and the additional problems with
+test isolation.
+
+*PM102 patched is not a top level module attribute*
+: You patched something like a method on a class. Because class methods can't be
+imported by themselves, this means all uses of the class will be affected, not
+just the module under test.
+
+*PM103 patched builtins*
+: You patched the builtins module instead of the built-in function in the module
+under test. Built-ins are actually added to every module and that's where they
+should be patched, to avoid similar issues to patching the implementation. There
+is a CPython detail that means the builtins module may be added to the lookup of
+each module, so patching the builtins module _can_ work, but it's not guaranteed
+and it still has problems with test isolation.
 
 [stdlibdocs]: https://docs.python.org/3/library/unittest.mock.html#where-to-patch
 [nedbat]: https://nedbatchelder.com/blog/201908/why_your_mock_doesnt_work.html
 
 ## Known issues
 
 * No --help text.
@@ -77,15 +68,14 @@
   require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
   "OK".
 * No pre-commit integration.
-* No strong, written justification for the reasons behind the errors.
 
 ## What's with the name?
 
 I thought it was funny that mock can also mean "make fun of" as well as the
 meaning of "mimic" that we use in testing. I imagined the linter cruelly calling
 out how you are using mocks incorrectly. Except I couldn't call it "mock", or
 "mock mocker", that would be confusing! So I picked a name with a similar
@@ -96,8 +86,7 @@
 Thank you for your interest in making a contribution.
 
 Please talk to the maintainer before making a pull request to make sure what you
 are adding is wanted.
 
 This project uses the Apache License 2.0. You will be credited in the git
 history, but for ease of maintenance copyright stays with the maintainer.
-
```

