# Comparing `tmp/djangocms-form-builder-0.1.tar.gz` & `tmp/djangocms_form_builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-form-builder-0.1.tar", last modified: Tue Jan 17 20:26:45 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `djangocms-form-builder-0.1.tar` & `djangocms_form_builder-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.112313 djangocms-form-builder-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-01-17 20:26:45.112313 djangocms-form-builder-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.104313 djangocms-form-builder-0.1/djangocms_form_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.108313 djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/ajax_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/form_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/entry_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.108313 djangocms-form-builder-0.1/djangocms_form_builder/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/frontends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/frontends/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/frontends/foundation6.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.108313 djangocms-form-builder-0.1/djangocms_form_builder/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/migrations/0002_alter_form_cmsplugin_ptr_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/recaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.112313 djangocms-form-builder-0.1/djangocms_form_builder/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/templatetags/form_builder_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/djangocms_form_builder/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.108313 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-01-17 20:26:45.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-17 20:26:45.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:26:45.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:26:44.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-17 20:26:45.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-17 20:26:45.000000 djangocms-form-builder-0.1/djangocms_form_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-17 20:26:45.112313 djangocms-form-builder-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:45.112313 djangocms-form-builder-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_form_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_formeditor.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-17 20:26:36.000000 djangocms-form-builder-0.1/tests/urls.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/__init__.py
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/actions.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/admin.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/apps.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/constants.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/entry_model.py
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/fields.py
+-rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/forms.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/helpers.py
+-rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/models.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/recaptcha.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/settings.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/urls.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/views.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/__init__.py
+-rw-r--r--   0        0        0    13955 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/ajax_plugins.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/form_plugins.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/legacy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/frontends/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/frontends/bootstrap5.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/frontends/foundation6.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/locale/sq/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/0001_initial.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/0002_alter_form_cmsplugin_ptr_and_more.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/0003_auto_20230129_1950.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/static/djangocms_form_builder/css/actions_form.css
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/static/djangocms_form_builder/css/button_group.css
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/static/djangocms_form_builder/js/actions_form.js
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/captcha/includes/js_v2_checkbox.html
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/captcha/includes/js_v2_invisible.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/ajax_base.html
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/ajax_form.html
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/admin/widgets/button_group.html
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/admin/widgets/button_group_color_option.html
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/admin/widgets/button_group_option.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/admin/widgets/icon_group_option.html
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/admin/widgets/select.html
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/form.html
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/render/field.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/render/form.html
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/render/section.html
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/widgets/base.html
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/bootstrap5/widgets/submit.html
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/mails/default/mail_html.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/widgets/input_option.html
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_form_builder/widgets/mutliple_input.html
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templates/djangocms_frontend/admin/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templatetags/__init__.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/djangocms_form_builder/templatetags/form_builder_tags.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/README.rst
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 djangocms_form_builder-0.1.1/PKG-INFO
```

### Comparing `djangocms-form-builder-0.1/LICENSE` & `djangocms_form_builder-0.1.1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Copyright (c) 2017, Divio AG
+Copyright (c) 2022, Fabian Braun
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
-    * Neither the name of Divio AG nor the
+    * Neither the name of Fabian Braun, the django CMS association nor the
       names of its contributors may be used to endorse or promote products
       derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL DIVIO AG BE LIABLE FOR ANY
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/__init__.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from django.utils.translation import gettext_lazy as _
 except ModuleNotFoundError:
     _ = lambda x: x
 
 
-__version__ = "0.1"
+__version__ = "0.1.1"
 
 _form_registry = {}
 
 
 def verbose_name(form_class):
     """returns the verbose_name property of a Meta class if present or else
     splits the camel-cased form class name"""
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/actions.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,135 @@
-import hashlib
+import copy
+import decimal
 
