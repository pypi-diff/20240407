# Comparing `tmp/django-intra-0.1.0.tar.gz` & `tmp/django-intra-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-intra-0.1.0.tar", last modified: Thu Apr  4 22:28:20 2024, max compression
+gzip compressed data, was "django-intra-0.2.0.tar", last modified: Sun Apr  7 00:07:02 2024, max compression
```

## Comparing `django-intra-0.1.0.tar` & `django-intra-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 22:28:14.000000 django-intra-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-04 22:28:20.300956 django-intra-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-04 22:28:14.000000 django-intra-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/django_intra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 22:28:20.000000 django-intra-0.1.0/django_intra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/intra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/intra_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 22:28:14.000000 django-intra-0.1.0/intra/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 22:28:14.000000 django-intra-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-04 22:28:20.304956 django-intra-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:28:14.000000 django-intra-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:20.300956 django-intra-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-04 22:28:14.000000 django-intra-0.1.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-07 00:06:57.000000 django-intra-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-07 00:07:02.736379 django-intra-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-07 00:06:57.000000 django-intra-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/django_intra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.732379 django-intra-0.2.0/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/intra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 00:06:57.000000 django-intra-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-07 00:07:02.736379 django-intra-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:06:57.000000 django-intra-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/urls.py
```

### Comparing `django-intra-0.1.0/LICENSE` & `django-intra-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/README.md` & `django-intra-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+[![PyPI](https://img.shields.io/pypi/v/django-intra)](https://pypi.org/project/django-intra/)
 [![Pylint](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/pylint.yml)
 [![Django CI](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/test.yml)
+[![Upload Python Package](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml/badge.svg)](https://github.com/ahmdhjj/django-intra/actions/workflows/release.yml)
 # django-intra
+## Docs
+https://ahmdhjj.github.io/django-intra/
+
+## Installation
+```
+pip install django-intra
+```
 ## Settings
 In your settings file:
+
 1. Add `'intra'` to `INSTALLED_APPS`.
-3. Add `'intra/templates'` to the `DIRS` option in the `TEMPLATES` setting.
+
+2. Add `'intra/templates'` to the `DIRS` option in the `TEMPLATES` setting:
 ```
   TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': ['intra/templates'],
         'APP_DIRS': True,
         'OPTIONS': {
```

### Comparing `django-intra-0.1.0/intra/urls.py` & `django-intra-0.2.0/intra/urls.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/setup.cfg` & `django-intra-0.2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [metadata]
 name = django-intra
-version = 0.1.0
+version = 0.2.0
 description = An extension of the Django admin application with special features
-long_description = An extension of the Django admin application with special features
+long_description = file: README.md
+long_description_content_type = text/markdown
 url = https://github.com/ahmdhjj/django-intra
+project_urls = 
+	Documentation = https://ahmdhjj.github.io/django-intra/
+	Source = https://github.com/ahmdhjj/django-intra
+	Tracker = https://github.com/ahmdhjj/django-intra/issues
 author = ahmdhjj
-author_email = ahmdhjj@example.com
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
-	Topic :: Internet :: WWW/HTTP
-	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	Django >= 4.2
```

### Comparing `django-intra-0.1.0/tests/settings.py` & `django-intra-0.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.1.0/tests/tests.py` & `django-intra-0.2.0/tests/tests.py`

 * *Files identical despite different names*

