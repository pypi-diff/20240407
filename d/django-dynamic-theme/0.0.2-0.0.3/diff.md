# Comparing `tmp/django_dynamic_theme-0.0.2.tar.gz` & `tmp/django_dynamic_theme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_theme-0.0.2.tar", max compression
+gzip compressed data, was "django_dynamic_theme-0.0.3.tar", max compression
```

## Comparing `django_dynamic_theme-0.0.2.tar` & `django_dynamic_theme-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,28 @@
--rw-r--r--   0        0        0     1068 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/LICENSE
--rw-r--r--   0        0        0     1322 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/__init__.py
--rw-r--r--   0        0        0      440 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/admin.py
--rw-r--r--   0        0        0      281 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/apps.py
--rw-r--r--   0        0        0      475 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/context_processor.py
--rw-r--r--   0        0        0      516 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0001_initial.py
--rw-r--r--   0        0        0      436 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0002_background_name.py
--rw-r--r--   0        0        0      484 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
--rw-r--r--   0        0        0     1241 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
--rw-r--r--   0        0        0      733 2024-03-28 19:44:44.823925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
--rw-r--r--   0        0        0      526 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0006_alter_theme_background.py
--rw-r--r--   0        0        0      664 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
--rw-r--r--   0        0        0      434 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0008_alter_theme_default.py
--rw-r--r--   0        0        0        0 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/__init__.py
--rw-r--r--   0        0        0     1998 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/models.py
--rw-r--r--   0        0        0        0 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/utill/__init__.py
--rw-r--r--   0        0        0      590 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/django_dynamic_theme/utill/scss_editor.py
--rw-r--r--   0        0        0      743 2024-03-28 19:44:44.827925 django_dynamic_theme-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1948 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1644 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/__init__.py
+-rw-r--r--   0        0        0      713 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/admin.py
+-rw-r--r--   0        0        0      498 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/apps.py
+-rw-r--r--   0        0        0      475 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/context_processor.py
+-rw-r--r--   0        0        0      516 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0001_initial.py
+-rw-r--r--   0        0        0      436 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0002_background_name.py
+-rw-r--r--   0        0        0      484 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
+-rw-r--r--   0        0        0     1241 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
+-rw-r--r--   0        0        0      733 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
+-rw-r--r--   0        0        0      526 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0006_alter_theme_background.py
+-rw-r--r--   0        0        0      664 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
+-rw-r--r--   0        0        0      434 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0008_alter_theme_default.py
+-rw-r--r--   0        0        0      976 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0009_navbar.py
+-rw-r--r--   0        0        0      507 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0010_theme_navbar.py
+-rw-r--r--   0        0        0      612 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0011_navbar_font_size.py
+-rw-r--r--   0        0        0      479 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0012_navbar_text_color.py
+-rw-r--r--   0        0        0      566 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
+-rw-r--r--   0        0        0      604 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
+-rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/__init__.py
+-rw-r--r--   0        0        0     4942 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/models.py
+-rw-r--r--   0        0        0      582 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/signals.py
+-rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/color_converter.py
+-rw-r--r--   0        0        0      740 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/scss_editor.py
+-rw-r--r--   0        0        0      743 2024-04-06 23:56:32.752440 django_dynamic_theme-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2270 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.3/PKG-INFO
```

### Comparing `django_dynamic_theme-0.0.2/LICENSE` & `django_dynamic_theme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/README.md` & `django_dynamic_theme-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-theme)
+[![](https://img.shields.io/pypi/djversions/django-dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
-
+[![Documentation Status](https://readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-theme.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-theme)
 
 # Django Dynamic Theme
 This allows an administrator of a django website to change the theme on the fly.
 
 ## Installation
 
@@ -45,13 +46,13 @@
 3. Assuming you have `base.html` add this to it before the `<body>` tag:
 ```html
 <html>
   ...
   {% load compress %}
   {% load static %}
   {% compress css %}
-  <link type="text/x-scss" rel="stylesheet" href="{% static 'theme.scss' %}" />
+  <link type="text/x-scss" rel="stylesheet" href="{% static theme_file %}" />
   ...
 </html>
 ```
 
 3. Visit `http://127.0.0.1:8000/admin/django_dynamic_theme/` to start customizing your theme.
```

#### html2text {}

```diff
@@ -1,19 +1,23 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-
-theme) [![codecov](https://codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/
-badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-
-theme) # Django Dynamic Theme This allows an administrator of a django website
-to change the theme on the fly. ## Installation ```sh pip install django-
-dynamic-theme ``` ## Quickstart 1. Add the following settings:: ```python
-INSTALLED_APPS = [ ..., "django_dynamic_theme", "compressor", ] ... # Default
-setting but you can set it to some other path. static_url = "static/
-" static_root = "static" STATICFILES_FINDERS = [ ...,
-"compressor.finders.CompressorFinder", ] COMPRESS_PRECOMPILERS = (("text/x-
-scss", "django_libsass.SassCompiler"),) TEMPLATES = { "OPTIONS":
-{ "context_processors": [ ..., "django_dynamic_theme-context_processor.theme",
-] } } ``` 2. Run `python manage.py migrate` 3. Assuming you have `base.html`
-add this to it before the `
+theme) [![](https://img.shields.io/pypi/djversions/django-dynamic-
+theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
+www.djangoproject.com/) [![Documentation Status](https://readthedocs.org/
+projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-
+theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://
+codecov.io/gh/Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This
+allows an administrator of a django website to change the theme on the fly. ##
+Installation ```sh pip install django-dynamic-theme ``` ## Quickstart 1. Add
+the following settings:: ```python INSTALLED_APPS = [ ...,
+"django_dynamic_theme", "compressor", ] ... # Default setting but you can set
+it to some other path. static_url = "static/" static_root = "static"
+STATICFILES_FINDERS = [ ..., "compressor.finders.CompressorFinder", ]
+COMPRESS_PRECOMPILERS = (("text/x-scss", "django_libsass.SassCompiler"),)
+TEMPLATES = { "OPTIONS": { "context_processors": [ ..., "django_dynamic_theme-
+context_processor.theme", ] } } ``` 2. Run `python manage.py migrate` 3.
+Assuming you have `base.html` add this to it before the `
 ` tag: ```html
 ... {% load compress %} {% load static %} {% compress css %}
 ...
 ``` 3. Visit `http://127.0.0.1:8000/admin/django_dynamic_theme/` to start
 customizing your theme.
```

### Comparing `django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0001_initial.py` & `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py` & `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py` & `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0006_alter_theme_background.py` & `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0006_alter_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py` & `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.2/pyproject.toml` & `django_dynamic_theme-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-dynamic-theme"
-version = "0.0.2"
+version = "0.0.3"
 description = "This enables the administrator of a django website to change the theme on the fly."
 authors = ["Segelzwerg <25705862+Segelzwerg@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 django = "^5.0"
```

### Comparing `django_dynamic_theme-0.0.2/PKG-INFO` & `django_dynamic_theme-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: django-dynamic-theme
-Version: 0.0.2
+Version: 0.0.3
 Summary: This enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg
 Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5.0,<6.0)
 Requires-Dist: django-colorfield (>=0.11.0,<0.12.0)
 Requires-Dist: django-compressor (>=4.4,<5.0)
 Requires-Dist: django-libsass (>=0.9,<0.10)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-theme)
+[![](https://img.shields.io/pypi/djversions/django-dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
-
+[![Documentation Status](https://readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-theme.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-theme)
 
 # Django Dynamic Theme
 This allows an administrator of a django website to change the theme on the fly.
 
 ## Installation
 
@@ -61,14 +62,14 @@
 3. Assuming you have `base.html` add this to it before the `<body>` tag:
 ```html
 <html>
   ...
   {% load compress %}
   {% load static %}
   {% compress css %}
-  <link type="text/x-scss" rel="stylesheet" href="{% static 'theme.scss' %}" />
+  <link type="text/x-scss" rel="stylesheet" href="{% static theme_file %}" />
   ...
 </html>
 ```
 
 3. Visit `http://127.0.0.1:8000/admin/django_dynamic_theme/` to start customizing your theme.
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.2 Summary: This
+Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.3 Summary: This
 enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.12,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: django
 (>=5.0,<6.0) Requires-Dist: django-colorfield (>=0.11.0,<0.12.0) Requires-Dist:
 django-compressor (>=4.4,<5.0) Requires-Dist: django-libsass (>=0.9,<0.10)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0) Description-Content-Type: text/
 markdown ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-django-dynamic-theme) [![codecov](https://codecov.io/gh/Segelzwerg/django-
-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/
-Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This allows an
-administrator of a django website to change the theme on the fly. ##
+django-dynamic-theme) [![](https://img.shields.io/pypi/djversions/django-
+dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
+www.djangoproject.com/) [![Documentation Status](https://readthedocs.org/
+projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-
+theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
+gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://
+codecov.io/gh/Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This
+allows an administrator of a django website to change the theme on the fly. ##
 Installation ```sh pip install django-dynamic-theme ``` ## Quickstart 1. Add
 the following settings:: ```python INSTALLED_APPS = [ ...,
 "django_dynamic_theme", "compressor", ] ... # Default setting but you can set
 it to some other path. static_url = "static/" static_root = "static"
 STATICFILES_FINDERS = [ ..., "compressor.finders.CompressorFinder", ]
 COMPRESS_PRECOMPILERS = (("text/x-scss", "django_libsass.SassCompiler"),)
 TEMPLATES = { "OPTIONS": { "context_processors": [ ..., "django_dynamic_theme-
```