-from django.core.exceptions import ImproperlyConfigured
-from django.core.mail import mail_admins, send_mail
-from django.template.loader import render_to_string
-from django.utils.html import strip_tags
-from django.utils.translation import gettext_lazy as _
-
-from .entry_model import FormEntry
-from .helpers import get_option
-
-_action_registry = {}
-
-
-def get_registered_actions():
-    """Creates a tuple for a ChoiceField to select form"""
-    result = tuple(
-        (hash, action_class.verbose_name)
-        for hash, action_class in _action_registry.items()
-    )
-    return result if result else ((_("No actions registered"), ()),)
-
-
-def register(action_class):
-    """Function to call or decorator for an Action class to make it available for the plugin"""
-
-    if not issubclass(action_class, FormAction):
-        raise ImproperlyConfigured(
-            "djangocms_form_builder.actions.register only "
-            "accepts subclasses of djangocms_form_builder.actions.FormAction"
+from django.apps import apps
+from django.db.models import ObjectDoesNotExist
+from django.template.exceptions import TemplateDoesNotExist
+from django.template.loader import select_template
+from django.utils.functional import lazy
+from django.utils.safestring import mark_safe
+
+from . import settings
+
+global_options = settings.FORM_OPTIONS
+
+
+def get_option(form, option, default=None):
+    form_options = getattr(getattr(form, "Meta", None), "options", {})
+    return form_options.get(option, global_options.get(option, default))
+
+
+def get_related_object(scope, field_name):
+    """
+    Returns the related field, referenced by the content of a ModelChoiceField.
+    """
+    try:
+        Model = apps.get_model(scope[field_name]["model"])
+        relobj = Model.objects.get(pk=scope[field_name]["pk"])
+    except (ObjectDoesNotExist, LookupError):
+        relobj = None
+    return relobj
+
+
+def insert_fields(
+    fieldsets, new_fields, block=None, position=-1, blockname=None, blockattrs=None
+):
+    """
+    creates a copy of fieldsets inserting the new fields either in the indexed block at the position,
+    or - if no block is given - at the end
+    """
+    if blockattrs is None:
+        blockattrs = dict()
+    if block is None:
+        fs = (
+            list(fieldsets[:position] if position != -1 else fieldsets)
+            + [
+                (
+                    blockname,
+                    {
+                        "classes": ("collapse",) if len(fieldsets) > 0 else (),
+                        "fields": list(new_fields),
+                        **blockattrs,
+                    },
+                )
+            ]
+            + list(fieldsets[position:] if position != -1 else [])
         )
-    if not action_class.verbose_name:
-        raise ImproperlyConfigured(
-            "FormActions need to have a verbose_name property to be registered",
+        return fs
+    modify = copy.deepcopy(fieldsets[block])
+    fields = modify[1]["fields"]
+    if position >= 0:
+        modify[1]["fields"] = (
+            list(fields[:position]) + list(new_fields) + list(fields[position:])
         )
-    hash = hashlib.sha1(action_class.__name__.encode("utf-8")).hexdigest()
-    _action_registry.update({hash: action_class})
-    return action_class
-
-
-def get_action_class(action):
-    return _action_registry.get(action, None)
+    else:
+        modify[1]["fields"] = (
+            list(fields[: position + 1] if position != -1 else fields)
+            + list(new_fields)
+            + list(fields[position + 1 :] if position != -1 else [])
+        )
+    fs = (
+        list(fieldsets[:block] if block != -1 else fieldsets)
+        + [modify]
+        + list(fieldsets[block + 1 :] if block != -1 else [])
+    )
+    return fs
 
 
-class FormAction:
-    verbose_name = None
+def first_choice(choices):
+    for value, verbose in choices:
+        if not isinstance(verbose, (tuple, list)):
+            return value
+        else:
+            first = first_choice(verbose)
+            if first is not None:
+                return first
+    return None
 
-    def execute(self, form, request):
-        raise NotImplementedError()
 
+def get_template_path(prefix, template, name):
+    return (
+        f"djangocms_form_builder/{settings.framework}/{prefix}/{template}/{name}.html"
+    )
 
-@register
-class SaveToDBAction(FormAction):
-    verbose_name = _("Save form submission")
 
-    def execute(self, form, request):
-        if get_option(form, "unique", False) and get_option(
-            form, "login_required", False
-        ):
-            keys = {
-                "form_name": get_option(form, "form_name"),
-                "form_user": request.user,
-            }
-            defaults = {}
+def get_plugin_template(instance, prefix, name, templates):
+    template = getattr(instance, "template", first_choice(templates))
+    template_path = get_template_path(prefix, template, name)
+
+    try:
+        select_template([template_path])
+    except TemplateDoesNotExist:
+        # TODO render a warning inside the template
+        template_path = get_template_path(prefix, "default", name)
+
+    return template_path
+
+
+# use mark_safe_lazy to delay the translation when using mark_safe
+# otherwise they will not be added to /locale/
+# https://docs.djangoproject.com/en/1.11/topics/i18n/translation/#other-uses-of-lazy-in-delayed-translations
+mark_safe_lazy = lazy(mark_safe, str)
+
+
+def add_plugin(placeholder, plugin):
+    """CMS version save function to add a plugin to a placeholder"""
+    if hasattr(placeholder, "add_plugin"):  # CMS v4?
+        placeholder.add_plugin(plugin)
+    else:  # CMS < v4
+        if plugin.parent:
+            plugin.position -= plugin.parent.position + 1
         else:
-            keys = {}
-            defaults = {
-                "form_name": get_option(form, "form_name"),
-                "form_user": request.user,
-            }
-        defaults.update(
-            {
-                "entry_data": form.cleaned_data,
-                "html_headers": dict(
-                    user_agent=request.headers["User-Agent"],
-                    referer=request.headers["Referer"],
-                ),
-            }
-        )
-        if keys:  # update_or_create only works if at least one key is given
-            try:
-                FormEntry.objects.update_or_create(**keys, defaults=defaults)
-            except FormEntry.MultipleObjectsReturned:  # Delete outdated objects
-                FormEntry.objects.filter(**keys).delete()
-                FormEntry.objects.create(**keys, **defaults)
-        else:
-            FormEntry.objects.create(**defaults), True
+            plugin.position = 0
+        plugin.save()
 
 
-SAVE_TO_DB_ACTION = next(iter(_action_registry)) if _action_registry else None
+def delete_plugin(plugin):
+    """CMS version save function to delete a plugin (and its descendants) from a placeholder"""
+    return plugin.placeholder.delete_plugin(plugin)
 
 
-@register
-class SendMailAction(FormAction):
-    verbose_name = _("Send email to administrators")
-    recipients = None
-    from_mail = None
-    template = "djangocms_form_builder/actions/mail.html"
-    subject = _("%(form_name)s form submission")
-
-    def execute(self, form, request):
-        context = dict(
-            cleaned_data=form.cleaned_data,
-            user=request.user,
-            user_agent=request.headers["User-Agent"],
-            referer=request.headers["Referer"],
-        )
-        html_message = render_to_string(self.template, context)
-        message = strip_tags(html_message)
-        if self.recipients is None:
-            mail_admins(
-                self.subject % dict(form_name=""),
-                message,
-                fail_silently=True,
-                html_message=html_message,
-            )
-        else:
-            send_mail(
-                self.subject % dict(form_name=""),
-                message,
-                self.recipients,
-                self.from_mail,
-                fail_silently=True,
-                html_message=html_message,
-            )
+def coerce_decimal(value):
+    try:
+        return decimal.Decimal(value)
+    except TypeError:
+        return None
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/admin.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/apps.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.urls import NoReverseMatch, clear_url_caches, include, path, reverse
 from django.utils.translation import gettext_lazy as _
 
 
 class FormsConfig(AppConfig):
     default_auto_field = "django.db.models.BigAutoField"
     name = "djangocms_form_builder"
-    verbose_name = _("django CMS form builder")
+    verbose_name = _("Form builder")
 
     def ready(self):
         """Install the URLs"""
         try:
             reverse("form_builder:ajaxview", args=(1,))
         except NoReverseMatch:  # Not installed yet
             urlconf_module = import_module(settings.ROOT_URLCONF)
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/__init__.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/ajax_plugins.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/ajax_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from urllib.parse import urlencode
 
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
 from django.http import Http404, JsonResponse
 from django.template.context_processors import csrf
 from django.template.loader import render_to_string
@@ -10,14 +11,15 @@
 from django.utils.translation import gettext_lazy as _
 from django.views.generic.edit import FormMixin
 from sekizai.context import SekizaiContext
 
 from djangocms_form_builder import settings
 
 from .. import forms, models, recaptcha
+from ..actions import ActionMixin
 from ..forms import SimpleFrontendForm
 from ..helpers import get_option, insert_fields, mark_safe_lazy
 
 
 class CMSAjaxBase(CMSPluginBase):
     def ajax_post(self, request, instance, parameter):
         return JsonResponse({})
@@ -42,26 +44,28 @@
                 "errors": errors,
                 "field_errors": {},
                 "content": content,
             }
         )
 
     def form_valid(self, form):
