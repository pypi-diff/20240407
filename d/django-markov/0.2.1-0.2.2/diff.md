# Comparing `tmp/django_markov-0.2.1.tar.gz` & `tmp/django_markov-0.2.2.tar.gz`

## Comparing `django_markov-0.2.1.tar` & `django_markov-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/admin.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/apps.py
--rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/py.typed
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0003_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.1/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/settings.py
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.1/tests/urls.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.1/.gitignore
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.1/LICENSE
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.1/README.md
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/apps.py
+-rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/py.typed
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/settings.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.2/README.md
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.2/PKG-INFO
```

### Comparing `django_markov-0.2.1/src/django_markov/models.py` & `django_markov-0.2.2/src/django_markov/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 sentence_generated = dispatch.Signal()
 
 
 def _get_corpus_char_limit() -> int:
     """Get the corpus character limit from settings or return a default."""
-    if not settings.MARKOV_CORPUS_MAX_CHAR_LIMIT or not isinstance(
+    if not hasattr(settings, "MARKOV_CORPUS_MAX_CHAR_LIMIT") or not isinstance(
         settings.MARKOV_CORPUS_MAX_CHAR_LIMIT, int
     ):
         return 0
     return settings.MARKOV_CORPUS_MAX_CHAR_LIMIT
 
 
 class MarkovTextModel(models.Model):
```

### Comparing `django_markov-0.2.1/src/django_markov/text_models.py` & `django_markov-0.2.2/src/django_markov/text_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/src/django_markov/migrations/0001_initial.py` & `django_markov-0.2.2/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.2.2/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/src/django_markov/migrations/0003_markovtextmodel_compiled.py` & `django_markov-0.2.2/src/django_markov/migrations/0003_markovtextmodel_compiled.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/tests/settings.py` & `django_markov-0.2.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/tests/test_models.py` & `django_markov-0.2.2/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 def test_get_char_limit(
     settings, override_value: int | None, expected_result: int
 ) -> None:
     settings.MARKOV_CORPUS_MAX_CHAR_LIMIT = override_value
     assert _get_corpus_char_limit() == expected_result
 
 
+def test_get_char_limit_missing_settings(settings):
+    del settings.MARKOV_CORPUS_MAX_CHAR_LIMIT
+    assert _get_corpus_char_limit() == 0  # Setting was not present
+
+
 def test_text_models_return_none_on_empty_directive():
     model = MarkovTextModel.objects.create()
     assert not model._as_text_model()
     assert not model._compiled_model
 
 
 def test_do_not_recompile_compiled_model(compiled_model):
```

### Comparing `django_markov-0.2.1/tests/urls.py` & `django_markov-0.2.2/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/LICENSE` & `django_markov-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/README.md` & `django_markov-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.1/pyproject.toml` & `django_markov-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-markov"
-version = "0.2.1"
+version = "0.2.2"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
     "django>=4.2",
     "markovify>=0.9.4",
@@ -224,15 +224,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.2.1"
+current_version = "0.2.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_markov-0.2.1/PKG-INFO` & `django_markov-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.2.1
+Version: 0.2.2
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