+        # Execute save method
         save = getattr(form, "save", None)
+        if callable(save):
+            result = form.save()
+        # Identify redirect
         redirect = get_option(form, "redirect", None)
         if isinstance(redirect, str):
             try:
                 redirect = reverse(redirect)
             except NoReverseMatch:
                 pass
         elif hasattr(redirect, "get_absolute_url"):
             redirect = redirect.get_absolute_url()
 
-        if callable(save):
-            form.save()
         get_success_context = "get_success_context"
         render_success = "render_success"
         if hasattr(form, "slug"):
             get_success_context += "_" + form.slug
             render_success += "_" + form.slug
 
         if get_option(form, render_success, None):
@@ -238,19 +242,19 @@
             "form": form,
             "uid": f"{instance.id}{getattr(form, 'slug', '')}-{context['form_counter']}",
         })
         return context
 
 
 @plugin_pool.register_plugin
-class FormPlugin(CMSAjaxForm):
+class FormPlugin(ActionMixin, CMSAjaxForm):
     name = _("Form")
     model = models.Form
 
-    # form = forms.FormsForm
+    form = forms.FormsForm
     render_template = f"djangocms_form_builder/{settings.framework}/form.html"
     change_form_template = "djangocms_frontend/admin/base.html"
     allow_children = True
 
     fieldsets = [
         (
             None,
@@ -263,60 +267,64 @@
                         "form_unique",
                     ),
                     "form_floating_labels",
                     "form_spacing",
                 ],
             },
         ),
-        (
-            _("Actions"),
-            {
-                "classes": ("collapse",),
-                "fields": ["form_actions"],
-            },
-        ),
     ]
 
     cache_parent_classes = False
 
     @classmethod
     def get_parent_classes(cls, slot, page, instance=None):
         """Only valid if not inside form"""
         parent = instance
         while parent is not None:
-            if parent.plugin_type == FormPlugin.__name__:
+            if parent.plugin_type == cls.__name__:
                 return [""]
             parent = parent.parent
         return super().get_parent_classes(slot, page, instance)
 
     def get_fieldsets(self, request, obj=None):
+        fieldsets = super().get_fieldsets(request, obj)
+        if obj is None or not obj.form_selection:  # No Actions if a Django form has been selected
+            fieldsets = insert_fields(
+                fieldsets,
+                ("form_actions",),
+                block=None,
+                position=1,
+                blockname=_("Actions"),
+                blockattrs={"classes": ("collapse", "action-auto-hide")},
+            )
         if recaptcha.installed:
             return insert_fields(
-                super().get_fieldsets(request, obj),
+                fieldsets,
                 ("captcha_widget", "captcha_requirement", "captcha_config"),
                 block=None,
                 position=1,
-                blockname=_("reCaptcha"),
+                blockname=_("Captcha"),
                 blockattrs={}
                 if recaptcha.keys_available
                 else dict(
                     description=mark_safe_lazy(
                         _(
                             '<blockquote style="color: var(--error-fg);">Please get a public and secret '
                             'key from <a href="{key_link}" target="_blank">Google</a> '
                             "and ensure that they are available through django settings "
                             "<code>RECAPTCHA_PUBLIC_KEY</code> and <code>RECAPTCHA_PRIVATE_KEY</code>. "
                             "Without these keys captcha protection will not work.</blockquote>"
                         ).format(key_link="https://developers.google.com/recaptcha")
                     )
                 ),
             )
-        return super().get_fieldsets(request, obj)
+        return fieldsets
 
     def get_form_class(self, slug=None):
+        """Retrieve or create form for this plugin"""
         if self.instance.child_plugin_instances is None:  # not set if in ajax_post
             self.instance.child_plugin_instances = [
                 child.get_plugin_instance()[0] for child in self.instance.get_children()
             ]
         if self.instance.child_plugin_instances:
             return self.create_form_class_from_plugins()
         if self.instance.form_selection:
@@ -341,30 +349,36 @@
                 traverse(child)
 
         fields = {}
         traverse(self.instance)
 
         # Add recaptcha field in necessary
         if recaptcha.installed and self.instance.captcha_widget:
-            fields[recaptcha.field_name] = recaptcha.get_recaptcha_field(self.instance.captcha_config)
+            fields[recaptcha.field_name] = recaptcha.get_recaptcha_field(self.instance)
 
         # Collect meta options for Meta class
         meta_options = dict(form_name=self.instance.form_name)
         if self.instance.form_floating_labels:
             meta_options["floating_labels"] = True
         meta_options[
             "field_sep"
         ] = f'{self.instance.form_spacing}'
         meta_options[
             "redirect"
         ] = self.instance.placeholder.page  # Default behavior: redirect to same page
         meta_options["login_required"] = self.instance.form_login_required
         meta_options["unique"] = self.instance.form_unique
-        meta_options["form_actions"] = self.instance.form_actions
-        fields["Meta"] = type("Meta", (), dict(options=meta_options))  # Meta class
+        form_actions = self.instance.form_actions or "[]"
+        meta_options["form_actions"] = json.loads(form_actions.replace("'", '"'))
+        meta_options["form_parameters"] = getattr(self.instance, "action_parameters", {})
+
+        fields["Meta"] = type("Meta", (), dict(
+            options=meta_options,
+            verbose_name=self.instance.form_name.replace("-", " ").replace("_", " ").capitalize(),
+        ))  # Meta class with options and verbose name
 
         return type(
             "FrontendAutoForm",
             (SimpleFrontendForm,),
             fields,
         )
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/form_plugins.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/form_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/cms_plugins/legacy.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/cms_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/constants.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/entry_model.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/entry_model.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/fields.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/forms.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import validate_slug
-from django.forms import ModelForm
 from django.utils.translation import gettext_lazy as _
 from entangled.forms import EntangledModelForm, EntangledModelFormMixin
 
 from . import (
     _form_registry,
     actions,
     constants,
     get_registered_forms,
+    models,
     recaptcha,
     settings,
 )
 from .entry_model import FormEntry
-from .fields import AttributesFormField, ButtonGroup, ChoicesFormField, TagTypeFormField
+from .fields import AttributesFormField, ButtonGroup, ChoicesFormField
 from .helpers import get_option, mark_safe_lazy
-from .models import FormField
 
 
 class Noop:
     pass
 
 
 def mixin_factory(x):
@@ -55,54 +54,65 @@
             Action = actions.get_action_class(action)
             if Action is not None:
                 results[action] = Action().execute(self, self._request)
             else:
                 results[action] = _("Action not available any more")
         if not form_actions:
             results[None] = _("No action registered")
+        return results
 
 
-class FormsForm(mixin_factory("Form"), ModelForm):
+class SelectMultipleActionsWidget(forms.CheckboxSelectMultiple):
+    def format_value(self, value):
+        import json
+
+        if isinstance(value, str):
+            value = json.loads(value.replace("'", '"'))
+        return super().format_value(value)
+
+
+class FormsForm(mixin_factory("Form"), EntangledModelForm):
     """
     Components > "Forms" Plugin
     https://getbootstrap.com/docs/5.1/forms/overview/
     """
 
     class Meta:
-        model = FormField
+        model = models.Form
         exclude = ()
+        untangled_fields = [
+            "form_selection",
+            "form_name",
+            "form_login_required",
+            "form_unique",
+            "form_floating_labels",
+            "form_spacing",
+            "form_actions",
+            "attributes",
+            "captcha_widget",
+            "captcha_requirement",
+            "captcha_config",
+        ]
         entangled_fields = {
-            "config": [
-                "form_selection",
-                "form_name",
-                "form_login_required",
-                "form_unique",
-                "form_floating_labels",
-                "form_spacing",
-                "form_actions",
-                "attributes",
-                "captcha_widget",
-                "captcha_requirement",
-                "captcha_config",
-            ]
+            "action_parameters": [],
         }
-        untangled_fields = ("tag_type",)
 
     form_selection = forms.ChoiceField(
         label=_("Form"),
         required=False,
         initial="",
     )
     form_name = forms.CharField(
-        label=_("Form name"),
+        label=_("Form identifier"),
         required=False,
         initial="",
         validators=[
             validate_slug,
         ],
+        help_text=_("Slug that allows to uniquely identify forms."),
     )
     form_login_required = forms.BooleanField(
         label=_("Login required to submit form"),
         required=False,
         initial=False,
         help_text=_(
             "To avoid issues with user experience use this type of form only on pages, "
@@ -117,29 +127,30 @@
         help_text=_('Requires "Login required" to be checked to work.'),
     )
 
     form_spacing = forms.ChoiceField(
         label=_("Margin between fields"),
         choices=settings.SPACER_SIZE_CHOICES,
         initial=settings.SPACER_SIZE_CHOICES[len(settings.SPACER_SIZE_CHOICES) // 2][0],
+        required=False,
     )
 
     form_actions = forms.MultipleChoiceField(
         label=_("Actions to be taken after form submission"),
-        widget=forms.CheckboxSelectMultiple(),
+        widget=SelectMultipleActionsWidget(),
         required=False,
     )
 
     attributes = AttributesFormField()
 
     captcha_widget = forms.ChoiceField(
-        label=_("reCaptcha widget"),
+        label=_("Captcha widget"),
         required=False,
         initial="v2-invisible" if recaptcha.installed else "",
-        choices=settings.EMPTY_CHOICE + recaptcha.RECAPTCHA_CHOICES,
+        choices=settings.EMPTY_CHOICE + recaptcha.CAPTCHA_CHOICES,
         help_text=mark_safe_lazy(
             _(
                 'Read more in the <a href="{link}" target="_blank">documentation</a>.'
             ).format(link="https://developers.google.com/recaptcha")
         ),
     )
     captcha_requirement = forms.DecimalField(
@@ -163,29 +174,36 @@
                 "Add these api parameters as attributes, e.g. <code>hl</code> to set the language."
             ).format(
                 attr_link="https://developers.google.com/recaptcha/docs/display#render_param",
                 api_link="https://developers.google.com/recaptcha/docs/display#javascript_resource_apijs_parameters",
             )
         ),
     )
-    tag_type = TagTypeFormField()
 
     def __init__(self, *args, **kwargs):
+        if (
+            not _form_registry
+            and "instance" in kwargs
+            and kwargs["instance"] is not None
+        ):
+            # remove form_selection data if widget will be hidden
+            kwargs["instance"].form_selection = ""
+
         super().__init__(*args, **kwargs)
         registered_forms = get_registered_forms()
         available_form_actions = actions.get_registered_actions()
         self.fields["form_selection"].widget = (
             forms.Select() if _form_registry else forms.HiddenInput()
         )
         self.fields["form_selection"].choices = settings.EMPTY_CHOICE + registered_forms
         self.fields["form_actions"].choices = available_form_actions
 
     def clean(self):
-        if self.cleaned_data["form_selection"] == "":
-            if not self.cleaned_data["form_name"]:
+        if self.cleaned_data.get("form_selection", "") == "":
+            if not self.cleaned_data.get("form_name", "-"):
                 raise ValidationError(
                     {
                         "form_name": _(
                             "Please provide a form name to be able to evaluate form submissions."
                         )
                     },
                     code="incomplete",
@@ -306,51 +324,51 @@
             "If selected form will not accept submissions with with empty data"
         ),
     )
 
 
 class CharFieldForm(mixin_factory("CharField"), FormFieldMixin, EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "min_length",
                 "max_length",
             ]
         }
 
     min_length = forms.IntegerField(
         label=_("Minimum text length"),
         required=False,
         initial=None,
     )
     max_length = forms.IntegerField(
-        label=_("Minimum text length"),
+        label=_("Maximum text length"),
         required=False,
         initial=None,
     )
 
 
 class EmailFieldForm(mixin_factory("EmailField"), FormFieldMixin, EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {"config": []}
 
 
 class UrlFieldForm(mixin_factory("URLField"), FormFieldMixin, EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {"config": []}
 
 
 class DecimalFieldForm(
     mixin_factory("DecimalField"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "min_value",
                 "max_value",
                 "decimal_places",
             ]
         }
@@ -371,15 +389,15 @@
     )
 
 
 class IntegerFieldForm(
     mixin_factory("IntegerField"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "min_value",
                 "max_value",
             ]
         }
 
@@ -393,15 +411,15 @@
     )
 
 
 class TextareaFieldForm(
     mixin_factory("TextareaField"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "min_length",
                 "max_length",
                 "field_rows",
             ]
         }
@@ -423,52 +441,52 @@
         required=False,
         initial=None,
     )
 
 
 class DateFieldForm(mixin_factory("DateField"), FormFieldMixin, EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {"config": []}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["field_placeholder"].help_text = _("Not visible on most browsers.")
 
 
 class DateTimeFieldForm(
     mixin_factory("DateTimeField"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {"config": []}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["field_placeholder"].help_text = _("Not visible on most browsers.")
 
 
 class TimeFieldForm(mixin_factory("TimeField"), FormFieldMixin, EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {"config": []}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["field_placeholder"].help_text = _("Not visible on most browsers.")
 
 
 class SelectFieldForm(mixin_factory("SelectField"), FormFieldMixin, EntangledModelForm):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if "instance" in kwargs and kwargs["instance"] is not None:
             self.fields["field_choices"].initial = kwargs["instance"].get_choices()
 
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "field_select",
             ]
         }
         untangled_fields = ("field_choices",)
 
@@ -502,15 +520,15 @@
                 }
             )
         return self.cleaned_data
 
 
 class ChoiceForm(EntangledModelForm):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "value",
                 "verbose",
             ]
         }
 
@@ -526,15 +544,15 @@
     )
 
 
 class BooleanFieldForm(
     mixin_factory("BooleanField"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "field_as_switch",
             ]
         }
 
     field_as_switch = forms.BooleanField(
@@ -555,15 +573,15 @@
         )
 
 
 class SubmitButtonForm(
     mixin_factory("SubmitButton"), FormFieldMixin, EntangledModelForm
 ):
     class Meta:
-        model = FormField
+        model = models.FormField
         entangled_fields = {
             "config": [
                 "submit_cta",
             ]
         }
 
     submit_cta = forms.CharField(
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/frontends/bootstrap5.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/frontends/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/frontends/foundation6.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/frontends/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/migrations/0001_initial.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/migrations/0002_alter_form_cmsplugin_ptr_and_more.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/migrations/0002_alter_form_cmsplugin_ptr_and_more.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/models.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.forms.widgets import Input
 from django.utils.html import conditional_escape, mark_safe
 from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
 
 from . import recaptcha, settings
 from .entry_model import FormEntry  # NoQA
-from .fields import AttributesField, TagTypeField
+from .fields import AttributesField
 from .helpers import coerce_decimal, mark_safe_lazy
 
 MAX_LENGTH = 256
 
 
 class Form(CMSPlugin):
     class Meta:
@@ -42,45 +42,49 @@
         blank=True,
         default=False,
         help_text=_(
             "To avoid issues with user experience use this type of form only on pages, "
             "which require login."
         ),
     )
-
     form_unique = models.BooleanField(
         verbose_name=_("User can reopen form"),
         default=False,
         help_text=_('Requires "Login required" to be checked to work.'),
     )
-
     form_floating_labels = models.BooleanField(
         verbose_name=_("Floating labels"),
         default=False,
     )
     form_spacing = models.CharField(
         verbose_name=_("Margin between fields"),
         max_length=16,
     )
 
     form_actions = models.CharField(
         verbose_name=_("Actions to be taken after form submission"),
         blank=True,
         max_length=4 * MAX_LENGTH,
-        # widget=forms.CheckboxSelectMultiple(),
+    )
+
+    action_parameters = models.JSONField(
+        default=dict,
+        encoder=DjangoJSONEncoder,
+        blank=True,
+        null=True,
     )
 
     attributes = AttributesField()
 
     captcha_widget = models.CharField(
-        verbose_name=_("reCaptcha widget"),
+        verbose_name=_("captcha widget"),
         max_length=16,
         blank=True,
         default="v2-invisible" if recaptcha.installed else "",
-        choices=settings.EMPTY_CHOICE + recaptcha.RECAPTCHA_CHOICES,
+        choices=settings.EMPTY_CHOICE + recaptcha.CAPTCHA_CHOICES,
         help_text=mark_safe_lazy(
             _(
                 'Read more in the <a href="{link}" target="_blank">documentation</a>.'
             ).format(link="https://developers.google.com/recaptcha")
         ),
     )
     captcha_requirement = models.DecimalField(
@@ -104,15 +108,14 @@
                 "Add these api parameters as attributes, e.g. <code>hl</code> to set the language."
             ).format(
                 attr_link="https://developers.google.com/recaptcha/docs/display#render_param",
                 api_link="https://developers.google.com/recaptcha/docs/display#javascript_resource_apijs_parameters",
             )
         ),
     )
-    tag_type = TagTypeField()
 
     def get_short_description(self):
         return f"({self.form_name})" if self.form_name else "<unnamed>"
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.id})"
 
@@ -123,15 +126,14 @@
     called "config".
     """
 
     class Meta:
         verbose_name = gettext("Form field item")
 
     ui_item = models.CharField(max_length=30)
-    tag_type = TagTypeField(blank=True)
     config = models.JSONField(default=dict, encoder=DjangoJSONEncoder)
 
     def __init__(self, *args, **kwargs):
         self._additional_classes = []
         super().__init__(*args, **kwargs)
 
     def __getattr__(self, item):
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/settings.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import importlib
 
 from django.conf import settings as django_settings
+from django.utils.translation import gettext_lazy as _
 
 EMPTY_CHOICE = (("", "-----"),)
 
 ADMIN_CSS = getattr(
     django_settings,
     "DJANGOCMS_FRONTEND_ADMIN_CSS",
     {},
 )
 
 
 FORM_OPTIONS = getattr(django_settings, "DJANGOCMS_FORMS_OPTIONS", {})
-
+MAIL_TEMPLATE_SETS = getattr(django_settings, "DJANGOCMS_MAIL_TEMPLATE_SETS", (
+    ("default", _("Default")),
+))
 
 framework = getattr(django_settings, "DJANGOCMS_FRONTEND_FRAMEWORK", "bootstrap5")
 theme = getattr(django_settings, "DJANGOCMS_FRONTEND_THEME", "djangocms_frontend")
 
-
-SPACER_SIZE_CHOICES = (("mb-3", "Default"),)
+DEFAULT_SPACER_SIZE_CHOICES = (("mb-3", "Default"),)
 TAG_CHOICES = (("div", "div"),)
 FORM_TEMPLATE = getattr(
     django_settings,
     "FORM_TEMPLATE",
     f"djangocms_form_builder/{framework}/render/form.html",
 )
 
 theme_render_path = f"{theme}.frameworks.{framework}"
 theme_forms_path = f"{theme}.forms"
 
+if not getattr(django_settings, 'DJANGO_FORM_BUILDER_SPACER_CHOICES', False):
+    if not getattr(django_settings, 'DJANGOCMS_FRONTEND_SPACER_SIZES', False):
+        SPACER_SIZE_CHOICES = DEFAULT_SPACER_SIZE_CHOICES
+    else:
+        SPACER_SIZE_CHOICES = ((f"mb-{key}", value) for key, value in django_settings.DJANGOCMS_FRONTEND_SPACER_SIZES)
+else:
+    SPACER_SIZE_CHOICES = django_settings.DJANGO_FORM_BUILDER_SPACER_CHOICES
+
 
 def render_factory(cls, theme_module, render_module):
     parents = tuple(
         getattr(module, cls, None)
         for module in (theme_module, render_module)
         if module is not None and getattr(module, cls, None) is not None
     )
```

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/templatetags/form_builder_tags.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/templatetags/form_builder_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-form-builder-0.1/djangocms_form_builder/views.py` & `djangocms_form_builder-0.1.1/djangocms_form_builder/views.py`

 * *Files identical despite different names*

