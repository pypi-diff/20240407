# Comparing `tmp/django-formset-1.3.8.tar.gz` & `tmp/django-formset-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.3.8.tar", last modified: Sun Feb 11 08:48:18 2024, max compression
+gzip compressed data, was "django-formset-1.3.9.tar", last modified: Fri Mar 29 22:28:36 2024, max compression
```

## Comparing `django-formset-1.3.8.tar` & `django-formset-1.3.9.tar`

### file list

```diff
@@ -1,452 +1,456 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.146271 django-formset-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-11 08:47:13.000000 django-formset-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-11 08:47:13.000000 django-formset-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-02-11 08:48:18.146271 django-formset-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-02-11 08:47:13.000000 django-formset-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.146271 django-formset-1.3.8/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-02-11 08:48:18.000000 django-formset-1.3.8/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14635 2024-02-11 08:48:18.000000 django-formset-1.3.8/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 08:48:18.000000 django-formset-1.3.8/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 08:48:17.000000 django-formset-1.3.8/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-11 08:48:18.000000 django-formset-1.3.8/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-11 08:48:18.000000 django-formset-1.3.8/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/af/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/bg/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.078270 django-formset-1.3.8/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.098271 django-formset-1.3.8/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/et/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/eu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/he_IL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.102271 django-formset-1.3.8/formset/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/he_IL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/hr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/hr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/hu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/hy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/hy/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ja/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/lt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.082270 django-formset-1.3.8/formset/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.106271 django-formset-1.3.8/formset/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sr_Latn_BA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.110271 django-formset-1.3.8/formset/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.086270 django-formset-1.3.8/formset/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.090270 django-formset-1.3.8/formset/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.114271 django-formset-1.3.8/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.090270 django-formset-1.3.8/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.090270 django-formset-1.3.8/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.118271 django-formset-1.3.8/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-11 08:48:10.000000 django-formset-1.3.8/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-11 08:48:10.000000 django-formset-1.3.8/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-11 08:48:10.000000 django-formset-1.3.8/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-11 08:48:10.000000 django-formset-1.3.8/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    35875 2024-02-11 08:48:10.000000 django-formset-1.3.8/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.118271 django-formset-1.3.8/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.122271 django-formset-1.3.8/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/Calendar-3E4D43HW.js
--rw-r--r--   0 runner    (1001) docker     (127)    44166 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/CountrySelectize-OY7UUXBC.js
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/DateTime-2CEEHEI3.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/DjangoSelectize-ALXOS5DF.js
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/DjangoSlug-SHZN726V.js
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/DualSelector-QBPMDGUD.js
--rw-r--r--   0 runner    (1001) docker     (127)   269129 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/PhoneNumber-W7FUG5CI.js
--rw-r--r--   0 runner    (1001) docker     (127)   318800 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/RichtextArea-7F64YF45.js
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/SortableSelect-MET5DDXS.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-65OJRBX6.js
--rw-r--r--   0 runner    (1001) docker     (127)    43949 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-7MZNI2NE.js
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-BZTEXDAH.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-FDUUONAQ.js
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-HLC47B2W.js
--rw-r--r--   0 runner    (1001) docker     (127)    56982 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-KMIZLVGN.js
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-LTR6QAFN.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-P2VM2T3G.js
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-SERXULES.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/chunk-W5RPWA2M.js
--rw-r--r--   0 runner    (1001) docker     (127)   116671 2024-02-11 08:48:12.000000 django-formset-1.3.8/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.122271 django-formset-1.3.8/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.090270 django-formset-1.3.8/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.090270 django-formset-1.3.8/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.122271 django-formset-1.3.8/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/calendar/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.126271 django-formset-1.3.8/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.130271 django-formset-1.3.8/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.130271 django-formset-1.3.8/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.130271 django-formset-1.3.8/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.134271 django-formset-1.3.8/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.134271 django-formset-1.3.8/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/country_selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.134271 django-formset-1.3.8/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.134271 django-formset-1.3.8/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.134271 django-formset-1.3.8/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.142271 django-formset-1.3.8/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.146271 django-formset-1.3.8/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.146271 django-formset-1.3.8/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 08:48:18.146271 django-formset-1.3.8/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templatetags/phonenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    19652 2024-02-11 08:47:13.000000 django-formset-1.3.8/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 08:48:18.146271 django-formset-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-11 08:47:13.000000 django-formset-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.803767 django-formset-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-29 22:28:12.000000 django-formset-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-29 22:28:12.000000 django-formset-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-03-29 22:28:36.803767 django-formset-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-03-29 22:28:12.000000 django-formset-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.803767 django-formset-1.3.9/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 22:28:36.000000 django-formset-1.3.9/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.731767 django-formset-1.3.9/formset/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/af/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.731767 django-formset-1.3.9/formset/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/bg/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.751767 django-formset-1.3.9/formset/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/et/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/eu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.755767 django-formset-1.3.9/formset/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/he_IL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/hr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/hr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.735767 django-formset-1.3.9/formset/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/hy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/hy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ja/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/lt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.759767 django-formset-1.3.9/formset/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.763767 django-formset-1.3.9/formset/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/sr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.739767 django-formset-1.3.9/formset/locale/sr_Latn_BA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.767767 django-formset-1.3.9/formset/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-03-29 22:28:35.000000 django-formset-1.3.9/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.771767 django-formset-1.3.9/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.771767 django-formset-1.3.9/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.771767 django-formset-1.3.9/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-29 22:28:32.000000 django-formset-1.3.9/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-29 22:28:32.000000 django-formset-1.3.9/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-29 22:28:32.000000 django-formset-1.3.9/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 22:28:32.000000 django-formset-1.3.9/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    35875 2024-03-29 22:28:33.000000 django-formset-1.3.9/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.771767 django-formset-1.3.9/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/Calendar-OQTG3ONX.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44166 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/CountrySelectize-NOGU4FDW.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/DateTime-WMTYZZNN.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/DjangoSelectize-R66DE3UZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/DjangoSlug-SHZN726V.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/DualSelector-RRDODSQ4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   269129 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/PhoneNumber-SS26COAZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)   318800 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/RichtextArea-X76JZ5BK.js
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/SortableSelect-XTYK7VPU.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-65OJRBX6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43949 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-7MZNI2NE.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-FDUUONAQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-HLC47B2W.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-JPH23CAJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-LVGJ2KIX.js
+-rw-r--r--   0 runner    (1001) docker     (127)    57771 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-ORXTVVOI.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-P2VM2T3G.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-SERXULES.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/chunk-W5RPWA2M.js
+-rw-r--r--   0 runner    (1001) docker     (127)   120994 2024-03-29 22:28:34.000000 django-formset-1.3.9/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.747767 django-formset-1.3.9/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.743767 django-formset-1.3.9/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/calendar/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.779767 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.783767 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.783767 django-formset-1.3.9/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.783767 django-formset-1.3.9/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.783767 django-formset-1.3.9/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.787767 django-formset-1.3.9/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.787767 django-formset-1.3.9/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/detached_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.787767 django-formset-1.3.9/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/country_selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.791767 django-formset-1.3.9/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.791767 django-formset-1.3.9/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.791767 django-formset-1.3.9/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.799767 django-formset-1.3.9/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.803767 django-formset-1.3.9/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.803767 django-formset-1.3.9/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:36.803767 django-formset-1.3.9/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templatetags/phonenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-29 22:28:12.000000 django-formset-1.3.9/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:28:36.803767 django-formset-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-29 22:28:12.000000 django-formset-1.3.9/setup.py
```

### Comparing `django-formset-1.3.8/LICENSE` & `django-formset-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/PKG-INFO` & `django-formset-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.3.8
-Summary: Prevalidate Django Forms in the browser
+Version: 1.3.9
+Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,19 +18,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.0
 
-# django-formset – Better UX for Django Forms 
+# django-formset – Better User Experience for Django Forms 
 
 This library handles single forms and collections of forms with a way better user experience than
 the internal Django implementation for
 [formsets](https://docs.djangoproject.com/en/stable/topics/forms/formsets/) offers.
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
@@ -43,15 +44,15 @@
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
     recipient = fields.CharField(label="Recipient")
-    postal_code = fields.CharField("Postal Code")
+    postal_code = fields.CharField(label="Postal Code")
     city = fields.CharField(label="City")
 ```
 
 After creating a
 [Django FormView](https://docs.djangoproject.com/en/stable/ref/class-based-views/generic-editing/#django.views.generic.edit.FormView)
 we can render the above form using a slightly modified template:
 
@@ -100,15 +101,15 @@
 ![Multiple Inputs](readmeimg/bootstrap-multiple-input.png)
 
 
 ### File Uploading Widget
 
 Uploading files is performed asynchronously, separating the payload upload from its form submission.
 It provides a drag-and-drop widget plus a file select button. This allows to preview uploaded files
-before form submission. It also make the submission much faster, because the file is already in a
+before form submission. It also makes the submission much faster, because the file is already in a
 temporary location on the server.
 
 | Empty file upload                         | Pending file upload                 |
 |-------------------------------------------|-------------------------------------|
 | ![](readmeimg/bootstrap-upload-empty.png) | ![](readmeimg/bootstrap-upload.png) |
 
 
@@ -137,18 +138,18 @@
   reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
-In **django-formset**, the button used for submission can hold a chain of actions. This for instance
-allows to disable the button, and/or add a spinning wheel while submitting data. It also is possible
-to specify the success page as a HTML link, rather than having it to hard-code inside the Django
-view. There is a complete set of predefined actions to select from, when designing the submit
+In **django-formset**, the button used for submission can hold a *chain of actions*. This for
+instance allows to disable the button, and/or add a spinning wheel while submitting data. It also is
+possible to specify the success page as an HTML link, rather than having it to hard-code inside the
+Django view. There is a complete set of predefined actions to select from, when designing the submit
 button.
 
 ![Button Actions (Bootstrap)](readmeimg/bootstrap-actions.gif)
 
 
 ## Immediate Form Validation
 
@@ -188,14 +189,27 @@
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
 By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
 `df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
+## Alternative Widgets
+
+**django-formset** provides alternative widgets for many fields provided by Django. For instance:
+
+### Widgets for Django's `DateField`
+
+Modern browsers provide a built-in date picker, which now can be used instead of the default
+`<input type="text">` widget. In addition to that, **django-formset** provides custom web components
+which adopt themselves to the chosen CSS framework. This allows to render the date picker in the
+same style as the rest of the form.
+
+
+
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
 Django 4. This allows to create special renderers for each of the supported CSS frameworks. In
 addition to the form structure proposed by those framework vendors, this library adds private HTML
@@ -203,15 +217,15 @@
 
 The form or the collections of forms then is wrapped by the provided
 [webcomponent](https://developer.mozilla.org/en-US/docs/Web/Web_Components) `<django-formset>`.
 The JavaScript part (actually TypeScript) making up that webcomponent then handles the form
 validation, its submission, instantiation or removal of collection siblings, etc.
 
 Some of the widgets described above (select with autocomplete, file upload) also require JavaScript
-code. The client side functionality of those widgets is also is handled by that webcomponent.
+code. The client side functionality of those widgets also is handled by that webcomponent.
 Widgets which require autocompletion use the same endpoint as that webcomponent itself. So there is
 no need to add extra endpoints to the URL router.
 
 This finally means, that an enduser must _only_ import this single JavaScript file and wrap its
 single form or collection of forms into a single HTML element such as
 
 ```html
@@ -226,21 +240,16 @@
 
 The form classes can be reused unaltered, except for replacing the widgets if desired or required
 (the `FileField` requires a different widget).
 
 
 ## Reference Documentation
 
-Reference documentation can be found on
-[Read The Docs](https://django-formset.readthedocs.io/en/latest/index.html).
-
-
-## Demo
-
-A [demo](https://django-formset.fly.dev/) showing all combinations of fields.
+Reference documentation with interactive samples can be found at
+[https://django-formset.fly.dev/](https://django-formset.fly.dev/).
 
 
 ## Motivation
 
 Instead of using a `<form>`-tag and include all its fields, here we wrap the complete form inside
 the special webcomponent `<django-formset>`. It allows the client to communicate with the Django
 view (we name this "endpoint") using the
@@ -260,15 +269,15 @@
 * Before submitting, all form fields are prevalidated by the browser, using the same constraints as
   declared for each Django form or model field in Python.
 * The form's data is sent by an Ajax request, preventing a full page reload. This gives a much
   better user experience.
 * Server side validation errors are sent back to the browser, and rendered near the offending
   form field.
 * Non-field validation errors are renderer together with the form.
-* CSRF-tokens are handled through a HTTP-Header, hence there is no need to add a hidden input field
+* CSRF-tokens are handled through an HTTP-Header, hence there is no need to add a hidden input field
   to each form.
 * Forms can be rendered for different CSS frameworks using their specific style-guides for arranging
   HTML. Curently **django-formset** includes renderers for:
 
   * [Bootstrap 5](https://getbootstrap.com/docs/5.0/forms/overview/),
   * [Bulma](https://bulma.io/documentation/form/general/),
   * [Foundation 6](https://get.foundation/sites/docs/forms.html),
@@ -289,9 +298,9 @@
   the data from this form or collection of forms is sent to the server as a group a separate
   entities.
 * Such a form-collection can be declared to have a list siblings, which can be changed in length
   using one "Add" and multiple "Remove" buttons.
 * Form fields or fieldsets can be hidden or disabled using a Boolean expression as condition.
 
 [^1]: Tailwind is special here, since it doesn't include purpose-built form control classes out of
-      the box. Instead **django-formset** offers an opinionated set of CSS classes suitable for
+      the box. Instead, **django-formset** offers an opinionated set of CSS classes suitable for
       Tailwind.
```

### Comparing `django-formset-1.3.8/README.md` & `django-formset-1.3.9/django_formset.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,37 @@
-# django-formset – Better UX for Django Forms 
+Metadata-Version: 2.1
+Name: django-formset
+Version: 1.3.9
+Summary: The missing widgets and form manipulation library for Django
+Home-page: https://github.com/jrief/django-formset
+Author: Jacob Rief
+Author-email: jacob.rief@gmail.com
+License: MIT
+Keywords: Django Forms,webcomponent
+Platform: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django>=4.0
+
+# django-formset – Better User Experience for Django Forms 
 
 This library handles single forms and collections of forms with a way better user experience than
 the internal Django implementation for
 [formsets](https://docs.djangoproject.com/en/stable/topics/forms/formsets/) offers.
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
@@ -15,15 +44,15 @@
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
     recipient = fields.CharField(label="Recipient")
-    postal_code = fields.CharField("Postal Code")
+    postal_code = fields.CharField(label="Postal Code")
     city = fields.CharField(label="City")
 ```
 
 After creating a
 [Django FormView](https://docs.djangoproject.com/en/stable/ref/class-based-views/generic-editing/#django.views.generic.edit.FormView)
 we can render the above form using a slightly modified template:
 
@@ -72,15 +101,15 @@
 ![Multiple Inputs](readmeimg/bootstrap-multiple-input.png)
 
 
 ### File Uploading Widget
 
 Uploading files is performed asynchronously, separating the payload upload from its form submission.
 It provides a drag-and-drop widget plus a file select button. This allows to preview uploaded files
-before form submission. It also make the submission much faster, because the file is already in a
+before form submission. It also makes the submission much faster, because the file is already in a
 temporary location on the server.
 
 | Empty file upload                         | Pending file upload                 |
 |-------------------------------------------|-------------------------------------|
 | ![](readmeimg/bootstrap-upload-empty.png) | ![](readmeimg/bootstrap-upload.png) |
 
 
@@ -109,18 +138,18 @@
   reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
-In **django-formset**, the button used for submission can hold a chain of actions. This for instance
-allows to disable the button, and/or add a spinning wheel while submitting data. It also is possible
-to specify the success page as a HTML link, rather than having it to hard-code inside the Django
-view. There is a complete set of predefined actions to select from, when designing the submit
+In **django-formset**, the button used for submission can hold a *chain of actions*. This for
+instance allows to disable the button, and/or add a spinning wheel while submitting data. It also is
+possible to specify the success page as an HTML link, rather than having it to hard-code inside the
+Django view. There is a complete set of predefined actions to select from, when designing the submit
 button.
 
 ![Button Actions (Bootstrap)](readmeimg/bootstrap-actions.gif)
 
 
 ## Immediate Form Validation
 
@@ -160,14 +189,27 @@
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
 By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
 `df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
+## Alternative Widgets
+
+**django-formset** provides alternative widgets for many fields provided by Django. For instance:
+
+### Widgets for Django's `DateField`
+
+Modern browsers provide a built-in date picker, which now can be used instead of the default
+`<input type="text">` widget. In addition to that, **django-formset** provides custom web components
+which adopt themselves to the chosen CSS framework. This allows to render the date picker in the
+same style as the rest of the form.
+
+
+
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
 Django 4. This allows to create special renderers for each of the supported CSS frameworks. In
 addition to the form structure proposed by those framework vendors, this library adds private HTML
@@ -175,15 +217,15 @@
 
 The form or the collections of forms then is wrapped by the provided
 [webcomponent](https://developer.mozilla.org/en-US/docs/Web/Web_Components) `<django-formset>`.
 The JavaScript part (actually TypeScript) making up that webcomponent then handles the form
 validation, its submission, instantiation or removal of collection siblings, etc.
 
 Some of the widgets described above (select with autocomplete, file upload) also require JavaScript
-code. The client side functionality of those widgets is also is handled by that webcomponent.
+code. The client side functionality of those widgets also is handled by that webcomponent.
 Widgets which require autocompletion use the same endpoint as that webcomponent itself. So there is
 no need to add extra endpoints to the URL router.
 
 This finally means, that an enduser must _only_ import this single JavaScript file and wrap its
 single form or collection of forms into a single HTML element such as
 
 ```html
@@ -198,21 +240,16 @@
 
 The form classes can be reused unaltered, except for replacing the widgets if desired or required
 (the `FileField` requires a different widget).
 
 
 ## Reference Documentation
 
-Reference documentation can be found on
-[Read The Docs](https://django-formset.readthedocs.io/en/latest/index.html).
-
-
-## Demo
-
-A [demo](https://django-formset.fly.dev/) showing all combinations of fields.
+Reference documentation with interactive samples can be found at
+[https://django-formset.fly.dev/](https://django-formset.fly.dev/).
 
 
 ## Motivation
 
 Instead of using a `<form>`-tag and include all its fields, here we wrap the complete form inside
 the special webcomponent `<django-formset>`. It allows the client to communicate with the Django
 view (we name this "endpoint") using the
@@ -232,15 +269,15 @@
 * Before submitting, all form fields are prevalidated by the browser, using the same constraints as
   declared for each Django form or model field in Python.
 * The form's data is sent by an Ajax request, preventing a full page reload. This gives a much
   better user experience.
 * Server side validation errors are sent back to the browser, and rendered near the offending
   form field.
 * Non-field validation errors are renderer together with the form.
-* CSRF-tokens are handled through a HTTP-Header, hence there is no need to add a hidden input field
+* CSRF-tokens are handled through an HTTP-Header, hence there is no need to add a hidden input field
   to each form.
 * Forms can be rendered for different CSS frameworks using their specific style-guides for arranging
   HTML. Curently **django-formset** includes renderers for:
 
   * [Bootstrap 5](https://getbootstrap.com/docs/5.0/forms/overview/),
   * [Bulma](https://bulma.io/documentation/form/general/),
   * [Foundation 6](https://get.foundation/sites/docs/forms.html),
@@ -261,9 +298,9 @@
   the data from this form or collection of forms is sent to the server as a group a separate
   entities.
 * Such a form-collection can be declared to have a list siblings, which can be changed in length
   using one "Add" and multiple "Remove" buttons.
 * Form fields or fieldsets can be hidden or disabled using a Boolean expression as condition.
 
 [^1]: Tailwind is special here, since it doesn't include purpose-built form control classes out of
-      the box. Instead **django-formset** offers an opinionated set of CSS classes suitable for
+      the box. Instead, **django-formset** offers an opinionated set of CSS classes suitable for
       Tailwind.
```

### Comparing `django-formset-1.3.8/django_formset.egg-info/PKG-INFO` & `django-formset-1.3.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,8 @@
-Metadata-Version: 2.1
-Name: django-formset
-Version: 1.3.8
-Summary: Prevalidate Django Forms in the browser
-Home-page: https://github.com/jrief/django-formset
-Author: Jacob Rief
-Author-email: jacob.rief@gmail.com
-License: MIT
-Keywords: Django Forms,webcomponent
-Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django>=4.0
-
-# django-formset – Better UX for Django Forms 
+# django-formset – Better User Experience for Django Forms 
 
 This library handles single forms and collections of forms with a way better user experience than
 the internal Django implementation for
 [formsets](https://docs.djangoproject.com/en/stable/topics/forms/formsets/) offers.
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
@@ -43,15 +15,15 @@
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
     recipient = fields.CharField(label="Recipient")
-    postal_code = fields.CharField("Postal Code")
+    postal_code = fields.CharField(label="Postal Code")
     city = fields.CharField(label="City")
 ```
 
 After creating a
 [Django FormView](https://docs.djangoproject.com/en/stable/ref/class-based-views/generic-editing/#django.views.generic.edit.FormView)
 we can render the above form using a slightly modified template:
 
@@ -100,15 +72,15 @@
 ![Multiple Inputs](readmeimg/bootstrap-multiple-input.png)
 
 
 ### File Uploading Widget
 
 Uploading files is performed asynchronously, separating the payload upload from its form submission.
 It provides a drag-and-drop widget plus a file select button. This allows to preview uploaded files
-before form submission. It also make the submission much faster, because the file is already in a
+before form submission. It also makes the submission much faster, because the file is already in a
 temporary location on the server.
 
 | Empty file upload                         | Pending file upload                 |
 |-------------------------------------------|-------------------------------------|
 | ![](readmeimg/bootstrap-upload-empty.png) | ![](readmeimg/bootstrap-upload.png) |
 
 
@@ -137,18 +109,18 @@
   reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
-In **django-formset**, the button used for submission can hold a chain of actions. This for instance
-allows to disable the button, and/or add a spinning wheel while submitting data. It also is possible
-to specify the success page as a HTML link, rather than having it to hard-code inside the Django
-view. There is a complete set of predefined actions to select from, when designing the submit
+In **django-formset**, the button used for submission can hold a *chain of actions*. This for
+instance allows to disable the button, and/or add a spinning wheel while submitting data. It also is
+possible to specify the success page as an HTML link, rather than having it to hard-code inside the
+Django view. There is a complete set of predefined actions to select from, when designing the submit
 button.
 
 ![Button Actions (Bootstrap)](readmeimg/bootstrap-actions.gif)
 
 
 ## Immediate Form Validation
 
@@ -188,14 +160,27 @@
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
 By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
 `df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
+## Alternative Widgets
+
+**django-formset** provides alternative widgets for many fields provided by Django. For instance:
+
+### Widgets for Django's `DateField`
+
+Modern browsers provide a built-in date picker, which now can be used instead of the default
+`<input type="text">` widget. In addition to that, **django-formset** provides custom web components
+which adopt themselves to the chosen CSS framework. This allows to render the date picker in the
+same style as the rest of the form.
+
+
+
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
 Django 4. This allows to create special renderers for each of the supported CSS frameworks. In
 addition to the form structure proposed by those framework vendors, this library adds private HTML
@@ -203,15 +188,15 @@
 
 The form or the collections of forms then is wrapped by the provided
 [webcomponent](https://developer.mozilla.org/en-US/docs/Web/Web_Components) `<django-formset>`.
 The JavaScript part (actually TypeScript) making up that webcomponent then handles the form
 validation, its submission, instantiation or removal of collection siblings, etc.
 
 Some of the widgets described above (select with autocomplete, file upload) also require JavaScript
-code. The client side functionality of those widgets is also is handled by that webcomponent.
+code. The client side functionality of those widgets also is handled by that webcomponent.
 Widgets which require autocompletion use the same endpoint as that webcomponent itself. So there is
 no need to add extra endpoints to the URL router.
 
 This finally means, that an enduser must _only_ import this single JavaScript file and wrap its
 single form or collection of forms into a single HTML element such as
 
 ```html
@@ -226,21 +211,16 @@
 
 The form classes can be reused unaltered, except for replacing the widgets if desired or required
 (the `FileField` requires a different widget).
 
 
 ## Reference Documentation
 
-Reference documentation can be found on
-[Read The Docs](https://django-formset.readthedocs.io/en/latest/index.html).
-
-
-## Demo
-
-A [demo](https://django-formset.fly.dev/) showing all combinations of fields.
+Reference documentation with interactive samples can be found at
+[https://django-formset.fly.dev/](https://django-formset.fly.dev/).
 
 
 ## Motivation
 
 Instead of using a `<form>`-tag and include all its fields, here we wrap the complete form inside
 the special webcomponent `<django-formset>`. It allows the client to communicate with the Django
 view (we name this "endpoint") using the
@@ -260,15 +240,15 @@
 * Before submitting, all form fields are prevalidated by the browser, using the same constraints as
   declared for each Django form or model field in Python.
 * The form's data is sent by an Ajax request, preventing a full page reload. This gives a much
   better user experience.
 * Server side validation errors are sent back to the browser, and rendered near the offending
   form field.
 * Non-field validation errors are renderer together with the form.
-* CSRF-tokens are handled through a HTTP-Header, hence there is no need to add a hidden input field
+* CSRF-tokens are handled through an HTTP-Header, hence there is no need to add a hidden input field
   to each form.
 * Forms can be rendered for different CSS frameworks using their specific style-guides for arranging
   HTML. Curently **django-formset** includes renderers for:
 
   * [Bootstrap 5](https://getbootstrap.com/docs/5.0/forms/overview/),
   * [Bulma](https://bulma.io/documentation/form/general/),
   * [Foundation 6](https://get.foundation/sites/docs/forms.html),
@@ -289,9 +269,9 @@
   the data from this form or collection of forms is sent to the server as a group a separate
   entities.
 * Such a form-collection can be declared to have a list siblings, which can be changed in length
   using one "Add" and multiple "Remove" buttons.
 * Form fields or fieldsets can be hidden or disabled using a Boolean expression as condition.
 
 [^1]: Tailwind is special here, since it doesn't include purpose-built form control classes out of
-      the box. Instead **django-formset** offers an opinionated set of CSS classes suitable for
+      the box. Instead, **django-formset** offers an opinionated set of CSS classes suitable for
       Tailwind.
```

### Comparing `django-formset-1.3.8/django_formset.egg-info/SOURCES.txt` & `django-formset-1.3.9/django_formset.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_formset.egg-info/not-zip-safe
 django_formset.egg-info/requires.txt
 django_formset.egg-info/top_level.txt
 formset/__init__.py
 formset/boundfield.py
 formset/calendar.py
 formset/collection.py
+formset/dialog.py
 formset/exceptions.py
 formset/fields.py
 formset/fieldset.py
 formset/ranges.py
 formset/upload.py
 formset/utils.py
 formset/validators.py
@@ -135,30 +136,30 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/Calendar-3E4D43HW.js
-formset/static/formset/js/CountrySelectize-OY7UUXBC.js
-formset/static/formset/js/DateTime-2CEEHEI3.js
-formset/static/formset/js/DjangoSelectize-ALXOS5DF.js
+formset/static/formset/js/Calendar-OQTG3ONX.js
+formset/static/formset/js/CountrySelectize-NOGU4FDW.js
+formset/static/formset/js/DateTime-WMTYZZNN.js
+formset/static/formset/js/DjangoSelectize-R66DE3UZ.js
 formset/static/formset/js/DjangoSlug-SHZN726V.js
-formset/static/formset/js/DualSelector-QBPMDGUD.js
-formset/static/formset/js/PhoneNumber-W7FUG5CI.js
-formset/static/formset/js/RichtextArea-7F64YF45.js
-formset/static/formset/js/SortableSelect-MET5DDXS.js
+formset/static/formset/js/DualSelector-RRDODSQ4.js
+formset/static/formset/js/PhoneNumber-SS26COAZ.js
+formset/static/formset/js/RichtextArea-X76JZ5BK.js
+formset/static/formset/js/SortableSelect-XTYK7VPU.js
 formset/static/formset/js/chunk-65OJRBX6.js
 formset/static/formset/js/chunk-7MZNI2NE.js
-formset/static/formset/js/chunk-BZTEXDAH.js
 formset/static/formset/js/chunk-FDUUONAQ.js
 formset/static/formset/js/chunk-HLC47B2W.js
-formset/static/formset/js/chunk-KMIZLVGN.js
-formset/static/formset/js/chunk-LTR6QAFN.js
+formset/static/formset/js/chunk-JPH23CAJ.js
+formset/static/formset/js/chunk-LVGJ2KIX.js
+formset/static/formset/js/chunk-ORXTVVOI.js
 formset/static/formset/js/chunk-P2VM2T3G.js
 formset/static/formset/js/chunk-SERXULES.js
 formset/static/formset/js/chunk-W5RPWA2M.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
@@ -190,33 +191,36 @@
 formset/templates/formset/bulma/widgets/checkbox.html
 formset/templates/formset/bulma/widgets/dual_selector.html
 formset/templates/formset/bulma/widgets/file.html
 formset/templates/formset/bulma/widgets/input_option.html
 formset/templates/formset/bulma/widgets/multiple_input.html
 formset/templates/formset/bulma/widgets/select.html
 formset/templates/formset/default/collection.html
+formset/templates/formset/default/detached_field.html
 formset/templates/formset/default/dialog_form.html
 formset/templates/formset/default/field_errors.html
 formset/templates/formset/default/field_group.html
 formset/templates/formset/default/fieldset.html
 formset/templates/formset/default/form.html
+formset/templates/formset/default/form_dialog.html
 formset/templates/formset/default/help_text.html
 formset/templates/formset/default/buttons/add_collection.html
 formset/templates/formset/default/buttons/move_all_left.html
 formset/templates/formset/default/buttons/move_all_right.html
 formset/templates/formset/default/buttons/move_selected_left.html
 formset/templates/formset/default/buttons/move_selected_right.html
 formset/templates/formset/default/buttons/redo_selected.html
 formset/templates/formset/default/buttons/remove_collection.html
 formset/templates/formset/default/buttons/richtext_align.html
 formset/templates/formset/default/buttons/richtext_color.html
 formset/templates/formset/default/buttons/richtext_control.html
 formset/templates/formset/default/buttons/richtext_heading.html
 formset/templates/formset/default/buttons/richtext_separator.html
 formset/templates/formset/default/buttons/undo_selected.html
+formset/templates/formset/default/widgets/button.html
 formset/templates/formset/default/widgets/calendar.html
 formset/templates/formset/default/widgets/country_selectize.html
 formset/templates/formset/default/widgets/datetime.html
 formset/templates/formset/default/widgets/dual_selector.html
 formset/templates/formset/default/widgets/file.html
 formset/templates/formset/default/widgets/multiple_input.html
 formset/templates/formset/default/widgets/richtextarea.html
```

### Comparing `django-formset-1.3.8/formset/boundfield.py` & `django-formset-1.3.9/formset/boundfield.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,65 +2,20 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models.fields.files import FieldFile
 from django.forms import boundfield
 from django.forms.fields import FileField, JSONField
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
+from formset.fields import Activator
+from formset.renderers import ClassList
 from formset.upload import get_file_info
 from formset.widgets import UploadedFileInput
 
 
-class ClassList(set):
-    """
-    Inspired by JavaScript's classlist on HTMLElement
-    """
-    __slots__ = ()
-
-    def __init__(self, css_classes=None):
-        if css_classes is None:
-            super().__init__()
-        elif isinstance(css_classes, (list, set, tuple)):
-            super().__init__(css_classes)
-        elif isinstance(css_classes, str):
-            super().__init__(css_classes.split())
-        else:
-            raise TypeError(f"Can not convert {css_classes.__class__} to ClassList")
-
-    def __bool__(self):
-        return len(self) > 0
-
-    def add(self, css_classes):
-        for css_class in ClassList(css_classes):
-            super().add(css_class)
-        return self
-
-    def remove(self, css_classes):
-        for css_class in ClassList(css_classes):
-            if css_class in self:
-                super().remove(css_class)
-        return self
-
-    def toggle(self, css_classes, condition=None):
-        for css_class in ClassList(css_classes):
-            if css_class in self:
-                if condition in (None, False):
-                    super().remove(css_class)
-            else:
-                if condition in (None, True):
-                    super().add(css_class)
-        return self
-
-    def render(self):
-        return ' '.join(self)
-
-    __str__ = render
-    __html__ = render
-
-
 class CheckboxInputMixin:
     """
     This hack is required for adding the field's label to the rendering context.
     This is to make the single checkbox to be rendered with its label after the input field.
     """
     def get_context(self, name, value, attrs):
         context = super().get_context(name, value, attrs)
@@ -96,14 +51,17 @@
         attrs = super().build_widget_attrs(attrs, widget)
         if hasattr(self.form, 'form_id'):
             attrs['form'] = self.form.form_id
         if hasattr(self.field, 'regex'):
             attrs['pattern'] = self.field.regex.pattern
         if isinstance(self.field, JSONField):
             attrs['use_json'] = True
+        if isinstance(self.field, Activator):
+            label = self.name.replace('_', ' ').title() if self.field.label is None else self.field.label
+            attrs['label'] = label  # remember label for ButtonWidget.get_context()
         return attrs
 
     def css_classes(self, extra_classes=None):
         """
         Return a string of space-separated CSS classes for this field.
         """
         extra_classes = ClassList(extra_classes)
```

### Comparing `django-formset-1.3.8/formset/calendar.py` & `django-formset-1.3.9/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/collection.py` & `django-formset-1.3.9/formset/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,44 @@
 from django.forms.utils import ErrorDict, ErrorList, RenderableMixin
 from django.forms.widgets import MediaDefiningClass
 from django.utils.datastructures import MultiValueDict
 from django.utils.text import get_text_list
 from django.utils.translation import gettext_lazy
 
 from formset.exceptions import FormCollectionError
+from formset.fields import Activator
 from formset.renderers.default import FormRenderer
-from formset.utils import MARKED_FOR_REMOVAL, FormMixin, FormsetErrorList, HolderMixin
+from formset.utils import MARKED_FOR_REMOVAL, FormMixin, FormsetErrorList, HolderMixin, RenderableDetachedFieldMixin
 
 COLLECTION_ERRORS = '_collection_errors_'
 
 
 class FormCollectionMeta(MediaDefiningClass):
     """
     Collect Forms declared on the base classes.
     """
     def __new__(cls, name, bases, attrs):
         # Collect forms and sub-collections from current class and remove them from attrs.
         attrs['declared_holders'] = {}
         for key, value in list(attrs.items()):
-            if isinstance(value, (BaseForm, BaseFormCollection)):
+            if isinstance(value, (BaseForm, BaseFormCollection, Activator)):
                 attrs.pop(key)
                 setattr(value, '_name', key)
+                if isinstance(value, Activator) and not isinstance(value, RenderableDetachedFieldMixin):
+                    value.__class__ = type(
+                        value.__class__.__name__,
+                        (RenderableDetachedFieldMixin, value.__class__),
+                        {}
+                    )
                 if isinstance(value, BaseForm) and not isinstance(value, FormMixin):
-                    value.__class__ = type(value.__class__.__name__, (FormMixin, value.__class__), {})
+                    value.__class__ = type(
+                        value.__class__.__name__,
+                        (FormMixin, value.__class__),
+                        {}
+                    )
                     value.error_class = FormsetErrorList
                 attrs['declared_holders'][key] = value
 
         new_class = super().__new__(cls, name, bases, attrs)
 
         # Walk through the MRO.
         declared_holders = {}
@@ -130,22 +141,23 @@
                 renderer=self.renderer,
                 ignore_marked_for_removal=self.ignore_marked_for_removal,
             )
             holder.is_single = True
             yield holder
 
     def iter_many(self):
-        num_siblings = max(self.min_siblings, self.extra_siblings)
         if self.initial:
             if not isinstance(self.initial, list):
                 errmsg = "{class_name} is declared to have siblings, but provided argument `{argument}` is not a list"
                 raise FormCollectionError(errmsg.format(class_name=self.__class__.__name__, argument='initial'))
-            num_siblings = max(num_siblings, len(self.initial)) + self.extra_siblings
+            num_siblings = max(self.min_siblings, len(self.initial) + self.extra_siblings)
             if self.max_siblings is not None:
                 num_siblings = min(self.max_siblings, num_siblings)
+        else:
+            num_siblings = max(self.min_siblings, self.extra_siblings)
 
         first, last = 0, len(self.declared_holders.items()) - 1
         # add initialized collections/forms
         for position in range(num_siblings):
             for item_num, (name, declared_holder) in enumerate(self.declared_holders.items()):
                 prefix = f'{self.prefix}.{position}.{name}' if self.prefix else f'{position}.{name}'
                 initial = None
@@ -225,15 +237,14 @@
             return False
 
         if self._errors is None:
             self.full_clean()
             self.validate_siblings_count()
         return is_valid(self._errors)
 
-
     def full_clean(self):
         if self.has_many:
             self.valid_holders = []
             self._errors = ErrorList()
             for index, data in enumerate(self.data):
                 if data is None:
                     continue
@@ -266,14 +277,17 @@
                     self.valid_holders.append(valid_holders)
                     self._errors.append(errors)
             self.validate_unique()
         else:
             self.valid_holders = {}
             self._errors = ErrorDict()
             for name, declared_holder in self.declared_holders.items():
+                if not isinstance(declared_holder, (BaseForm, BaseFormCollection)):
+                    # TODO: Button can have a value and could be validated since it is a field
+                    continue
                 if name in self.data:
                     instance = self.retrieve_instance(self.data[name])
                     holder = declared_holder.replicate(
                         data=self.data[name],
                         initial=self.initial.get(name, declared_holder.initial) if self.initial else None,
                         instance=instance,
                         ignore_marked_for_removal=self.ignore_marked_for_removal,
@@ -415,15 +429,15 @@
                     object_data[name] = model_to_dict(instance, opts.fields, opts.exclude)
                 else:
                     object_data[name] = model_to_dict(instance)
         return object_data
 
     def models_to_list(self, queryset):
         """
-        Create initial data from a queryset. This queryset is traversed recusively and shall be
+        Create initial data from a queryset. This queryset is traversed recursively and shall be
         used to fill the initial data for this collection and all its sub-collections and forms.
 
         Forms and Collections which do not correspond to the model given by the starting instance,
         are responsible themselves to override this method in order to access the proper referenced
         models by following the reverse relations through the given foreign keys.
         """
         assert self.has_many, "Method `models_to_list()` can be applied only on a collection with siblings"
```

### Comparing `django-formset-1.3.8/formset/fields.py` & `django-formset-1.3.9/formset/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 from django.core import checks
 from django.db.models.fields.related import ManyToManyField
+from django.forms import fields
 
-from formset.widgets import DualSortableSelector
+from formset.utils import HolderMixin
+from formset.widgets import Button, DualSortableSelector
+
+
+class Activator(HolderMixin, fields.Field):
+    widget = Button
+    default_renderer = None
+    # template_name = 'formset/default/activator.html'
+
+    def __init__(self, **kwargs):
+        kwargs.update(
+            required=False,
+            validators=[],
+            label_suffix='',
+        )
+        super().__init__(**kwargs)
 
 
 class SortableMultipleChoiceMixin:
     def clean(self, value):
         qs = super().clean(value)
         return qs, value
```

### Comparing `django-formset-1.3.8/formset/fieldset.py` & `django-formset-1.3.9/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/af/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/af/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/af/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/af/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ar/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ar/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/bg/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/bg/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ca/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ca/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/cs/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/cs/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/da/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/da/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.3.9/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.3.9/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/de/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/de/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/el/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/el/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eo/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eo/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/es/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/es/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/et/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/et/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eu/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eu/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/eu_ES/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fa/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fa/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fi/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fi/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fr/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/fr/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/he/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/he/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/he_IL/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/he_IL/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hr/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/hr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hr/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/hr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hu/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hu/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hy/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/hy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/hy/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/hy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/it/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/it/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ja/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ja/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ko_KR/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/lt/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/lt/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/lv/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/lv/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/mn/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/mn/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/nb/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/nb/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/nl/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/nl/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pl/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pl/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ro/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ro/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ru/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/ru/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sk/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sk/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sl/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sl/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sv/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/sv/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/tr_TR/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/uk/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/uk/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `django-formset-1.3.9/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `django-formset-1.3.9/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/ranges.py` & `django-formset-1.3.9/formset/ranges.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/renderers/bootstrap.py` & `django-formset-1.3.9/formset/renderers/bootstrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.utils.html import format_html
 
-from formset.boundfield import ClassList
+from formset.renderers import ButtonVariant, ClassList
 from formset.renderers.default import FormRenderer as DefaultFormRenderer
 
 
 class FormRenderer(DefaultFormRenderer):
     max_options_per_line = 4
     framework = 'bootstrap'
 
@@ -32,14 +32,21 @@
         context['widget']['attrs']['class'] = ClassList('form-check-input')
         return context
 
     def _amend_select(self, context):
         context['widget']['attrs']['class'] = ClassList('form-select')
         return context
 
+    def _amend_button(self, context):
+        variant = context['widget']['variant']
+        if not isinstance(variant, ButtonVariant):
+            variant = 'outline-secondary'
+        context['widget']['attrs']['class'] = ClassList(f'btn btn-{variant}')
+        return context
+
     def _amend_dual_selector(self, context):
         context.update(
             select_classes='form-select',
             lookup_field_classes='form-control form-control-sm',
         )
         return context
 
@@ -60,45 +67,57 @@
     def _amend_fieldset(self, context):
         context = super()._amend_fieldset(context)
         context.update(
             help_text_template='formset/bootstrap/help_text.html',
         )
         return context
 
+    def _amend_detached_field(self, context):
+        context.update(
+            help_text_template='formset/bootstrap/help_text.html',
+        )
+        return context
+
     def _amend_collection(self, context):
         context = super()._amend_collection(context)
         context.update(
             add_collection_button='formset/bootstrap/buttons/add_collection.html',
             remove_collection_button='formset/bootstrap/buttons/remove_collection.html',
             help_text_template='formset/bootstrap/help_text.html',
         )
         return context
 
+    def _amend_form_dialog(self, context):
+        return context
+
     _context_modifiers = dict(DefaultFormRenderer._context_modifiers, **{
         'django/forms/label.html': _amend_label,
         'django/forms/widgets/text.html': _amend_input,
         'django/forms/widgets/email.html': _amend_input,
         'django/forms/widgets/date.html': _amend_input,
         'django/forms/widgets/datetime.html': _amend_input,
         'django/forms/widgets/number.html': _amend_input,
         'django/forms/widgets/url.html': _amend_input,
         'django/forms/widgets/password.html': _amend_input,
         'django/forms/widgets/textarea.html': _amend_input,
         'django/forms/widgets/select.html': _amend_select,
         'django/forms/widgets/checkbox.html': _amend_checkbox,
         'django/forms/widgets/checkbox_select.html': _amend_multiple_input,
         'django/forms/widgets/radio.html': _amend_multiple_input,
+        'formset/default/widgets/button.html': _amend_button,
         'formset/default/widgets/calendar.html': _amend_input,
         'formset/default/widgets/datetime.html': _amend_input,
         'formset/default/widgets/file.html': _amend_file,
         'formset/default/widgets/selectize.html': _amend_select,
         'formset/default/widgets/country_selectize.html': _amend_select,
         'formset/default/widgets/dual_selector.html': _amend_dual_selector,
         'formset/default/fieldset.html': _amend_fieldset,
+        'formset/default/detached_field.html': _amend_detached_field,
         'formset/default/collection.html': _amend_collection,
+        'formset/default/form_dialog.html': _amend_form_dialog,
         'formset/default/widgets/richtextarea.html': _amend_input,
     })
 
 
 def richtext_attributes(attrs):
     """
     Converts the internal representation of node attributes into a specific string such as
```

### Comparing `django-formset-1.3.8/formset/renderers/bulma.py` & `django-formset-1.3.9/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/renderers/default.py` & `django-formset-1.3.9/formset/renderers/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import types
 
 from django.forms.renderers import DjangoTemplates
 from django.utils.html import format_html
 
-from formset.boundfield import ClassList
+from formset.renderers import ClassList
 
 
 class FormRenderer(DjangoTemplates):
     """
     The form renderer used for the proper representation of elements from **django-formset**.
     """
 
@@ -52,20 +52,23 @@
         return context
 
     def _amend_label(self, context, hide_checkbox_label=False):
         if self.label_css_classes:
             if not isinstance(context['attrs'], dict):
                 context['attrs'] = {}
             context['attrs']['class'] = ClassList(self.label_css_classes)
-        if hide_checkbox_label and context['field'].widget_type == 'checkbox':
+        widget_type = context['field'].widget_type
+        if hide_checkbox_label and widget_type == 'checkbox':
             # `<label>Label:</label>` is rendered by `{{ field }}`, so remove it to
             # prevent double rendering.
-            context.pop('label', None)
+
             context['attrs'].pop('for', None)
             context['use_tag'] = bool(self.control_css_classes)
+        if widget_type == 'button' and 'label' in context:
+            context['attrs']['content'] = context.pop('label')
         return context
 
     def _amend_feedback(self, context):
         if self.exempt_feedback:
             context['widget']['attrs']['class'].add('dj-exempt-feedback')
         return context
 
@@ -90,33 +93,44 @@
     def _amend_fieldset(self, context):
         context.update(
             css_classes=self.fieldset_css_classes,
             help_text_template='formset/default/help_text.html',
         )
         return context
 
+    def _amend_detached_field(self, context):
+        context.update(
+            help_text_template='formset/default/help_text.html',
+        )
+        return context
+
     def _amend_collection(self, context):
         context.update(
             add_collection_button='formset/default/buttons/add_collection.html',
             remove_collection_button='formset/default/buttons/remove_collection.html',
             help_text_template='formset/default/help_text.html',
             css_classes=self.collection_css_classes,
             add_collection_label=context['collection'].add_label,
         )
         return context
 
+    def _amend_form_dialog(self, context):
+        return context
+
     _context_modifiers = {
         'django/forms/div.html': _amend_form,
         'django/forms/default.html': _amend_form,
         'formset/default/form.html': _amend_form,
         'django/forms/label.html': _amend_label,
         'django/forms/widgets/checkbox_select.html': _amend_multiple_input,
         'django/forms/widgets/radio.html': _amend_multiple_input,
         'formset/default/fieldset.html': _amend_fieldset,
+        'formset/default/detached_field.html': _amend_detached_field,
         'formset/default/collection.html': _amend_collection,
+        'formset/default/form_dialog.html': _amend_form_dialog,
     }
 
     @classmethod
     def _copy_context(cls, context):
         """
         Make a semi-deep copy of context. This is required since the amend-methods
         modify the context before rendering. Python's `copy.deepcopy()` doesn't work
```

### Comparing `django-formset-1.3.8/formset/renderers/foundation.py` & `django-formset-1.3.9/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/renderers/tailwind.py` & `django-formset-1.3.9/formset/renderers/tailwind.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,31 @@
 
     def _amend_checkbox_select(self, context):
         return self._amend_multiple_input(context, 'formset-checkbox-multiple')
 
     def _amend_radio(self, context):
         return self._amend_multiple_input(context, 'formset-radio-select')
 
+    def _amend_button(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-button-default')
+        return context
+
     def _amend_fieldset(self, context):
         context = super()._amend_fieldset(context)
         context.update(
             help_text_template='formset/tailwind/help_text.html',
         )
         return context
 
+    def _amend_detached_field(self, context):
+        context.update(
+            help_text_template='formset/tailwind/help_text.html',
+        )
+        return context
+
     def _amend_collection(self, context):
         context = super()._amend_collection(context)
         context.update(
             add_collection_button='formset/tailwind/buttons/add_collection.html',
             remove_collection_button='formset/tailwind/buttons/remove_collection.html',
             help_text_template='formset/tailwind/help_text.html',
         )
@@ -103,16 +113,18 @@
         'django/forms/widgets/number.html': _amend_number_input,
         'django/forms/widgets/password.html': _amend_password_input,
         'django/forms/widgets/textarea.html': _amend_textarea,
         'django/forms/widgets/select.html': _amend_select,
         'django/forms/widgets/checkbox.html': _amend_checkbox,
         'django/forms/widgets/checkbox_select.html': _amend_checkbox_select,
         'django/forms/widgets/radio.html': _amend_radio,
+        'formset/default/widgets/button.html': _amend_button,
         'formset/default/widgets/datepicker.html': _amend_date_input,
         'formset/default/widgets/datetimepicker.html': _amend_date_input,
         'formset/default/widgets/selectize.html': _amend_select,
         'formset/default/widgets/country_selectize.html': _amend_select,
         'formset/default/widgets/dual_selector.html': _amend_dual_selector,
+        'formset/default/detached_field.html': _amend_detached_field,
         'formset/default/fieldset.html': _amend_fieldset,
         'formset/default/collection.html': _amend_collection,
         'formset/default/widgets/richtextarea.html': _amend_textarea,
     })
```

### Comparing `django-formset-1.3.8/formset/renderers/uikit.py` & `django-formset-1.3.9/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/richtext/controls.py` & `django-formset-1.3.9/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/richtext/dialogs.py` & `django-formset-1.3.9/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/richtext/widgets.py` & `django-formset-1.3.9/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/css/bootstrap5-extra.css` & `django-formset-1.3.9/formset/static/formset/css/bootstrap5-extra.css`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 }
 django-formset dialog {
   padding: 0;
   word-wrap: break-word;
   background-color: #fff;
   border: 1px solid var(--bs-border-color-translucent);
   border-radius: 0.5rem;
+  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
+  z-index: 1;
 }
 django-formset dialog .dialog-header {
   display: flex;
   flex-shrink: 0;
   align-items: center;
   justify-content: space-between;
   padding: 1rem 1rem;
   border-bottom: 1px solid var(--bs-border-color);
   border-top-left-radius: calc(0.5rem - 1px);
   border-top-right-radius: calc(0.5rem - 1px);
 }
-django-formset dialog .dialog-header .modal-title {
-  line-height: 1.5;
-  font-weight: bolder;
-  font-size: larger;
+django-formset dialog .dialog-header h3 {
+  margin: 0;
 }
 django-formset dialog .dialog-body {
   position: relative;
   flex: 1 1 auto;
   padding: 1rem;
 }
 django-formset dialog .dialog-footer {
```

### Comparing `django-formset-1.3.8/formset/static/formset/css/bootstrap5-extra.css.map` & `django-formset-1.3.9/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "'AAIC;EACC;IACC;;;AAKD;EACC;EACA;;AAGD;EACC;EACA;EACA;EACA;;AAGD;EACC;;AAIF;EACC;;AAGD;EACC;;AAKC;EACC;;AAKH;EACC;EACA;EAEA,kBCxCS;EDyCT;EACA,eC8b4B;ED7b5B,YCoc4B;EDnc5B;;AAEA;EACC;EACA;EACA;EACA;EACA,SC20CiC;ED10CjC;EACA,wBC8zCiC;ED7zCjC,yBC6zCiC;;AD3zCjC;EACC;;AAGF;EACC;EACA;EACA,SC8SM;;AD5SP;EACC;EACA;EACA;EACA;EACA;EACA,SCsSM;EDpSN;EACA,4BCyyCiC;EDxyCjC,2BCwyCiC;;ADvyCjC;EACC;;;AAMJ;EACC;;;AAED;EACC;EACA;;;AAGA;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC; […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "bootstrap5-extra.css",
-    "mappings": "AAIC;EACC;IACC;;;AAKD;EACC;EACA;;AAGD;EACC;EACA;EACA;EACA;;AAGD;EACC;;AAIF;EACC;;AAGD;EACC;;AAKC;EACC;;AAKH;EACC;EACA;EAEA,kBCxCS;EDyCT;EACA,eC8b4B;;AD7b5B;EACC;EACA;EACA;EACA;EACA,SC80CiC;ED70CjC;EACA,wBCi0CiC;EDh0CjC,yBCg0CiC;;AD/zCjC;EACC,aCuf0B;EDtf1B;EACA;;AAGF;EACC;EACA;EACA,SCgTM;;AD9SP;EACC;EACA;EACA;EACA;EACA;EACA,SCwSM;EDtSN;EACA,4BC2yCiC;ED1yCjC,2BC0yCiC;;ADzyCjC;EACC;;;AAMJ;EACC;;;AAED;EACC;EACA;;;AAGA;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC",
+    "mappings": "AAIC;EACC;IACC;;;AAKD;EACC;EACA;;AAGD;EACC;EACA;EACA;EACA;;AAGD;EACC;;AAIF;EACC;;AAGD;EACC;;AAKC;EACC;;AAKH;EACC;EACA;EAEA,kBCxCS;EDyCT;EACA,eC8b4B;ED7b5B,YCoc4B;EDnc5B;;AAEA;EACC;EACA;EACA;EACA;EACA,SC20CiC;ED10CjC;EACA,wBC8zCiC;ED7zCjC,yBC6zCiC;;AD3zCjC;EACC;;AAGF;EACC;EACA;EACA,SC8SM;;AD5SP;EACC;EACA;EACA;EACA;EACA;EACA,SCsSM;EDpSN;EACA,4BCyyCiC;EDxyCjC,2BCwyCiC;;ADvyCjC;EACC;;;AAMJ;EACC;;;AAED;EACC;EACA;;;AAGA;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC;;;AADD;EACC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../scss/bootstrap5-extra.scss",
         "../../../../node_modules/bootstrap/scss/_variables.scss"
     ],
     "version": 3
```

### Comparing `django-formset-1.3.8/formset/static/formset/css/collections.css` & `django-formset-1.3.9/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/css/tailwind.css` & `django-formset-1.3.9/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-audio.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-empty.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-font.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-missing.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-picture.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-video.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/icons/file-zip.svg` & `django-formset-1.3.9/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/CountrySelectize-OY7UUXBC.js` & `django-formset-1.3.9/formset/static/formset/js/CountrySelectize-NOGU4FDW.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as f
-} from "./chunk-KMIZLVGN.js";
+} from "./chunk-ORXTVVOI.js";
 import "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as m
 } from "./chunk-FDUUONAQ.js";
 import "./chunk-65OJRBX6.js";
 import {
```

### Comparing `django-formset-1.3.8/formset/static/formset/js/DateTime-2CEEHEI3.js` & `django-formset-1.3.9/formset/static/formset/js/DateTime-WMTYZZNN.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as v
-} from "./chunk-BZTEXDAH.js";
+} from "./chunk-JPH23CAJ.js";
 import {
     b as m
 } from "./chunk-W5RPWA2M.js";
 import {
     b as x,
     c as f,
     d as g,
@@ -224,17 +224,17 @@
         }
         get nextInputField() {
             let e = this.hasFocus,
                 t = this.inputFieldsOrder.indexOf(this.inputFields.indexOf(e));
             if (t < this.inputFieldsOrder.length - 1) return this.inputFields[this.inputFieldsOrder[t + 1]]
         }
         transferStyles() {
-            let e = document.createElement("style"),
-                t = !1;
+            let e = document.createElement("style");
             e.innerText = E, document.head.appendChild(e), this.inputElement.style.transition = "none";
+            let t = !1;
             for (let i = 0; e.sheet && i < e.sheet.cssRules.length; i++) {
                 let n = e.sheet.cssRules.item(i),
                     s;
                 switch (n.selectorText) {
                     case this.baseSelector:
                         t = !0;
                         break;
```

### Comparing `django-formset-1.3.8/formset/static/formset/js/DjangoSlug-SHZN726V.js` & `django-formset-1.3.9/formset/static/formset/js/DjangoSlug-SHZN726V.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/DualSelector-QBPMDGUD.js` & `django-formset-1.3.9/formset/static/formset/js/DualSelector-RRDODSQ4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as u
 } from "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as d
-} from "./chunk-LTR6QAFN.js";
+} from "./chunk-LVGJ2KIX.js";
 import "./chunk-7MZNI2NE.js";
 import {
     a as L
 } from "./chunk-FDUUONAQ.js";
 import {
     a as r
 } from "./chunk-65OJRBX6.js";
```

### Comparing `django-formset-1.3.8/formset/static/formset/js/PhoneNumber-W7FUG5CI.js` & `django-formset-1.3.9/formset/static/formset/js/PhoneNumber-SS26COAZ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/RichtextArea-7F64YF45.js` & `django-formset-1.3.9/formset/static/formset/js/RichtextArea-X76JZ5BK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-65OJRBX6.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-65OJRBX6.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-7MZNI2NE.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-7MZNI2NE.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-BZTEXDAH.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-JPH23CAJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-FDUUONAQ.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-FDUUONAQ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-HLC47B2W.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-HLC47B2W.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-KMIZLVGN.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-ORXTVVOI.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,69 +1,69 @@
 import {
-    a as Re
+    a as $e
 } from "./chunk-SERXULES.js";
 import {
-    a as st
+    a as it
 } from "./chunk-FDUUONAQ.js";
 import {
-    a as re
+    a as ie
 } from "./chunk-65OJRBX6.js";
 import {
-    a as Pe,
+    a as Re,
     b as be,
-    c as L
+    c as x
 } from "./chunk-P2VM2T3G.js";
-var Ve = Pe((ye, $e) => {
-    (function(i, u) {
-        typeof ye == "object" && typeof $e < "u" ? u(ye) : typeof define == "function" && define.amd ? define(["exports"], u) : (i = typeof globalThis < "u" ? globalThis : i || self, u(i.sifter = {}))
-    })(ye, function(i) {
+var Ke = Re((ye, Ve) => {
+    (function(r, c) {
+        typeof ye == "object" && typeof Ve < "u" ? c(ye) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.sifter = {}))
+    })(ye, function(r) {
         "use strict";
-        let u = l => (l = l.filter(Boolean), l.length < 2 ? l[0] || "" : o(l) == 1 ? "[" + l.join("") + "]" : "(?:" + l.join("|") + ")"),
+        let c = l => (l = l.filter(Boolean), l.length < 2 ? l[0] || "" : o(l) == 1 ? "[" + l.join("") + "]" : "(?:" + l.join("|") + ")"),
             e = l => {
                 if (!n(l)) return l.join("");
                 let a = "",
-                    c = 0,
+                    u = 0,
                     d = () => {
-                        c > 1 && (a += "{" + c + "}")
+                        u > 1 && (a += "{" + u + "}")
                     };
-                return l.forEach((w, v) => {
-                    if (w === l[v - 1]) {
-                        c++;
+                return l.forEach((T, m) => {
+                    if (T === l[m - 1]) {
+                        u++;
                         return
                     }
-                    d(), a += w, c = 1
+                    d(), a += T, u = 1
                 }), d(), a
             },
             t = l => {
-                let a = p(l);
-                return u(a)
+                let a = f(l);
+                return c(a)
             },
             n = l => new Set(l).size !== l.length,
             s = l => (l + "").replace(/([\$\(-\+\.\?\[-\^\{-\}])/g, "\\$1"),
-            o = l => l.reduce((a, c) => Math.max(a, r(c)), 0),
-            r = l => p(l).length,
-            p = l => Array.from(l);
-        let m = l => {
+            o = l => l.reduce((a, u) => Math.max(a, i(u)), 0),
+            i = l => f(l).length,
+            f = l => Array.from(l);
+        let g = l => {
             if (l.length === 1) return [
                 [l]
             ];
             let a = [],
-                c = l.substring(1);
-            return m(c).forEach(function(w) {
-                let v = w.slice(0);
-                v[0] = l.charAt(0) + v[0], a.push(v), v = w.slice(0), v.unshift(l.charAt(0)), a.push(v)
+                u = l.substring(1);
+            return g(u).forEach(function(T) {
+                let m = T.slice(0);
+                m[0] = l.charAt(0) + m[0], a.push(m), m = T.slice(0), m.unshift(l.charAt(0)), a.push(m)
             }), a
         };
-        let g = [
+        let v = [
                 [0, 65535]
             ],
             E = "[\u0300-\u036F\xB7\u02BE\u02BC]",
-            y, W, U = 3,
-            f = {},
-            z = {
+            M, X, U = 3,
+            h = {},
+            Y = {
                 "/": "\u2044\u2215",
                 0: "\u07C0",
                 a: "\u2C65\u0250\u0251",
                 aa: "\uA733",
                 ae: "\xE6\u01FD\u01E3",
                 ao: "\uA735",
                 au: "\uA737",
@@ -98,396 +98,396 @@
                 v: "\u028B\uA75F\u028C",
                 vy: "\uA761",
                 w: "\u2C73",
                 y: "\u01B4\u024F\u1EFF",
                 z: "\u01B6\u0225\u0240\u2C6C\uA763",
                 hv: "\u0195"
             };
-        for (let l in z) {
-            let a = z[l] || "";
-            for (let c = 0; c < a.length; c++) {
-                let d = a.substring(c, c + 1);
-                f[d] = l
+        for (let l in Y) {
+            let a = Y[l] || "";
+            for (let u = 0; u < a.length; u++) {
+                let d = a.substring(u, u + 1);
+                h[d] = l
             }
         }
-        let k = new RegExp(Object.keys(f).join("|") + "|" + E, "gu"),
+        let H = new RegExp(Object.keys(h).join("|") + "|" + E, "gu"),
             N = l => {
-                y === void 0 && (y = x(l || g))
+                M === void 0 && (M = A(l || v))
             },
             b = (l, a = "NFKD") => l.normalize(a),
-            R = l => p(l).reduce((a, c) => a + Z(c), ""),
-            Z = l => (l = b(l).toLowerCase().replace(k, a => f[a] || ""), b(l, "NFC"));
+            $ = l => f(l).reduce((a, u) => a + W(u), ""),
+            W = l => (l = b(l).toLowerCase().replace(H, a => h[a] || ""), b(l, "NFC"));
 
-        function* $(l) {
-            for (let [a, c] of l)
-                for (let d = a; d <= c; d++) {
-                    let w = String.fromCharCode(d),
-                        v = R(w);
-                    v != w.toLowerCase() && (v.length > U || v.length != 0 && (yield {
-                        folded: v,
-                        composed: w,
+        function* oe(l) {
+            for (let [a, u] of l)
+                for (let d = a; d <= u; d++) {
+                    let T = String.fromCharCode(d),
+                        m = $(T);
+                    m != T.toLowerCase() && (m.length > U || m.length != 0 && (yield {
+                        folded: m,
+                        composed: T,
                         code_point: d
                     }))
                 }
         }
-        let F = l => {
+        let V = l => {
                 let a = {},
-                    c = (d, w) => {
-                        let v = a[d] || new Set,
-                            S = new RegExp("^" + t(v) + "$", "iu");
-                        w.match(S) || (v.add(s(w)), a[d] = v)
+                    u = (d, T) => {
+                        let m = a[d] || new Set,
+                            O = new RegExp("^" + t(m) + "$", "iu");
+                        T.match(O) || (m.add(s(T)), a[d] = m)
                     };
-                for (let d of $(l)) c(d.folded, d.folded), c(d.folded, d.composed);
+                for (let d of oe(l)) u(d.folded, d.folded), u(d.folded, d.composed);
                 return a
             },
-            x = l => {
-                let a = F(l),
-                    c = {},
+            A = l => {
+                let a = V(l),
+                    u = {},
                     d = [];
-                for (let v in a) {
-                    let S = a[v];
-                    S && (c[v] = t(S)), v.length > 1 && d.push(s(v))
-                }
-                d.sort((v, S) => S.length - v.length);
-                let w = u(d);
-                return W = new RegExp("^" + w, "u"), c
-            },
-            q = (l, a = 1) => {
-                let c = 0;
-                return l = l.map(d => (y[d] && (c += d.length), y[d] || d)), c >= a ? e(l) : ""
-            },
-            V = (l, a = 1) => (a = Math.max(a, l.length - 1), u(m(l).map(c => q(c, a)))),
-            Q = (l, a = !0) => {
-                let c = l.length > 1 ? 1 : 0;
-                return u(l.map(d => {
-                    let w = [],
-                        v = a ? d.length() : d.length() - 1;
-                    for (let S = 0; S < v; S++) w.push(V(d.substrs[S] || "", c));
-                    return e(w)
+                for (let m in a) {
+                    let O = a[m];
+                    O && (u[m] = t(O)), m.length > 1 && d.push(s(m))
+                }
+                d.sort((m, O) => O.length - m.length);
+                let T = c(d);
+                return X = new RegExp("^" + T, "u"), u
+            },
+            S = (l, a = 1) => {
+                let u = 0;
+                return l = l.map(d => (M[d] && (u += d.length), M[d] || d)), u >= a ? e(l) : ""
+            },
+            q = (l, a = 1) => (a = Math.max(a, l.length - 1), c(g(l).map(u => S(u, a)))),
+            P = (l, a = !0) => {
+                let u = l.length > 1 ? 1 : 0;
+                return c(l.map(d => {
+                    let T = [],
+                        m = a ? d.length() : d.length() - 1;
+                    for (let O = 0; O < m; O++) T.push(q(d.substrs[O] || "", u));
+                    return e(T)
                 }))
             },
-            X = (l, a) => {
-                for (let c of a) {
-                    if (c.start != l.start || c.end != l.end || c.substrs.join("") !== l.substrs.join("")) continue;
+            z = (l, a) => {
+                for (let u of a) {
+                    if (u.start != l.start || u.end != l.end || u.substrs.join("") !== l.substrs.join("")) continue;
                     let d = l.parts,
-                        w = S => {
-                            for (let M of d) {
-                                if (M.start === S.start && M.substr === S.substr) return !1;
-                                if (!(S.length == 1 || M.length == 1) && (S.start < M.start && S.end > M.start || M.start < S.start && M.end > S.start)) return !0
+                        T = O => {
+                            for (let F of d) {
+                                if (F.start === O.start && F.substr === O.substr) return !1;
+                                if (!(O.length == 1 || F.length == 1) && (O.start < F.start && O.end > F.start || F.start < O.start && F.end > O.start)) return !0
                             }
                             return !1
                         };
-                    if (!(c.parts.filter(w).length > 0)) return !0
+                    if (!(u.parts.filter(T).length > 0)) return !0
                 }
                 return !1
             };
-        class ue {
+        class se {
             constructor() {
                 this.parts = [], this.substrs = [], this.start = 0, this.end = 0
             }
             add(a) {
                 a && (this.parts.push(a), this.substrs.push(a.substr), this.start = Math.min(a.start, this.start), this.end = Math.max(a.end, this.end))
             }
             last() {
                 return this.parts[this.parts.length - 1]
             }
             length() {
                 return this.parts.length
             }
-            clone(a, c) {
-                let d = new ue,
-                    w = JSON.parse(JSON.stringify(this.parts)),
-                    v = w.pop();
-                for (let B of w) d.add(B);
-                let S = c.substr.substring(0, a - v.start),
-                    M = S.length;
+            clone(a, u) {
+                let d = new se,
+                    T = JSON.parse(JSON.stringify(this.parts)),
+                    m = T.pop();
+                for (let G of T) d.add(G);
+                let O = u.substr.substring(0, a - m.start),
+                    F = O.length;
                 return d.add({
-                    start: v.start,
-                    end: v.start + M,
-                    length: M,
-                    substr: S
+                    start: m.start,
+                    end: m.start + F,
+                    length: F,
+                    substr: O
                 }), d
             }
         }
-        let h = l => {
-                N(), l = R(l);
+        let p = l => {
+                N(), l = $(l);
                 let a = "",
-                    c = [new ue];
+                    u = [new se];
                 for (let d = 0; d < l.length; d++) {
-                    let v = l.substring(d).match(W),
-                        S = l.substring(d, d + 1),
-                        M = v ? v[0] : null,
-                        B = [],
+                    let m = l.substring(d).match(X),
+                        O = l.substring(d, d + 1),
+                        F = m ? m[0] : null,
+                        G = [],
                         C = new Set;
-                    for (let A of c) {
-                        let H = A.last();
-                        if (!H || H.length == 1 || H.end <= d)
-                            if (M) {
-                                let J = M.length;
-                                A.add({
+                    for (let L of u) {
+                        let k = L.last();
+                        if (!k || k.length == 1 || k.end <= d)
+                            if (F) {
+                                let J = F.length;
+                                L.add({
                                     start: d,
                                     end: d + J,
                                     length: J,
-                                    substr: M
+                                    substr: F
                                 }), C.add("1")
-                            } else A.add({
+                            } else L.add({
                                 start: d,
                                 end: d + 1,
                                 length: 1,
-                                substr: S
+                                substr: O
                             }), C.add("2");
-                        else if (M) {
-                            let J = A.clone(d, H),
-                                ce = M.length;
+                        else if (F) {
+                            let J = L.clone(d, k),
+                                ue = F.length;
                             J.add({
                                 start: d,
-                                end: d + ce,
-                                length: ce,
-                                substr: M
-                            }), B.push(J)
+                                end: d + ue,
+                                length: ue,
+                                substr: F
+                            }), G.push(J)
                         } else C.add("3")
                     }
-                    if (B.length > 0) {
-                        B = B.sort((A, H) => A.length() - H.length());
-                        for (let A of B) X(A, c) || c.push(A);
+                    if (G.length > 0) {
+                        G = G.sort((L, k) => L.length() - k.length());
+                        for (let L of G) z(L, u) || u.push(L);
                         continue
                     }
                     if (d > 0 && C.size == 1 && !C.has("3")) {
-                        a += Q(c, !1);
-                        let A = new ue,
-                            H = c[0];
-                        H && A.add(H.last()), c = [A]
+                        a += P(u, !1);
+                        let L = new se,
+                            k = u[0];
+                        k && L.add(k.last()), u = [L]
                     }
                 }
-                return a += Q(c, !0), a
+                return a += P(u, !0), a
             },
-            T = (l, a) => {
+            _ = (l, a) => {
                 if (l) return l[a]
             },
-            O = (l, a) => {
+            w = (l, a) => {
                 if (l) {
-                    for (var c, d = a.split(".");
-                        (c = d.shift()) && (l = l[c]););
+                    for (var u, d = a.split(".");
+                        (u = d.shift()) && (l = l[u]););
                     return l
                 }
             },
-            _ = (l, a, c) => {
-                var d, w;
-                return !l || (l = l + "", a.regex == null) || (w = l.search(a.regex), w === -1) ? 0 : (d = a.string.length / l.length, w === 0 && (d += .5), d * c)
-            },
-            P = (l, a) => {
-                var c = l[a];
-                if (typeof c == "function") return c;
-                c && !Array.isArray(c) && (l[a] = [c])
+            y = (l, a, u) => {
+                var d, T;
+                return !l || (l = l + "", a.regex == null) || (T = l.search(a.regex), T === -1) ? 0 : (d = a.string.length / l.length, T === 0 && (d += .5), d * u)
+            },
+            R = (l, a) => {
+                var u = l[a];
+                if (typeof u == "function") return u;
+                u && !Array.isArray(u) && (l[a] = [u])
             },
             I = (l, a) => {
                 if (Array.isArray(l)) l.forEach(a);
                 else
-                    for (var c in l) l.hasOwnProperty(c) && a(l[c], c)
+                    for (var u in l) l.hasOwnProperty(u) && a(l[u], u)
             },
-            K = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = R(l + "").toLowerCase(), a = R(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
-        class Y {
-            constructor(a, c) {
-                this.items = void 0, this.settings = void 0, this.items = a, this.settings = c || {
+            K = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = $(l + "").toLowerCase(), a = $(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
+        class B {
+            constructor(a, u) {
+                this.items = void 0, this.settings = void 0, this.items = a, this.settings = u || {
                     diacritics: !0
                 }
             }
-            tokenize(a, c, d) {
+            tokenize(a, u, d) {
                 if (!a || !a.length) return [];
-                let w = [],
-                    v = a.split(/\s+/);
-                var S;
-                return d && (S = new RegExp("^(" + Object.keys(d).map(s).join("|") + "):(.*)$")), v.forEach(M => {
-                    let B, C = null,
-                        A = null;
-                    S && (B = M.match(S)) && (C = B[1], M = B[2]), M.length > 0 && (this.settings.diacritics ? A = h(M) || null : A = s(M), A && c && (A = "\\b" + A)), w.push({
-                        string: M,
-                        regex: A ? new RegExp(A, "iu") : null,
+                let T = [],
+                    m = a.split(/\s+/);
+                var O;
+                return d && (O = new RegExp("^(" + Object.keys(d).map(s).join("|") + "):(.*)$")), m.forEach(F => {
+                    let G, C = null,
+                        L = null;
+                    O && (G = F.match(O)) && (C = G[1], F = G[2]), F.length > 0 && (this.settings.diacritics ? L = p(F) || null : L = s(F), L && u && (L = "\\b" + L)), T.push({
+                        string: F,
+                        regex: L ? new RegExp(L, "iu") : null,
                         field: C
                     })
-                }), w
+                }), T
             }
-            getScoreFunction(a, c) {
-                var d = this.prepareSearch(a, c);
+            getScoreFunction(a, u) {
+                var d = this.prepareSearch(a, u);
                 return this._getScoreFunction(d)
             }
             _getScoreFunction(a) {
-                let c = a.tokens,
-                    d = c.length;
+                let u = a.tokens,
+                    d = u.length;
                 if (!d) return function() {
                     return 0
                 };
-                let w = a.options.fields,
-                    v = a.weights,
-                    S = w.length,
-                    M = a.getAttrFn;
-                if (!S) return function() {
+                let T = a.options.fields,
+                    m = a.weights,
+                    O = T.length,
+                    F = a.getAttrFn;
+                if (!O) return function() {
                     return 1
                 };
-                let B = function() {
-                    return S === 1 ? function(C, A) {
-                        let H = w[0].field;
-                        return _(M(A, H), C, v[H] || 1)
-                    } : function(C, A) {
-                        var H = 0;
+                let G = function() {
+                    return O === 1 ? function(C, L) {
+                        let k = T[0].field;
+                        return y(F(L, k), C, m[k] || 1)
+                    } : function(C, L) {
+                        var k = 0;
                         if (C.field) {
-                            let J = M(A, C.field);
-                            !C.regex && J ? H += 1 / S : H += _(J, C, 1)
-                        } else I(v, (J, ce) => {
-                            H += _(M(A, ce), C, J)
+                            let J = F(L, C.field);
+                            !C.regex && J ? k += 1 / O : k += y(J, C, 1)
+                        } else I(m, (J, ue) => {
+                            k += y(F(L, ue), C, J)
                         });
-                        return H / S
+                        return k / O
                     }
                 }();
                 return d === 1 ? function(C) {
-                    return B(c[0], C)
+                    return G(u[0], C)
                 } : a.options.conjunction === "and" ? function(C) {
-                    var A, H = 0;
-                    for (let J of c) {
-                        if (A = B(J, C), A <= 0) return 0;
-                        H += A
+                    var L, k = 0;
+                    for (let J of u) {
+                        if (L = G(J, C), L <= 0) return 0;
+                        k += L
                     }
-                    return H / d
+                    return k / d
                 } : function(C) {
-                    var A = 0;
-                    return I(c, H => {
-                        A += B(H, C)
-                    }), A / d
+                    var L = 0;
+                    return I(u, k => {
+                        L += G(k, C)
+                    }), L / d
                 }
             }
-            getSortFunction(a, c) {
-                var d = this.prepareSearch(a, c);
+            getSortFunction(a, u) {
+                var d = this.prepareSearch(a, u);
                 return this._getSortFunction(d)
             }
             _getSortFunction(a) {
-                var c, d = [];
-                let w = this,
-                    v = a.options,
-                    S = !a.query && v.sort_empty ? v.sort_empty : v.sort;
-                if (typeof S == "function") return S.bind(this);
-                let M = function(A, H) {
-                    return A === "$score" ? H.score : a.getAttrFn(w.items[H.id], A)
+                var u, d = [];
+                let T = this,
+                    m = a.options,
+                    O = !a.query && m.sort_empty ? m.sort_empty : m.sort;
+                if (typeof O == "function") return O.bind(this);
+                let F = function(L, k) {
+                    return L === "$score" ? k.score : a.getAttrFn(T.items[k.id], L)
                 };
-                if (S)
-                    for (let C of S)(a.query || C.field !== "$score") && d.push(C);
+                if (O)
+                    for (let C of O)(a.query || C.field !== "$score") && d.push(C);
                 if (a.query) {
-                    c = !0;
+                    u = !0;
                     for (let C of d)
                         if (C.field === "$score") {
-                            c = !1;
+                            u = !1;
                             break
-                        } c && d.unshift({
+                        } u && d.unshift({
                         field: "$score",
                         direction: "desc"
                     })
                 } else d = d.filter(C => C.field !== "$score");
-                return d.length ? function(C, A) {
-                    var H, J;
-                    for (let ce of d)
-                        if (J = ce.field, H = (ce.direction === "desc" ? -1 : 1) * K(M(J, C), M(J, A)), H) return H;
+                return d.length ? function(C, L) {
+                    var k, J;
+                    for (let ue of d)
+                        if (J = ue.field, k = (ue.direction === "desc" ? -1 : 1) * K(F(J, C), F(J, L)), k) return k;
                     return 0
                 } : null
             }
-            prepareSearch(a, c) {
+            prepareSearch(a, u) {
                 let d = {};
-                var w = Object.assign({}, c);
-                if (P(w, "sort"), P(w, "sort_empty"), w.fields) {
-                    P(w, "fields");
-                    let v = [];
-                    w.fields.forEach(S => {
-                        typeof S == "string" && (S = {
-                            field: S,
+                var T = Object.assign({}, u);
+                if (R(T, "sort"), R(T, "sort_empty"), T.fields) {
+                    R(T, "fields");
+                    let m = [];
+                    T.fields.forEach(O => {
+                        typeof O == "string" && (O = {
+                            field: O,
                             weight: 1
-                        }), v.push(S), d[S.field] = "weight" in S ? S.weight : 1
-                    }), w.fields = v
+                        }), m.push(O), d[O.field] = "weight" in O ? O.weight : 1
+                    }), T.fields = m
                 }
                 return {
-                    options: w,
+                    options: T,
                     query: a.toLowerCase().trim(),
-                    tokens: this.tokenize(a, w.respect_word_boundaries, d),
+                    tokens: this.tokenize(a, T.respect_word_boundaries, d),
                     total: 0,
                     items: [],
                     weights: d,
-                    getAttrFn: w.nesting ? O : T
+                    getAttrFn: T.nesting ? w : _
                 }
             }
-            search(a, c) {
+            search(a, u) {
                 var d = this,
-                    w, v;
-                v = this.prepareSearch(a, c), c = v.options, a = v.query;
-                let S = c.score || d._getScoreFunction(v);
-                a.length ? I(d.items, (B, C) => {
-                    w = S(B), (c.filter === !1 || w > 0) && v.items.push({
-                        score: w,
+                    T, m;
+                m = this.prepareSearch(a, u), u = m.options, a = m.query;
+                let O = u.score || d._getScoreFunction(m);
+                a.length ? I(d.items, (G, C) => {
+                    T = O(G), (u.filter === !1 || T > 0) && m.items.push({
+                        score: T,
                         id: C
                     })
-                }) : I(d.items, (B, C) => {
-                    v.items.push({
+                }) : I(d.items, (G, C) => {
+                    m.items.push({
                         score: 1,
                         id: C
                     })
                 });
-                let M = d._getSortFunction(v);
-                return M && v.items.sort(M), v.total = v.items.length, typeof c.limit == "number" && (v.items = v.items.slice(0, c.limit)), v
+                let F = d._getSortFunction(m);
+                return F && m.items.sort(F), m.total = m.items.length, typeof u.limit == "number" && (m.items = m.items.slice(0, u.limit)), m
             }
         }
-        i.Sifter = Y, i.cmp = K, i.getAttr = T, i.getAttrNesting = O, i.getPattern = h, i.iterate = I, i.propToArray = P, i.scoreValue = _, Object.defineProperty(i, "__esModule", {
+        r.Sifter = B, r.cmp = K, r.getAttr = _, r.getAttrNesting = w, r.getPattern = p, r.iterate = I, r.propToArray = R, r.scoreValue = y, Object.defineProperty(r, "__esModule", {
             value: !0
         })
     })
 });
-var Le = Pe((_e, Ke) => {
-    (function(i, u) {
-        typeof _e == "object" && typeof Ke < "u" ? u(_e) : typeof define == "function" && define.amd ? define(["exports"], u) : (i = typeof globalThis < "u" ? globalThis : i || self, u(i.diacritics = {}))
-    })(_e, function(i) {
+var Ie = Re((_e, je) => {
+    (function(r, c) {
+        typeof _e == "object" && typeof je < "u" ? c(_e) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.diacritics = {}))
+    })(_e, function(r) {
         "use strict";
-        let u = h => (h = h.filter(Boolean), h.length < 2 ? h[0] || "" : o(h) == 1 ? "[" + h.join("") + "]" : "(?:" + h.join("|") + ")"),
-            e = h => {
-                if (!n(h)) return h.join("");
-                let T = "",
-                    O = 0,
-                    _ = () => {
-                        O > 1 && (T += "{" + O + "}")
+        let c = p => (p = p.filter(Boolean), p.length < 2 ? p[0] || "" : o(p) == 1 ? "[" + p.join("") + "]" : "(?:" + p.join("|") + ")"),
+            e = p => {
+                if (!n(p)) return p.join("");
+                let _ = "",
+                    w = 0,
+                    y = () => {
+                        w > 1 && (_ += "{" + w + "}")
                     };
-                return h.forEach((P, I) => {
-                    if (P === h[I - 1]) {
-                        O++;
+                return p.forEach((R, I) => {
+                    if (R === p[I - 1]) {
+                        w++;
                         return
                     }
-                    _(), T += P, O = 1
-                }), _(), T
+                    y(), _ += R, w = 1
+                }), y(), _
             },
-            t = h => {
-                let T = p(h);
-                return u(T)
-            },
-            n = h => new Set(h).size !== h.length,
-            s = h => (h + "").replace(/([\$\(\)\*\+\.\?\[\]\^\{\|\}\\])/gu, "\\$1"),
-            o = h => h.reduce((T, O) => Math.max(T, r(O)), 0),
-            r = h => p(h).length,
-            p = h => Array.from(h),
-            m = h => {
-                if (h.length === 1) return [
-                    [h]
+            t = p => {
+                let _ = f(p);
+                return c(_)
+            },
+            n = p => new Set(p).size !== p.length,
+            s = p => (p + "").replace(/([\$\(\)\*\+\.\?\[\]\^\{\|\}\\])/gu, "\\$1"),
+            o = p => p.reduce((_, w) => Math.max(_, i(w)), 0),
+            i = p => f(p).length,
+            f = p => Array.from(p),
+            g = p => {
+                if (p.length === 1) return [
+                    [p]
                 ];
-                let T = [],
-                    O = h.substring(1);
-                return m(O).forEach(function(P) {
-                    let I = P.slice(0);
-                    I[0] = h.charAt(0) + I[0], T.push(I), I = P.slice(0), I.unshift(h.charAt(0)), T.push(I)
-                }), T
+                let _ = [],
+                    w = p.substring(1);
+                return g(w).forEach(function(R) {
+                    let I = R.slice(0);
+                    I[0] = p.charAt(0) + I[0], _.push(I), I = R.slice(0), I.unshift(p.charAt(0)), _.push(I)
+                }), _
             },
-            g = [
+            v = [
                 [0, 65535]
             ],
             E = "[\u0300-\u036F\xB7\u02BE\u02BC]";
-        i.unicode_map = void 0;
-        let y, W = 3,
+        r.unicode_map = void 0;
+        let M, X = 3,
             U = {},
-            f = {
+            h = {
                 "/": "\u2044\u2215",
                 0: "\u07C0",
                 a: "\u2C65\u0250\u0251",
                 aa: "\uA733",
                 ae: "\xE6\u01FD\u01E3",
                 ao: "\uA735",
                 au: "\uA737",
@@ -522,373 +522,373 @@
                 v: "\u028B\uA75F\u028C",
                 vy: "\uA761",
                 w: "\u2C73",
                 y: "\u01B4\u024F\u1EFF",
                 z: "\u01B6\u0225\u0240\u2C6C\uA763",
                 hv: "\u0195"
             };
-        for (let h in f) {
-            let T = f[h] || "";
-            for (let O = 0; O < T.length; O++) {
-                let _ = T.substring(O, O + 1);
-                U[_] = h
+        for (let p in h) {
+            let _ = h[p] || "";
+            for (let w = 0; w < _.length; w++) {
+                let y = _.substring(w, w + 1);
+                U[y] = p
             }
         }
-        let z = new RegExp(Object.keys(U).join("|") + "|" + E, "gu"),
-            k = h => {
-                i.unicode_map === void 0 && (i.unicode_map = F(h || g))
-            },
-            N = (h, T = "NFKD") => h.normalize(T),
-            b = h => p(h).reduce((T, O) => T + R(O), ""),
-            R = h => (h = N(h).toLowerCase().replace(z, T => U[T] || ""), N(h, "NFC"));
+        let Y = new RegExp(Object.keys(U).join("|") + "|" + E, "gu"),
+            H = p => {
+                r.unicode_map === void 0 && (r.unicode_map = V(p || v))
+            },
+            N = (p, _ = "NFKD") => p.normalize(_),
+            b = p => f(p).reduce((_, w) => _ + $(w), ""),
+            $ = p => (p = N(p).toLowerCase().replace(Y, _ => U[_] || ""), N(p, "NFC"));
 
-        function* Z(h) {
-            for (let [T, O] of h)
-                for (let _ = T; _ <= O; _++) {
-                    let P = String.fromCharCode(_),
-                        I = b(P);
-                    I != P.toLowerCase() && (I.length > W || I.length != 0 && (yield {
+        function* W(p) {
+            for (let [_, w] of p)
+                for (let y = _; y <= w; y++) {
+                    let R = String.fromCharCode(y),
+                        I = b(R);
+                    I != R.toLowerCase() && (I.length > X || I.length != 0 && (yield {
                         folded: I,
-                        composed: P,
-                        code_point: _
+                        composed: R,
+                        code_point: y
                     }))
                 }
         }
-        let $ = h => {
-                let T = {},
-                    O = (_, P) => {
-                        let I = T[_] || new Set,
+        let oe = p => {
+                let _ = {},
+                    w = (y, R) => {
+                        let I = _[y] || new Set,
                             K = new RegExp("^" + t(I) + "$", "iu");
-                        P.match(K) || (I.add(s(P)), T[_] = I)
+                        R.match(K) || (I.add(s(R)), _[y] = I)
                     };
-                for (let _ of Z(h)) O(_.folded, _.folded), O(_.folded, _.composed);
-                return T
+                for (let y of W(p)) w(y.folded, y.folded), w(y.folded, y.composed);
+                return _
             },
-            F = h => {
-                let T = $(h),
-                    O = {},
-                    _ = [];
-                for (let I in T) {
-                    let K = T[I];
-                    K && (O[I] = t(K)), I.length > 1 && _.push(s(I))
-                }
-                _.sort((I, K) => K.length - I.length);
-                let P = u(_);
-                return y = new RegExp("^" + P, "u"), O
-            },
-            x = (h, T = 1) => {
-                let O = 0;
-                return h = h.map(_ => (i.unicode_map[_] && (O += _.length), i.unicode_map[_] || _)), O >= T ? e(h) : ""
-            },
-            q = (h, T = 1) => (T = Math.max(T, h.length - 1), u(m(h).map(O => x(O, T)))),
-            V = (h, T = !0) => {
-                let O = h.length > 1 ? 1 : 0;
-                return u(h.map(_ => {
-                    let P = [],
-                        I = T ? _.length() : _.length() - 1;
-                    for (let K = 0; K < I; K++) P.push(q(_.substrs[K] || "", O));
-                    return e(P)
+            V = p => {
+                let _ = oe(p),
+                    w = {},
+                    y = [];
+                for (let I in _) {
+                    let K = _[I];
+                    K && (w[I] = t(K)), I.length > 1 && y.push(s(I))
+                }
+                y.sort((I, K) => K.length - I.length);
+                let R = c(y);
+                return M = new RegExp("^" + R, "u"), w
+            },
+            A = (p, _ = 1) => {
+                let w = 0;
+                return p = p.map(y => (r.unicode_map[y] && (w += y.length), r.unicode_map[y] || y)), w >= _ ? e(p) : ""
+            },
+            S = (p, _ = 1) => (_ = Math.max(_, p.length - 1), c(g(p).map(w => A(w, _)))),
+            q = (p, _ = !0) => {
+                let w = p.length > 1 ? 1 : 0;
+                return c(p.map(y => {
+                    let R = [],
+                        I = _ ? y.length() : y.length() - 1;
+                    for (let K = 0; K < I; K++) R.push(S(y.substrs[K] || "", w));
+                    return e(R)
                 }))
             },
-            Q = (h, T) => {
-                for (let O of T) {
-                    if (O.start != h.start || O.end != h.end || O.substrs.join("") !== h.substrs.join("")) continue;
-                    let _ = h.parts,
-                        P = K => {
-                            for (let Y of _) {
-                                if (Y.start === K.start && Y.substr === K.substr) return !1;
-                                if (!(K.length == 1 || Y.length == 1) && (K.start < Y.start && K.end > Y.start || Y.start < K.start && Y.end > K.start)) return !0
+            P = (p, _) => {
+                for (let w of _) {
+                    if (w.start != p.start || w.end != p.end || w.substrs.join("") !== p.substrs.join("")) continue;
+                    let y = p.parts,
+                        R = K => {
+                            for (let B of y) {
+                                if (B.start === K.start && B.substr === K.substr) return !1;
+                                if (!(K.length == 1 || B.length == 1) && (K.start < B.start && K.end > B.start || B.start < K.start && B.end > K.start)) return !0
                             }
                             return !1
                         };
-                    if (!(O.parts.filter(P).length > 0)) return !0
+                    if (!(w.parts.filter(R).length > 0)) return !0
                 }
                 return !1
             };
-        class X {
+        class z {
             constructor() {
                 this.parts = [], this.substrs = [], this.start = 0, this.end = 0
             }
-            add(T) {
-                T && (this.parts.push(T), this.substrs.push(T.substr), this.start = Math.min(T.start, this.start), this.end = Math.max(T.end, this.end))
+            add(_) {
+                _ && (this.parts.push(_), this.substrs.push(_.substr), this.start = Math.min(_.start, this.start), this.end = Math.max(_.end, this.end))
             }
             last() {
                 return this.parts[this.parts.length - 1]
             }
             length() {
                 return this.parts.length
             }
-            clone(T, O) {
-                let _ = new X,
-                    P = JSON.parse(JSON.stringify(this.parts)),
-                    I = P.pop();
-                for (let l of P) _.add(l);
-                let K = O.substr.substring(0, T - I.start),
-                    Y = K.length;
-                return _.add({
+            clone(_, w) {
+                let y = new z,
+                    R = JSON.parse(JSON.stringify(this.parts)),
+                    I = R.pop();
+                for (let l of R) y.add(l);
+                let K = w.substr.substring(0, _ - I.start),
+                    B = K.length;
+                return y.add({
                     start: I.start,
-                    end: I.start + Y,
-                    length: Y,
+                    end: I.start + B,
+                    length: B,
                     substr: K
-                }), _
+                }), y
             }
         }
-        let ue = h => {
-            k(), h = b(h);
-            let T = "",
-                O = [new X];
-            for (let _ = 0; _ < h.length; _++) {
-                let I = h.substring(_).match(y),
-                    K = h.substring(_, _ + 1),
-                    Y = I ? I[0] : null,
+        let se = p => {
+            H(), p = b(p);
+            let _ = "",
+                w = [new z];
+            for (let y = 0; y < p.length; y++) {
+                let I = p.substring(y).match(M),
+                    K = p.substring(y, y + 1),
+                    B = I ? I[0] : null,
                     l = [],
                     a = new Set;
-                for (let c of O) {
-                    let d = c.last();
-                    if (!d || d.length == 1 || d.end <= _)
-                        if (Y) {
-                            let w = Y.length;
-                            c.add({
-                                start: _,
-                                end: _ + w,
-                                length: w,
-                                substr: Y
+                for (let u of w) {
+                    let d = u.last();
+                    if (!d || d.length == 1 || d.end <= y)
+                        if (B) {
+                            let T = B.length;
+                            u.add({
+                                start: y,
+                                end: y + T,
+                                length: T,
+                                substr: B
                             }), a.add("1")
-                        } else c.add({
-                            start: _,
-                            end: _ + 1,
+                        } else u.add({
+                            start: y,
+                            end: y + 1,
                             length: 1,
                             substr: K
                         }), a.add("2");
-                    else if (Y) {
-                        let w = c.clone(_, d),
-                            v = Y.length;
-                        w.add({
-                            start: _,
-                            end: _ + v,
-                            length: v,
-                            substr: Y
-                        }), l.push(w)
+                    else if (B) {
+                        let T = u.clone(y, d),
+                            m = B.length;
+                        T.add({
+                            start: y,
+                            end: y + m,
+                            length: m,
+                            substr: B
+                        }), l.push(T)
                     } else a.add("3")
                 }
                 if (l.length > 0) {
-                    l = l.sort((c, d) => c.length() - d.length());
-                    for (let c of l) Q(c, O) || O.push(c);
+                    l = l.sort((u, d) => u.length() - d.length());
+                    for (let u of l) P(u, w) || w.push(u);
                     continue
                 }
-                if (_ > 0 && a.size == 1 && !a.has("3")) {
-                    T += V(O, !1);
-                    let c = new X,
-                        d = O[0];
-                    d && c.add(d.last()), O = [c]
+                if (y > 0 && a.size == 1 && !a.has("3")) {
+                    _ += q(w, !1);
+                    let u = new z,
+                        d = w[0];
+                    d && u.add(d.last()), w = [u]
                 }
             }
-            return T += V(O, !0), T
+            return _ += q(w, !0), _
         };
-        i._asciifold = R, i.asciifold = b, i.code_points = g, i.escape_regex = s, i.generateMap = F, i.generateSets = $, i.generator = Z, i.getPattern = ue, i.initialize = k, i.mapSequence = x, i.normalize = N, i.substringsToPattern = q, Object.defineProperty(i, "__esModule", {
+        r._asciifold = $, r.asciifold = b, r.code_points = v, r.escape_regex = s, r.generateMap = V, r.generateSets = oe, r.generator = W, r.getPattern = se, r.initialize = H, r.mapSequence = A, r.normalize = N, r.substringsToPattern = S, Object.defineProperty(r, "__esModule", {
             value: !0
         })
     })
 });
 
-function Ee(i, u) {
-    i.split(/\s+/).forEach(e => {
-        u(e)
+function Ee(r, c) {
+    r.split(/\s+/).forEach(e => {
+        c(e)
     })
 }
 var fe = class {
     constructor() {
-        L(this, "_events");
+        x(this, "_events");
         this._events = {}
     }
-    on(u, e) {
-        Ee(u, t => {
+    on(c, e) {
+        Ee(c, t => {
             let n = this._events[t] || [];
             n.push(e), this._events[t] = n
         })
     }
-    off(u, e) {
+    off(c, e) {
         var t = arguments.length;
         if (t === 0) {
             this._events = {};
             return
         }
-        Ee(u, n => {
+        Ee(c, n => {
             if (t === 1) {
                 delete this._events[n];
                 return
             }
             let s = this._events[n];
             s !== void 0 && (s.splice(s.indexOf(e), 1), this._events[n] = s)
         })
     }
-    trigger(u, ...e) {
+    trigger(c, ...e) {
         var t = this;
-        Ee(u, n => {
+        Ee(c, n => {
             let s = t._events[n];
             s !== void 0 && s.forEach(o => {
                 o.apply(t, e)
             })
         })
     }
 };
 
-function xe(i) {
-    return i.plugins = {}, class extends i {
+function xe(r) {
+    return r.plugins = {}, class extends r {
         constructor() {
             super(...arguments);
-            L(this, "plugins", {
+            x(this, "plugins", {
                 names: [],
                 settings: {},
                 requested: {},
                 loaded: {}
             })
         }
         static define(e, t) {
-            i.plugins[e] = {
+            r.plugins[e] = {
                 name: e,
                 fn: t
             }
         }
         initializePlugins(e) {
             var t, n;
             let s = this,
                 o = [];
-            if (Array.isArray(e)) e.forEach(r => {
-                typeof r == "string" ? o.push(r) : (s.plugins.settings[r.name] = r.options, o.push(r.name))
+            if (Array.isArray(e)) e.forEach(i => {
+                typeof i == "string" ? o.push(i) : (s.plugins.settings[i.name] = i.options, o.push(i.name))
             });
             else if (e)
                 for (t in e) e.hasOwnProperty(t) && (s.plugins.settings[t] = e[t], o.push(t));
             for (; n = o.shift();) s.require(n)
         }
         loadPlugin(e) {
             var t = this,
                 n = t.plugins,
-                s = i.plugins[e];
-            if (!i.plugins.hasOwnProperty(e)) throw new Error('Unable to find "' + e + '" plugin');
+                s = r.plugins[e];
+            if (!r.plugins.hasOwnProperty(e)) throw new Error('Unable to find "' + e + '" plugin');
             n.requested[e] = !0, n.loaded[e] = s.fn.apply(t, [t.plugins.settings[e] || {}]), n.names.push(e)
         }
         require(e) {
             var t = this,
                 n = t.plugins;
             if (!t.plugins.loaded.hasOwnProperty(e)) {
                 if (n.requested[e]) throw new Error('Plugin has circular dependency ("' + e + '")');
                 t.loadPlugin(e)
             }
             return n.loaded[e]
         }
     }
 }
-var ne = be(Ve()),
-    We = be(Le());
-var rt = be(Le());
-var oe = (i, u) => {
-    if (Array.isArray(i)) i.forEach(u);
+var te = be(Ke()),
+    Ze = be(Ie());
+var rt = be(Ie());
+var le = (r, c) => {
+    if (Array.isArray(r)) r.forEach(c);
     else
-        for (var e in i) i.hasOwnProperty(e) && u(i[e], e)
+        for (var e in r) r.hasOwnProperty(e) && c(r[e], e)
 };
-var ee = i => {
-        if (i.jquery) return i[0];
-        if (i instanceof HTMLElement) return i;
-        if (Ie(i)) {
-            var u = document.createElement("template");
-            return u.innerHTML = i.trim(), u.content.firstChild
+var Z = r => {
+        if (r.jquery) return r[0];
+        if (r instanceof HTMLElement) return r;
+        if (Le(r)) {
+            var c = document.createElement("template");
+            return c.innerHTML = r.trim(), c.content.firstChild
         }
-        return document.querySelector(i)
+        return document.querySelector(r)
     },
-    Ie = i => typeof i == "string" && i.indexOf("<") > -1,
-    je = i => i.replace(/['"\\]/g, "\\$&"),
-    we = (i, u) => {
+    Le = r => typeof r == "string" && r.indexOf("<") > -1,
+    De = r => r.replace(/['"\\]/g, "\\$&"),
+    Te = (r, c) => {
         var e = document.createEvent("HTMLEvents");
-        e.initEvent(u, !0, !1), i.dispatchEvent(e)
+        e.initEvent(c, !0, !1), r.dispatchEvent(e)
     },
-    he = (i, u) => {
-        Object.assign(i.style, u)
+    he = (r, c) => {
+        Object.assign(r.style, c)
     },
-    te = (i, ...u) => {
-        var e = De(u);
-        i = Ne(i), i.map(t => {
+    ee = (r, ...c) => {
+        var e = Ne(c);
+        r = qe(r), r.map(t => {
             e.map(n => {
                 t.classList.add(n)
             })
         })
     },
-    ie = (i, ...u) => {
-        var e = De(u);
-        i = Ne(i), i.map(t => {
+    re = (r, ...c) => {
+        var e = Ne(c);
+        r = qe(r), r.map(t => {
             e.map(n => {
                 t.classList.remove(n)
             })
         })
     },
-    De = i => {
-        var u = [];
-        return oe(i, e => {
-            typeof e == "string" && (e = e.trim().split(/[\11\12\14\15\40]/)), Array.isArray(e) && (u = u.concat(e))
-        }), u.filter(Boolean)
+    Ne = r => {
+        var c = [];
+        return le(r, e => {
+            typeof e == "string" && (e = e.trim().split(/[\11\12\14\15\40]/)), Array.isArray(e) && (c = c.concat(e))
+        }), c.filter(Boolean)
     },
-    Ne = i => (Array.isArray(i) || (i = [i]), i),
-    Te = (i, u, e) => {
-        if (!(e && !e.contains(i)))
-            for (; i && i.matches;) {
-                if (i.matches(u)) return i;
-                i = i.parentNode
+    qe = r => (Array.isArray(r) || (r = [r]), r),
+    we = (r, c, e) => {
+        if (!(e && !e.contains(r)))
+            for (; r && r.matches;) {
+                if (r.matches(c)) return r;
+                r = r.parentNode
             }
     },
-    Ae = (i, u = 0) => u > 0 ? i[i.length - 1] : i[0],
-    qe = i => Object.keys(i).length === 0,
-    Ce = (i, u) => {
-        if (!i) return -1;
-        u = u || i.nodeName;
-        for (var e = 0; i = i.previousElementSibling;) i.matches(u) && e++;
+    Ae = (r, c = 0) => c > 0 ? r[r.length - 1] : r[0],
+    ze = r => Object.keys(r).length === 0,
+    Ce = (r, c) => {
+        if (!r) return -1;
+        c = c || r.nodeName;
+        for (var e = 0; r = r.previousElementSibling;) r.matches(c) && e++;
         return e
     },
-    D = (i, u) => {
-        oe(u, (e, t) => {
-            e == null ? i.removeAttribute(t) : i.setAttribute(t, "" + e)
+    D = (r, c) => {
+        le(c, (e, t) => {
+            e == null ? r.removeAttribute(t) : r.setAttribute(t, "" + e)
         })
     },
-    ge = (i, u) => {
-        i.parentNode && i.parentNode.replaceChild(u, i)
+    ge = (r, c) => {
+        r.parentNode && r.parentNode.replaceChild(c, r)
     };
-var ze = (i, u) => {
-        if (u === null) return;
-        if (typeof u == "string") {
-            if (!u.length) return;
-            u = new RegExp(u, "i")
+var Ye = (r, c) => {
+        if (c === null) return;
+        if (typeof c == "string") {
+            if (!c.length) return;
+            c = new RegExp(c, "i")
         }
         let e = s => {
-                var o = s.data.match(u);
+                var o = s.data.match(c);
                 if (o && s.data.length > 0) {
-                    var r = document.createElement("span");
-                    r.className = "highlight";
-                    var p = s.splitText(o.index);
-                    p.splitText(o[0].length);
-                    var m = p.cloneNode(!0);
-                    return r.appendChild(m), ge(p, r), 1
+                    var i = document.createElement("span");
+                    i.className = "highlight";
+                    var f = s.splitText(o.index);
+                    f.splitText(o[0].length);
+                    var g = f.cloneNode(!0);
+                    return i.appendChild(g), ge(f, i), 1
                 }
                 return 0
             },
             t = s => {
                 s.nodeType === 1 && s.childNodes && !/(script|style)/i.test(s.tagName) && (s.className !== "highlight" || s.tagName !== "SPAN") && Array.from(s.childNodes).forEach(o => {
                     n(o)
                 })
             },
             n = s => s.nodeType === 3 ? e(s) : (t(s), 0);
-        n(i)
+        n(r)
     },
-    Ye = i => {
-        var u = i.querySelectorAll("span.highlight");
-        Array.prototype.forEach.call(u, function(e) {
+    Be = r => {
+        var c = r.querySelectorAll("span.highlight");
+        Array.prototype.forEach.call(c, function(e) {
             var t = e.parentNode;
             t.replaceChild(e.firstChild, e), t.normalize()
         })
     };
-var it = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
-    me = it ? "metaKey" : "ctrlKey";
+var ot = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
+    me = ot ? "metaKey" : "ctrlKey";
 var Me = {
     options: [],
     optgroups: [],
     plugins: [],
     delimiter: ",",
     splitOn: null,
     persist: !0,
@@ -903,14 +903,15 @@
     maxItems: null,
     hideSelected: null,
     duplicates: !1,
     addPrecedence: !1,
     selectOnTab: !1,
     preload: null,
     allowEmptyOption: !1,
+    refreshThrottle: 300,
     loadThrottle: 300,
     loadingClass: "loading",
     dataAttr: null,
     optgroupField: "optgroup",
     valueField: "value",
     labelField: "text",
     disabledField: "disabled",
@@ -928,310 +929,314 @@
     itemClass: "item",
     optionClass: "option",
     dropdownParent: null,
     controlInput: '<input type="text" autocomplete="off" size="1" />',
     copyClassesToDropdown: !1,
     placeholder: null,
     hidePlaceholder: null,
-    shouldLoad: function(i) {
-        return i.length > 0
+    shouldLoad: function(r) {
+        return r.length > 0
     },
     render: {}
 };
-var se = i => typeof i > "u" || i === null ? null : ve(i),
-    ve = i => typeof i == "boolean" ? i ? "1" : "0" : i + "",
-    de = i => (i + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
-    Be = (i, u) => {
+var ne = r => typeof r > "u" || r === null ? null : ve(r),
+    ve = r => typeof r == "boolean" ? r ? "1" : "0" : r + "",
+    de = r => (r + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
+    Ge = (r, c) => c > 0 ? setTimeout(r, c) : (r.call(null), null),
+    Qe = (r, c) => {
         var e;
         return function(t, n) {
             var s = this;
             e && (s.loading = Math.max(s.loading - 1, 0), clearTimeout(e)), e = setTimeout(function() {
-                e = null, s.loadedSearches[t] = !0, i.call(s, t, n)
-            }, u)
+                e = null, s.loadedSearches[t] = !0, r.call(s, t, n)
+            }, c)
         }
     },
-    Fe = (i, u, e) => {
-        var t, n = i.trigger,
+    Fe = (r, c, e) => {
+        var t, n = r.trigger,
             s = {};
-        i.trigger = function() {
+        r.trigger = function() {
             var o = arguments[0];
-            if (u.indexOf(o) !== -1) s[o] = arguments;
-            else return n.apply(i, arguments)
-        }, e.apply(i, []), i.trigger = n;
-        for (t of u) t in s && n.apply(i, s[t])
+            if (c.indexOf(o) !== -1) s[o] = arguments;
+            else return n.apply(r, arguments)
+        }, e.apply(r, []), r.trigger = n;
+        for (t of c) t in s && n.apply(r, s[t])
     },
-    Ge = i => ({
-        start: i.selectionStart || 0,
-        length: (i.selectionEnd || 0) - (i.selectionStart || 0)
+    Ue = r => ({
+        start: r.selectionStart || 0,
+        length: (r.selectionEnd || 0) - (r.selectionStart || 0)
     }),
-    j = (i, u = !1) => {
-        i && (i.preventDefault(), u && i.stopPropagation())
+    j = (r, c = !1) => {
+        r && (r.preventDefault(), c && r.stopPropagation())
     },
-    G = (i, u, e, t) => {
-        i.addEventListener(u, e, t)
+    Q = (r, c, e, t) => {
+        r.addEventListener(c, e, t)
     },
-    le = (i, u) => {
-        if (!u || !u[i]) return !1;
-        var e = (u.altKey ? 1 : 0) + (u.ctrlKey ? 1 : 0) + (u.shiftKey ? 1 : 0) + (u.metaKey ? 1 : 0);
+    ae = (r, c) => {
+        if (!c || !c[r]) return !1;
+        var e = (c.altKey ? 1 : 0) + (c.ctrlKey ? 1 : 0) + (c.shiftKey ? 1 : 0) + (c.metaKey ? 1 : 0);
         return e === 1
     },
-    Oe = (i, u) => {
-        let e = i.getAttribute("id");
-        return e || (i.setAttribute("id", u), u)
+    Se = (r, c) => {
+        let e = r.getAttribute("id");
+        return e || (r.setAttribute("id", c), c)
     },
-    He = i => i.replace(/[\\"']/g, "\\$&"),
-    ae = (i, u) => {
-        u && i.append(u)
+    ke = r => r.replace(/[\\"']/g, "\\$&"),
+    ce = (r, c) => {
+        c && r.append(c)
     };
 
-function Se(i, u) {
-    var e = Object.assign({}, Me, u),
+function Oe(r, c) {
+    var e = Object.assign({}, Me, c),
         t = e.dataAttr,
         n = e.labelField,
         s = e.valueField,
         o = e.disabledField,
-        r = e.optgroupField,
-        p = e.optgroupLabelField,
-        m = e.optgroupValueField,
-        g = i.tagName.toLowerCase(),
-        E = i.getAttribute("placeholder") || i.getAttribute("data-placeholder");
+        i = e.optgroupField,
+        f = e.optgroupLabelField,
+        g = e.optgroupValueField,
+        v = r.tagName.toLowerCase(),
+        E = r.getAttribute("placeholder") || r.getAttribute("data-placeholder");
     if (!E && !e.allowEmptyOption) {
-        let f = i.querySelector('option[value=""]');
-        f && (E = f.textContent)
+        let h = r.querySelector('option[value=""]');
+        h && (E = h.textContent)
     }
-    var y = {
+    var M = {
             placeholder: E,
             options: [],
             optgroups: [],
             items: [],
             maxItems: null
         },
-        W = () => {
-            var f, z = y.options,
-                k = {},
-                N = 1,
-                b = $ => {
-                    var F = Object.assign({}, $.dataset),
-                        x = t && F[t];
-                    return typeof x == "string" && x.length && (F = Object.assign(F, JSON.parse(x))), F
+        X = () => {
+            var h, Y = M.options,
+                H = {},
+                N = 1;
+            let b = 0;
+            var $ = V => {
+                    var A = Object.assign({}, V.dataset),
+                        S = t && A[t];
+                    return typeof S == "string" && S.length && (A = Object.assign(A, JSON.parse(S))), A
                 },
-                R = ($, F) => {
-                    var x = se($.value);
-                    if (x != null && !(!x && !e.allowEmptyOption)) {
-                        if (k.hasOwnProperty(x)) {
-                            if (F) {
-                                var q = k[x][r];
-                                q ? Array.isArray(q) ? q.push(F) : k[x][r] = [q, F] : k[x][r] = F
+                W = (V, A) => {
+                    var S = ne(V.value);
+                    if (S != null && !(!S && !e.allowEmptyOption)) {
+                        if (H.hasOwnProperty(S)) {
+                            if (A) {
+                                var q = H[S][i];
+                                q ? Array.isArray(q) ? q.push(A) : H[S][i] = [q, A] : H[S][i] = A
                             }
                         } else {
-                            var V = b($);
-                            V[n] = V[n] || $.textContent, V[s] = V[s] || x, V[o] = V[o] || $.disabled, V[r] = V[r] || F, V.$option = $, k[x] = V, z.push(V)
+                            var P = $(V);
+                            P[n] = P[n] || V.textContent, P[s] = P[s] || S, P[o] = P[o] || V.disabled, P[i] = P[i] || A, P.$option = V, P.$order = P.$order || ++b, H[S] = P, Y.push(P)
                         }
-                        $.selected && y.items.push(x)
+                        V.selected && M.items.push(S)
                     }
                 },
-                Z = $ => {
-                    var F, x;
-                    x = b($), x[p] = x[p] || $.getAttribute("label") || "", x[m] = x[m] || N++, x[o] = x[o] || $.disabled, y.optgroups.push(x), F = x[m], oe($.children, q => {
-                        R(q, F)
+                oe = V => {
+                    var A, S;
+                    S = $(V), S[f] = S[f] || V.getAttribute("label") || "", S[g] = S[g] || N++, S[o] = S[o] || V.disabled, S.$order = S.$order || ++b, M.optgroups.push(S), A = S[g], le(V.children, q => {
+                        W(q, A)
                     })
                 };
-            y.maxItems = i.hasAttribute("multiple") ? null : 1, oe(i.children, $ => {
-                f = $.tagName.toLowerCase(), f === "optgroup" ? Z($) : f === "option" && R($)
+            M.maxItems = r.hasAttribute("multiple") ? null : 1, le(r.children, V => {
+                h = V.tagName.toLowerCase(), h === "optgroup" ? oe(V) : h === "option" && W(V)
             })
         },
         U = () => {
-            let f = i.getAttribute(t);
-            if (f) y.options = JSON.parse(f), oe(y.options, k => {
-                y.items.push(k[s])
+            let h = r.getAttribute(t);
+            if (h) M.options = JSON.parse(h), le(M.options, H => {
+                M.items.push(H[s])
             });
             else {
-                var z = i.value.trim() || "";
-                if (!e.allowEmptyOption && !z.length) return;
-                let k = z.split(e.delimiter);
-                oe(k, N => {
+                var Y = r.value.trim() || "";
+                if (!e.allowEmptyOption && !Y.length) return;
+                let H = Y.split(e.delimiter);
+                le(H, N => {
                     let b = {};
-                    b[n] = N, b[s] = N, y.options.push(b)
-                }), y.items = k
+                    b[n] = N, b[s] = N, M.options.push(b)
+                }), M.items = H
             }
         };
-    return g === "select" ? W() : U(), Object.assign({}, Me, y, u)
+    return v === "select" ? X() : U(), Object.assign({}, Me, M, c)
 }
-var Je = 0,
+var Xe = 0,
     pe = class extends xe(fe) {
         constructor(e, t) {
             super();
-            L(this, "control_input");
-            L(this, "wrapper");
-            L(this, "dropdown");
-            L(this, "control");
-            L(this, "dropdown_content");
-            L(this, "focus_node");
-            L(this, "order", 0);
-            L(this, "settings");
-            L(this, "input");
-            L(this, "tabIndex");
-            L(this, "is_select_tag");
-            L(this, "rtl");
-            L(this, "inputId");
-            L(this, "_destroy");
-            L(this, "sifter");
-            L(this, "isOpen", !1);
-            L(this, "isDisabled", !1);
-            L(this, "isRequired");
-            L(this, "isInvalid", !1);
-            L(this, "isValid", !0);
-            L(this, "isLocked", !1);
-            L(this, "isFocused", !1);
-            L(this, "isInputHidden", !1);
-            L(this, "isSetup", !1);
-            L(this, "ignoreFocus", !1);
-            L(this, "ignoreHover", !1);
-            L(this, "hasOptions", !1);
-            L(this, "currentResults");
-            L(this, "lastValue", "");
-            L(this, "caretPos", 0);
-            L(this, "loading", 0);
-            L(this, "loadedSearches", {});
-            L(this, "activeOption", null);
-            L(this, "activeItems", []);
-            L(this, "optgroups", {});
-            L(this, "options", {});
-            L(this, "userOptions", {});
-            L(this, "items", []);
-            Je++;
-            var n, s = ee(e);
+            x(this, "control_input");
+            x(this, "wrapper");
+            x(this, "dropdown");
+            x(this, "control");
+            x(this, "dropdown_content");
+            x(this, "focus_node");
+            x(this, "order", 0);
+            x(this, "settings");
+            x(this, "input");
+            x(this, "tabIndex");
+            x(this, "is_select_tag");
+            x(this, "rtl");
+            x(this, "inputId");
+            x(this, "_destroy");
+            x(this, "sifter");
+            x(this, "isOpen", !1);
+            x(this, "isDisabled", !1);
+            x(this, "isReadOnly", !1);
+            x(this, "isRequired");
+            x(this, "isInvalid", !1);
+            x(this, "isValid", !0);
+            x(this, "isLocked", !1);
+            x(this, "isFocused", !1);
+            x(this, "isInputHidden", !1);
+            x(this, "isSetup", !1);
+            x(this, "ignoreFocus", !1);
+            x(this, "ignoreHover", !1);
+            x(this, "hasOptions", !1);
+            x(this, "currentResults");
+            x(this, "lastValue", "");
+            x(this, "caretPos", 0);
+            x(this, "loading", 0);
+            x(this, "loadedSearches", {});
+            x(this, "activeOption", null);
+            x(this, "activeItems", []);
+            x(this, "optgroups", {});
+            x(this, "options", {});
+            x(this, "userOptions", {});
+            x(this, "items", []);
+            x(this, "refreshTimeout", null);
+            Xe++;
+            var n, s = Z(e);
             if (s.tomselect) throw new Error("Tom Select already initialized on this element");
             s.tomselect = this;
             var o = window.getComputedStyle && window.getComputedStyle(s, null);
             n = o.getPropertyValue("direction");
-            let r = Se(s, t);
-            this.settings = r, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = Oe(s, "tomselect-" + Je), this.isRequired = s.required, this.sifter = new ne.Sifter(this.options, {
-                diacritics: r.diacritics
-            }), r.mode = r.mode || (r.maxItems === 1 ? "single" : "multi"), typeof r.hideSelected != "boolean" && (r.hideSelected = r.mode === "multi"), typeof r.hidePlaceholder != "boolean" && (r.hidePlaceholder = r.mode !== "multi");
-            var p = r.createFilter;
-            typeof p != "function" && (typeof p == "string" && (p = new RegExp(p)), p instanceof RegExp ? r.createFilter = k => p.test(k) : r.createFilter = k => this.settings.duplicates || !this.options[k]), this.initializePlugins(r.plugins), this.setupCallbacks(), this.setupTemplates();
-            let m = ee("<div>"),
-                g = ee("<div>"),
+            let i = Oe(s, t);
+            this.settings = i, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = Se(s, "tomselect-" + Xe), this.isRequired = s.required, this.sifter = new te.Sifter(this.options, {
+                diacritics: i.diacritics
+            }), i.mode = i.mode || (i.maxItems === 1 ? "single" : "multi"), typeof i.hideSelected != "boolean" && (i.hideSelected = i.mode === "multi"), typeof i.hidePlaceholder != "boolean" && (i.hidePlaceholder = i.mode !== "multi");
+            var f = i.createFilter;
+            typeof f != "function" && (typeof f == "string" && (f = new RegExp(f)), f instanceof RegExp ? i.createFilter = H => f.test(H) : i.createFilter = H => this.settings.duplicates || !this.options[H]), this.initializePlugins(i.plugins), this.setupCallbacks(), this.setupTemplates();
+            let g = Z("<div>"),
+                v = Z("<div>"),
                 E = this._render("dropdown"),
-                y = ee('<div role="listbox" tabindex="-1">'),
-                W = this.input.getAttribute("class") || "",
-                U = r.mode;
-            var f;
-            if (te(m, r.wrapperClass, W, U), te(g, r.controlClass), ae(m, g), te(E, r.dropdownClass, U), r.copyClassesToDropdown && te(E, W), te(y, r.dropdownContentClass), ae(E, y), ee(r.dropdownParent || m).appendChild(E), Ie(r.controlInput)) {
-                f = ee(r.controlInput);
-                var z = ["autocorrect", "autocapitalize", "autocomplete"];
-                (0, ne.iterate)(z, k => {
-                    s.getAttribute(k) && D(f, {
-                        [k]: s.getAttribute(k)
+                M = Z('<div role="listbox" tabindex="-1">'),
+                X = this.input.getAttribute("class") || "",
+                U = i.mode;
+            var h;
+            if (ee(g, i.wrapperClass, X, U), ee(v, i.controlClass), ce(g, v), ee(E, i.dropdownClass, U), i.copyClassesToDropdown && ee(E, X), ee(M, i.dropdownContentClass), ce(E, M), Z(i.dropdownParent || g).appendChild(E), Le(i.controlInput)) {
+                h = Z(i.controlInput);
+                var Y = ["autocorrect", "autocapitalize", "autocomplete", "spellcheck"];
+                (0, te.iterate)(Y, H => {
+                    s.getAttribute(H) && D(h, {
+                        [H]: s.getAttribute(H)
                     })
-                }), f.tabIndex = -1, g.appendChild(f), this.focus_node = f
-            } else r.controlInput ? (f = ee(r.controlInput), this.focus_node = f) : (f = ee("<input/>"), this.focus_node = g);
-            this.wrapper = m, this.dropdown = E, this.dropdown_content = y, this.control = g, this.control_input = f, this.setup()
+                }), h.tabIndex = -1, v.appendChild(h), this.focus_node = h
+            } else i.controlInput ? (h = Z(i.controlInput), this.focus_node = h) : (h = Z("<input/>"), this.focus_node = v);
+            this.wrapper = g, this.dropdown = E, this.dropdown_content = M, this.control = v, this.control_input = h, this.setup()
         }
         setup() {
             let e = this,
                 t = e.settings,
                 n = e.control_input,
                 s = e.dropdown,
                 o = e.dropdown_content,
-                r = e.wrapper,
-                p = e.control,
-                m = e.input,
-                g = e.focus_node,
+                i = e.wrapper,
+                f = e.control,
+                g = e.input,
+                v = e.focus_node,
                 E = {
                     passive: !0
                 },
-                y = e.inputId + "-ts-dropdown";
+                M = e.inputId + "-ts-dropdown";
             D(o, {
-                id: y
-            }), D(g, {
+                id: M
+            }), D(v, {
                 role: "combobox",
                 "aria-haspopup": "listbox",
                 "aria-expanded": "false",
-                "aria-controls": y
+                "aria-controls": M
             });
-            let W = Oe(g, e.inputId + "-ts-control"),
-                U = "label[for='" + je(e.inputId) + "']",
-                f = document.querySelector(U),
-                z = e.focus.bind(e);
-            if (f) {
-                G(f, "click", z), D(f, {
-                    for: W
+            let X = Se(v, e.inputId + "-ts-control"),
+                U = "label[for='" + De(e.inputId) + "']",
+                h = document.querySelector(U),
+                Y = e.focus.bind(e);
+            if (h) {
+                Q(h, "click", Y), D(h, {
+                    for: X
                 });
-                let b = Oe(f, e.inputId + "-ts-label");
-                D(g, {
+                let b = Se(h, e.inputId + "-ts-label");
+                D(v, {
                     "aria-labelledby": b
                 }), D(o, {
                     "aria-labelledby": b
                 })
             }
-            if (r.style.width = m.style.width, e.plugins.names.length) {
+            if (i.style.width = g.style.width, e.plugins.names.length) {
                 let b = "plugin-" + e.plugins.names.join(" plugin-");
-                te([r, s], b)
-            }(t.maxItems === null || t.maxItems > 1) && e.is_select_tag && D(m, {
+                ee([i, s], b)
+            }(t.maxItems === null || t.maxItems > 1) && e.is_select_tag && D(g, {
                 multiple: "multiple"
             }), t.placeholder && D(n, {
                 placeholder: t.placeholder
-            }), !t.splitOn && t.delimiter && (t.splitOn = new RegExp("\\s*" + (0, We.escape_regex)(t.delimiter) + "+\\s*")), t.load && t.loadThrottle && (t.load = Be(t.load, t.loadThrottle)), e.control_input.type = m.type, G(s, "mousemove", () => {
+            }), !t.splitOn && t.delimiter && (t.splitOn = new RegExp("\\s*" + (0, Ze.escape_regex)(t.delimiter) + "+\\s*")), t.load && t.loadThrottle && (t.load = Qe(t.load, t.loadThrottle)), Q(s, "mousemove", () => {
                 e.ignoreHover = !1
-            }), G(s, "mouseenter", b => {
-                var R = Te(b.target, "[data-selectable]", s);
-                R && e.onOptionHover(b, R)
+            }), Q(s, "mouseenter", b => {
+                var $ = we(b.target, "[data-selectable]", s);
+                $ && e.onOptionHover(b, $)
             }, {
                 capture: !0
-            }), G(s, "click", b => {
-                let R = Te(b.target, "[data-selectable]");
-                R && (e.onOptionSelect(b, R), j(b, !0))
-            }), G(p, "click", b => {
-                var R = Te(b.target, "[data-ts-item]", p);
-                if (R && e.onItemSelect(b, R)) {
+            }), Q(s, "click", b => {
+                let $ = we(b.target, "[data-selectable]");
+                $ && (e.onOptionSelect(b, $), j(b, !0))
+            }), Q(f, "click", b => {
+                var $ = we(b.target, "[data-ts-item]", f);
+                if ($ && e.onItemSelect(b, $)) {
                     j(b, !0);
                     return
                 }
                 n.value == "" && (e.onClick(), j(b, !0))
-            }), G(g, "keydown", b => e.onKeyDown(b)), G(n, "keypress", b => e.onKeyPress(b)), G(n, "input", b => e.onInput(b)), G(g, "blur", b => e.onBlur(b)), G(g, "focus", b => e.onFocus(b)), G(n, "paste", b => e.onPaste(b));
-            let k = b => {
-                    let R = b.composedPath()[0];
-                    if (!r.contains(R) && !s.contains(R)) {
+            }), Q(v, "keydown", b => e.onKeyDown(b)), Q(n, "keypress", b => e.onKeyPress(b)), Q(n, "input", b => e.onInput(b)), Q(v, "blur", b => e.onBlur(b)), Q(v, "focus", b => e.onFocus(b)), Q(n, "paste", b => e.onPaste(b));
+            let H = b => {
+                    let $ = b.composedPath()[0];
+                    if (!i.contains($) && !s.contains($)) {
                         e.isFocused && e.blur(), e.inputState();
                         return
                     }
-                    R == n && e.isOpen ? b.stopPropagation() : j(b, !0)
+                    $ == n && e.isOpen ? b.stopPropagation() : j(b, !0)
                 },
                 N = () => {
                     e.isOpen && e.positionDropdown()
                 };
-            G(document, "mousedown", k), G(window, "scroll", N, E), G(window, "resize", N, E), this._destroy = () => {
-                document.removeEventListener("mousedown", k), window.removeEventListener("scroll", N), window.removeEventListener("resize", N), f && f.removeEventListener("click", z)
+            Q(document, "mousedown", H), Q(window, "scroll", N, E), Q(window, "resize", N, E), this._destroy = () => {
+                document.removeEventListener("mousedown", H), window.removeEventListener("scroll", N), window.removeEventListener("resize", N), h && h.removeEventListener("click", Y)
             }, this.revertSettings = {
-                innerHTML: m.innerHTML,
-                tabIndex: m.tabIndex
-            }, m.tabIndex = -1, m.insertAdjacentElement("afterend", e.wrapper), e.sync(!1), t.items = [], delete t.optgroups, delete t.options, G(m, "invalid", () => {
+                innerHTML: g.innerHTML,
+                tabIndex: g.tabIndex
+            }, g.tabIndex = -1, g.insertAdjacentElement("afterend", e.wrapper), e.sync(!1), t.items = [], delete t.optgroups, delete t.options, Q(g, "invalid", () => {
                 e.isValid && (e.isValid = !1, e.isInvalid = !0, e.refreshState())
-            }), e.updateOriginalInput(), e.refreshItems(), e.close(!1), e.inputState(), e.isSetup = !0, m.disabled ? e.disable() : e.enable(), e.on("change", this.onChange), te(m, "tomselected", "ts-hidden-accessible"), e.trigger("initialize"), t.preload === !0 && e.preload()
+            }), e.updateOriginalInput(), e.refreshItems(), e.close(!1), e.inputState(), e.isSetup = !0, g.disabled ? e.disable() : g.readOnly ? e.setReadOnly(!0) : e.enable(), e.on("change", this.onChange), ee(g, "tomselected", "ts-hidden-accessible"), e.trigger("initialize"), t.preload === !0 && e.preload()
         }
         setupOptions(e = [], t = []) {
-            this.addOptions(e), (0, ne.iterate)(t, n => {
+            this.addOptions(e), (0, te.iterate)(t, n => {
                 this.registerOptionGroup(n)
             })
         }
         setupTemplates() {
             var e = this,
                 t = e.settings.labelField,
                 n = e.settings.optgroupLabelField,
                 s = {
                     optgroup: o => {
-                        let r = document.createElement("div");
-                        return r.className = "optgroup", r.appendChild(o.options), r
+                        let i = document.createElement("div");
+                        return i.className = "optgroup", i.appendChild(o.options), i
                     },
-                    optgroup_header: (o, r) => '<div class="optgroup-header">' + r(o[n]) + "</div>",
-                    option: (o, r) => "<div>" + r(o[t]) + "</div>",
-                    item: (o, r) => "<div>" + r(o[t]) + "</div>",
-                    option_create: (o, r) => '<div class="create">Add <strong>' + r(o.input) + "</strong>&hellip;</div>",
+                    optgroup_header: (o, i) => '<div class="optgroup-header">' + i(o[n]) + "</div>",
+                    option: (o, i) => "<div>" + i(o[t]) + "</div>",
+                    item: (o, i) => "<div>" + i(o[t]) + "</div>",
+                    option_create: (o, i) => '<div class="create">Add <strong>' + i(o.input) + "</strong>&hellip;</div>",
                     no_results: () => '<div class="no-results">No results found</div>',
                     loading: () => '<div class="spinner"></div>',
                     not_loading: () => {},
                     dropdown: () => "<div></div>"
                 };
             e.settings.render = Object.assign({}, s, e.settings.render)
         }
@@ -1256,43 +1261,43 @@
                 focus: "onFocus",
                 blur: "onBlur"
             };
             for (e in n) t = this.settings[n[e]], t && this.on(e, t)
         }
         sync(e = !0) {
             let t = this,
-                n = e ? Se(t.input, {
+                n = e ? Oe(t.input, {
                     delimiter: t.settings.delimiter
                 }) : t.settings;
             t.setupOptions(n.options, n.optgroups), t.setValue(n.items || [], !0), t.lastQuery = null
         }
         onClick() {
             var e = this;
             if (e.activeItems.length > 0) {
                 e.clearActiveItems(), e.focus();
                 return
             }
             e.isFocused && e.isOpen ? e.blur() : e.focus()
         }
         onMouseDown() {}
         onChange() {
-            we(this.input, "input"), we(this.input, "change")
+            Te(this.input, "input"), Te(this.input, "change")
         }
         onPaste(e) {
             var t = this;
             if (t.isInputHidden || t.isLocked) {
                 j(e);
                 return
             }
             t.settings.splitOn && setTimeout(() => {
                 var n = t.inputValue();
                 if (n.match(t.settings.splitOn)) {
                     var s = n.trim().split(t.settings.splitOn);
-                    (0, ne.iterate)(s, o => {
-                        se(o) && (this.options[o] ? t.addItem(o) : t.createItem(o))
+                    (0, te.iterate)(s, o => {
+                        ne(o) && (this.options[o] ? t.addItem(o) : t.createItem(o))
                     })
                 }
             }, 0)
         }
         onKeyPress(e) {
             var t = this;
             if (t.isLocked) {
@@ -1309,15 +1314,15 @@
             var t = this;
             if (t.ignoreHover = !0, t.isLocked) {
                 e.keyCode !== 9 && j(e);
                 return
             }
             switch (e.keyCode) {
                 case 65:
-                    if (le(me, e) && t.control_input.value == "") {
+                    if (ae(me, e) && t.control_input.value == "") {
                         j(e), t.selectAll();
                         return
                     }
                     break;
                 case 27:
                     t.isOpen && (j(e, !0), t.close()), t.clearActiveItems();
                     return;
@@ -1349,34 +1354,44 @@
                     t.settings.selectOnTab && (t.canSelect(t.activeOption) && (t.onOptionSelect(e, t.activeOption), j(e)), t.settings.create && t.createItem() && j(e));
                     return;
                 case 8:
                 case 46:
                     t.deleteSelection(e);
                     return
             }
-            t.isInputHidden && !le(me, e) && j(e)
+            t.isInputHidden && !ae(me, e) && j(e)
         }
         onInput(e) {
-            var t = this;
-            if (!t.isLocked) {
-                var n = t.inputValue();
-                t.lastValue !== n && (t.lastValue = n, t.settings.shouldLoad.call(t, n) && t.load(n), t.refreshOptions(), t.trigger("type", n))
+            if (this.isLocked) return;
+            let t = this.inputValue();
+            if (this.lastValue !== t) {
+                if (this.lastValue = t, t == "") {
+                    this._onInput();
+                    return
+                }
+                this.refreshTimeout && clearTimeout(this.refreshTimeout), this.refreshTimeout = Ge(() => {
+                    this.refreshTimeout = null, this._onInput()
+                }, this.settings.refreshThrottle)
             }
         }
+        _onInput() {
+            let e = this.lastValue;
+            this.settings.shouldLoad.call(this, e) && this.load(e), this.refreshOptions(), this.trigger("type", e)
+        }
         onOptionHover(e, t) {
             this.ignoreHover || this.setActiveOption(t, !1)
         }
         onFocus(e) {
             var t = this,
                 n = t.isFocused;
-            if (t.isDisabled) {
+            if (t.isDisabled || t.isReadOnly) {
                 t.blur(), j(e);
                 return
             }
-            t.ignoreFocus || (t.isFocused = !0, t.settings.preload === "focus" && t.preload(), n || t.trigger("focus"), t.activeItems.length || (t.showInput(), t.refreshOptions(!!t.settings.openOnFocus)), t.refreshState())
+            t.ignoreFocus || (t.isFocused = !0, t.settings.preload === "focus" && t.preload(), n || t.trigger("focus"), t.activeItems.length || (t.inputState(), t.refreshOptions(!!t.settings.openOnFocus)), t.refreshState())
         }
         onBlur(e) {
             if (document.hasFocus() !== !1) {
                 var t = this;
                 if (t.isFocused) {
                     t.isFocused = !1, t.ignoreFocus = !1;
                     var n = () => {
@@ -1401,30 +1416,30 @@
         }
         canLoad(e) {
             return !(!this.settings.load || this.loadedSearches.hasOwnProperty(e))
         }
         load(e) {
             let t = this;
             if (!t.canLoad(e)) return;
-            te(t.wrapper, t.settings.loadingClass), t.loading++;
+            ee(t.wrapper, t.settings.loadingClass), t.loading++;
             let n = t.loadCallback.bind(t);
             t.settings.load.call(t, e, n)
         }
         loadCallback(e, t) {
             let n = this;
-            n.loading = Math.max(n.loading - 1, 0), n.lastQuery = null, n.clearActiveOption(), n.setupOptions(e, t), n.refreshOptions(n.isFocused && !n.isInputHidden), n.loading || ie(n.wrapper, n.settings.loadingClass), n.trigger("load", e, t)
+            n.loading = Math.max(n.loading - 1, 0), n.lastQuery = null, n.clearActiveOption(), n.setupOptions(e, t), n.refreshOptions(n.isFocused && !n.isInputHidden), n.loading || re(n.wrapper, n.settings.loadingClass), n.trigger("load", e, t)
         }
         preload() {
             var e = this.wrapper.classList;
             e.contains("preloaded") || (e.add("preloaded"), this.load(""))
         }
         setTextboxValue(e = "") {
             var t = this.control_input,
                 n = t.value !== e;
-            n && (t.value = e, we(t, "update"), this.lastValue = e)
+            n && (t.value = e, Te(t, "update"), this.lastValue = e)
         }
         getValue() {
             return this.is_select_tag && this.input.hasAttribute("multiple") ? this.items : this.items.join(this.settings.delimiter)
         }
         setValue(e, t) {
             var n = t ? [] : ["change"];
             Fe(this, n, () => {
@@ -1432,94 +1447,88 @@
             })
         }
         setMaxItems(e) {
             e === 0 && (e = null), this.settings.maxItems = e, this.refreshState()
         }
         setActiveItem(e, t) {
             var n = this,
-                s, o, r, p, m, g;
+                s, o, i, f, g, v;
             if (n.settings.mode !== "single") {
                 if (!e) {
-                    n.clearActiveItems(), n.isFocused && n.showInput();
+                    n.clearActiveItems(), n.isFocused && n.inputState();
                     return
                 }
-                if (s = t && t.type.toLowerCase(), s === "click" && le("shiftKey", t) && n.activeItems.length) {
-                    for (g = n.getLastActive(), r = Array.prototype.indexOf.call(n.control.children, g), p = Array.prototype.indexOf.call(n.control.children, e), r > p && (m = r, r = p, p = m), o = r; o <= p; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
+                if (s = t && t.type.toLowerCase(), s === "click" && ae("shiftKey", t) && n.activeItems.length) {
+                    for (v = n.getLastActive(), i = Array.prototype.indexOf.call(n.control.children, v), f = Array.prototype.indexOf.call(n.control.children, e), i > f && (g = i, i = f, f = g), o = i; o <= f; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
                     j(t)
-                } else s === "click" && le(me, t) || s === "keydown" && le("shiftKey", t) ? e.classList.contains("active") ? n.removeActiveItem(e) : n.setActiveItemClass(e) : (n.clearActiveItems(), n.setActiveItemClass(e));
-                n.hideInput(), n.isFocused || n.focus()
+                } else s === "click" && ae(me, t) || s === "keydown" && ae("shiftKey", t) ? e.classList.contains("active") ? n.removeActiveItem(e) : n.setActiveItemClass(e) : (n.clearActiveItems(), n.setActiveItemClass(e));
+                n.inputState(), n.isFocused || n.focus()
             }
         }
         setActiveItemClass(e) {
             let t = this,
                 n = t.control.querySelector(".last-active");
-            n && ie(n, "last-active"), te(e, "active last-active"), t.trigger("item_select", e), t.activeItems.indexOf(e) == -1 && t.activeItems.push(e)
+            n && re(n, "last-active"), ee(e, "active last-active"), t.trigger("item_select", e), t.activeItems.indexOf(e) == -1 && t.activeItems.push(e)
         }
         removeActiveItem(e) {
             var t = this.activeItems.indexOf(e);
-            this.activeItems.splice(t, 1), ie(e, "active")
+            this.activeItems.splice(t, 1), re(e, "active")
         }
         clearActiveItems() {
-            ie(this.activeItems, "active"), this.activeItems = []
+            re(this.activeItems, "active"), this.activeItems = []
         }
         setActiveOption(e, t = !0) {
             e !== this.activeOption && (this.clearActiveOption(), e && (this.activeOption = e, D(this.focus_node, {
                 "aria-activedescendant": e.getAttribute("id")
             }), D(e, {
                 "aria-selected": "true"
-            }), te(e, "active"), t && this.scrollToOption(e)))
+            }), ee(e, "active"), t && this.scrollToOption(e)))
         }
         scrollToOption(e, t) {
             if (!e) return;
             let n = this.dropdown_content,
                 s = n.clientHeight,
                 o = n.scrollTop || 0,
-                r = e.offsetHeight,
-                p = e.getBoundingClientRect().top - n.getBoundingClientRect().top + o;
-            p + r > s + o ? this.scroll(p - s + r, t) : p < o && this.scroll(p, t)
+                i = e.offsetHeight,
+                f = e.getBoundingClientRect().top - n.getBoundingClientRect().top + o;
+            f + i > s + o ? this.scroll(f - s + i, t) : f < o && this.scroll(f, t)
         }
         scroll(e, t) {
             let n = this.dropdown_content;
             t && (n.style.scrollBehavior = t), n.scrollTop = e, n.style.scrollBehavior = ""
         }
         clearActiveOption() {
-            this.activeOption && (ie(this.activeOption, "active"), D(this.activeOption, {
+            this.activeOption && (re(this.activeOption, "active"), D(this.activeOption, {
                 "aria-selected": null
             })), this.activeOption = null, D(this.focus_node, {
                 "aria-activedescendant": null
             })
         }
         selectAll() {
             let e = this;
             if (e.settings.mode === "single") return;
             let t = e.controlChildren();
-            t.length && (e.hideInput(), e.close(), e.activeItems = t, (0, ne.iterate)(t, n => {
+            t.length && (e.inputState(), e.close(), e.activeItems = t, (0, te.iterate)(t, n => {
                 e.setActiveItemClass(n)
             }))
         }
         inputState() {
             var e = this;
             e.control.contains(e.control_input) && (D(e.control_input, {
                 placeholder: e.settings.placeholder
             }), e.activeItems.length > 0 || !e.isFocused && e.settings.hidePlaceholder && e.items.length > 0 ? (e.setTextboxValue(), e.isInputHidden = !0) : (e.settings.hidePlaceholder && e.items.length > 0 && D(e.control_input, {
                 placeholder: ""
             }), e.isInputHidden = !1), e.wrapper.classList.toggle("input-hidden", e.isInputHidden))
         }
-        hideInput() {
-            this.inputState()
-        }
-        showInput() {
-            this.inputState()
-        }
         inputValue() {
             return this.control_input.value.trim()
         }
         focus() {
             var e = this;
-            e.isDisabled || (e.ignoreFocus = !0, e.control_input.offsetWidth ? e.control_input.focus() : e.focus_node.focus(), setTimeout(() => {
+            e.isDisabled || e.isReadOnly || (e.ignoreFocus = !0, e.control_input.offsetWidth ? e.control_input.focus() : e.focus_node.focus(), setTimeout(() => {
                 e.ignoreFocus = !1, e.onFocus()
             }, 0))
         }
         blur() {
             this.focus_node.blur(), this.onBlur()
         }
         getScoreFunction(e) {
@@ -1539,105 +1548,117 @@
         }
         search(e) {
             var t, n, s = this,
                 o = this.getSearchOptions();
             if (s.settings.score && (n = s.settings.score.call(s, e), typeof n != "function")) throw new Error('Tom Select "score" setting must be a function that returns a function');
             return e !== s.lastQuery ? (s.lastQuery = e, t = s.sifter.search(e, Object.assign(o, {
                 score: n
-            })), s.currentResults = t) : t = Object.assign({}, s.currentResults), s.settings.hideSelected && (t.items = t.items.filter(r => {
-                let p = se(r.id);
-                return !(p && s.items.indexOf(p) !== -1)
+            })), s.currentResults = t) : t = Object.assign({}, s.currentResults), s.settings.hideSelected && (t.items = t.items.filter(i => {
+                let f = ne(i.id);
+                return !(f && s.items.indexOf(f) !== -1)
             })), t
         }
         refreshOptions(e = !0) {
-            var t, n, s, o, r, p, m, g, E, y;
-            let W = {},
+            var t, n, s, o, i, f, g, v, E, M;
+            let X = {},
                 U = [];
-            var f = this,
-                z = f.inputValue();
-            let k = z === f.lastQuery || z == "" && f.lastQuery == null;
-            var N = f.search(z),
+            var h = this,
+                Y = h.inputValue();
+            let H = Y === h.lastQuery || Y == "" && h.lastQuery == null;
+            var N = h.search(Y),
                 b = null,
-                R = f.settings.shouldOpen || !1,
-                Z = f.dropdown_content;
-            for (k && (b = f.activeOption, b && (E = b.closest("[data-group]"))), o = N.items.length, typeof f.settings.maxOptions == "number" && (o = Math.min(o, f.settings.maxOptions)), o > 0 && (R = !0), t = 0; t < o; t++) {
-                let F = N.items[t];
-                if (!F) continue;
-                let x = F.id,
-                    q = f.options[x];
+                $ = h.settings.shouldOpen || !1,
+                W = h.dropdown_content;
+            H && (b = h.activeOption, b && (E = b.closest("[data-group]"))), o = N.items.length, typeof h.settings.maxOptions == "number" && (o = Math.min(o, h.settings.maxOptions)), o > 0 && ($ = !0);
+            let oe = (A, S) => {
+                let q = X[A];
+                if (q !== void 0) {
+                    let z = U[q];
+                    if (z !== void 0) return [q, z.fragment]
+                }
+                let P = document.createDocumentFragment();
+                return q = U.length, U.push({
+                    fragment: P,
+                    order: S,
+                    optgroup: A
+                }), [q, P]
+            };
+            for (t = 0; t < o; t++) {
+                let A = N.items[t];
+                if (!A) continue;
+                let S = A.id,
+                    q = h.options[S];
                 if (q === void 0) continue;
-                let V = ve(x),
-                    Q = f.getOption(V, !0);
-                for (f.settings.hideSelected || Q.classList.toggle("selected", f.items.includes(V)), r = q[f.settings.optgroupField] || "", p = Array.isArray(r) ? r : [r], n = 0, s = p && p.length; n < s; n++) {
-                    r = p[n], f.optgroups.hasOwnProperty(r) || (r = "");
-                    let X = W[r];
-                    X === void 0 && (X = document.createDocumentFragment(), U.push(r)), n > 0 && (Q = Q.cloneNode(!0), D(Q, {
+                let P = ve(S),
+                    z = h.getOption(P, !0);
+                for (h.settings.hideSelected || z.classList.toggle("selected", h.items.includes(P)), i = q[h.settings.optgroupField] || "", f = Array.isArray(i) ? i : [i], n = 0, s = f && f.length; n < s; n++) {
+                    i = f[n];
+                    let se = q.$order,
+                        p = h.optgroups[i];
+                    p === void 0 ? i = "" : se = p.$order;
+                    let [_, w] = oe(i, se);
+                    n > 0 && (z = z.cloneNode(!0), D(z, {
                         id: q.$id + "-clone-" + n,
                         "aria-selected": null
-                    }), Q.classList.add("ts-cloned"), ie(Q, "active"), f.activeOption && f.activeOption.dataset.value == x && E && E.dataset.group === r.toString() && (b = Q)), X.appendChild(Q), W[r] = X
+                    }), z.classList.add("ts-cloned"), re(z, "active"), h.activeOption && h.activeOption.dataset.value == S && E && E.dataset.group === i.toString() && (b = z)), w.appendChild(z), i != "" && (X[i] = _)
                 }
             }
-            f.settings.lockOptgroupOrder && U.sort((F, x) => {
-                let q = f.optgroups[F],
-                    V = f.optgroups[x],
-                    Q = q && q.$order || 0,
-                    X = V && V.$order || 0;
-                return Q - X
-            }), m = document.createDocumentFragment(), (0, ne.iterate)(U, F => {
-                let x = W[F];
-                if (!x || !x.children.length) return;
-                let q = f.optgroups[F];
-                if (q !== void 0) {
-                    let V = document.createDocumentFragment(),
-                        Q = f.render("optgroup_header", q);
-                    ae(V, Q), ae(V, x);
-                    let X = f.render("optgroup", {
-                        group: q,
-                        options: V
+            h.settings.lockOptgroupOrder && U.sort((A, S) => A.order - S.order), g = document.createDocumentFragment(), (0, te.iterate)(U, A => {
+                let S = A.fragment,
+                    q = A.optgroup;
+                if (!S || !S.children.length) return;
+                let P = h.optgroups[q];
+                if (P !== void 0) {
+                    let z = document.createDocumentFragment(),
+                        se = h.render("optgroup_header", P);
+                    ce(z, se), ce(z, S);
+                    let p = h.render("optgroup", {
+                        group: P,
+                        options: z
                     });
-                    ae(m, X)
-                } else ae(m, x)
-            }), Z.innerHTML = "", ae(Z, m), f.settings.highlight && (Ye(Z), N.query.length && N.tokens.length && (0, ne.iterate)(N.tokens, F => {
-                ze(Z, F.regex)
+                    ce(g, p)
+                } else ce(g, S)
+            }), W.innerHTML = "", ce(W, g), h.settings.highlight && (Be(W), N.query.length && N.tokens.length && (0, te.iterate)(N.tokens, A => {
+                Ye(W, A.regex)
             }));
-            var $ = F => {
-                let x = f.render(F, {
-                    input: z
+            var V = A => {
+                let S = h.render(A, {
+                    input: Y
                 });
-                return x && (R = !0, Z.insertBefore(x, Z.firstChild)), x
+                return S && ($ = !0, W.insertBefore(S, W.firstChild)), S
             };
-            if (f.loading ? $("loading") : f.settings.shouldLoad.call(f, z) ? N.items.length === 0 && $("no_results") : $("not_loading"), g = f.canCreate(z), g && (y = $("option_create")), f.hasOptions = N.items.length > 0 || g, R) {
+            if (h.loading ? V("loading") : h.settings.shouldLoad.call(h, Y) ? N.items.length === 0 && V("no_results") : V("not_loading"), v = h.canCreate(Y), v && (M = V("option_create")), h.hasOptions = N.items.length > 0 || v, $) {
                 if (N.items.length > 0) {
-                    if (!b && f.settings.mode === "single" && f.items[0] != null && (b = f.getOption(f.items[0])), !Z.contains(b)) {
-                        let F = 0;
-                        y && !f.settings.addPrecedence && (F = 1), b = f.selectable()[F]
+                    if (!b && h.settings.mode === "single" && h.items[0] != null && (b = h.getOption(h.items[0])), !W.contains(b)) {
+                        let A = 0;
+                        M && !h.settings.addPrecedence && (A = 1), b = h.selectable()[A]
                     }
-                } else y && (b = y);
-                e && !f.isOpen && (f.open(), f.scrollToOption(b, "auto")), f.setActiveOption(b)
-            } else f.clearActiveOption(), e && f.isOpen && f.close(!1)
+                } else M && (b = M);
+                e && !h.isOpen && (h.open(), h.scrollToOption(b, "auto")), h.setActiveOption(b)
+            } else h.clearActiveOption(), e && h.isOpen && h.close(!1)
         }
         selectable() {
             return this.dropdown_content.querySelectorAll("[data-selectable]")
         }
         addOption(e, t = !1) {
             let n = this;
             if (Array.isArray(e)) return n.addOptions(e, t), !1;
-            let s = se(e[n.settings.valueField]);
+            let s = ne(e[n.settings.valueField]);
             return s === null || n.options.hasOwnProperty(s) ? !1 : (e.$order = e.$order || ++n.order, e.$id = n.inputId + "-opt-" + e.$order, n.options[s] = e, n.lastQuery = null, t && (n.userOptions[s] = t, n.trigger("option_add", s, e)), s)
         }
         addOptions(e, t = !1) {
-            (0, ne.iterate)(e, n => {
+            (0, te.iterate)(e, n => {
                 this.addOption(n, t)
             })
         }
         registerOption(e) {
             return this.addOption(e)
         }
         registerOptionGroup(e) {
-            var t = se(e[this.settings.optgroupValueField]);
+            var t = ne(e[this.settings.optgroupValueField]);
             return t === null ? !1 : (e.$order = e.$order || ++this.order, this.optgroups[t] = e, t)
         }
         addOptionGroup(e, t) {
             var n;
             t[this.settings.optgroupValueField] = e, (n = this.registerOptionGroup(t)) && this.trigger("optgroup_add", n, t)
         }
         removeOptionGroup(e) {
@@ -1645,164 +1666,164 @@
         }
         clearOptionGroups() {
             this.optgroups = {}, this.clearCache(), this.trigger("optgroup_clear")
         }
         updateOption(e, t) {
             let n = this;
             var s, o;
-            let r = se(e),
-                p = se(t[n.settings.valueField]);
-            if (r === null) return;
-            let m = n.options[r];
-            if (m == null) return;
-            if (typeof p != "string") throw new Error("Value must be set in option data");
-            let g = n.getOption(r),
-                E = n.getItem(r);
-            if (t.$order = t.$order || m.$order, delete n.options[r], n.uncacheValue(p), n.options[p] = t, g) {
-                if (n.dropdown_content.contains(g)) {
-                    let y = n._render("option", t);
-                    ge(g, y), n.activeOption === g && n.setActiveOption(y)
+            let i = ne(e),
+                f = ne(t[n.settings.valueField]);
+            if (i === null) return;
+            let g = n.options[i];
+            if (g == null) return;
+            if (typeof f != "string") throw new Error("Value must be set in option data");
+            let v = n.getOption(i),
+                E = n.getItem(i);
+            if (t.$order = t.$order || g.$order, delete n.options[i], n.uncacheValue(f), n.options[f] = t, v) {
+                if (n.dropdown_content.contains(v)) {
+                    let M = n._render("option", t);
+                    ge(v, M), n.activeOption === v && n.setActiveOption(M)
                 }
-                g.remove()
+                v.remove()
             }
-            E && (o = n.items.indexOf(r), o !== -1 && n.items.splice(o, 1, p), s = n._render("item", t), E.classList.contains("active") && te(s, "active"), ge(E, s)), n.lastQuery = null
+            E && (o = n.items.indexOf(i), o !== -1 && n.items.splice(o, 1, f), s = n._render("item", t), E.classList.contains("active") && ee(s, "active"), ge(E, s)), n.lastQuery = null
         }
         removeOption(e, t) {
             let n = this;
             e = ve(e), n.uncacheValue(e), delete n.userOptions[e], delete n.options[e], n.lastQuery = null, n.trigger("option_remove", e), n.removeItem(e, t)
         }
         clearOptions(e) {
             let t = (e || this.clearFilter).bind(this);
             this.loadedSearches = {}, this.userOptions = {}, this.clearCache();
             let n = {};
-            (0, ne.iterate)(this.options, (s, o) => {
+            (0, te.iterate)(this.options, (s, o) => {
                 t(s, o) && (n[o] = s)
             }), this.options = this.sifter.items = n, this.lastQuery = null, this.trigger("option_clear")
         }
         clearFilter(e, t) {
             return this.items.indexOf(t) >= 0
         }
         getOption(e, t = !1) {
-            let n = se(e);
+            let n = ne(e);
             if (n === null) return null;
             let s = this.options[n];
             if (s != null) {
                 if (s.$div) return s.$div;
                 if (t) return this._render("option", s)
             }
             return null
         }
         getAdjacent(e, t, n = "option") {
             var s = this,
                 o;
             if (!e) return null;
             n == "item" ? o = s.controlChildren() : o = s.dropdown_content.querySelectorAll("[data-selectable]");
-            for (let r = 0; r < o.length; r++)
-                if (o[r] == e) return t > 0 ? o[r + 1] : o[r - 1];
+            for (let i = 0; i < o.length; i++)
+                if (o[i] == e) return t > 0 ? o[i + 1] : o[i - 1];
             return null
         }
         getItem(e) {
             if (typeof e == "object") return e;
-            var t = se(e);
-            return t !== null ? this.control.querySelector(`[data-value="${He(t)}"]`) : null
+            var t = ne(e);
+            return t !== null ? this.control.querySelector(`[data-value="${ke(t)}"]`) : null
         }
         addItems(e, t) {
             var n = this,
                 s = Array.isArray(e) ? e : [e];
-            s = s.filter(r => n.items.indexOf(r) === -1);
+            s = s.filter(i => n.items.indexOf(i) === -1);
             let o = s[s.length - 1];
-            s.forEach(r => {
-                n.isPending = r !== o, n.addItem(r, t)
+            s.forEach(i => {
+                n.isPending = i !== o, n.addItem(i, t)
             })
         }
         addItem(e, t) {
             var n = t ? [] : ["change", "dropdown_close"];
             Fe(this, n, () => {
                 var s, o;
-                let r = this,
-                    p = r.settings.mode,
-                    m = se(e);
-                if (!(m && r.items.indexOf(m) !== -1 && (p === "single" && r.close(), p === "single" || !r.settings.duplicates)) && !(m === null || !r.options.hasOwnProperty(m)) && (p === "single" && r.clear(t), !(p === "multi" && r.isFull()))) {
-                    if (s = r._render("item", r.options[m]), r.control.contains(s) && (s = s.cloneNode(!0)), o = r.isFull(), r.items.splice(r.caretPos, 0, m), r.insertAtCaret(s), r.isSetup) {
-                        if (!r.isPending && r.settings.hideSelected) {
-                            let g = r.getOption(m),
-                                E = r.getAdjacent(g, 1);
-                            E && r.setActiveOption(E)
-                        }!r.isPending && !r.settings.closeAfterSelect && r.refreshOptions(r.isFocused && p !== "single"), r.settings.closeAfterSelect != !1 && r.isFull() ? r.close() : r.isPending || r.positionDropdown(), r.trigger("item_add", m, s), r.isPending || r.updateOriginalInput({
+                let i = this,
+                    f = i.settings.mode,
+                    g = ne(e);
+                if (!(g && i.items.indexOf(g) !== -1 && (f === "single" && i.close(), f === "single" || !i.settings.duplicates)) && !(g === null || !i.options.hasOwnProperty(g)) && (f === "single" && i.clear(t), !(f === "multi" && i.isFull()))) {
+                    if (s = i._render("item", i.options[g]), i.control.contains(s) && (s = s.cloneNode(!0)), o = i.isFull(), i.items.splice(i.caretPos, 0, g), i.insertAtCaret(s), i.isSetup) {
+                        if (!i.isPending && i.settings.hideSelected) {
+                            let v = i.getOption(g),
+                                E = i.getAdjacent(v, 1);
+                            E && i.setActiveOption(E)
+                        }!i.isPending && !i.settings.closeAfterSelect && i.refreshOptions(i.isFocused && f !== "single"), i.settings.closeAfterSelect != !1 && i.isFull() ? i.close() : i.isPending || i.positionDropdown(), i.trigger("item_add", g, s), i.isPending || i.updateOriginalInput({
                             silent: t
                         })
-                    }(!r.isPending || !o && r.isFull()) && (r.inputState(), r.refreshState())
+                    }(!i.isPending || !o && i.isFull()) && (i.inputState(), i.refreshState())
                 }
             })
         }
         removeItem(e = null, t) {
             let n = this;
             if (e = n.getItem(e), !e) return;
             var s, o;
-            let r = e.dataset.value;
-            s = Ce(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), ie(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(r) && n.removeOption(r, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
+            let i = e.dataset.value;
+            s = Ce(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), re(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(i) && n.removeOption(i, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
                 silent: t
-            }), n.refreshState(), n.positionDropdown(), n.trigger("item_remove", r, e)
+            }), n.refreshState(), n.positionDropdown(), n.trigger("item_remove", i, e)
         }
         createItem(e = null, t = () => {}) {
             arguments.length === 3 && (t = arguments[2]), typeof t != "function" && (t = () => {});
             var n = this,
                 s = n.caretPos,
                 o;
             if (e = e || n.inputValue(), !n.canCreate(e)) return t(), !1;
             n.lock();
-            var r = !1,
-                p = m => {
-                    if (n.unlock(), !m || typeof m != "object") return t();
-                    var g = se(m[n.settings.valueField]);
-                    if (typeof g != "string") return t();
-                    n.setTextboxValue(), n.addOption(m, !0), n.setCaret(s), n.addItem(g), t(m), r = !0
+            var i = !1,
+                f = g => {
+                    if (n.unlock(), !g || typeof g != "object") return t();
+                    var v = ne(g[n.settings.valueField]);
+                    if (typeof v != "string") return t();
+                    n.setTextboxValue(), n.addOption(g, !0), n.setCaret(s), n.addItem(v), t(g), i = !0
                 };
-            return typeof n.settings.create == "function" ? o = n.settings.create.call(this, e, p) : o = {
+            return typeof n.settings.create == "function" ? o = n.settings.create.call(this, e, f) : o = {
                 [n.settings.labelField]: e,
                 [n.settings.valueField]: e
-            }, r || p(o), !0
+            }, i || f(o), !0
         }
         refreshItems() {
             var e = this;
             e.lastQuery = null, e.isSetup && e.addItems(e.items), e.updateOriginalInput(), e.refreshState()
         }
         refreshState() {
             let e = this;
             e.refreshValidityState();
             let t = e.isFull(),
                 n = e.isLocked;
             e.wrapper.classList.toggle("rtl", e.rtl);
             let s = e.wrapper.classList;
-            s.toggle("focus", e.isFocused), s.toggle("disabled", e.isDisabled), s.toggle("required", e.isRequired), s.toggle("invalid", !e.isValid), s.toggle("locked", n), s.toggle("full", t), s.toggle("input-active", e.isFocused && !e.isInputHidden), s.toggle("dropdown-active", e.isOpen), s.toggle("has-options", qe(e.options)), s.toggle("has-items", e.items.length > 0)
+            s.toggle("focus", e.isFocused), s.toggle("disabled", e.isDisabled), s.toggle("readonly", e.isReadOnly), s.toggle("required", e.isRequired), s.toggle("invalid", !e.isValid), s.toggle("locked", n), s.toggle("full", t), s.toggle("input-active", e.isFocused && !e.isInputHidden), s.toggle("dropdown-active", e.isOpen), s.toggle("has-options", ze(e.options)), s.toggle("has-items", e.items.length > 0)
         }
         refreshValidityState() {
             var e = this;
             e.input.validity && (e.isValid = e.input.validity.valid, e.isInvalid = !e.isValid)
         }
         isFull() {
             return this.settings.maxItems !== null && this.items.length >= this.settings.maxItems
         }
         updateOriginalInput(e = {}) {
             let t = this;
             var n, s;
             let o = t.input.querySelector('option[value=""]');
             if (t.is_select_tag) {
-                let m = function(g, E, y) {
-                        return g || (g = ee('<option value="' + de(E) + '">' + de(y) + "</option>")), g != o && t.input.append(g), r.push(g), (g != o || p > 0) && (g.selected = !0), g
+                let g = function(v, E, M) {
+                        return v || (v = Z('<option value="' + de(E) + '">' + de(M) + "</option>")), v != o && t.input.append(v), i.push(v), (v != o || f > 0) && (v.selected = !0), v
                     },
-                    r = [],
-                    p = t.input.querySelectorAll("option:checked").length;
-                t.input.querySelectorAll("option:checked").forEach(g => {
-                    g.selected = !1
-                }), t.items.length == 0 && t.settings.mode == "single" ? m(o, "", "") : t.items.forEach(g => {
-                    if (n = t.options[g], s = n[t.settings.labelField] || "", r.includes(n.$option)) {
-                        let E = t.input.querySelector(`option[value="${He(g)}"]:not(:checked)`);
-                        m(E, g, s)
-                    } else n.$option = m(n.$option, g, s)
+                    i = [],
+                    f = t.input.querySelectorAll("option:checked").length;
+                t.input.querySelectorAll("option:checked").forEach(v => {
+                    v.selected = !1
+                }), t.items.length == 0 && t.settings.mode == "single" ? g(o, "", "") : t.items.forEach(v => {
+                    if (n = t.options[v], s = n[t.settings.labelField] || "", i.includes(n.$option)) {
+                        let E = t.input.querySelector(`option[value="${ke(v)}"]:not(:checked)`);
+                        g(E, v, s)
+                    } else n.$option = g(n.$option, v, s)
                 })
             } else t.input.value = t.getValue();
             t.isSetup && (e.silent || t.trigger("change", t.getValue()))
         }
         open() {
             var e = this;
             e.isLocked || e.isOpen || e.settings.mode === "multi" && e.isFull() || (e.isOpen = !0, D(e.focus_node, {
@@ -1814,15 +1835,15 @@
                 visibility: "visible",
                 display: "block"
             }), e.focus(), e.trigger("dropdown_open", e.dropdown))
         }
         close(e = !0) {
             var t = this,
                 n = t.isOpen;
-            e && (t.setTextboxValue(), t.settings.mode === "single" && t.items.length && t.hideInput()), t.isOpen = !1, D(t.focus_node, {
+            e && (t.setTextboxValue(), t.settings.mode === "single" && t.items.length && t.inputState()), t.isOpen = !1, D(t.focus_node, {
                 "aria-expanded": "false"
             }), he(t.dropdown, {
                 display: "none"
             }), t.settings.hideSelected && t.clearActiveOption(), t.refreshState(), n && t.trigger("dropdown_close", t.dropdown)
         }
         positionDropdown() {
             if (this.settings.dropdownParent === "body") {
@@ -1837,46 +1858,46 @@
                 })
             }
         }
         clear(e) {
             var t = this;
             if (t.items.length) {
                 var n = t.controlChildren();
-                (0, ne.iterate)(n, s => {
+                (0, te.iterate)(n, s => {
                     t.removeItem(s, !0)
-                }), t.showInput(), e || t.updateOriginalInput(), t.trigger("clear")
+                }), t.inputState(), e || t.updateOriginalInput(), t.trigger("clear")
             }
         }
         insertAtCaret(e) {
             let t = this,
                 n = t.caretPos,
                 s = t.control;
             s.insertBefore(e, s.children[n] || null), t.setCaret(n + 1)
         }
         deleteSelection(e) {
-            var t, n, s, o, r = this;
-            t = e && e.keyCode === 8 ? -1 : 1, n = Ge(r.control_input);
-            let p = [];
-            if (r.activeItems.length) o = Ae(r.activeItems, t), s = Ce(o), t > 0 && s++, (0, ne.iterate)(r.activeItems, m => p.push(m));
-            else if ((r.isFocused || r.settings.mode === "single") && r.items.length) {
-                let m = r.controlChildren(),
-                    g;
-                t < 0 && n.start === 0 && n.length === 0 ? g = m[r.caretPos - 1] : t > 0 && n.start === r.inputValue().length && (g = m[r.caretPos]), g !== void 0 && p.push(g)
-            }
-            if (!r.shouldDelete(p, e)) return !1;
-            for (j(e, !0), typeof s < "u" && r.setCaret(s); p.length;) r.removeItem(p.pop());
-            return r.showInput(), r.positionDropdown(), r.refreshOptions(!1), !0
+            var t, n, s, o, i = this;
+            t = e && e.keyCode === 8 ? -1 : 1, n = Ue(i.control_input);
+            let f = [];
+            if (i.activeItems.length) o = Ae(i.activeItems, t), s = Ce(o), t > 0 && s++, (0, te.iterate)(i.activeItems, g => f.push(g));
+            else if ((i.isFocused || i.settings.mode === "single") && i.items.length) {
+                let g = i.controlChildren(),
+                    v;
+                t < 0 && n.start === 0 && n.length === 0 ? v = g[i.caretPos - 1] : t > 0 && n.start === i.inputValue().length && (v = g[i.caretPos]), v !== void 0 && f.push(v)
+            }
+            if (!i.shouldDelete(f, e)) return !1;
+            for (j(e, !0), typeof s < "u" && i.setCaret(s); f.length;) i.removeItem(f.pop());
+            return i.inputState(), i.positionDropdown(), i.refreshOptions(!1), !0
         }
         shouldDelete(e, t) {
             let n = e.map(s => s.dataset.value);
             return !(!n.length || typeof this.settings.onDelete == "function" && this.settings.onDelete(n, t) === !1)
         }
         advanceSelection(e, t) {
             var n, s, o = this;
-            o.rtl && (e *= -1), !o.inputValue().length && (le(me, t) || le("shiftKey", t) ? (n = o.getLastActive(e), n ? n.classList.contains("active") ? s = o.getAdjacent(n, e, "item") : s = n : e > 0 ? s = o.control_input.nextElementSibling : s = o.control_input.previousElementSibling, s && (s.classList.contains("active") && o.removeActiveItem(n), o.setActiveItemClass(s))) : o.moveCaret(e))
+            o.rtl && (e *= -1), !o.inputValue().length && (ae(me, t) || ae("shiftKey", t) ? (n = o.getLastActive(e), n ? n.classList.contains("active") ? s = o.getAdjacent(n, e, "item") : s = n : e > 0 ? s = o.control_input.nextElementSibling : s = o.control_input.previousElementSibling, s && (s.classList.contains("active") && o.removeActiveItem(n), o.setActiveItemClass(s))) : o.moveCaret(e))
         }
         moveCaret(e) {}
         getLastActive(e) {
             let t = this.control.querySelector(".last-active");
             if (t) return t;
             var n = this.control.querySelectorAll(".active");
             if (n) return Ae(n, e)
@@ -1884,114 +1905,122 @@
         setCaret(e) {
             this.caretPos = this.items.length
         }
         controlChildren() {
             return Array.from(this.control.querySelectorAll("[data-ts-item]"))
         }
         lock() {
-            this.isLocked = !0, this.refreshState()
+            this.setLocked(!0)
         }
         unlock() {
-            this.isLocked = !1, this.refreshState()
+            this.setLocked(!1)
+        }
+        setLocked(e = this.isReadOnly || this.isDisabled) {
+            this.isLocked = e, this.refreshState()
         }
         disable() {
-            var e = this;
-            e.input.disabled = !0, e.control_input.disabled = !0, e.focus_node.tabIndex = -1, e.isDisabled = !0, this.close(), e.lock()
+            this.setDisabled(!0), this.close()
         }
         enable() {
-            var e = this;
-            e.input.disabled = !1, e.control_input.disabled = !1, e.focus_node.tabIndex = e.tabIndex, e.isDisabled = !1, e.unlock()
+            this.setDisabled(!1)
+        }
+        setDisabled(e) {
+            this.focus_node.tabIndex = e ? -1 : this.tabIndex, this.isDisabled = e, this.input.disabled = e, this.control_input.disabled = e, this.setLocked()
+        }
+        setReadOnly(e) {
+            this.isReadOnly = e, this.input.readOnly = e, this.control_input.readOnly = e, this.setLocked()
         }
         destroy() {
             var e = this,
                 t = e.revertSettings;
-            e.trigger("destroy"), e.off(), e.wrapper.remove(), e.dropdown.remove(), e.input.innerHTML = t.innerHTML, e.input.tabIndex = t.tabIndex, ie(e.input, "tomselected", "ts-hidden-accessible"), e._destroy(), delete e.input.tomselect
+            e.trigger("destroy"), e.off(), e.wrapper.remove(), e.dropdown.remove(), e.input.innerHTML = t.innerHTML, e.input.tabIndex = t.tabIndex, re(e.input, "tomselected", "ts-hidden-accessible"), e._destroy(), delete e.input.tomselect
         }
         render(e, t) {
             var n, s;
             let o = this;
             if (typeof this.settings.render[e] != "function" || (s = o.settings.render[e].call(this, t, de), !s)) return null;
-            if (s = ee(s), e === "option" || e === "option_create" ? t[o.settings.disabledField] ? D(s, {
+            if (s = Z(s), e === "option" || e === "option_create" ? t[o.settings.disabledField] ? D(s, {
                     "aria-disabled": "true"
                 }) : D(s, {
                     "data-selectable": ""
                 }) : e === "optgroup" && (n = t.group[o.settings.optgroupValueField], D(s, {
                     "data-group": n
                 }), t.group[o.settings.disabledField] && D(s, {
                     "data-disabled": ""
                 })), e === "option" || e === "item") {
-                let r = ve(t[o.settings.valueField]);
+                let i = ve(t[o.settings.valueField]);
                 D(s, {
-                    "data-value": r
-                }), e === "item" ? (te(s, o.settings.itemClass), D(s, {
+                    "data-value": i
+                }), e === "item" ? (ee(s, o.settings.itemClass), D(s, {
                     "data-ts-item": ""
-                })) : (te(s, o.settings.optionClass), D(s, {
+                })) : (ee(s, o.settings.optionClass), D(s, {
                     role: "option",
                     id: t.$id
-                }), t.$div = s, o.options[r] = t)
+                }), t.$div = s, o.options[i] = t)
             }
             return s
         }
         _render(e, t) {
             let n = this.render(e, t);
             if (n == null) throw "HTMLElement expected";
             return n
         }
         clearCache() {
-            (0, ne.iterate)(this.options, e => {
+            (0, te.iterate)(this.options, e => {
                 e.$div && (e.$div.remove(), delete e.$div)
             })
         }
         uncacheValue(e) {
             let t = this.getOption(e);
             t && t.remove()
         }
         canCreate(e) {
             return this.settings.create && e.length > 0 && this.settings.createFilter.call(this, e)
         }
         hook(e, t, n) {
             var s = this,
                 o = s[t];
             s[t] = function() {
-                var r, p;
-                return e === "after" && (r = o.apply(s, arguments)), p = n.apply(s, arguments), e === "instead" ? p : (e === "before" && (r = o.apply(s, arguments)), r)
+                var i, f;
+                return e === "after" && (i = o.apply(s, arguments)), f = n.apply(s, arguments), e === "instead" ? f : (e === "before" && (i = o.apply(s, arguments)), i)
             }
         }
     };
 
-function Xe(i) {
-    let u = Object.assign({
+function et(r) {
+    let c = Object.assign({
         label: "&times;",
         title: "Remove",
         className: "remove",
         append: !0
-    }, i);
+    }, r);
     var e = this;
-    if (u.append) {
-        var t = '<a href="javascript:void(0)" class="' + u.className + '" tabindex="-1" title="' + de(u.title) + '">' + u.label + "</a>";
+    if (c.append) {
+        var t = '<a href="javascript:void(0)" class="' + c.className + '" tabindex="-1" title="' + de(c.title) + '">' + c.label + "</a>";
         e.hook("after", "setupTemplates", () => {
             var n = e.settings.render.item;
             e.settings.render.item = (s, o) => {
-                var r = ee(n.call(e, s, o)),
-                    p = ee(t);
-                return r.appendChild(p), G(p, "mousedown", m => {
-                    j(m, !0)
-                }), G(p, "click", m => {
-                    j(m, !0), !e.isLocked && e.shouldDelete([r], m) && (e.removeItem(r), e.refreshOptions(!1), e.inputState())
-                }), r
+                var i = Z(n.call(e, s, o)),
+                    f = Z(t);
+                return i.appendChild(f), Q(f, "mousedown", g => {
+                    j(g, !0)
+                }), Q(f, "click", g => {
+                    e.isLocked || (j(g, !0), !e.isLocked && e.shouldDelete([i], g) && (e.removeItem(i), e.refreshOptions(!1), e.inputState()))
+                }), i
             }
         })
     }
 }
-var nt = be(st());
-var Ze = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{--dummy-style: none}.ts-wrapper.disabled .ts-control{--dummy-style: none}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background-color:#f8f8f8;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable][aria-selected=true]{background-color:rgba(0,0,0,.05)}.ts-wrapper .ts-dropdown [data-selectable].selected{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
-pe.define("remove_button", Xe);
-var ke = class extends Re {
+var st = be(it());
+var tt = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{--dummy-style: none}.ts-wrapper.disabled .ts-control{--dummy-style: none}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background-color:#f8f8f8;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable][aria-selected=true]{background-color:rgba(0,0,0,.05)}.ts-wrapper .ts-dropdown [data-selectable].selected{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
+pe.define("remove_button", et);
+var Pe = class extends $e {
         constructor(e) {
             super(e);
+            this.extraStyleSheet = new CSSStyleSheet;
             this.numOptions = 12;
             this.baseSelector = ".ts-wrapper";
             this.getValue = () => this.currentValue;
             this.load = (e, t) => {
                 this.loadOptions(this.buildFetchQuery(0, e), n => {
                     t(n, this.extractOptGroups(n))
                 })
@@ -2012,15 +2041,15 @@
             let t = !1;
             e.hasAttribute("multiple") && (e.removeAttribute("multiple"), t = !0);
             let n = {
                 ...window.getComputedStyle(e)
             };
             t && e.setAttribute("multiple", "multiple"), this.numOptions = parseInt(e.getAttribute("options") ?? this.numOptions.toString()), this.tomSelect = new pe(e, this.getSettings()), this.observer = new MutationObserver(this.attributesChanged), this.observer.observe(this.tomInput, {
                 attributes: !0
-            }), this.initialValue = this.currentValue, this.shadowRoot = this.wrapInShadowRoot(), re.stylesAreInstalled(this.baseSelector) || this.transferStyles(e, n), e.classList.add("dj-concealed"), this.validateInput(this.initialValue), this.tomSelect.on("change", s => this.validateInput(s)), this.setupFilters(e)
+            }), this.initialValue = this.currentValue, this.shadowRoot = this.wrapInShadowRoot(), this.transferStyles(n), e.classList.add("dj-concealed"), this.validateInput(this.initialValue), this.tomSelect.on("change", s => this.validateInput(s)), this.setupFilters(e)
         }
         getSettings() {
             var n, s, o;
             let e = {
                     create: !1,
                     valueField: "id",
                     labelField: "label",
@@ -2038,40 +2067,40 @@
                     onFocus: this.touch,
                     onBlur: this.blurred,
                     onType: this.inputted
                 },
                 t = (n = this.tomInput.parentElement) == null ? void 0 : n.querySelector("template.select-no-results");
             if (t && (e.render = {
                     ...e.render,
-                    no_results: r => (0, nt.default)(t.innerHTML)(r)
+                    no_results: i => (0, st.default)(t.innerHTML)(i)
                 }), this.isIncomplete && (e.load = this.load), this.tomInput.hasAttribute("multiple")) {
                 e.maxItems = parseInt(this.tomInput.getAttribute("max_items") ?? "3");
-                let r = (s = this.tomInput.parentElement) == null ? void 0 : s.querySelector("template.selectize-remove-item");
+                let i = (s = this.tomInput.parentElement) == null ? void 0 : s.querySelector("template.selectize-remove-item");
                 e.plugins = {
                     ...e.plugins,
                     remove_button: {
-                        title: (r == null ? void 0 : r.innerHTML) ?? "Remove item"
+                        title: (i == null ? void 0 : i.innerHTML) ?? "Remove item"
                     }
                 };
-                let p = `${this.tomInput.getAttribute("id")}_initial`;
-                e.items = JSON.parse(((o = document.getElementById(p)) == null ? void 0 : o.textContent) ?? "[]")
+                let f = `${this.tomInput.getAttribute("id")}_initial`;
+                e.items = JSON.parse(((o = document.getElementById(f)) == null ? void 0 : o.textContent) ?? "[]")
             }
             return e
         }
         async formResetted(e) {
             this.getValue = () => this.initialValue, this.tomSelect.setValue(this.initialValue, !0), await this.reloadOptions(), this.getValue = () => this.currentValue
         }
         formSubmitted(e) {}
         async reloadOptions(e) {
             let t = this.getValue();
-            this.tomSelect.clear(!0), this.tomSelect.clearOptions(), this.tomInput.replaceChildren(), this.fieldGroup.classList.remove("dj-dirty", "dj-touched", "dj-validated"), this.fieldGroup.classList.add("dj-untouched", "dj-pristine");
+            this.tomSelect.clear(!0), this.fieldGroup.classList.remove("dj-dirty", "dj-touched", "dj-validated"), this.fieldGroup.classList.add("dj-untouched", "dj-pristine");
             let n = this.fieldGroup.querySelector(".dj-errorlist > .dj-placeholder");
-            n && (n.innerHTML = ""), await this.loadOptions(this.buildFetchQuery(0), s => {
+            n && (n.innerHTML = ""), this.isIncomplete && (this.tomSelect.clearOptions(), this.tomInput.replaceChildren(), await this.loadOptions(this.buildFetchQuery(0), s => {
                 this.tomSelect.addOptions(s)
-            }), this.tomSelect.setValue(t, e)
+            })), this.tomSelect.setValue(t, e)
         }
         get currentValue() {
             let e = this.tomSelect.getValue();
             return Array.isArray(e) ? [...e] : e
         }
         extractOptGroups(e) {
             let t = new Set;
@@ -2096,76 +2125,88 @@
             let e = document.createElement("div");
             e.classList.add("shadow-wrapper");
             let t = e.attachShadow({
                     mode: "open",
                     delegatesFocus: !0
                 }),
                 n = document.createElement("style");
-            t.appendChild(n).textContent = Ze, this.tomInput.insertAdjacentElement("beforebegin", e);
+            t.appendChild(n).textContent = tt, this.tomInput.insertAdjacentElement("beforebegin", e);
             let s = this.tomInput.parentElement.removeChild(this.tomSelect.wrapper);
             return t.appendChild(s), t
         }
-        transferStyles(e, t) {
-            let n = !1;
-            this.shadowRoot.host.style.setProperty("display", t.display);
-            let o = window.getComputedStyle(e).getPropertyValue("line-height"),
-                r = e.querySelector("option"),
-                p = this.shadowRoot.styleSheets.item(0),
-                m = Math.min(Math.max(this.numOptions, 8), 25);
-            for (let g = 0; p && g < p.cssRules.length; g++) {
-                let E = p.cssRules.item(g),
-                    y;
-                switch (E.selectorText) {
+        transferStyles(e) {
+            this.shadowRoot.host.style.setProperty("display", e.display);
+            let n = window.getComputedStyle(this.tomInput).getPropertyValue("line-height"),
+                s = this.tomInput.querySelector("option"),
+                o = this.shadowRoot.styleSheets.item(0),
+                i = Math.min(Math.max(this.numOptions, 8), 25),
+                f = !1;
+            for (let g = 0; o && g < o.cssRules.length; g++) {
+                let v = o.cssRules.item(g),
+                    E = null;
+                switch (v.selectorText) {
                     case this.baseSelector:
-                        y = re.extractStyles(e, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space"]), p.insertRule(`${E.selectorText}{${y}}`, ++g), n = !0;
+                        E = ie.extractStyles(this.tomInput, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space"]), f = !0;
                         break;
                     case `${this.baseSelector} .ts-control`:
-                        y = re.extractStyles(e, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${t.width}; min-height: ${t.height};`), p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        E = ie.extractStyles(this.tomInput, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${e.width}; min-height: ${e.height};`);
                         break;
                     case `${this.baseSelector} .ts-control > input`:
                     case `${this.baseSelector} .ts-control > div`:
-                        r && (y = re.extractStyles(r, ["padding-left", "padding-right"]), p.insertRule(`${E.selectorText}{${y}}`, ++g));
+                        s && (E = ie.extractStyles(s, ["padding-left", "padding-right"]));
                         break;
                     case `${this.baseSelector} .ts-control > input::placeholder`:
-                        e.classList.add("-placeholder-"), y = re.extractStyles(e, ["background-color", "color"]), e.classList.remove("-placeholder-"), p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        this.tomInput.classList.add("-placeholder-"), E = ie.extractStyles(this.tomInput, ["background-color", "color"]), this.tomInput.classList.remove("-placeholder-");
                         break;
                     case `${this.baseSelector}.focus .ts-control`:
-                        e.style.transition = "none", e.classList.add("-focus-"), y = re.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-"), p.insertRule(`${E.selectorText}{${y}}`, ++g), e.style.transition = "";
+                        this.tomInput.style.transition = "none", this.tomInput.classList.add("-focus-"), E = ie.extractStyles(this.tomInput, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), this.tomInput.classList.remove("-focus-"), this.tomInput.style.transition = "";
                         break;
                     case `${this.baseSelector}.disabled .ts-control`:
-                        e.classList.add("-disabled-"), y = re.extractStyles(e, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), e.classList.remove("-disabled-"), p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        this.tomInput.classList.add("-disabled-"), E = ie.extractStyles(this.tomInput, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), this.tomInput.classList.remove("-disabled-");
                         break;
                     case `${this.baseSelector} .ts-dropdown`:
-                        y = re.extractStyles(e, ["border-right", "border-bottom", "border-left", "color"]).concat(parseFloat(o) > 0 ? `line-height: calc(${o} * 1.2);` : "line-height: 1.4em;"), p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        E = ie.extractStyles(this.tomInput, ["border-right", "border-bottom", "border-left", "color"]).concat(parseFloat(n) > 0 ? `line-height: calc(${n} * 1.2);` : "line-height: 1.4em;");
                         break;
                     case `${this.baseSelector} .ts-dropdown .ts-dropdown-content`:
-                        parseFloat(o) > 0 ? y = `max-height: calc(${o} * 1.2 * ${m});` : y = `max-height: ${m*1.4}em;`, p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        parseFloat(n) > 0 ? E = `max-height: calc(${n} * 1.2 * ${i});` : E = `max-height: ${i*1.4}em;`;
                         break;
                     case `${this.baseSelector} .ts-dropdown [data-selectable]`:
-                        y = re.extractStyles(e, ["padding-left"]), p.insertRule(`${E.selectorText}{${y}}`, ++g);
+                        E = ie.extractStyles(this.tomInput, ["padding-left"]);
                         break;
                     case ':host-context([role="group"].dj-submitted) .ts-wrapper.invalid.focus .ts-control':
-                        e.style.transition = "none", e.classList.add("-focus-", "-invalid-", "is-invalid"), y = re.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-", "-invalid-", "is-invalid"), p.insertRule(`${E.selectorText}{${y}}`, ++g), e.style.transition = "";
+                        this.tomInput.style.transition = "none", this.tomInput.classList.add("-focus-", "-invalid-", "is-invalid"), E = ie.extractStyles(this.tomInput, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), this.tomInput.classList.remove("-focus-", "-invalid-", "is-invalid"), this.tomInput.style.transition = "";
                         break;
                     default:
                         break
                 }
+                E && this.extraStyleSheet.insertRule(`${v.selectorText}{${E}}`)
+            }
+            if (!f) throw new Error(`Could not load styles for ${this.baseSelector}`)
+        }
+        initialize() {
+            let e = this.shadowRoot.styleSheets.item(0);
+            for (let t = 0; t < this.extraStyleSheet.cssRules.length; t++) {
+                let n = this.extraStyleSheet.cssRules.item(t);
+                e.insertRule(n.cssText)
             }
-            if (!n) throw new Error(`Could not load styles for ${this.baseSelector}`)
         }
     },
-    et = Symbol("DjangoSelectize"),
-    tt = class extends HTMLSelectElement {
+    He = Symbol("DjangoSelectize"),
+    nt = class extends HTMLSelectElement {
+        constructor() {
+            super();
+            this[He] = new Pe(this)
+        }
         connectedCallback() {
-            "tomselect" in this || (this[et] = new ke(this))
+            this[He].initialize()
         }
     };
-et;
+He;
 export {
-    ke as a, tt as b
+    Pe as a, nt as b
 };
 /*! Bundled license information:
 
 @orchidjs/sifter/dist/umd/sifter.js:
   (*! sifter.js | https://github.com/orchidjs/sifter.js | Apache License (v2) *)
   (*! @orchidjs/unicode-variants | https://github.com/orchidjs/unicode-variants | Apache License (v2) *)
```

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-LTR6QAFN.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-LVGJ2KIX.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-P2VM2T3G.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-P2VM2T3G.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-SERXULES.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-SERXULES.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/chunk-W5RPWA2M.js` & `django-formset-1.3.9/formset/static/formset/js/chunk-W5RPWA2M.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/static/formset/js/django-formset.js` & `django-formset-1.3.9/formset/static/formset/js/django-formset.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1468 +1,1468 @@
 import {
-    a as Ar
+    a as _r
 } from "./chunk-W5RPWA2M.js";
 import {
-    b as kr
+    b as Fr
 } from "./chunk-7MZNI2NE.js";
 import {
-    a as wr
+    a as Cr
 } from "./chunk-FDUUONAQ.js";
 import {
-    a as Cr
+    a as Ze
 } from "./chunk-65OJRBX6.js";
 import {
-    a as Ze,
-    b as he
+    a as Qe,
+    b as be
 } from "./chunk-P2VM2T3G.js";
-var Br = Ze((Dl, Rr) => {
-    var Eo = "Expected a function",
-        Lr = "__lodash_hash_undefined__",
-        $r = 1 / 0,
-        wo = "[object Function]",
-        ko = "[object GeneratorFunction]",
-        Ao = "[object Symbol]",
+var Vr = Qe((Dl, Nr) => {
+    var wo = "Expected a function",
+        Mr = "__lodash_hash_undefined__",
+        Pr = 1 / 0,
+        ko = "[object Function]",
+        Ao = "[object GeneratorFunction]",
+        To = "[object Symbol]",
         Co = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        To = /^\w*$/,
-        Fo = /^\./,
-        _o = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        So = /[\\^$.*+?()[\]{}|]/g,
+        Fo = /^\w*$/,
+        _o = /^\./,
+        So = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
+        $o = /[\\^$.*+?()[\]{}|]/g,
         Lo = /\\(\\)?/g,
-        $o = /^\[object .+?Constructor\]$/,
-        Io = typeof global == "object" && global && global.Object === Object && global,
-        Mo = typeof self == "object" && self && self.Object === Object && self,
-        _t = Io || Mo || Function("return this")();
+        Io = /^\[object .+?Constructor\]$/,
+        Mo = typeof global == "object" && global && global.Object === Object && global,
+        Po = typeof self == "object" && self && self.Object === Object && self,
+        $t = Mo || Po || Function("return this")();
 
-    function Po(t, e) {
+    function Oo(t, e) {
         return t == null ? void 0 : t[e]
     }
 
     function Do(t) {
         var e = !1;
         if (t != null && typeof t.toString != "function") try {
             e = !!(t + "")
         } catch {}
         return e
     }
-    var Oo = Array.prototype,
-        Ho = Function.prototype,
-        Ir = Object.prototype,
-        Ft = _t["__core-js_shared__"],
-        Tr = function() {
-            var t = /[^.]+$/.exec(Ft && Ft.keys && Ft.keys.IE_PROTO || "");
+    var Ho = Array.prototype,
+        Ro = Function.prototype,
+        Or = Object.prototype,
+        St = $t["__core-js_shared__"],
+        Sr = function() {
+            var t = /[^.]+$/.exec(St && St.keys && St.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        Mr = Ho.toString,
-        St = Ir.hasOwnProperty,
-        Pr = Ir.toString,
-        Ro = RegExp("^" + Mr.call(St).replace(So, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        Fr = _t.Symbol,
-        Bo = Oo.splice,
-        qo = Dr(_t, "Map"),
-        Se = Dr(Object, "create"),
-        _r = Fr ? Fr.prototype : void 0,
-        Sr = _r ? _r.toString : void 0;
+        Dr = Ro.toString,
+        Lt = Or.hasOwnProperty,
+        Hr = Or.toString,
+        Bo = RegExp("^" + Dr.call(Lt).replace($o, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        $r = $t.Symbol,
+        qo = Ho.splice,
+        No = Rr($t, "Map"),
+        Se = Rr(Object, "create"),
+        Lr = $r ? $r.prototype : void 0,
+        Ir = Lr ? Lr.toString : void 0;
 
     function te(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function No() {
+    function Vo() {
         this.__data__ = Se ? Se(null) : {}
     }
 
-    function Vo(t) {
+    function Go(t) {
         return this.has(t) && delete this.__data__[t]
     }
 
-    function Go(t) {
+    function zo(t) {
         var e = this.__data__;
         if (Se) {
             var r = e[t];
-            return r === Lr ? void 0 : r
+            return r === Mr ? void 0 : r
         }
-        return St.call(e, t) ? e[t] : void 0
+        return Lt.call(e, t) ? e[t] : void 0
     }
 
-    function zo(t) {
+    function Uo(t) {
         var e = this.__data__;
-        return Se ? e[t] !== void 0 : St.call(e, t)
+        return Se ? e[t] !== void 0 : Lt.call(e, t)
     }
 
-    function Uo(t, e) {
+    function Xo(t, e) {
         var r = this.__data__;
-        return r[t] = Se && e === void 0 ? Lr : e, this
+        return r[t] = Se && e === void 0 ? Mr : e, this
     }
-    te.prototype.clear = No;
-    te.prototype.delete = Vo;
-    te.prototype.get = Go;
-    te.prototype.has = zo;
-    te.prototype.set = Uo;
+    te.prototype.clear = Vo;
+    te.prototype.delete = Go;
+    te.prototype.get = zo;
+    te.prototype.has = Uo;
+    te.prototype.set = Xo;
 
-    function be(t) {
+    function je(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
     function Ko() {
         this.__data__ = []
     }
 
-    function Jo(t) {
+    function Yo(t) {
         var e = this.__data__,
-            r = Ye(e, t);
+            r = We(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : Bo.call(e, r, 1), !0
+        return r == n ? e.pop() : qo.call(e, r, 1), !0
     }
 
-    function Wo(t) {
+    function Jo(t) {
         var e = this.__data__,
-            r = Ye(e, t);
+            r = We(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function Xo(t) {
-        return Ye(this.__data__, t) > -1
+    function Qo(t) {
+        return We(this.__data__, t) > -1
     }
 
     function Zo(t, e) {
         var r = this.__data__,
-            n = Ye(r, t);
+            n = We(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    be.prototype.clear = Ko;
-    be.prototype.delete = Jo;
-    be.prototype.get = Wo;
-    be.prototype.has = Xo;
-    be.prototype.set = Zo;
+    je.prototype.clear = Ko;
+    je.prototype.delete = Yo;
+    je.prototype.get = Jo;
+    je.prototype.has = Qo;
+    je.prototype.set = Zo;
 
     function re(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function Yo() {
+    function Wo() {
         this.__data__ = {
             hash: new te,
-            map: new(qo || be),
+            map: new(No || je),
             string: new te
         }
     }
 
-    function Qo(t) {
-        return Qe(this, t).delete(t)
-    }
-
     function ei(t) {
-        return Qe(this, t).get(t)
+        return et(this, t).delete(t)
     }
 
     function ti(t) {
-        return Qe(this, t).has(t)
+        return et(this, t).get(t)
     }
 
-    function ri(t, e) {
-        return Qe(this, t).set(t, e), this
+    function ri(t) {
+        return et(this, t).has(t)
+    }
+
+    function ni(t, e) {
+        return et(this, t).set(t, e), this
     }
-    re.prototype.clear = Yo;
-    re.prototype.delete = Qo;
-    re.prototype.get = ei;
-    re.prototype.has = ti;
-    re.prototype.set = ri;
+    re.prototype.clear = Wo;
+    re.prototype.delete = ei;
+    re.prototype.get = ti;
+    re.prototype.has = ri;
+    re.prototype.set = ni;
 
-    function Ye(t, e) {
+    function We(t, e) {
         for (var r = t.length; r--;)
-            if (pi(t[r][0], e)) return r;
+            if (mi(t[r][0], e)) return r;
         return -1
     }
 
-    function ni(t, e) {
-        e = si(e, t) ? [e] : ai(e);
-        for (var r = 0, n = e.length; t != null && r < n;) t = t[ui(e[r++])];
+    function oi(t, e) {
+        e = li(e, t) ? [e] : si(e);
+        for (var r = 0, n = e.length; t != null && r < n;) t = t[fi(e[r++])];
         return r && r == n ? t : void 0
     }
 
-    function oi(t) {
-        if (!Hr(t) || di(t)) return !1;
-        var e = mi(t) || Do(t) ? Ro : $o;
-        return e.test(fi(t))
+    function ii(t) {
+        if (!qr(t) || ci(t)) return !1;
+        var e = gi(t) || Do(t) ? Bo : Io;
+        return e.test(pi(t))
     }
 
-    function ii(t) {
+    function ai(t) {
         if (typeof t == "string") return t;
-        if ($t(t)) return Sr ? Sr.call(t) : "";
+        if (Mt(t)) return Ir ? Ir.call(t) : "";
         var e = t + "";
-        return e == "0" && 1 / t == -$r ? "-0" : e
+        return e == "0" && 1 / t == -Pr ? "-0" : e
     }
 
-    function ai(t) {
-        return Or(t) ? t : ci(t)
+    function si(t) {
+        return Br(t) ? t : ui(t)
     }
 
-    function Qe(t, e) {
+    function et(t, e) {
         var r = t.__data__;
-        return li(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return di(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function Dr(t, e) {
-        var r = Po(t, e);
-        return oi(r) ? r : void 0
+    function Rr(t, e) {
+        var r = Oo(t, e);
+        return ii(r) ? r : void 0
     }
 
-    function si(t, e) {
-        if (Or(t)) return !1;
+    function li(t, e) {
+        if (Br(t)) return !1;
         var r = typeof t;
-        return r == "number" || r == "symbol" || r == "boolean" || t == null || $t(t) ? !0 : To.test(t) || !Co.test(t) || e != null && t in Object(e)
+        return r == "number" || r == "symbol" || r == "boolean" || t == null || Mt(t) ? !0 : Fo.test(t) || !Co.test(t) || e != null && t in Object(e)
     }
 
-    function li(t) {
+    function di(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function di(t) {
-        return !!Tr && Tr in t
+    function ci(t) {
+        return !!Sr && Sr in t
     }
-    var ci = Lt(function(t) {
-        t = hi(t);
+    var ui = It(function(t) {
+        t = bi(t);
         var e = [];
-        return Fo.test(t) && e.push(""), t.replace(_o, function(r, n, i, o) {
+        return _o.test(t) && e.push(""), t.replace(So, function(r, n, i, o) {
             e.push(i ? o.replace(Lo, "$1") : n || r)
         }), e
     });
 
-    function ui(t) {
-        if (typeof t == "string" || $t(t)) return t;
+    function fi(t) {
+        if (typeof t == "string" || Mt(t)) return t;
         var e = t + "";
-        return e == "0" && 1 / t == -$r ? "-0" : e
+        return e == "0" && 1 / t == -Pr ? "-0" : e
     }
 
-    function fi(t) {
+    function pi(t) {
         if (t != null) {
             try {
-                return Mr.call(t)
+                return Dr.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function Lt(t, e) {
-        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(Eo);
+    function It(t, e) {
+        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(wo);
         var r = function() {
             var n = arguments,
                 i = e ? e.apply(this, n) : n[0],
                 o = r.cache;
             if (o.has(i)) return o.get(i);
-            var l = t.apply(this, n);
-            return r.cache = o.set(i, l), l
+            var a = t.apply(this, n);
+            return r.cache = o.set(i, a), a
         };
-        return r.cache = new(Lt.Cache || re), r
+        return r.cache = new(It.Cache || re), r
     }
-    Lt.Cache = re;
+    It.Cache = re;
 
-    function pi(t, e) {
+    function mi(t, e) {
         return t === e || t !== t && e !== e
     }
-    var Or = Array.isArray;
+    var Br = Array.isArray;
 
-    function mi(t) {
-        var e = Hr(t) ? Pr.call(t) : "";
-        return e == wo || e == ko
+    function gi(t) {
+        var e = qr(t) ? Hr.call(t) : "";
+        return e == ko || e == Ao
     }
 
-    function Hr(t) {
+    function qr(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
-    function gi(t) {
+    function hi(t) {
         return !!t && typeof t == "object"
     }
 
-    function $t(t) {
-        return typeof t == "symbol" || gi(t) && Pr.call(t) == Ao
+    function Mt(t) {
+        return typeof t == "symbol" || hi(t) && Hr.call(t) == To
     }
 
-    function hi(t) {
-        return t == null ? "" : ii(t)
+    function bi(t) {
+        return t == null ? "" : ai(t)
     }
 
-    function bi(t, e, r) {
-        var n = t == null ? void 0 : ni(t, e);
+    function ji(t, e, r) {
+        var n = t == null ? void 0 : oi(t, e);
         return n === void 0 ? r : n
     }
-    Rr.exports = bi
+    Nr.exports = ji
 });
-var en = Ze((Ol, Qr) => {
-    var ji = "Expected a function",
-        zr = "__lodash_hash_undefined__",
-        Ur = 1 / 0,
-        yi = 9007199254740991,
-        vi = "[object Function]",
-        xi = "[object GeneratorFunction]",
-        Ei = "[object Symbol]",
-        wi = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        ki = /^\w*$/,
-        Ai = /^\./,
+var nn = Qe((Hl, rn) => {
+    var yi = "Expected a function",
+        Kr = "__lodash_hash_undefined__",
+        Yr = 1 / 0,
+        vi = 9007199254740991,
+        xi = "[object Function]",
+        Ei = "[object GeneratorFunction]",
+        wi = "[object Symbol]",
+        ki = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+        Ai = /^\w*$/,
+        Ti = /^\./,
         Ci = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        Ti = /[\\^$.*+?()[\]{}|]/g,
-        Fi = /\\(\\)?/g,
-        _i = /^\[object .+?Constructor\]$/,
-        Si = /^(?:0|[1-9]\d*)$/,
+        Fi = /[\\^$.*+?()[\]{}|]/g,
+        _i = /\\(\\)?/g,
+        Si = /^\[object .+?Constructor\]$/,
+        $i = /^(?:0|[1-9]\d*)$/,
         Li = typeof global == "object" && global && global.Object === Object && global,
-        $i = typeof self == "object" && self && self.Object === Object && self,
-        Mt = Li || $i || Function("return this")();
+        Ii = typeof self == "object" && self && self.Object === Object && self,
+        Ot = Li || Ii || Function("return this")();
 
-    function Ii(t, e) {
+    function Mi(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function Mi(t) {
+    function Pi(t) {
         var e = !1;
         if (t != null && typeof t.toString != "function") try {
             e = !!(t + "")
         } catch {}
         return e
     }
-    var Pi = Array.prototype,
+    var Oi = Array.prototype,
         Di = Function.prototype,
-        Kr = Object.prototype,
-        It = Mt["__core-js_shared__"],
-        qr = function() {
-            var t = /[^.]+$/.exec(It && It.keys && It.keys.IE_PROTO || "");
+        Jr = Object.prototype,
+        Pt = Ot["__core-js_shared__"],
+        Gr = function() {
+            var t = /[^.]+$/.exec(Pt && Pt.keys && Pt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        Jr = Di.toString,
-        tt = Kr.hasOwnProperty,
-        Wr = Kr.toString,
-        Oi = RegExp("^" + Jr.call(tt).replace(Ti, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        Nr = Mt.Symbol,
-        Hi = Pi.splice,
-        Ri = Xr(Mt, "Map"),
-        Le = Xr(Object, "create"),
-        Vr = Nr ? Nr.prototype : void 0,
-        Gr = Vr ? Vr.toString : void 0;
+        Qr = Di.toString,
+        rt = Jr.hasOwnProperty,
+        Zr = Jr.toString,
+        Hi = RegExp("^" + Qr.call(rt).replace(Fi, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        zr = Ot.Symbol,
+        Ri = Oi.splice,
+        Bi = Wr(Ot, "Map"),
+        $e = Wr(Object, "create"),
+        Ur = zr ? zr.prototype : void 0,
+        Xr = Ur ? Ur.toString : void 0;
 
     function ne(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function Bi() {
-        this.__data__ = Le ? Le(null) : {}
+    function qi() {
+        this.__data__ = $e ? $e(null) : {}
     }
 
-    function qi(t) {
+    function Ni(t) {
         return this.has(t) && delete this.__data__[t]
     }
 
-    function Ni(t) {
+    function Vi(t) {
         var e = this.__data__;
-        if (Le) {
+        if ($e) {
             var r = e[t];
-            return r === zr ? void 0 : r
+            return r === Kr ? void 0 : r
         }
-        return tt.call(e, t) ? e[t] : void 0
+        return rt.call(e, t) ? e[t] : void 0
     }
 
-    function Vi(t) {
+    function Gi(t) {
         var e = this.__data__;
-        return Le ? e[t] !== void 0 : tt.call(e, t)
+        return $e ? e[t] !== void 0 : rt.call(e, t)
     }
 
-    function Gi(t, e) {
+    function zi(t, e) {
         var r = this.__data__;
-        return r[t] = Le && e === void 0 ? zr : e, this
+        return r[t] = $e && e === void 0 ? Kr : e, this
     }
-    ne.prototype.clear = Bi;
-    ne.prototype.delete = qi;
-    ne.prototype.get = Ni;
-    ne.prototype.has = Vi;
-    ne.prototype.set = Gi;
+    ne.prototype.clear = qi;
+    ne.prototype.delete = Ni;
+    ne.prototype.get = Vi;
+    ne.prototype.has = Gi;
+    ne.prototype.set = zi;
 
-    function je(t) {
+    function ye(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function zi() {
+    function Ui() {
         this.__data__ = []
     }
 
-    function Ui(t) {
+    function Xi(t) {
         var e = this.__data__,
-            r = rt(e, t);
+            r = nt(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : Hi.call(e, r, 1), !0
+        return r == n ? e.pop() : Ri.call(e, r, 1), !0
     }
 
     function Ki(t) {
         var e = this.__data__,
-            r = rt(e, t);
+            r = nt(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function Ji(t) {
-        return rt(this.__data__, t) > -1
+    function Yi(t) {
+        return nt(this.__data__, t) > -1
     }
 
-    function Wi(t, e) {
+    function Ji(t, e) {
         var r = this.__data__,
-            n = rt(r, t);
+            n = nt(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    je.prototype.clear = zi;
-    je.prototype.delete = Ui;
-    je.prototype.get = Ki;
-    je.prototype.has = Ji;
-    je.prototype.set = Wi;
+    ye.prototype.clear = Ui;
+    ye.prototype.delete = Xi;
+    ye.prototype.get = Ki;
+    ye.prototype.has = Yi;
+    ye.prototype.set = Ji;
 
     function oe(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function Xi() {
+    function Qi() {
         this.__data__ = {
             hash: new ne,
-            map: new(Ri || je),
+            map: new(Bi || ye),
             string: new ne
         }
     }
 
     function Zi(t) {
-        return nt(this, t).delete(t)
+        return ot(this, t).delete(t)
     }
 
-    function Yi(t) {
-        return nt(this, t).get(t)
+    function Wi(t) {
+        return ot(this, t).get(t)
     }
 
-    function Qi(t) {
-        return nt(this, t).has(t)
+    function ea(t) {
+        return ot(this, t).has(t)
     }
 
-    function ea(t, e) {
-        return nt(this, t).set(t, e), this
+    function ta(t, e) {
+        return ot(this, t).set(t, e), this
     }
-    oe.prototype.clear = Xi;
+    oe.prototype.clear = Qi;
     oe.prototype.delete = Zi;
-    oe.prototype.get = Yi;
-    oe.prototype.has = Qi;
-    oe.prototype.set = ea;
+    oe.prototype.get = Wi;
+    oe.prototype.has = ea;
+    oe.prototype.set = ta;
 
-    function ta(t, e, r) {
+    function ra(t, e, r) {
         var n = t[e];
-        (!(tt.call(t, e) && Zr(n, r)) || r === void 0 && !(e in t)) && (t[e] = r)
+        (!(rt.call(t, e) && en(n, r)) || r === void 0 && !(e in t)) && (t[e] = r)
     }
 
-    function rt(t, e) {
+    function nt(t, e) {
         for (var r = t.length; r--;)
-            if (Zr(t[r][0], e)) return r;
+            if (en(t[r][0], e)) return r;
         return -1
     }
 
-    function ra(t) {
-        if (!et(t) || da(t)) return !1;
-        var e = pa(t) || Mi(t) ? Oi : _i;
-        return e.test(fa(t))
-    }
-
-    function na(t, e, r, n) {
-        if (!et(t)) return t;
-        e = sa(e, t) ? [e] : ia(e);
-        for (var i = -1, o = e.length, l = o - 1, c = t; c != null && ++i < o;) {
-            var u = ua(e[i]),
-                a = r;
-            if (i != l) {
-                var m = c[u];
-                a = n ? n(m, u, c) : void 0, a === void 0 && (a = et(m) ? m : aa(e[i + 1]) ? [] : {})
+    function na(t) {
+        if (!tt(t) || ca(t)) return !1;
+        var e = ma(t) || Pi(t) ? Hi : Si;
+        return e.test(pa(t))
+    }
+
+    function oa(t, e, r, n) {
+        if (!tt(t)) return t;
+        e = la(e, t) ? [e] : aa(e);
+        for (var i = -1, o = e.length, a = o - 1, c = t; c != null && ++i < o;) {
+            var u = fa(e[i]),
+                s = r;
+            if (i != a) {
+                var p = c[u];
+                s = n ? n(p, u, c) : void 0, s === void 0 && (s = tt(p) ? p : sa(e[i + 1]) ? [] : {})
             }
-            ta(c, u, a), c = c[u]
+            ra(c, u, s), c = c[u]
         }
         return t
     }
 
-    function oa(t) {
+    function ia(t) {
         if (typeof t == "string") return t;
-        if (Dt(t)) return Gr ? Gr.call(t) : "";
+        if (Ht(t)) return Xr ? Xr.call(t) : "";
         var e = t + "";
-        return e == "0" && 1 / t == -Ur ? "-0" : e
+        return e == "0" && 1 / t == -Yr ? "-0" : e
     }
 
-    function ia(t) {
-        return Yr(t) ? t : ca(t)
+    function aa(t) {
+        return tn(t) ? t : ua(t)
     }
 
-    function nt(t, e) {
+    function ot(t, e) {
         var r = t.__data__;
-        return la(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return da(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function Xr(t, e) {
-        var r = Ii(t, e);
-        return ra(r) ? r : void 0
+    function Wr(t, e) {
+        var r = Mi(t, e);
+        return na(r) ? r : void 0
     }
 
-    function aa(t, e) {
-        return e = e ?? yi, !!e && (typeof t == "number" || Si.test(t)) && t > -1 && t % 1 == 0 && t < e
+    function sa(t, e) {
+        return e = e ?? vi, !!e && (typeof t == "number" || $i.test(t)) && t > -1 && t % 1 == 0 && t < e
     }
 
-    function sa(t, e) {
-        if (Yr(t)) return !1;
+    function la(t, e) {
+        if (tn(t)) return !1;
         var r = typeof t;
-        return r == "number" || r == "symbol" || r == "boolean" || t == null || Dt(t) ? !0 : ki.test(t) || !wi.test(t) || e != null && t in Object(e)
+        return r == "number" || r == "symbol" || r == "boolean" || t == null || Ht(t) ? !0 : Ai.test(t) || !ki.test(t) || e != null && t in Object(e)
     }
 
-    function la(t) {
+    function da(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function da(t) {
-        return !!qr && qr in t
+    function ca(t) {
+        return !!Gr && Gr in t
     }
-    var ca = Pt(function(t) {
-        t = ga(t);
+    var ua = Dt(function(t) {
+        t = ha(t);
         var e = [];
-        return Ai.test(t) && e.push(""), t.replace(Ci, function(r, n, i, o) {
-            e.push(i ? o.replace(Fi, "$1") : n || r)
+        return Ti.test(t) && e.push(""), t.replace(Ci, function(r, n, i, o) {
+            e.push(i ? o.replace(_i, "$1") : n || r)
         }), e
     });
 
-    function ua(t) {
-        if (typeof t == "string" || Dt(t)) return t;
+    function fa(t) {
+        if (typeof t == "string" || Ht(t)) return t;
         var e = t + "";
-        return e == "0" && 1 / t == -Ur ? "-0" : e
+        return e == "0" && 1 / t == -Yr ? "-0" : e
     }
 
-    function fa(t) {
+    function pa(t) {
         if (t != null) {
             try {
-                return Jr.call(t)
+                return Qr.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function Pt(t, e) {
-        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(ji);
+    function Dt(t, e) {
+        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(yi);
         var r = function() {
             var n = arguments,
                 i = e ? e.apply(this, n) : n[0],
                 o = r.cache;
             if (o.has(i)) return o.get(i);
-            var l = t.apply(this, n);
-            return r.cache = o.set(i, l), l
+            var a = t.apply(this, n);
+            return r.cache = o.set(i, a), a
         };
-        return r.cache = new(Pt.Cache || oe), r
+        return r.cache = new(Dt.Cache || oe), r
     }
-    Pt.Cache = oe;
+    Dt.Cache = oe;
 
-    function Zr(t, e) {
+    function en(t, e) {
         return t === e || t !== t && e !== e
     }
-    var Yr = Array.isArray;
+    var tn = Array.isArray;
 
-    function pa(t) {
-        var e = et(t) ? Wr.call(t) : "";
-        return e == vi || e == xi
+    function ma(t) {
+        var e = tt(t) ? Zr.call(t) : "";
+        return e == xi || e == Ei
     }
 
-    function et(t) {
+    function tt(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
-    function ma(t) {
+    function ga(t) {
         return !!t && typeof t == "object"
     }
 
-    function Dt(t) {
-        return typeof t == "symbol" || ma(t) && Wr.call(t) == Ei
+    function Ht(t) {
+        return typeof t == "symbol" || ga(t) && Zr.call(t) == wi
     }
 
-    function ga(t) {
-        return t == null ? "" : oa(t)
+    function ha(t) {
+        return t == null ? "" : ia(t)
     }
 
-    function ha(t, e, r) {
-        return t == null ? t : na(t, e, r)
+    function ba(t, e, r) {
+        return t == null ? t : oa(t, e, r)
     }
-    Qr.exports = ha
+    rn.exports = ba
 });
-var Dn = Ze(($e, ve) => {
-    var ba = 200,
-        Kt = "__lodash_hash_undefined__",
-        ut = 1,
-        pn = 2,
-        mn = 9007199254740991,
-        ot = "[object Arguments]",
-        Bt = "[object Array]",
-        ja = "[object AsyncFunction]",
-        gn = "[object Boolean]",
-        hn = "[object Date]",
-        bn = "[object Error]",
-        jn = "[object Function]",
-        ya = "[object GeneratorFunction]",
-        it = "[object Map]",
-        yn = "[object Number]",
-        va = "[object Null]",
-        ye = "[object Object]",
-        tn = "[object Promise]",
-        xa = "[object Proxy]",
-        vn = "[object RegExp]",
-        at = "[object Set]",
-        xn = "[object String]",
-        Ea = "[object Symbol]",
-        wa = "[object Undefined]",
-        qt = "[object WeakMap]",
-        En = "[object ArrayBuffer]",
-        st = "[object DataView]",
-        ka = "[object Float32Array]",
-        Aa = "[object Float64Array]",
+var Rn = Qe((Le, xe) => {
+    var ja = 200,
+        Yt = "__lodash_hash_undefined__",
+        ft = 1,
+        hn = 2,
+        bn = 9007199254740991,
+        it = "[object Arguments]",
+        Nt = "[object Array]",
+        ya = "[object AsyncFunction]",
+        jn = "[object Boolean]",
+        yn = "[object Date]",
+        vn = "[object Error]",
+        xn = "[object Function]",
+        va = "[object GeneratorFunction]",
+        at = "[object Map]",
+        En = "[object Number]",
+        xa = "[object Null]",
+        ve = "[object Object]",
+        on = "[object Promise]",
+        Ea = "[object Proxy]",
+        wn = "[object RegExp]",
+        st = "[object Set]",
+        kn = "[object String]",
+        wa = "[object Symbol]",
+        ka = "[object Undefined]",
+        Vt = "[object WeakMap]",
+        An = "[object ArrayBuffer]",
+        lt = "[object DataView]",
+        Aa = "[object Float32Array]",
+        Ta = "[object Float64Array]",
         Ca = "[object Int8Array]",
-        Ta = "[object Int16Array]",
-        Fa = "[object Int32Array]",
-        _a = "[object Uint8Array]",
-        Sa = "[object Uint8ClampedArray]",
+        Fa = "[object Int16Array]",
+        _a = "[object Int32Array]",
+        Sa = "[object Uint8Array]",
+        $a = "[object Uint8ClampedArray]",
         La = "[object Uint16Array]",
-        $a = "[object Uint32Array]",
-        Ia = /[\\^$.*+?()[\]{}|]/g,
-        Ma = /^\[object .+?Constructor\]$/,
-        Pa = /^(?:0|[1-9]\d*)$/,
+        Ia = "[object Uint32Array]",
+        Ma = /[\\^$.*+?()[\]{}|]/g,
+        Pa = /^\[object .+?Constructor\]$/,
+        Oa = /^(?:0|[1-9]\d*)$/,
         S = {};
-    S[ka] = S[Aa] = S[Ca] = S[Ta] = S[Fa] = S[_a] = S[Sa] = S[La] = S[$a] = !0;
-    S[ot] = S[Bt] = S[En] = S[gn] = S[st] = S[hn] = S[bn] = S[jn] = S[it] = S[yn] = S[ye] = S[vn] = S[at] = S[xn] = S[qt] = !1;
-    var wn = typeof global == "object" && global && global.Object === Object && global,
+    S[Aa] = S[Ta] = S[Ca] = S[Fa] = S[_a] = S[Sa] = S[$a] = S[La] = S[Ia] = !0;
+    S[it] = S[Nt] = S[An] = S[jn] = S[lt] = S[yn] = S[vn] = S[xn] = S[at] = S[En] = S[ve] = S[wn] = S[st] = S[kn] = S[Vt] = !1;
+    var Tn = typeof global == "object" && global && global.Object === Object && global,
         Da = typeof self == "object" && self && self.Object === Object && self,
-        J = wn || Da || Function("return this")(),
-        kn = typeof $e == "object" && $e && !$e.nodeType && $e,
-        rn = kn && typeof ve == "object" && ve && !ve.nodeType && ve,
-        An = rn && rn.exports === kn,
-        Ot = An && wn.process,
-        nn = function() {
+        K = Tn || Da || Function("return this")(),
+        Cn = typeof Le == "object" && Le && !Le.nodeType && Le,
+        an = Cn && typeof xe == "object" && xe && !xe.nodeType && xe,
+        Fn = an && an.exports === Cn,
+        Rt = Fn && Tn.process,
+        sn = function() {
             try {
-                return Ot && Ot.binding && Ot.binding("util")
+                return Rt && Rt.binding && Rt.binding("util")
             } catch {}
         }(),
-        on = nn && nn.isTypedArray;
+        ln = sn && sn.isTypedArray;
 
-    function Oa(t, e) {
+    function Ha(t, e) {
         for (var r = -1, n = t == null ? 0 : t.length, i = 0, o = []; ++r < n;) {
-            var l = t[r];
-            e(l, r, t) && (o[i++] = l)
+            var a = t[r];
+            e(a, r, t) && (o[i++] = a)
         }
         return o
     }
 
-    function Ha(t, e) {
+    function Ra(t, e) {
         for (var r = -1, n = e.length, i = t.length; ++r < n;) t[i + r] = e[r];
         return t
     }
 
-    function Ra(t, e) {
+    function Ba(t, e) {
         for (var r = -1, n = t == null ? 0 : t.length; ++r < n;)
             if (e(t[r], r, t)) return !0;
         return !1
     }
 
-    function Ba(t, e) {
+    function qa(t, e) {
         for (var r = -1, n = Array(t); ++r < t;) n[r] = e(r);
         return n
     }
 
-    function qa(t) {
+    function Na(t) {
         return function(e) {
             return t(e)
         }
     }
 
-    function Na(t, e) {
+    function Va(t, e) {
         return t.has(e)
     }
 
-    function Va(t, e) {
+    function Ga(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function Ga(t) {
+    function za(t) {
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n, i) {
             r[++e] = [i, n]
         }), r
     }
 
-    function za(t, e) {
+    function Ua(t, e) {
         return function(r) {
             return t(e(r))
         }
     }
 
-    function Ua(t) {
+    function Xa(t) {
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n) {
             r[++e] = n
         }), r
     }
     var Ka = Array.prototype,
-        Ja = Function.prototype,
-        ft = Object.prototype,
-        Ht = J["__core-js_shared__"],
-        Cn = Ja.toString,
-        U = ft.hasOwnProperty,
-        an = function() {
-            var t = /[^.]+$/.exec(Ht && Ht.keys && Ht.keys.IE_PROTO || "");
+        Ya = Function.prototype,
+        pt = Object.prototype,
+        Bt = K["__core-js_shared__"],
+        _n = Ya.toString,
+        U = pt.hasOwnProperty,
+        dn = function() {
+            var t = /[^.]+$/.exec(Bt && Bt.keys && Bt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        Tn = ft.toString,
-        Wa = RegExp("^" + Cn.call(U).replace(Ia, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        sn = An ? J.Buffer : void 0,
-        lt = J.Symbol,
-        ln = J.Uint8Array,
-        Fn = ft.propertyIsEnumerable,
-        Xa = Ka.splice,
-        ie = lt ? lt.toStringTag : void 0,
-        dn = Object.getOwnPropertySymbols,
-        Za = sn ? sn.isBuffer : void 0,
-        Ya = za(Object.keys, Object),
-        Nt = xe(J, "DataView"),
-        Ie = xe(J, "Map"),
-        Vt = xe(J, "Promise"),
-        Gt = xe(J, "Set"),
-        zt = xe(J, "WeakMap"),
-        Me = xe(Object, "create"),
-        Qa = le(Nt),
-        es = le(Ie),
-        ts = le(Vt),
-        rs = le(Gt),
-        ns = le(zt),
-        cn = lt ? lt.prototype : void 0,
-        Rt = cn ? cn.valueOf : void 0;
+        Sn = pt.toString,
+        Ja = RegExp("^" + _n.call(U).replace(Ma, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        cn = Fn ? K.Buffer : void 0,
+        dt = K.Symbol,
+        un = K.Uint8Array,
+        $n = pt.propertyIsEnumerable,
+        Qa = Ka.splice,
+        ie = dt ? dt.toStringTag : void 0,
+        fn = Object.getOwnPropertySymbols,
+        Za = cn ? cn.isBuffer : void 0,
+        Wa = Ua(Object.keys, Object),
+        Gt = Ee(K, "DataView"),
+        Ie = Ee(K, "Map"),
+        zt = Ee(K, "Promise"),
+        Ut = Ee(K, "Set"),
+        Xt = Ee(K, "WeakMap"),
+        Me = Ee(Object, "create"),
+        es = le(Gt),
+        ts = le(Ie),
+        rs = le(zt),
+        ns = le(Ut),
+        os = le(Xt),
+        pn = dt ? dt.prototype : void 0,
+        qt = pn ? pn.valueOf : void 0;
 
     function ae(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function os() {
+    function is() {
         this.__data__ = Me ? Me(null) : {}, this.size = 0
     }
 
-    function is(t) {
+    function as(t) {
         var e = this.has(t) && delete this.__data__[t];
         return this.size -= e ? 1 : 0, e
     }
 
-    function as(t) {
+    function ss(t) {
         var e = this.__data__;
         if (Me) {
             var r = e[t];
-            return r === Kt ? void 0 : r
+            return r === Yt ? void 0 : r
         }
         return U.call(e, t) ? e[t] : void 0
     }
 
-    function ss(t) {
+    function ls(t) {
         var e = this.__data__;
         return Me ? e[t] !== void 0 : U.call(e, t)
     }
 
-    function ls(t, e) {
+    function ds(t, e) {
         var r = this.__data__;
-        return this.size += this.has(t) ? 0 : 1, r[t] = Me && e === void 0 ? Kt : e, this
+        return this.size += this.has(t) ? 0 : 1, r[t] = Me && e === void 0 ? Yt : e, this
     }
-    ae.prototype.clear = os;
-    ae.prototype.delete = is;
-    ae.prototype.get = as;
-    ae.prototype.has = ss;
-    ae.prototype.set = ls;
+    ae.prototype.clear = is;
+    ae.prototype.delete = as;
+    ae.prototype.get = ss;
+    ae.prototype.has = ls;
+    ae.prototype.set = ds;
 
-    function W(t) {
+    function Y(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function ds() {
+    function cs() {
         this.__data__ = [], this.size = 0
     }
 
-    function cs(t) {
+    function us(t) {
         var e = this.__data__,
-            r = pt(e, t);
+            r = mt(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : Xa.call(e, r, 1), --this.size, !0
+        return r == n ? e.pop() : Qa.call(e, r, 1), --this.size, !0
     }
 
-    function us(t) {
+    function fs(t) {
         var e = this.__data__,
-            r = pt(e, t);
+            r = mt(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function fs(t) {
-        return pt(this.__data__, t) > -1
+    function ps(t) {
+        return mt(this.__data__, t) > -1
     }
 
-    function ps(t, e) {
+    function ms(t, e) {
         var r = this.__data__,
-            n = pt(r, t);
+            n = mt(r, t);
         return n < 0 ? (++this.size, r.push([t, e])) : r[n][1] = e, this
     }
-    W.prototype.clear = ds;
-    W.prototype.delete = cs;
-    W.prototype.get = us;
-    W.prototype.has = fs;
-    W.prototype.set = ps;
+    Y.prototype.clear = cs;
+    Y.prototype.delete = us;
+    Y.prototype.get = fs;
+    Y.prototype.has = ps;
+    Y.prototype.set = ms;
 
     function se(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function ms() {
+    function gs() {
         this.size = 0, this.__data__ = {
             hash: new ae,
-            map: new(Ie || W),
+            map: new(Ie || Y),
             string: new ae
         }
     }
 
-    function gs(t) {
-        var e = mt(this, t).delete(t);
+    function hs(t) {
+        var e = gt(this, t).delete(t);
         return this.size -= e ? 1 : 0, e
     }
 
-    function hs(t) {
-        return mt(this, t).get(t)
+    function bs(t) {
+        return gt(this, t).get(t)
     }
 
-    function bs(t) {
-        return mt(this, t).has(t)
+    function js(t) {
+        return gt(this, t).has(t)
     }
 
-    function js(t, e) {
-        var r = mt(this, t),
+    function ys(t, e) {
+        var r = gt(this, t),
             n = r.size;
         return r.set(t, e), this.size += r.size == n ? 0 : 1, this
     }
-    se.prototype.clear = ms;
-    se.prototype.delete = gs;
-    se.prototype.get = hs;
-    se.prototype.has = bs;
-    se.prototype.set = js;
+    se.prototype.clear = gs;
+    se.prototype.delete = hs;
+    se.prototype.get = bs;
+    se.prototype.has = js;
+    se.prototype.set = ys;
 
-    function dt(t) {
+    function ct(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.__data__ = new se; ++e < r;) this.add(t[e])
     }
 
-    function ys(t) {
-        return this.__data__.set(t, Kt), this
+    function vs(t) {
+        return this.__data__.set(t, Yt), this
     }
 
-    function vs(t) {
+    function xs(t) {
         return this.__data__.has(t)
     }
-    dt.prototype.add = dt.prototype.push = ys;
-    dt.prototype.has = vs;
+    ct.prototype.add = ct.prototype.push = vs;
+    ct.prototype.has = xs;
 
     function ee(t) {
-        var e = this.__data__ = new W(t);
+        var e = this.__data__ = new Y(t);
         this.size = e.size
     }
 
-    function xs() {
-        this.__data__ = new W, this.size = 0
+    function Es() {
+        this.__data__ = new Y, this.size = 0
     }
 
-    function Es(t) {
+    function ws(t) {
         var e = this.__data__,
             r = e.delete(t);
         return this.size = e.size, r
     }
 
-    function ws(t) {
+    function ks(t) {
         return this.__data__.get(t)
     }
 
-    function ks(t) {
+    function As(t) {
         return this.__data__.has(t)
     }
 
-    function As(t, e) {
+    function Ts(t, e) {
         var r = this.__data__;
-        if (r instanceof W) {
+        if (r instanceof Y) {
             var n = r.__data__;
-            if (!Ie || n.length < ba - 1) return n.push([t, e]), this.size = ++r.size, this;
+            if (!Ie || n.length < ja - 1) return n.push([t, e]), this.size = ++r.size, this;
             r = this.__data__ = new se(n)
         }
         return r.set(t, e), this.size = r.size, this
     }
-    ee.prototype.clear = xs;
-    ee.prototype.delete = Es;
-    ee.prototype.get = ws;
-    ee.prototype.has = ks;
-    ee.prototype.set = As;
+    ee.prototype.clear = Es;
+    ee.prototype.delete = ws;
+    ee.prototype.get = ks;
+    ee.prototype.has = As;
+    ee.prototype.set = Ts;
 
     function Cs(t, e) {
-        var r = ct(t),
-            n = !r && qs(t),
-            i = !r && !n && Ut(t),
-            o = !r && !n && !i && Pn(t),
-            l = r || n || i || o,
-            c = l ? Ba(t.length, String) : [],
+        var r = ut(t),
+            n = !r && Ns(t),
+            i = !r && !n && Kt(t),
+            o = !r && !n && !i && Hn(t),
+            a = r || n || i || o,
+            c = a ? qa(t.length, String) : [],
             u = c.length;
-        for (var a in t)(e || U.call(t, a)) && !(l && (a == "length" || i && (a == "offset" || a == "parent") || o && (a == "buffer" || a == "byteLength" || a == "byteOffset") || Ds(a, u))) && c.push(a);
+        for (var s in t)(e || U.call(t, s)) && !(a && (s == "length" || i && (s == "offset" || s == "parent") || o && (s == "buffer" || s == "byteLength" || s == "byteOffset") || Ds(s, u))) && c.push(s);
         return c
     }
 
-    function pt(t, e) {
+    function mt(t, e) {
         for (var r = t.length; r--;)
-            if (Ln(t[r][0], e)) return r;
+            if (Mn(t[r][0], e)) return r;
         return -1
     }
 
-    function Ts(t, e, r) {
+    function Fs(t, e, r) {
         var n = e(t);
-        return ct(t) ? n : Ha(n, r(t))
+        return ut(t) ? n : Ra(n, r(t))
     }
 
-    function De(t) {
-        return t == null ? t === void 0 ? wa : va : ie && ie in Object(t) ? Ms(t) : Bs(t)
+    function Oe(t) {
+        return t == null ? t === void 0 ? ka : xa : ie && ie in Object(t) ? Ps(t) : qs(t)
     }
 
-    function un(t) {
-        return Pe(t) && De(t) == ot
+    function mn(t) {
+        return Pe(t) && Oe(t) == it
     }
 
-    function _n(t, e, r, n, i) {
-        return t === e ? !0 : t == null || e == null || !Pe(t) && !Pe(e) ? t !== t && e !== e : Fs(t, e, r, n, _n, i)
+    function Ln(t, e, r, n, i) {
+        return t === e ? !0 : t == null || e == null || !Pe(t) && !Pe(e) ? t !== t && e !== e : _s(t, e, r, n, Ln, i)
     }
 
-    function Fs(t, e, r, n, i, o) {
-        var l = ct(t),
-            c = ct(e),
-            u = l ? Bt : Q(t),
-            a = c ? Bt : Q(e);
-        u = u == ot ? ye : u, a = a == ot ? ye : a;
-        var m = u == ye,
-            j = a == ye,
-            A = u == a;
-        if (A && Ut(t)) {
-            if (!Ut(e)) return !1;
-            l = !0, m = !1
+    function _s(t, e, r, n, i, o) {
+        var a = ut(t),
+            c = ut(e),
+            u = a ? Nt : W(t),
+            s = c ? Nt : W(e);
+        u = u == it ? ve : u, s = s == it ? ve : s;
+        var p = u == ve,
+            j = s == ve,
+            A = u == s;
+        if (A && Kt(t)) {
+            if (!Kt(e)) return !1;
+            a = !0, p = !1
         }
-        if (A && !m) return o || (o = new ee), l || Pn(t) ? Sn(t, e, r, n, i, o) : $s(t, e, u, r, n, i, o);
-        if (!(r & ut)) {
-            var L = m && U.call(t, "__wrapped__"),
+        if (A && !p) return o || (o = new ee), a || Hn(t) ? In(t, e, r, n, i, o) : Is(t, e, u, r, n, i, o);
+        if (!(r & ft)) {
+            var $ = p && U.call(t, "__wrapped__"),
                 M = j && U.call(e, "__wrapped__");
-            if (L || M) {
-                var B = L ? t.value() : t,
+            if ($ || M) {
+                var B = $ ? t.value() : t,
                     q = M ? e.value() : e;
                 return o || (o = new ee), i(B, q, r, n, o)
             }
         }
-        return A ? (o || (o = new ee), Is(t, e, r, n, i, o)) : !1
+        return A ? (o || (o = new ee), Ms(t, e, r, n, i, o)) : !1
     }
 
-    function _s(t) {
-        if (!Mn(t) || Hs(t)) return !1;
-        var e = $n(t) ? Wa : Ma;
+    function Ss(t) {
+        if (!Dn(t) || Rs(t)) return !1;
+        var e = Pn(t) ? Ja : Pa;
         return e.test(le(t))
     }
 
-    function Ss(t) {
-        return Pe(t) && In(t.length) && !!S[De(t)]
+    function $s(t) {
+        return Pe(t) && On(t.length) && !!S[Oe(t)]
     }
 
     function Ls(t) {
-        if (!Rs(t)) return Ya(t);
+        if (!Bs(t)) return Wa(t);
         var e = [];
         for (var r in Object(t)) U.call(t, r) && r != "constructor" && e.push(r);
         return e
     }
 
-    function Sn(t, e, r, n, i, o) {
-        var l = r & ut,
+    function In(t, e, r, n, i, o) {
+        var a = r & ft,
             c = t.length,
             u = e.length;
-        if (c != u && !(l && u > c)) return !1;
-        var a = o.get(t);
-        if (a && o.get(e)) return a == e;
-        var m = -1,
+        if (c != u && !(a && u > c)) return !1;
+        var s = o.get(t);
+        if (s && o.get(e)) return s == e;
+        var p = -1,
             j = !0,
-            A = r & pn ? new dt : void 0;
-        for (o.set(t, e), o.set(e, t); ++m < c;) {
-            var L = t[m],
-                M = e[m];
-            if (n) var B = l ? n(M, L, m, e, t, o) : n(L, M, m, t, e, o);
+            A = r & hn ? new ct : void 0;
+        for (o.set(t, e), o.set(e, t); ++p < c;) {
+            var $ = t[p],
+                M = e[p];
+            if (n) var B = a ? n(M, $, p, e, t, o) : n($, M, p, t, e, o);
             if (B !== void 0) {
                 if (B) continue;
                 j = !1;
                 break
             }
             if (A) {
-                if (!Ra(e, function(q, G) {
-                        if (!Na(A, G) && (L === q || i(L, q, r, n, o))) return A.push(G)
+                if (!Ba(e, function(q, G) {
+                        if (!Va(A, G) && ($ === q || i($, q, r, n, o))) return A.push(G)
                     })) {
                     j = !1;
                     break
                 }
-            } else if (!(L === M || i(L, M, r, n, o))) {
+            } else if (!($ === M || i($, M, r, n, o))) {
                 j = !1;
                 break
             }
         }
         return o.delete(t), o.delete(e), j
     }
 
-    function $s(t, e, r, n, i, o, l) {
+    function Is(t, e, r, n, i, o, a) {
         switch (r) {
-            case st:
+            case lt:
                 if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
                 t = t.buffer, e = e.buffer;
-            case En:
-                return !(t.byteLength != e.byteLength || !o(new ln(t), new ln(e)));
-            case gn:
-            case hn:
+            case An:
+                return !(t.byteLength != e.byteLength || !o(new un(t), new un(e)));
+            case jn:
             case yn:
-                return Ln(+t, +e);
-            case bn:
-                return t.name == e.name && t.message == e.message;
+            case En:
+                return Mn(+t, +e);
             case vn:
-            case xn:
+                return t.name == e.name && t.message == e.message;
+            case wn:
+            case kn:
                 return t == e + "";
-            case it:
-                var c = Ga;
             case at:
-                var u = n & ut;
-                if (c || (c = Ua), t.size != e.size && !u) return !1;
-                var a = l.get(t);
-                if (a) return a == e;
-                n |= pn, l.set(t, e);
-                var m = Sn(c(t), c(e), n, i, o, l);
-                return l.delete(t), m;
-            case Ea:
-                if (Rt) return Rt.call(t) == Rt.call(e)
+                var c = za;
+            case st:
+                var u = n & ft;
+                if (c || (c = Xa), t.size != e.size && !u) return !1;
+                var s = a.get(t);
+                if (s) return s == e;
+                n |= hn, a.set(t, e);
+                var p = In(c(t), c(e), n, i, o, a);
+                return a.delete(t), p;
+            case wa:
+                if (qt) return qt.call(t) == qt.call(e)
         }
         return !1
     }
 
-    function Is(t, e, r, n, i, o) {
-        var l = r & ut,
-            c = fn(t),
+    function Ms(t, e, r, n, i, o) {
+        var a = r & ft,
+            c = gn(t),
             u = c.length,
-            a = fn(e),
-            m = a.length;
-        if (u != m && !l) return !1;
+            s = gn(e),
+            p = s.length;
+        if (u != p && !a) return !1;
         for (var j = u; j--;) {
             var A = c[j];
-            if (!(l ? A in e : U.call(e, A))) return !1
+            if (!(a ? A in e : U.call(e, A))) return !1
         }
-        var L = o.get(t);
-        if (L && o.get(e)) return L == e;
+        var $ = o.get(t);
+        if ($ && o.get(e)) return $ == e;
         var M = !0;
         o.set(t, e), o.set(e, t);
-        for (var B = l; ++j < u;) {
+        for (var B = a; ++j < u;) {
             A = c[j];
             var q = t[A],
                 G = e[A];
-            if (n) var O = l ? n(G, q, A, e, t, o) : n(q, G, A, t, e, o);
-            if (!(O === void 0 ? q === G || i(q, G, r, n, o) : O)) {
+            if (n) var D = a ? n(G, q, A, e, t, o) : n(q, G, A, t, e, o);
+            if (!(D === void 0 ? q === G || i(q, G, r, n, o) : D)) {
                 M = !1;
                 break
             }
             B || (B = A == "constructor")
         }
         if (M && !B) {
             var b = t.constructor,
                 _ = e.constructor;
             b != _ && "constructor" in t && "constructor" in e && !(typeof b == "function" && b instanceof b && typeof _ == "function" && _ instanceof _) && (M = !1)
         }
         return o.delete(t), o.delete(e), M
     }
 
-    function fn(t) {
-        return Ts(t, Gs, Ps)
+    function gn(t) {
+        return Fs(t, zs, Os)
     }
 
-    function mt(t, e) {
+    function gt(t, e) {
         var r = t.__data__;
-        return Os(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return Hs(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function xe(t, e) {
-        var r = Va(t, e);
-        return _s(r) ? r : void 0
+    function Ee(t, e) {
+        var r = Ga(t, e);
+        return Ss(r) ? r : void 0
     }
 
-    function Ms(t) {
+    function Ps(t) {
         var e = U.call(t, ie),
             r = t[ie];
         try {
             t[ie] = void 0;
             var n = !0
         } catch {}
-        var i = Tn.call(t);
+        var i = Sn.call(t);
         return n && (e ? t[ie] = r : delete t[ie]), i
     }
-    var Ps = dn ? function(t) {
-            return t == null ? [] : (t = Object(t), Oa(dn(t), function(e) {
-                return Fn.call(t, e)
+    var Os = fn ? function(t) {
+            return t == null ? [] : (t = Object(t), Ha(fn(t), function(e) {
+                return $n.call(t, e)
             }))
-        } : zs,
-        Q = De;
-    (Nt && Q(new Nt(new ArrayBuffer(1))) != st || Ie && Q(new Ie) != it || Vt && Q(Vt.resolve()) != tn || Gt && Q(new Gt) != at || zt && Q(new zt) != qt) && (Q = function(t) {
-        var e = De(t),
-            r = e == ye ? t.constructor : void 0,
+        } : Us,
+        W = Oe;
+    (Gt && W(new Gt(new ArrayBuffer(1))) != lt || Ie && W(new Ie) != at || zt && W(zt.resolve()) != on || Ut && W(new Ut) != st || Xt && W(new Xt) != Vt) && (W = function(t) {
+        var e = Oe(t),
+            r = e == ve ? t.constructor : void 0,
             n = r ? le(r) : "";
         if (n) switch (n) {
-            case Qa:
-                return st;
             case es:
-                return it;
+                return lt;
             case ts:
-                return tn;
-            case rs:
                 return at;
+            case rs:
+                return on;
             case ns:
-                return qt
+                return st;
+            case os:
+                return Vt
         }
         return e
     });
 
     function Ds(t, e) {
-        return e = e ?? mn, !!e && (typeof t == "number" || Pa.test(t)) && t > -1 && t % 1 == 0 && t < e
+        return e = e ?? bn, !!e && (typeof t == "number" || Oa.test(t)) && t > -1 && t % 1 == 0 && t < e
     }
 
-    function Os(t) {
+    function Hs(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function Hs(t) {
-        return !!an && an in t
+    function Rs(t) {
+        return !!dn && dn in t
     }
 
-    function Rs(t) {
+    function Bs(t) {
         var e = t && t.constructor,
-            r = typeof e == "function" && e.prototype || ft;
+            r = typeof e == "function" && e.prototype || pt;
         return t === r
     }
 
-    function Bs(t) {
-        return Tn.call(t)
+    function qs(t) {
+        return Sn.call(t)
     }
 
     function le(t) {
         if (t != null) {
             try {
-                return Cn.call(t)
+                return _n.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function Ln(t, e) {
+    function Mn(t, e) {
         return t === e || t !== t && e !== e
     }
-    var qs = un(function() {
+    var Ns = mn(function() {
             return arguments
-        }()) ? un : function(t) {
-            return Pe(t) && U.call(t, "callee") && !Fn.call(t, "callee")
+        }()) ? mn : function(t) {
+            return Pe(t) && U.call(t, "callee") && !$n.call(t, "callee")
         },
-        ct = Array.isArray;
+        ut = Array.isArray;
 
-    function Ns(t) {
-        return t != null && In(t.length) && !$n(t)
+    function Vs(t) {
+        return t != null && On(t.length) && !Pn(t)
     }
-    var Ut = Za || Us;
+    var Kt = Za || Xs;
 
-    function Vs(t, e) {
-        return _n(t, e)
+    function Gs(t, e) {
+        return Ln(t, e)
     }
 
-    function $n(t) {
-        if (!Mn(t)) return !1;
-        var e = De(t);
-        return e == jn || e == ya || e == ja || e == xa
+    function Pn(t) {
+        if (!Dn(t)) return !1;
+        var e = Oe(t);
+        return e == xn || e == va || e == ya || e == Ea
     }
 
-    function In(t) {
-        return typeof t == "number" && t > -1 && t % 1 == 0 && t <= mn
+    function On(t) {
+        return typeof t == "number" && t > -1 && t % 1 == 0 && t <= bn
     }
 
-    function Mn(t) {
+    function Dn(t) {
         var e = typeof t;
         return t != null && (e == "object" || e == "function")
     }
 
     function Pe(t) {
         return t != null && typeof t == "object"
     }
-    var Pn = on ? qa(on) : Ss;
+    var Hn = ln ? Na(ln) : $s;
 
-    function Gs(t) {
-        return Ns(t) ? Cs(t) : Ls(t)
+    function zs(t) {
+        return Vs(t) ? Cs(t) : Ls(t)
     }
 
-    function zs() {
+    function Us() {
         return []
     }
 
-    function Us() {
+    function Xs() {
         return !1
     }
-    ve.exports = Vs
+    xe.exports = Gs
 });
-var Wn = Ze((Oe, Ee) => {
+var Zn = Qe((De, we) => {
     var Ks = 9007199254740991,
-        Js = "[object Arguments]",
-        Ws = "[object Function]",
-        Xs = "[object GeneratorFunction]",
-        Wt = "[object Map]",
+        Ys = "[object Arguments]",
+        Js = "[object Function]",
+        Qs = "[object GeneratorFunction]",
+        Qt = "[object Map]",
         Zs = "[object Object]",
-        On = "[object Promise]",
-        Xt = "[object Set]",
-        Hn = "[object WeakMap]",
-        Rn = "[object DataView]",
-        Ys = /[\\^$.*+?()[\]{}|]/g,
-        Qs = /^\[object .+?Constructor\]$/,
-        el = typeof global == "object" && global && global.Object === Object && global,
-        tl = typeof self == "object" && self && self.Object === Object && self,
-        ce = el || tl || Function("return this")(),
-        Vn = typeof Oe == "object" && Oe && !Oe.nodeType && Oe,
-        Bn = Vn && typeof Ee == "object" && Ee && !Ee.nodeType && Ee,
-        rl = Bn && Bn.exports === Vn;
+        Bn = "[object Promise]",
+        Zt = "[object Set]",
+        qn = "[object WeakMap]",
+        Nn = "[object DataView]",
+        Ws = /[\\^$.*+?()[\]{}|]/g,
+        el = /^\[object .+?Constructor\]$/,
+        tl = typeof global == "object" && global && global.Object === Object && global,
+        rl = typeof self == "object" && self && self.Object === Object && self,
+        ce = tl || rl || Function("return this")(),
+        Un = typeof De == "object" && De && !De.nodeType && De,
+        Vn = Un && typeof we == "object" && we && !we.nodeType && we,
+        nl = Vn && Vn.exports === Un;
 
-    function nl(t, e) {
+    function ol(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function ol(t) {
+    function il(t) {
         var e = !1;
         if (t != null && typeof t.toString != "function") try {
             e = !!(t + "")
         } catch {}
         return e
     }
 
-    function il(t, e) {
+    function al(t, e) {
         return function(r) {
             return t(e(r))
         }
     }
-    var al = Function.prototype,
-        gt = Object.prototype,
+    var sl = Function.prototype,
+        ht = Object.prototype,
         Jt = ce["__core-js_shared__"],
-        qn = function() {
+        Gn = function() {
             var t = /[^.]+$/.exec(Jt && Jt.keys && Jt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        Gn = al.toString,
-        rr = gt.hasOwnProperty,
-        ht = gt.toString,
-        sl = RegExp("^" + Gn.call(rr).replace(Ys, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        Nn = rl ? ce.Buffer : void 0,
-        zn = gt.propertyIsEnumerable,
-        ll = Nn ? Nn.isBuffer : void 0,
-        dl = il(Object.keys, Object),
-        Zt = He(ce, "DataView"),
-        Yt = He(ce, "Map"),
-        Qt = He(ce, "Promise"),
-        er = He(ce, "Set"),
-        tr = He(ce, "WeakMap"),
-        cl = !zn.call({
+        Xn = sl.toString,
+        or = ht.hasOwnProperty,
+        bt = ht.toString,
+        ll = RegExp("^" + Xn.call(or).replace(Ws, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        zn = nl ? ce.Buffer : void 0,
+        Kn = ht.propertyIsEnumerable,
+        dl = zn ? zn.isBuffer : void 0,
+        cl = al(Object.keys, Object),
+        Wt = He(ce, "DataView"),
+        er = He(ce, "Map"),
+        tr = He(ce, "Promise"),
+        rr = He(ce, "Set"),
+        nr = He(ce, "WeakMap"),
+        ul = !Kn.call({
             valueOf: 1
         }, "valueOf"),
-        ul = ue(Zt),
-        fl = ue(Yt),
-        pl = ue(Qt),
-        ml = ue(er),
-        gl = ue(tr);
+        fl = ue(Wt),
+        pl = ue(er),
+        ml = ue(tr),
+        gl = ue(rr),
+        hl = ue(nr);
 
-    function hl(t) {
-        return ht.call(t)
+    function bl(t) {
+        return bt.call(t)
     }
 
-    function bl(t) {
-        if (!Jn(t) || jl(t)) return !1;
-        var e = Kn(t) || ol(t) ? sl : Qs;
+    function jl(t) {
+        if (!Qn(t) || yl(t)) return !1;
+        var e = Jn(t) || il(t) ? ll : el;
         return e.test(ue(t))
     }
 
     function He(t, e) {
-        var r = nl(t, e);
-        return bl(r) ? r : void 0
+        var r = ol(t, e);
+        return jl(r) ? r : void 0
     }
-    var de = hl;
-    (Zt && de(new Zt(new ArrayBuffer(1))) != Rn || Yt && de(new Yt) != Wt || Qt && de(Qt.resolve()) != On || er && de(new er) != Xt || tr && de(new tr) != Hn) && (de = function(t) {
-        var e = ht.call(t),
+    var de = bl;
+    (Wt && de(new Wt(new ArrayBuffer(1))) != Nn || er && de(new er) != Qt || tr && de(tr.resolve()) != Bn || rr && de(new rr) != Zt || nr && de(new nr) != qn) && (de = function(t) {
+        var e = bt.call(t),
             r = e == Zs ? t.constructor : void 0,
             n = r ? ue(r) : void 0;
         if (n) switch (n) {
-            case ul:
-                return Rn;
             case fl:
-                return Wt;
+                return Nn;
             case pl:
-                return On;
+                return Qt;
             case ml:
-                return Xt;
+                return Bn;
             case gl:
-                return Hn
+                return Zt;
+            case hl:
+                return qn
         }
         return e
     });
 
-    function jl(t) {
-        return !!qn && qn in t
+    function yl(t) {
+        return !!Gn && Gn in t
     }
 
-    function yl(t) {
+    function vl(t) {
         var e = t && t.constructor,
-            r = typeof e == "function" && e.prototype || gt;
+            r = typeof e == "function" && e.prototype || ht;
         return t === r
     }
 
     function ue(t) {
         if (t != null) {
             try {
-                return Gn.call(t)
+                return Xn.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function vl(t) {
-        return El(t) && rr.call(t, "callee") && (!zn.call(t, "callee") || ht.call(t) == Js)
+    function xl(t) {
+        return wl(t) && or.call(t, "callee") && (!Kn.call(t, "callee") || bt.call(t) == Ys)
     }
-    var xl = Array.isArray;
+    var El = Array.isArray;
 
-    function Un(t) {
-        return t != null && Al(t.length) && !Kn(t)
+    function Yn(t) {
+        return t != null && Tl(t.length) && !Jn(t)
     }
 
-    function El(t) {
-        return Cl(t) && Un(t)
+    function wl(t) {
+        return Cl(t) && Yn(t)
     }
-    var wl = ll || Tl;
+    var kl = dl || Fl;
 
-    function kl(t) {
-        if (Un(t) && (xl(t) || typeof t == "string" || typeof t.splice == "function" || wl(t) || vl(t))) return !t.length;
+    function Al(t) {
+        if (Yn(t) && (El(t) || typeof t == "string" || typeof t.splice == "function" || kl(t) || xl(t))) return !t.length;
         var e = de(t);
-        if (e == Wt || e == Xt) return !t.size;
-        if (cl || yl(t)) return !dl(t).length;
+        if (e == Qt || e == Zt) return !t.size;
+        if (ul || vl(t)) return !cl(t).length;
         for (var r in t)
-            if (rr.call(t, r)) return !1;
+            if (or.call(t, r)) return !1;
         return !0
     }
 
-    function Kn(t) {
-        var e = Jn(t) ? ht.call(t) : "";
-        return e == Ws || e == Xs
+    function Jn(t) {
+        var e = Qn(t) ? bt.call(t) : "";
+        return e == Js || e == Qs
     }
 
-    function Al(t) {
+    function Tl(t) {
         return typeof t == "number" && t > -1 && t % 1 == 0 && t <= Ks
     }
 
-    function Jn(t) {
+    function Qn(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
     function Cl(t) {
         return !!t && typeof t == "object"
     }
 
-    function Tl() {
+    function Fl() {
         return !1
     }
-    Ee.exports = kl
+    we.exports = Al
 });
 (function() {
     "use strict";
     var t = function(g, f) {
-        var h = function(C) {
-                for (var w = 0, $ = C.length; w < $; w++) v(C[w])
+        var h = function(T) {
+                for (var w = 0, L = T.length; w < L; w++) v(T[w])
             },
-            v = function(C) {
-                var w = C.target,
-                    $ = C.attributeName,
-                    P = C.oldValue;
-                w.attributeChangedCallback($, P, w.getAttribute($))
+            v = function(T) {
+                var w = T.target,
+                    L = T.attributeName,
+                    P = T.oldValue;
+                w.attributeChangedCallback(L, P, w.getAttribute(L))
             };
-        return function(x, C) {
+        return function(x, T) {
             var w = x.constructor.observedAttributes;
-            return w && g(C).then(function() {
+            return w && g(T).then(function() {
                 new f(h).observe(x, {
                     attributes: !0,
                     attributeOldValue: !0,
                     attributeFilter: w
                 });
-                for (var $ = 0, P = w.length; $ < P; $++) x.hasAttribute(w[$]) && v({
+                for (var L = 0, P = w.length; L < P; L++) x.hasAttribute(w[L]) && v({
                     target: x,
-                    attributeName: w[$],
+                    attributeName: w[L],
                     oldValue: null
                 })
             }), x
         }
     };
 
     function e(g, f) {
@@ -1502,384 +1502,384 @@
                     },
                     f: x
                 }
             }
             throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
         }
-        var C = !0,
+        var T = !0,
             w = !1,
-            $;
+            L;
         return {
             s: function() {
                 h = h.call(g)
             },
             n: function() {
                 var P = h.next();
-                return C = P.done, P
+                return T = P.done, P
             },
             e: function(P) {
-                w = !0, $ = P
+                w = !0, L = P
             },
             f: function() {
                 try {
-                    !C && h.return != null && h.return()
+                    !T && h.return != null && h.return()
                 } finally {
-                    if (w) throw $
+                    if (w) throw L
                 }
             }
         }
     }
     var i = !0,
         o = !1,
-        l = "querySelectorAll",
+        a = "querySelectorAll",
         c = function(f) {
             var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
                 v = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
                 x = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : ["*"],
-                C = function P(Z, Y, R, k, I, D) {
-                    var V = n(Z),
-                        ge;
+                T = function P(Q, Z, R, k, I, O) {
+                    var V = n(Q),
+                        he;
                     try {
-                        for (V.s(); !(ge = V.n()).done;) {
-                            var H = ge.value;
-                            (D || l in H) && (I ? R.has(H) || (R.add(H), k.delete(H), f(H, I)) : k.has(H) || (k.add(H), R.delete(H), f(H, I)), D || P(H[l](Y), Y, R, k, I, i))
+                        for (V.s(); !(he = V.n()).done;) {
+                            var H = he.value;
+                            (O || a in H) && (I ? R.has(H) || (R.add(H), k.delete(H), f(H, I)) : k.has(H) || (k.add(H), R.delete(H), f(H, I)), O || P(H[a](Z), Z, R, k, I, i))
                         }
-                    } catch (Tt) {
-                        V.e(Tt)
+                    } catch (_t) {
+                        V.e(_t)
                     } finally {
                         V.f()
                     }
                 },
                 w = new v(function(P) {
                     if (x.length) {
-                        var Z = x.join(","),
-                            Y = new Set,
+                        var Q = x.join(","),
+                            Z = new Set,
                             R = new Set,
                             k = n(P),
                             I;
                         try {
                             for (k.s(); !(I = k.n()).done;) {
-                                var D = I.value,
-                                    V = D.addedNodes,
-                                    ge = D.removedNodes;
-                                C(ge, Z, Y, R, o, o), C(V, Z, Y, R, i, o)
+                                var O = I.value,
+                                    V = O.addedNodes,
+                                    he = O.removedNodes;
+                                T(he, Q, Z, R, o, o), T(V, Q, Z, R, i, o)
                             }
                         } catch (H) {
                             k.e(H)
                         } finally {
                             k.f()
                         }
                     }
                 }),
-                $ = w.observe;
+                L = w.observe;
             return (w.observe = function(P) {
-                return $.call(w, P, {
+                return L.call(w, P, {
                     subtree: i,
                     childList: i
                 })
             })(h), w
         },
         u = "querySelectorAll",
-        a = self,
-        m = a.document,
-        j = a.Element,
-        A = a.MutationObserver,
-        L = a.Set,
-        M = a.WeakMap,
+        s = self,
+        p = s.document,
+        j = s.Element,
+        A = s.MutationObserver,
+        $ = s.Set,
+        M = s.WeakMap,
         B = function(f) {
             return u in f
         },
         q = [].filter,
         G = function(g) {
             var f = new M,
                 h = function(k) {
-                    for (var I = 0, D = k.length; I < D; I++) f.delete(k[I])
+                    for (var I = 0, O = k.length; I < O; I++) f.delete(k[I])
                 },
                 v = function() {
-                    for (var k = Z.takeRecords(), I = 0, D = k.length; I < D; I++) w(q.call(k[I].removedNodes, B), !1), w(q.call(k[I].addedNodes, B), !0)
+                    for (var k = Q.takeRecords(), I = 0, O = k.length; I < O; I++) w(q.call(k[I].removedNodes, B), !1), w(q.call(k[I].addedNodes, B), !0)
                 },
                 x = function(k) {
                     return k.matches || k.webkitMatchesSelector || k.msMatchesSelector
                 },
-                C = function(k, I) {
-                    var D;
+                T = function(k, I) {
+                    var O;
                     if (I)
-                        for (var V, ge = x(k), H = 0, Tt = $.length; H < Tt; H++) ge.call(k, V = $[H]) && (f.has(k) || f.set(k, new L), D = f.get(k), D.has(V) || (D.add(V), g.handle(k, I, V)));
-                    else f.has(k) && (D = f.get(k), f.delete(k), D.forEach(function(xo) {
-                        g.handle(k, I, xo)
+                        for (var V, he = x(k), H = 0, _t = L.length; H < _t; H++) he.call(k, V = L[H]) && (f.has(k) || f.set(k, new $), O = f.get(k), O.has(V) || (O.add(V), g.handle(k, I, V)));
+                    else f.has(k) && (O = f.get(k), f.delete(k), O.forEach(function(Eo) {
+                        g.handle(k, I, Eo)
                     }))
                 },
                 w = function(k) {
-                    for (var I = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, D = 0, V = k.length; D < V; D++) C(k[D], I)
+                    for (var I = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, O = 0, V = k.length; O < V; O++) T(k[O], I)
                 },
-                $ = g.query,
-                P = g.root || m,
-                Z = c(C, P, A, $),
-                Y = j.prototype.attachShadow;
-            return Y && (j.prototype.attachShadow = function(R) {
-                var k = Y.call(this, R);
-                return Z.observe(k), k
-            }), $.length && w(P[u]($)), {
+                L = g.query,
+                P = g.root || p,
+                Q = c(T, P, A, L),
+                Z = j.prototype.attachShadow;
+            return Z && (j.prototype.attachShadow = function(R) {
+                var k = Z.call(this, R);
+                return Q.observe(k), k
+            }), L.length && w(P[u](L)), {
                 drop: h,
                 flush: v,
-                observer: Z,
+                observer: Q,
                 parse: w
             }
         },
-        O = self,
-        b = O.document,
-        _ = O.Map,
-        xt = O.MutationObserver,
-        pe = O.Object,
-        me = O.Set,
-        Be = O.WeakMap,
-        X = O.Element,
-        qe = O.HTMLElement,
-        Ne = O.Node,
-        Ce = O.Error,
-        y = O.TypeError,
-        Ve = O.Reflect,
-        p = pe.defineProperty,
-        d = pe.keys,
-        s = pe.getOwnPropertyNames,
-        F = pe.setPrototypeOf,
-        T = !self.customElements,
+        D = self,
+        b = D.document,
+        _ = D.Map,
+        wt = D.MutationObserver,
+        me = D.Object,
+        ge = D.Set,
+        Be = D.WeakMap,
+        J = D.Element,
+        qe = D.HTMLElement,
+        Ne = D.Node,
+        Te = D.Error,
+        y = D.TypeError,
+        Ve = D.Reflect,
+        m = me.defineProperty,
+        d = me.keys,
+        l = me.getOwnPropertyNames,
+        F = me.setPrototypeOf,
+        C = !self.customElements,
         N = function(f) {
-            for (var h = d(f), v = [], x = h.length, C = 0; C < x; C++) v[C] = f[h[C]], delete f[h[C]];
+            for (var h = d(f), v = [], x = h.length, T = 0; T < x; T++) v[T] = f[h[T]], delete f[h[T]];
             return function() {
                 for (var w = 0; w < x; w++) f[h[w]] = v[w]
             }
         };
-    if (T) {
+    if (C) {
         var E = function() {
                 var f = this.constructor;
                 if (!Fe.has(f)) throw new y("Illegal constructor");
                 var h = Fe.get(f);
-                if (ze) return fr(ze, h);
-                var v = Te.call(b, h);
-                return fr(F(v, f.prototype), h)
+                if (ze) return hr(ze, h);
+                var v = Ce.call(b, h);
+                return hr(F(v, f.prototype), h)
             },
-            Te = b.createElement,
+            Ce = b.createElement,
             Fe = new _,
             Ge = new _,
-            cr = new _,
+            mr = new _,
             _e = new _,
-            ur = [],
-            ao = function(f, h, v) {
-                var x = cr.get(v);
+            gr = [],
+            so = function(f, h, v) {
+                var x = mr.get(v);
                 if (h && !x.isPrototypeOf(f)) {
-                    var C = N(f);
+                    var T = N(f);
                     ze = F(f, x);
                     try {
                         new x.constructor
                     } finally {
-                        ze = null, C()
+                        ze = null, T()
                     }
                 }
                 var w = "".concat(h ? "" : "dis", "connectedCallback");
                 w in x && f[w]()
             },
-            so = G({
-                query: ur,
-                handle: ao
+            lo = G({
+                query: gr,
+                handle: so
             }),
-            lo = so.parse,
+            co = lo.parse,
             ze = null,
-            Et = function(f) {
+            kt = function(f) {
                 if (!Ge.has(f)) {
                     var h, v = new Promise(function(x) {
                         h = x
                     });
                     Ge.set(f, {
                         $: v,
                         _: h
                     })
                 }
                 return Ge.get(f).$
             },
-            fr = t(Et, xt);
+            hr = t(kt, wt);
         self.customElements = {
             define: function(f, h) {
-                if (_e.has(f)) throw new Ce('the name "'.concat(f, '" has already been used with this registry'));
-                Fe.set(h, f), cr.set(f, h.prototype), _e.set(f, h), ur.push(f), Et(f).then(function() {
-                    lo(b.querySelectorAll(f))
+                if (_e.has(f)) throw new Te('the name "'.concat(f, '" has already been used with this registry'));
+                Fe.set(h, f), mr.set(f, h.prototype), _e.set(f, h), gr.push(f), kt(f).then(function() {
+                    co(b.querySelectorAll(f))
                 }), Ge.get(f)._(h)
             },
             get: function(f) {
                 return _e.get(f)
             },
-            whenDefined: Et
-        }, p(E.prototype = qe.prototype, "constructor", {
+            whenDefined: kt
+        }, m(E.prototype = qe.prototype, "constructor", {
             value: E
         }), self.HTMLElement = E, b.createElement = function(g, f) {
             var h = f && f.is,
                 v = h ? _e.get(h) : _e.get(g);
-            return v ? new v : Te.call(b, g)
-        }, "isConnected" in Ne.prototype || p(Ne.prototype, "isConnected", {
+            return v ? new v : Ce.call(b, g)
+        }, "isConnected" in Ne.prototype || m(Ne.prototype, "isConnected", {
             configurable: !0,
             get: function() {
                 return !(this.ownerDocument.compareDocumentPosition(this) & this.DOCUMENT_POSITION_DISCONNECTED)
             }
         })
-    } else if (T = !self.customElements.get("extends-li"), T) try {
-        var pr = function g() {
+    } else if (C = !self.customElements.get("extends-li"), C) try {
+        var br = function g() {
             return self.Reflect.construct(HTMLLIElement, [], g)
         };
-        pr.prototype = HTMLLIElement.prototype;
-        var mr = "extends-li";
-        self.customElements.define("extends-li", pr, {
+        br.prototype = HTMLLIElement.prototype;
+        var jr = "extends-li";
+        self.customElements.define("extends-li", br, {
             extends: "li"
-        }), T = b.createElement("li", {
-            is: mr
-        }).outerHTML.indexOf(mr) < 0;
-        var gr = self.customElements,
-            co = gr.get,
-            uo = gr.whenDefined;
+        }), C = b.createElement("li", {
+            is: jr
+        }).outerHTML.indexOf(jr) < 0;
+        var yr = self.customElements,
+            uo = yr.get,
+            fo = yr.whenDefined;
         self.customElements.whenDefined = function(g) {
             var f = this;
-            return uo.call(this, g).then(function(h) {
-                return h || co.call(f, g)
+            return fo.call(this, g).then(function(h) {
+                return h || uo.call(f, g)
             })
         }
     } catch {}
-    if (T) {
-        var hr = function(f) {
-                var h = wt.get(f);
-                xr(h.querySelectorAll(this), f.isConnected)
+    if (C) {
+        var vr = function(f) {
+                var h = At.get(f);
+                Ar(h.querySelectorAll(this), f.isConnected)
             },
             z = self.customElements,
-            br = b.createElement,
-            fo = z.define,
-            po = z.get,
-            mo = z.upgrade,
-            go = Ve || {
+            xr = b.createElement,
+            po = z.define,
+            mo = z.get,
+            go = z.upgrade,
+            ho = Ve || {
                 construct: function(f) {
                     return f.call(this)
                 }
             },
-            ho = go.construct,
-            wt = new Be,
-            kt = new me,
+            bo = ho.construct,
+            At = new Be,
+            Tt = new ge,
             Ue = new _,
+            Xe = new _,
+            Er = new _,
             Ke = new _,
-            jr = new _,
-            Je = new _,
-            yr = [],
-            We = [],
-            vr = function(f) {
-                return Je.get(f) || po.call(z, f)
+            wr = [],
+            Ye = [],
+            kr = function(f) {
+                return Ke.get(f) || mo.call(z, f)
             },
-            bo = function(f, h, v) {
-                var x = jr.get(v);
+            jo = function(f, h, v) {
+                var x = Er.get(v);
                 if (h && !x.isPrototypeOf(f)) {
-                    var C = N(f);
-                    Xe = F(f, x);
+                    var T = N(f);
+                    Je = F(f, x);
                     try {
                         new x.constructor
                     } finally {
-                        Xe = null, C()
+                        Je = null, T()
                     }
                 }
                 var w = "".concat(h ? "" : "dis", "connectedCallback");
                 w in x && f[w]()
             },
-            jo = G({
-                query: We,
-                handle: bo
-            }),
-            xr = jo.parse,
             yo = G({
-                query: yr,
+                query: Ye,
+                handle: jo
+            }),
+            Ar = yo.parse,
+            vo = G({
+                query: wr,
                 handle: function(f, h) {
-                    wt.has(f) && (h ? kt.add(f) : kt.delete(f), We.length && hr.call(We, f))
+                    At.has(f) && (h ? Tt.add(f) : Tt.delete(f), Ye.length && vr.call(Ye, f))
                 }
             }),
-            vo = yo.parse,
-            Er = X.prototype.attachShadow;
-        Er && (X.prototype.attachShadow = function(g) {
-            var f = Er.call(this, g);
-            return wt.set(this, f), f
+            xo = vo.parse,
+            Tr = J.prototype.attachShadow;
+        Tr && (J.prototype.attachShadow = function(g) {
+            var f = Tr.call(this, g);
+            return At.set(this, f), f
         });
-        var At = function(f) {
-                if (!Ke.has(f)) {
+        var Ct = function(f) {
+                if (!Xe.has(f)) {
                     var h, v = new Promise(function(x) {
                         h = x
                     });
-                    Ke.set(f, {
+                    Xe.set(f, {
                         $: v,
                         _: h
                     })
                 }
-                return Ke.get(f).$
+                return Xe.get(f).$
             },
-            Ct = t(At, xt),
-            Xe = null;
-        s(self).filter(function(g) {
+            Ft = t(Ct, wt),
+            Je = null;
+        l(self).filter(function(g) {
             return /^HTML.*Element$/.test(g)
         }).forEach(function(g) {
             var f = self[g];
 
             function h() {
                 var v = this.constructor;
                 if (!Ue.has(v)) throw new y("Illegal constructor");
                 var x = Ue.get(v),
-                    C = x.is,
+                    T = x.is,
                     w = x.tag;
-                if (C) {
-                    if (Xe) return Ct(Xe, C);
-                    var $ = br.call(b, w);
-                    return $.setAttribute("is", C), Ct(F($, v.prototype), C)
-                } else return ho.call(this, f, [], v)
+                if (T) {
+                    if (Je) return Ft(Je, T);
+                    var L = xr.call(b, w);
+                    return L.setAttribute("is", T), Ft(F(L, v.prototype), T)
+                } else return bo.call(this, f, [], v)
             }
-            p(h.prototype = f.prototype, "constructor", {
+            m(h.prototype = f.prototype, "constructor", {
                 value: h
-            }), p(self, g, {
+            }), m(self, g, {
                 value: h
             })
         }), b.createElement = function(g, f) {
             var h = f && f.is;
             if (h) {
-                var v = Je.get(h);
+                var v = Ke.get(h);
                 if (v && Ue.get(v).tag === g) return new v
             }
-            var x = br.call(b, g);
+            var x = xr.call(b, g);
             return h && x.setAttribute("is", h), x
-        }, z.get = vr, z.whenDefined = At, z.upgrade = function(g) {
+        }, z.get = kr, z.whenDefined = Ct, z.upgrade = function(g) {
             var f = g.getAttribute("is");
             if (f) {
-                var h = Je.get(f);
+                var h = Ke.get(f);
                 if (h) {
-                    Ct(F(g, h.prototype), f);
+                    Ft(F(g, h.prototype), f);
                     return
                 }
             }
-            mo.call(z, g)
+            go.call(z, g)
         }, z.define = function(g, f, h) {
-            if (vr(g)) throw new Ce("'".concat(g, "' has already been defined as a custom element"));
+            if (kr(g)) throw new Te("'".concat(g, "' has already been defined as a custom element"));
             var v, x = h && h.extends;
             Ue.set(f, x ? {
                 is: g,
                 tag: x
             } : {
                 is: "",
                 tag: g
-            }), x ? (v = "".concat(x, '[is="').concat(g, '"]'), jr.set(v, f.prototype), Je.set(g, f), We.push(v)) : (fo.apply(z, arguments), yr.push(v = g)), At(g).then(function() {
-                x ? (xr(b.querySelectorAll(v)), kt.forEach(hr, [v])) : vo(b.querySelectorAll(v))
-            }), Ke.get(g)._(f)
+            }), x ? (v = "".concat(x, '[is="').concat(g, '"]'), Er.set(v, f.prototype), Ke.set(g, f), Ye.push(v)) : (po.apply(z, arguments), wr.push(v = g)), Ct(g).then(function() {
+                x ? (Ar(b.querySelectorAll(v)), Tt.forEach(vr, [v])) : xo(b.querySelectorAll(v))
+            }), Xe.get(g)._(f)
         }
     }
 })();
-var Ae = he(Br()),
-    to = he(en()),
-    ro = he(Dn()),
-    no = he(Wn()),
-    oo = he(wr());
-var Xn = he(wr()),
-    bt = class {
+var Ae = be(Vr()),
+    no = be(nn()),
+    pr = be(Rn()),
+    oo = be(Zn()),
+    io = be(Cr());
+var Wn = be(Cr()),
+    jt = class {
         constructor(e, r) {
             this.progressBar = null;
             this.fileDrop = e => {
                 this.swallowEvent(e), e.dataTransfer && (this.fieldGroup.touch(), this.inputElement.files = e.dataTransfer.files, this.uploadFiles(this.inputElement.files).then(() => {
                     this.fieldGroup.inputted(), this.fieldGroup.validate()
                 }))
             };
@@ -1891,15 +1891,15 @@
                 e.stopPropagation(), e.preventDefault()
             };
             if (this.fieldGroup = e, this.inputElement = r, this.maxUploadSize = parseInt(this.inputElement.getAttribute("max-size") ?? "0"), this.dropbox = this.fieldGroup.element.querySelector("figure.dj-dropbox"), !this.dropbox) throw new Error('Element <input type="file"> requires sibling element <figure class="dj-dropbox"></figure>');
             if (this.chooseFileButton = this.fieldGroup.element.querySelector("button.dj-choose-file"), !this.chooseFileButton) throw new Error('Element <input type="file"> requires sibling element <button class="dj-choose-file"></button>');
             if (this.progressBar = this.fieldGroup.element.querySelector("progress"), this.progressBar && (this.progressBar.style.visibility = "hidden"), this.emptyDropboxItem = this.dropbox.querySelector("div.dj-empty-item"), !this.emptyDropboxItem) throw new Error('Element <input type="file"> requires sibling element <figure><div class="dj-empty-item"></div></figure>');
             let n = this.fieldGroup.element.querySelector(".dj-dropbox-items");
             if (!n) throw new Error('Element <input type="file"> requires sibling element <template class="dj-dropbox-items"></template>');
-            this.dropboxItemTemplate = (0, Xn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
+            this.dropboxItemTemplate = (0, Wn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
                 attributes: !0
             }), this.chooseFileButton.disabled = r.disabled;
             let i = document.getElementById(`initial_${r.id}`);
             i != null && i.textContent ? (this.uploadedFiles = this.initialData = [JSON.parse(i.textContent)], this.renderDropbox()) : this.uploadedFiles = this.initialData = [], this.dropbox.addEventListener("dragenter", this.swallowEvent), this.dropbox.addEventListener("dragover", this.swallowEvent), this.dropbox.addEventListener("drop", this.fileDrop), this.chooseFileButton.addEventListener("click", () => {
                 r.click()
             }), r.addEventListener("change", () => this.uploadFiles(this.inputElement.files).then(() => {
                 this.fieldGroup.inputted(), this.fieldGroup.validate()
@@ -1918,27 +1918,27 @@
                     n()
                 }) : n()
             })
         }
         async uploadFile(e, r) {
             let n = this;
 
-            function i(l) {
-                let c = l.lengthComputable ? l.loaded / l.total : 0;
+            function i(a) {
+                let c = a.lengthComputable ? a.loaded / a.total : 0;
                 n.progressBar && (n.progressBar.style.visibility = "visible", n.progressBar.value = .97 * c)
             }
             let o = new FormData;
-            return o.append("temp_file", e), o.append("image_height", r.toString()), new Promise((l, c) => {
+            return o.append("temp_file", e), o.append("image_height", r.toString()), new Promise((a, c) => {
                 function u() {
-                    n.progressBar && (n.progressBar.value = 1, window.setTimeout(() => n.progressBar.style.visibility = "hidden", 333)), a.status === 200 ? l(a.response) : c(a.response)
+                    n.progressBar && (n.progressBar.value = 1, window.setTimeout(() => n.progressBar.style.visibility = "hidden", 333)), s.status === 200 ? a(s.response) : c(s.response)
                 }
-                let a = new XMLHttpRequest;
-                n.progressBar && (a.addEventListener("loadstart", i), a.upload.addEventListener("progress", i, !1)), a.addEventListener("loadend", u), a.open("POST", this.fieldGroup.form.formset.endpoint, !0);
-                let m = this.fieldGroup.form.formset.CSRFToken;
-                m && a.setRequestHeader("X-CSRFToken", m), a.responseType = "json", a.send(o)
+                let s = new XMLHttpRequest;
+                n.progressBar && (s.addEventListener("loadstart", i), s.upload.addEventListener("progress", i, !1)), s.addEventListener("loadend", u), s.open("POST", this.fieldGroup.form.formset.endpoint, !0);
+                let p = this.fieldGroup.form.formset.CSRFToken;
+                p && s.setRequestHeader("X-CSRFToken", p), s.responseType = "json", s.send(o)
             })
         }
         renderDropbox() {
             let e = [];
             for (let n of this.uploadedFiles) e.push(this.dropboxItemTemplate(n));
             e.length > 0 ? this.dropbox.innerHTML = e.join("") : this.dropbox.replaceChildren(this.emptyDropboxItem);
             let r = this.dropbox.querySelector(".dj-delete-file");
@@ -1953,508 +1953,509 @@
             return !!this.inputElement.files && this.inputElement.files.length > 0 && !this.uploadedFiles.length
         }
         resetToInitial() {
             this.uploadedFiles = this.initialData, this.renderDropbox()
         }
     };
 
-function nr(t, e, r) {
+function ir(t, e, r) {
     return r = r || " ", t.length > e ? t : (e -= t.length, r += r.repeat(e), t + r.slice(0, e))
 }
 var Re = class t extends Error {
     constructor(r, n, i, o) {
         super();
         this.message = r, this.expected = n, this.found = i, this.location = o, this.name = "SyntaxError", typeof Object.setPrototypeOf == "function" ? Object.setPrototypeOf(this, t.prototype) : this.__proto__ = t.prototype, typeof Error.captureStackTrace == "function" && Error.captureStackTrace(this, t)
     }
     static buildMessage(r, n) {
-        function i(m) {
-            return m.charCodeAt(0).toString(16).toUpperCase()
+        function i(p) {
+            return p.charCodeAt(0).toString(16).toUpperCase()
         }
 
-        function o(m) {
-            return m.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
+        function o(p) {
+            return p.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
         }
 
-        function l(m) {
-            return m.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
+        function a(p) {
+            return p.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
         }
 
-        function c(m) {
-            switch (m.type) {
+        function c(p) {
+            switch (p.type) {
                 case "literal":
-                    return '"' + o(m.text) + '"';
+                    return '"' + o(p.text) + '"';
                 case "class":
-                    let j = m.parts.map(A => Array.isArray(A) ? l(A[0]) + "-" + l(A[1]) : l(A));
-                    return "[" + (m.inverted ? "^" : "") + j + "]";
+                    let j = p.parts.map(A => Array.isArray(A) ? a(A[0]) + "-" + a(A[1]) : a(A));
+                    return "[" + (p.inverted ? "^" : "") + j + "]";
                 case "any":
                     return "any character";
                 case "end":
                     return "end of input";
                 case "other":
-                    return m.description
+                    return p.description
             }
         }
 
-        function u(m) {
-            let j = m.map(c),
-                A, L;
+        function u(p) {
+            let j = p.map(c),
+                A, $;
             if (j.sort(), j.length > 0) {
-                for (A = 1, L = 1; A < j.length; A++) j[A - 1] !== j[A] && (j[L] = j[A], L++);
-                j.length = L
+                for (A = 1, $ = 1; A < j.length; A++) j[A - 1] !== j[A] && (j[$] = j[A], $++);
+                j.length = $
             }
             switch (j.length) {
                 case 1:
                     return j[0];
                 case 2:
                     return j[0] + " or " + j[1];
                 default:
                     return j.slice(0, -1).join(", ") + ", or " + j[j.length - 1]
             }
         }
 
-        function a(m) {
-            return m ? '"' + o(m) + '"' : "end of input"
+        function s(p) {
+            return p ? '"' + o(p) + '"' : "end of input"
         }
-        return "Expected " + u(r) + " but " + a(n) + " found."
+        return "Expected " + u(r) + " but " + s(n) + " found."
     }
     format(r) {
         let n = "Error: " + this.message;
         if (this.location) {
             let i = null,
                 o;
             for (o = 0; o < r.length; o++)
                 if (r[o].source === this.location.source) {
                     i = r[o].text.split(/\r\n|\n|\r/g);
                     break
-                } let l = this.location.start,
-                c = this.location.source + ":" + l.line + ":" + l.column;
+                } let a = this.location.start,
+                c = this.location.source + ":" + a.line + ":" + a.column;
             if (i) {
                 let u = this.location.end,
-                    a = nr("", l.line.toString().length, " "),
-                    m = i[l.line - 1],
-                    j = l.line === u.line ? u.column : m.length + 1;
+                    s = ir("", a.line.toString().length, " "),
+                    p = i[a.line - 1],
+                    j = a.line === u.line ? u.column : p.length + 1;
                 n += `
  --> ` + c + `
-` + a + ` |
-` + l.line + " | " + m + `
-` + a + " | " + nr("", l.column - 1, " ") + nr("", j - l.column, "^")
+` + s + ` |
+` + a.line + " | " + p + `
+` + s + " | " + ir("", a.column - 1, " ") + ir("", j - a.column, "^")
             } else n += `
  at ` + c
         }
         return n
     }
 };
 
-function Fl(t, e) {
+function _l(t, e) {
     e = e !== void 0 ? e : {};
     let r = {},
         n = e.grammarSource,
         i = {
-            Actions: 5,
-            Expression: 0
+            Actions: 8,
+            Expression: 0,
+            InduceExpression: 5
         },
-        o = 5,
-        l = [function(p, d) {
-            return d.reduce(function(s, F) {
-                return s + F[1] + F[3]
-            }, p)
+        o = 8,
+        a = [function(m, d) {
+            return d.reduce((l, F) => l + F[1] + F[3], m)
         }, function() {
             return "false"
-        }, "===", b("===", !1), "==", b("==", !1), "!==", b("!==", !1), "!=", b("!=", !1), "<=", b("<=", !1), ">=", b(">=", !1), "<", b("<", !1), ">", b(">", !1), "+", b("+", !1), "-", b("-", !1), "*", b("*", !1), "/", b("/", !1), "&&", b("&&", !1), "&", b("&", !1), "||", b("||", !1), "|", b("|", !1), "!", b("!", !1), "(", b("(", !1), ")", b(")", !1), function(p) {
-            return "(" + p + ")"
-        }, function(p) {
-            return "'" + p + "'"
-        }, function(p) {
-            return "this.getDataValue([" + p.split(".").map(s => "'" + s + "'").join(",") + "])"
-        }, "!~", b("!~", !1), function(p, d) {
+        }, "===", b("===", !1), "==", b("==", !1), "!==", b("!==", !1), "!=", b("!=", !1), "<=", b("<=", !1), ">=", b(">=", !1), "<", b("<", !1), ">", b(">", !1), "+", b("+", !1), "-", b("-", !1), "*", b("*", !1), "/", b("/", !1), "&&", b("&&", !1), "&", b("&", !1), "||", b("||", !1), "|", b("|", !1), "!", b("!", !1), "(", b("(", !1), ")", b(")", !1), function(m) {
+            return `(${m})`
+        }, function(m) {
+            return `this.getDataValue([${m.split(".").map(l=>`'${l}'`).join(",")}])`
+        }, ":", b(":", !1), function(m, d) {
+            return `this.isButtonActive([${m.split(".").map(F=>`'${F}'`).join(",")}],'${d}')`
+        }, "!~", b("!~", !1), function(m, d) {
             return {
-                successChain: p,
+                successChain: m,
                 rejectChain: d
             }
-        }, function(p) {
+        }, function(m) {
             return {
-                successChain: p,
+                successChain: m,
                 rejectChain: []
             }
-        }, "->", b("->", !1), function(p, d) {
-            return [p].concat(d)
-        }, function(p) {
-            return [p]
-        }, function(p, d) {
+        }, "->", b("->", !1), function(m, d) {
+            return [m].concat(d)
+        }, function(m) {
+            return [m]
+        }, function(m, d) {
             return {
-                funcname: p,
+                funcname: m,
                 args: d
             }
-        }, "()", b("()", !1), function(p) {
+        }, "()", b("()", !1), function(m) {
             return {
-                funcname: p,
+                funcname: m,
                 args: []
             }
-        }, ",", b(",", !1), function(p) {
-            return [p]
+        }, function(m) {
+            return `'${m}'`
+        }, ",", b(",", !1), function(m) {
+            return [m]
         }, /^[ \t\n\r]/, _([" ", "	", `
-`, "\r"], !1, !1), "[", b("[", !1), "{", b("{", !1), "]", b("]", !1), "}", b("}", !1), ":", b(":", !1), function(p, d) {
+`, "\r"], !1, !1), "[", b("[", !1), "{", b("{", !1), "]", b("]", !1), "}", b("}", !1), function(m, d) {
             return d
-        }, function(p, d) {
-            var s = {};
-            return [p].concat(d).forEach(function(F) {
-                s[F.name] = F.value
-            }), s
-        }, function(p) {
-            return p !== null ? p : {}
-        }, function(p, d) {
+        }, function(m, d) {
+            var l = {};
+            return [m].concat(d).forEach(function(F) {
+                l[F.name] = F.value
+            }), l
+        }, function(m) {
+            return m !== null ? m : {}
+        }, function(m, d) {
             return {
-                name: p,
+                name: m,
                 value: d
             }
         }, /^[$A-Za-z_]/, _(["$", ["A", "Z"],
             ["a", "z"], "_"
         ], !1, !1), /^[$0-9A-Za-z_]/, _(["$", ["0", "9"],
             ["A", "Z"],
             ["a", "z"], "_"
-        ], !1, !1), function(p, d) {
+        ], !1, !1), function(m, d) {
             return d
-        }, function(p, d) {
-            return [p].concat(d)
-        }, function(p) {
-            return p !== null ? p : []
-        }, me("number"), function() {
+        }, function(m, d) {
+            return [m].concat(d)
+        }, function(m) {
+            return m !== null ? m : []
+        }, ge("number"), function() {
             return parseFloat(B())
         }, ".", b(".", !1), /^[1-9]/, _([
             ["1", "9"]
-        ], !1, !1), /^[eE]/, _(["e", "E"], !1, !1), "0", b("0", !1), me("string"), '"', b('"', !1), function(p) {
-            return p
+        ], !1, !1), /^[eE]/, _(["e", "E"], !1, !1), "0", b("0", !1), ge("string"), '"', b('"', !1), function(m) {
+            return m
         }, "'", b("'", !1), /^[^\0-\x1F"\\]/, _([
             ["\0", ""], '"', "\\"
         ], !0, !1), '\\"', b('\\"', !1), function() {
             return '"'
         }, /^[^\0-\x1F'\\]/, _([
             ["\0", ""], "'", "\\"
         ], !0, !1), "\\'", b("\\'", !1), function() {
             return "'"
-        }, "\\\\", b("\\\\", !1), "\\b", b("\\b", !1), "\\f", b("\\f", !1), "\\n", b("\\n", !1), "\\r", b("\\r", !1), "\\t", b("\\t", !1), "\\u", b("\\u", !1), function(p) {
-            return String.fromCharCode(parseInt(p, 16))
-        }, me("boolean"), function() {
+        }, "\\\\", b("\\\\", !1), "\\b", b("\\b", !1), "\\f", b("\\f", !1), "\\n", b("\\n", !1), "\\r", b("\\r", !1), "\\t", b("\\t", !1), "\\u", b("\\u", !1), function(m) {
+            return String.fromCharCode(parseInt(m, 16))
+        }, ge("boolean"), function() {
             return !0
         }, function() {
             return !1
         }, function() {
             return null
-        }, "false", b("false", !1), "true", b("true", !1), "null", b("null", !1), function(p, d) {
-            return d.reduce(function(s, F) {
-                return s + "." + F[1]
-            }, p)
-        }, "...", b("...", !1), "..", b("..", !1), function(p, d) {
-            return p + d
-        }, function(p, d) {
-            return p + d
+        }, "false", b("false", !1), "true", b("true", !1), "null", b("null", !1), function(m, d) {
+            return d.reduce(function(l, F) {
+                return l + "." + F[1]
+            }, m)
+        }, "...", b("...", !1), "..", b("..", !1), function(m, d) {
+            return m + d
+        }, function(m, d) {
+            return m + d
         }, /^[$a-zA-Z_]/, _(["$", ["a", "z"],
             ["A", "Z"], "_"
         ], !1, !1), /^[$a-zA-Z0-9_]/, _(["$", ["a", "z"],
             ["A", "Z"],
             ["0", "9"], "_"
-        ], !1, !1), function(p) {
-            return p instanceof Array ? p.join("") : p
+        ], !1, !1), function(m) {
+            return m instanceof Array ? m.join("") : m
         }, /^[0-9]/, _([
             ["0", "9"]
         ], !1, !1), /^[0-9a-f]/i, _([
             ["0", "9"],
             ["a", "f"]
         ], !1, !0)],
-        c = [y(`%;*/\x9E#;#/\x95$;*/\x8C$$%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#0H*%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#&/2$;*/)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;*/& 8!:!! )`), y(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), y('2B""6B7C'), y(`%2D""6D7E/R#;*/I$; /@$;*/7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.A &;6.; &;D.5 &;$./ &%;@/' 8!:I!! )`), y("%;H/' 8!:J!! )"), y(`%;&/\\#;*/S$2K""6K7L/D$;*/;$;&/2$;*/)$8&:M&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;&/' 8!:N!! )`), y(`%;'/\\#;*/S$2O""6O7P/D$;*/;$;&/2$;*/)$8&:Q&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;'/' 8!:R!! )`), y(`%;*/i#%;4/"!&,)/Y$2D""6D7E/J$;(/A$2F""6F7G/2$;*/)$8&:S&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;4/"!&,)/7#2T""6T7U/($8":V"!!)("'#&'#.6 &%%;4/"!&,)/' 8!:V!! )`), y(`%;)/S#;*/J$2W""6W7X/;$;*/2$;(/)$8%:Q%"$ )(%'#($'#(#'#("'#&'#./ &%;)/' 8!:Y!! )`), y(";6./ &;@.) &;2.# &;5"), y('$4Z""5!7[0)*4Z""5!7[&'), y(`%;*/;#2\\""6\\7]/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2^""6^7_/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2\`""6\`7a/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2b""6b7c/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2d""6d7e/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2W""6W7X/,$;*/#$+#)(#'#("'#&'#`), y(";D.5 &;2./ &;5.) &;6.# &;@"), y(`%;,/\x91#%;3/k#$%;0/2#;3/)$8":f""$ )("'#&'#0<*%;0/2#;3/)$8":f""$ )("'#&'#&/)$8":g""! )("'#&'#." &"/1$;./($8#:h#!!)(#'#("'#&'#`), y(`%;@/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#.L &%%;4/"!&,)/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#`), y(`%4j""5!7k/?#$4l""5!7m0)*4l""5!7m&/#$+")("'#&'#`), y(`%;+/\x91#%;1/k#$%;0/2#;1/)$8":n""$ )("'#&'#0<*%;0/2#;1/)$8":n""$ )("'#&'#&/)$8":o""! )("'#&'#." &"/1$;-/($8#:p#!!)(#'#("'#&'#`), y(`<%;=." &"/L#;</C$;;." &"/5$;:." &"/'$8$:r$ )($'#(#'#("'#&'#=." 7q`), y('2s""6s7t'), y('4u""5!7v'), y('4w""5!7x'), y(`%;9/M#;=.# &;>." &"/9$$;M/&#0#*;M&&&#/#$+#)(#'#("'#&'#`), y(`%;7/9#$;M/&#0#*;M&&&#/#$+")("'#&'#`), y(`;?.= &%;8/3#$;M0#*;M&/#$+")("'#&'#`), y('24""6475'), y('22""6273'), y('2y""6y7z'), y(`<%2|""6|7}/N#%$;A0#*;A&/"!&,)/7$2|""6|7}/($8#:~#!!)(#'#("'#&'#.^ &%2\x7F""6\x7F7\x80/N#%$;B0#*;B&/"!&,)/7$2\x7F""6\x7F7\x80/($8#:~#!!)(#'#("'#&'#=." 7{`), y('4\x81""5!7\x82.: &%2\x83""6\x837\x84/& 8!:\x85! ).# &;C'), y('4\x86""5!7\x87.: &%2\x88""6\x887\x89/& 8!:\x8A! ).# &;C'), y(`2\x8B""6\x8B7\x8C.\xA9 &2\x8D""6\x8D7\x8E.\x9D &2\x8F""6\x8F7\x90.\x91 &2\x91""6\x917\x92.\x85 &2\x93""6\x937\x94.y &2\x95""6\x957\x96.m &%2\x97""6\x977\x98/]#%%;N/>#;N/5$;N/,$;N/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x99"! )("'#&'#`), y('<%;F/& 8!:\x9B! ).? &%;E/& 8!:\x9C! ).. &%;G/& 8!:\x9D! )=." 7\x9A'), y('2\x9E""6\x9E7\x9F'), y('2\xA0""6\xA07\xA1'), y('2\xA2""6\xA27\xA3'), y(`%;I/\x91#$%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#0O*%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#&/)$8":\xA4""! )("'#&'#`), y(`%2\xA5""6\xA57\xA6.5 &2\xA7""6\xA77\xA8.) &2s""6s7t/2#;J/)$8":\xA9""! )("'#&'#.# &;J`), y(`%;K/2#;L/)$8":\xAA""! )("'#&'#`), y('4\xAB""5!7\xAC'), y(`%$4\xAD""5!7\xAE0)*4\xAD""5!7\xAE&/' 8!:\xAF!! )`), y('4\xB0""5!7\xB1'), y('4\xB2""5!7\xB3')],
+        c = [y(`%;./\x9E#;#/\x95$;./\x8C$$%;./>#;!/5$;./,$; /#$+$)($'#(#'#("'#&'#0H*%;./>#;!/5$;./,$; /#$+$)($'#(#'#("'#&'#&/2$;./)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;./& 8!:!! )`), y(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), y('2B""6B7C'), y(`%2D""6D7E/R#;./I$; /@$;./7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.) &;$.# &;+`), y("%;L/' 8!:I!! )"), y(`%;./\x9E#;&/\x95$;./\x8C$$%;./>#;!/5$;./,$;%/#$+$)($'#(#'#("'#&'#0H*%;./>#;!/5$;./,$;%/#$+$)($'#(#'#("'#&'#&/2$;./)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;./& 8!:!! )`), y(`%2D""6D7E/R#;./I$;%/@$;./7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#./ &;'.) &;$.# &;+`), y(`%;L/A#2J""6J7K/2$;N/)$8#:L#"" )(#'#("'#&'#`), y(`%;)/\\#;./S$2M""6M7N/D$;./;$;)/2$;./)$8&:O&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;)/' 8!:P!! )`), y(`%;*/\\#;./S$2Q""6Q7R/D$;./;$;)/2$;./)$8&:S&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;*/' 8!:T!! )`), y(`%;./i#%;8/"!&,)/Y$2D""6D7E/J$;,/A$2F""6F7G/2$;./)$8&:U&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;8/"!&,)/7#2V""6V7W/($8":X"!!)("'#&'#.6 &%%;8/"!&,)/' 8!:X!! )`), y(";:.5 &;H./ &%;D/' 8!:Y!! )"), y(`%;-/S#;./J$2Z""6Z7[/;$;./2$;,/)$8%:S%"$ )(%'#($'#(#'#("'#&'#./ &%;-/' 8!:\\!! )`), y(";:./ &;D.) &;6.# &;9"), y('$4]""5!7^0)*4]""5!7^&'), y(`%;./;#2_""6_7\`/,$;./#$+#)(#'#("'#&'#`), y(`%;./;#2a""6a7b/,$;./#$+#)(#'#("'#&'#`), y(`%;./;#2c""6c7d/,$;./#$+#)(#'#("'#&'#`), y(`%;./;#2e""6e7f/,$;./#$+#)(#'#("'#&'#`), y(`%;./;#2J""6J7K/,$;./#$+#)(#'#("'#&'#`), y(`%;./;#2Z""6Z7[/,$;./#$+#)(#'#("'#&'#`), y(";H.5 &;6./ &;9.) &;:.# &;D"), y(`%;0/\x91#%;7/k#$%;4/2#;7/)$8":g""$ )("'#&'#0<*%;4/2#;7/)$8":g""$ )("'#&'#&/)$8":h""! )("'#&'#." &"/1$;2/($8#:i#!!)(#'#("'#&'#`), y(`%;D/;#;3/2$;5/)$8#:j#"" )(#'#("'#&'#.L &%%;8/"!&,)/;#;3/2$;5/)$8#:j#"" )(#'#("'#&'#`), y(`%4k""5!7l/?#$4m""5!7n0)*4m""5!7n&/#$+")("'#&'#`), y(`%;//\x91#%;5/k#$%;4/2#;5/)$8":o""$ )("'#&'#0<*%;4/2#;5/)$8":o""$ )("'#&'#&/)$8":p""! )("'#&'#." &"/1$;1/($8#:q#!!)(#'#("'#&'#`), y(`<%;A." &"/L#;@/C$;?." &"/5$;>." &"/'$8$:s$ )($'#(#'#("'#&'#=." 7r`), y('2t""6t7u'), y('4v""5!7w'), y('4x""5!7y'), y(`%;=/M#;A.# &;B." &"/9$$;Q/&#0#*;Q&&&#/#$+#)(#'#("'#&'#`), y(`%;;/9#$;Q/&#0#*;Q&&&#/#$+")("'#&'#`), y(`;C.= &%;</3#$;Q0#*;Q&/#$+")("'#&'#`), y('24""6475'), y('22""6273'), y('2z""6z7{'), y(`<%2}""6}7~/N#%$;E0#*;E&/"!&,)/7$2}""6}7~/($8#:\x7F#!!)(#'#("'#&'#.^ &%2\x80""6\x807\x81/N#%$;F0#*;F&/"!&,)/7$2\x80""6\x807\x81/($8#:\x7F#!!)(#'#("'#&'#=." 7|`), y('4\x82""5!7\x83.: &%2\x84""6\x847\x85/& 8!:\x86! ).# &;G'), y('4\x87""5!7\x88.: &%2\x89""6\x897\x8A/& 8!:\x8B! ).# &;G'), y(`2\x8C""6\x8C7\x8D.\xA9 &2\x8E""6\x8E7\x8F.\x9D &2\x90""6\x907\x91.\x91 &2\x92""6\x927\x93.\x85 &2\x94""6\x947\x95.y &2\x96""6\x967\x97.m &%2\x98""6\x987\x99/]#%%;R/>#;R/5$;R/,$;R/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x9A"! )("'#&'#`), y('<%;J/& 8!:\x9C! ).? &%;I/& 8!:\x9D! ).. &%;K/& 8!:\x9E! )=." 7\x9B'), y('2\x9F""6\x9F7\xA0'), y('2\xA1""6\xA17\xA2'), y('2\xA3""6\xA37\xA4'), y(`%;M/\x91#$%2t""6t7u/?#;N.0 &$;Q/&#0#*;Q&&&#/#$+")("'#&'#0O*%2t""6t7u/?#;N.0 &$;Q/&#0#*;Q&&&#/#$+")("'#&'#&/)$8":\xA5""! )("'#&'#`), y(`%2\xA6""6\xA67\xA7.5 &2\xA8""6\xA87\xA9.) &2t""6t7u/2#;N/)$8":\xAA""! )("'#&'#.# &;N`), y(`%;O/2#;P/)$8":\xAB""! )("'#&'#`), y('4\xAC""5!7\xAD'), y(`%$4\xAE""5!7\xAF0)*4\xAE""5!7\xAF&/' 8!:\xB0!! )`), y('4\xB1""5!7\xB2'), y('4\xB3""5!7\xB4')],
         u = 0,
-        a = 0,
-        m = [{
+        s = 0,
+        p = [{
             line: 1,
             column: 1
         }],
         j = 0,
         A = [],
-        L = 0,
+        $ = 0,
         M;
     if (e.startRule !== void 0) {
         if (!(e.startRule in i)) throw new Error(`Can't start parsing from rule "` + e.startRule + '".');
         o = i[e.startRule]
     }
 
     function B() {
-        return t.substring(a, u)
+        return t.substring(s, u)
     }
 
     function q() {
-        return X(a, u)
+        return J(s, u)
     }
 
-    function G(p, d) {
-        throw d = d !== void 0 ? d : X(a, u), Ce([me(p)], t.substring(a, u), d)
+    function G(m, d) {
+        throw d = d !== void 0 ? d : J(s, u), Te([ge(m)], t.substring(s, u), d)
     }
 
-    function O(p, d) {
-        throw d = d !== void 0 ? d : X(a, u), Ne(p, d)
+    function D(m, d) {
+        throw d = d !== void 0 ? d : J(s, u), Ne(m, d)
     }
 
-    function b(p, d) {
+    function b(m, d) {
         return {
             type: "literal",
-            text: p,
+            text: m,
             ignoreCase: d
         }
     }
 
-    function _(p, d, s) {
+    function _(m, d, l) {
         return {
             type: "class",
-            parts: p,
+            parts: m,
             inverted: d,
-            ignoreCase: s
+            ignoreCase: l
         }
     }
 
-    function xt() {
+    function wt() {
         return {
             type: "any"
         }
     }
 
-    function pe() {
+    function me() {
         return {
             type: "end"
         }
     }
 
-    function me(p) {
+    function ge(m) {
         return {
             type: "other",
-            description: p
+            description: m
         }
     }
 
-    function Be(p) {
-        let d = m[p],
-            s;
+    function Be(m) {
+        let d = p[m],
+            l;
         if (d) return d;
-        for (s = p - 1; !m[s];) s--;
-        for (d = m[s], d = {
+        for (l = m - 1; !p[l];) l--;
+        for (d = p[l], d = {
                 line: d.line,
                 column: d.column
-            }; s < p;) t.charCodeAt(s) === 10 ? (d.line++, d.column = 1) : d.column++, s++;
-        return m[p] = d, d
+            }; l < m;) t.charCodeAt(l) === 10 ? (d.line++, d.column = 1) : d.column++, l++;
+        return p[m] = d, d
     }
 
-    function X(p, d) {
-        let s = Be(p),
+    function J(m, d) {
+        let l = Be(m),
             F = Be(d);
         return {
             source: n,
             start: {
-                offset: p,
-                line: s.line,
-                column: s.column
+                offset: m,
+                line: l.line,
+                column: l.column
             },
             end: {
                 offset: d,
                 line: F.line,
                 column: F.column
             }
         }
     }
 
-    function qe(p) {
-        u < j || (u > j && (j = u, A = []), A.push(p))
+    function qe(m) {
+        u < j || (u > j && (j = u, A = []), A.push(m))
     }
 
-    function Ne(p, d) {
-        return new Re(p, [], "", d)
+    function Ne(m, d) {
+        return new Re(m, [], "", d)
     }
 
-    function Ce(p, d, s) {
-        return new Re(Re.buildMessage(p, d), p, d, s)
+    function Te(m, d, l) {
+        return new Re(Re.buildMessage(m, d), m, d, l)
     }
 
-    function y(p) {
-        return p.split("").map(d => d.charCodeAt(0) - 32)
+    function y(m) {
+        return m.split("").map(d => d.charCodeAt(0) - 32)
     }
 
-    function Ve(p) {
-        let d = c[p],
-            s = 0,
+    function Ve(m) {
+        let d = c[m],
+            l = 0,
             F = [],
-            T = d.length,
+            C = d.length,
             N = [],
             E = [],
-            Te;
+            Ce;
         for (;;) {
-            for (; s < T;) switch (d[s]) {
+            for (; l < C;) switch (d[l]) {
                 case 0:
-                    E.push(l[d[s + 1]]), s += 2;
+                    E.push(a[d[l + 1]]), l += 2;
                     break;
                 case 1:
-                    E.push(void 0), s++;
+                    E.push(void 0), l++;
                     break;
                 case 2:
-                    E.push(null), s++;
+                    E.push(null), l++;
                     break;
                 case 3:
-                    E.push(r), s++;
+                    E.push(r), l++;
                     break;
                 case 4:
-                    E.push([]), s++;
+                    E.push([]), l++;
                     break;
                 case 5:
-                    E.push(u), s++;
+                    E.push(u), l++;
                     break;
                 case 6:
-                    E.pop(), s++;
+                    E.pop(), l++;
                     break;
                 case 7:
-                    u = E.pop(), s++;
+                    u = E.pop(), l++;
                     break;
                 case 8:
-                    E.length -= d[s + 1], s += 2;
+                    E.length -= d[l + 1], l += 2;
                     break;
                 case 9:
-                    E.splice(-2, 1), s++;
+                    E.splice(-2, 1), l++;
                     break;
                 case 10:
-                    E[E.length - 2].push(E.pop()), s++;
+                    E[E.length - 2].push(E.pop()), l++;
                     break;
                 case 11:
-                    E.push(E.splice(E.length - d[s + 1], d[s + 1])), s += 2;
+                    E.push(E.splice(E.length - d[l + 1], d[l + 1])), l += 2;
                     break;
                 case 12:
-                    E.push(t.substring(E.pop(), u)), s++;
+                    E.push(t.substring(E.pop(), u)), l++;
                     break;
                 case 13:
-                    N.push(T), F.push(s + 3 + d[s + 1] + d[s + 2]), E[E.length - 1] ? (T = s + 3 + d[s + 1], s += 3) : (T = s + 3 + d[s + 1] + d[s + 2], s += 3 + d[s + 1]);
+                    N.push(C), F.push(l + 3 + d[l + 1] + d[l + 2]), E[E.length - 1] ? (C = l + 3 + d[l + 1], l += 3) : (C = l + 3 + d[l + 1] + d[l + 2], l += 3 + d[l + 1]);
                     break;
                 case 14:
-                    N.push(T), F.push(s + 3 + d[s + 1] + d[s + 2]), E[E.length - 1] === r ? (T = s + 3 + d[s + 1], s += 3) : (T = s + 3 + d[s + 1] + d[s + 2], s += 3 + d[s + 1]);
+                    N.push(C), F.push(l + 3 + d[l + 1] + d[l + 2]), E[E.length - 1] === r ? (C = l + 3 + d[l + 1], l += 3) : (C = l + 3 + d[l + 1] + d[l + 2], l += 3 + d[l + 1]);
                     break;
                 case 15:
-                    N.push(T), F.push(s + 3 + d[s + 1] + d[s + 2]), E[E.length - 1] !== r ? (T = s + 3 + d[s + 1], s += 3) : (T = s + 3 + d[s + 1] + d[s + 2], s += 3 + d[s + 1]);
+                    N.push(C), F.push(l + 3 + d[l + 1] + d[l + 2]), E[E.length - 1] !== r ? (C = l + 3 + d[l + 1], l += 3) : (C = l + 3 + d[l + 1] + d[l + 2], l += 3 + d[l + 1]);
                     break;
                 case 16:
-                    E[E.length - 1] !== r ? (N.push(T), F.push(s), T = s + 2 + d[s + 1], s += 2) : s += 2 + d[s + 1];
+                    E[E.length - 1] !== r ? (N.push(C), F.push(l), C = l + 2 + d[l + 1], l += 2) : l += 2 + d[l + 1];
                     break;
                 case 17:
-                    N.push(T), F.push(s + 3 + d[s + 1] + d[s + 2]), t.length > u ? (T = s + 3 + d[s + 1], s += 3) : (T = s + 3 + d[s + 1] + d[s + 2], s += 3 + d[s + 1]);
+                    N.push(C), F.push(l + 3 + d[l + 1] + d[l + 2]), t.length > u ? (C = l + 3 + d[l + 1], l += 3) : (C = l + 3 + d[l + 1] + d[l + 2], l += 3 + d[l + 1]);
                     break;
                 case 18:
-                    N.push(T), F.push(s + 4 + d[s + 2] + d[s + 3]), t.substr(u, l[d[s + 1]].length) === l[d[s + 1]] ? (T = s + 4 + d[s + 2], s += 4) : (T = s + 4 + d[s + 2] + d[s + 3], s += 4 + d[s + 2]);
+                    N.push(C), F.push(l + 4 + d[l + 2] + d[l + 3]), t.substr(u, a[d[l + 1]].length) === a[d[l + 1]] ? (C = l + 4 + d[l + 2], l += 4) : (C = l + 4 + d[l + 2] + d[l + 3], l += 4 + d[l + 2]);
                     break;
                 case 19:
-                    N.push(T), F.push(s + 4 + d[s + 2] + d[s + 3]), t.substr(u, l[d[s + 1]].length).toLowerCase() === l[d[s + 1]] ? (T = s + 4 + d[s + 2], s += 4) : (T = s + 4 + d[s + 2] + d[s + 3], s += 4 + d[s + 2]);
+                    N.push(C), F.push(l + 4 + d[l + 2] + d[l + 3]), t.substr(u, a[d[l + 1]].length).toLowerCase() === a[d[l + 1]] ? (C = l + 4 + d[l + 2], l += 4) : (C = l + 4 + d[l + 2] + d[l + 3], l += 4 + d[l + 2]);
                     break;
                 case 20:
-                    N.push(T), F.push(s + 4 + d[s + 2] + d[s + 3]), l[d[s + 1]].test(t.charAt(u)) ? (T = s + 4 + d[s + 2], s += 4) : (T = s + 4 + d[s + 2] + d[s + 3], s += 4 + d[s + 2]);
+                    N.push(C), F.push(l + 4 + d[l + 2] + d[l + 3]), a[d[l + 1]].test(t.charAt(u)) ? (C = l + 4 + d[l + 2], l += 4) : (C = l + 4 + d[l + 2] + d[l + 3], l += 4 + d[l + 2]);
                     break;
                 case 21:
-                    E.push(t.substr(u, d[s + 1])), u += d[s + 1], s += 2;
+                    E.push(t.substr(u, d[l + 1])), u += d[l + 1], l += 2;
                     break;
                 case 22:
-                    E.push(l[d[s + 1]]), u += l[d[s + 1]].length, s += 2;
+                    E.push(a[d[l + 1]]), u += a[d[l + 1]].length, l += 2;
                     break;
                 case 23:
-                    E.push(r), L === 0 && qe(l[d[s + 1]]), s += 2;
+                    E.push(r), $ === 0 && qe(a[d[l + 1]]), l += 2;
                     break;
                 case 24:
-                    a = E[E.length - 1 - d[s + 1]], s += 2;
+                    s = E[E.length - 1 - d[l + 1]], l += 2;
                     break;
                 case 25:
-                    a = u, s++;
+                    s = u, l++;
                     break;
                 case 26:
-                    Te = d.slice(s + 4, s + 4 + d[s + 3]).map(function(Fe) {
+                    Ce = d.slice(l + 4, l + 4 + d[l + 3]).map(function(Fe) {
                         return E[E.length - 1 - Fe]
-                    }), E.splice(E.length - d[s + 2], d[s + 2], l[d[s + 1]].apply(null, Te)), s += 4 + d[s + 3];
+                    }), E.splice(E.length - d[l + 2], d[l + 2], a[d[l + 1]].apply(null, Ce)), l += 4 + d[l + 3];
                     break;
                 case 27:
-                    E.push(Ve(d[s + 1])), s += 2;
+                    E.push(Ve(d[l + 1])), l += 2;
                     break;
                 case 28:
-                    L++, s++;
+                    $++, l++;
                     break;
                 case 29:
-                    L--, s++;
+                    $--, l++;
                     break;
                 default:
-                    throw new Error("Invalid opcode: " + d[s] + ".")
+                    throw new Error("Invalid opcode: " + d[l] + ".")
             }
-            if (N.length > 0) T = N.pop(), s = F.pop();
+            if (N.length > 0) C = N.pop(), l = F.pop();
             else break
         }
         return E[0]
     }
     if (M = Ve(o), M !== r && u === t.length) return M;
-    throw M !== r && u < t.length && qe(pe()), Ce(A, j < t.length ? t.charAt(j) : null, j < t.length ? X(j, j + 1) : X(j, j))
+    throw M !== r && u < t.length && qe(me()), Te(A, j < t.length ? t.charAt(j) : null, j < t.length ? J(j, j + 1) : J(j, j))
 }
-var we = Fl;
-var Zn = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) input[is^=django]:invalid+[role=textbox]:not(.focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=regex]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=regex]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty input[is^=django]:valid+[role=textbox]:not(.focus){border-color:var(--django-formset-color-valid);background-image:var(--django-formset-icon-valid) !important}django-formset [role=group][hidden]{display:none}django-formset [role=group].dj-required>label,django-formset [role=group].dj-required-any>label{font-weight:bolder}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=regex]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=regex]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted input[is^=django]:invalid+[role=textbox]{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted input[is^=django]:focus:invalid+[role=textbox],django-formset [role=group].dj-submitted input[is^=django]:invalid+[role=textbox].focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] input,django-formset [role=group] [role=textbox]{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset [role=group] input[type^=date]{position:relative}django-formset [role=group] input[type^=date]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset [role=group] input[type^=date]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset [role=group] input[type^=date]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset [role=group] select,django-formset [role=group] textarea{background-image:none !important}django-formset [role=group] select.dj-concealed,django-formset [role=group] textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset [role=group] .dj-help-text{font-style:oblique}django-formset [role=group] .dj-form-optgroup{margin-bottom:.5rem}django-formset [role=group] .dj-form-optgroup>em{margin-left:.75rem}django-formset [role=group] .dj-form-inlined{display:inline-block}django-formset [role=group] input[type=file]{width:0 !important;height:0 !important}django-formset [role=group] .dj-control-panel{display:flex}django-formset [role=group] .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset [role=group] .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset [role=group] figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset [role=group] figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset [role=group] figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset [role=group] figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset [role=group] figure.dj-dropbox>figcaption dl dd{margin:0}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset [role=group] .dj-dual-selector{display:flex}django-formset [role=group] .dj-dual-selector .left-column,django-formset [role=group] .dj-dual-selector .right-column,django-formset [role=group] .dj-dual-selector .control-column,django-formset [role=group] .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset [role=group] .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset [role=group] .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset [role=group] .dj-dual-selector select,django-formset [role=group] .dj-dual-selector django-sortable-select{min-width:10rem}django-formset [role=group] .dj-dual-selector select{height:auto}django-formset [role=group] .dj-dual-selector input{z-index:1}django-formset [role=group] .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus){border-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>input,django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>select,django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>django-sortable-select{border-color:var(--django-formset-color-invalid)}django-formset [is^=django-][hidden]{display:block !important;width:0 !important;height:0 !important;padding:0 !important;margin:0 !important;border:none !important;outline:none !important;box-shadow:none !important}django-formset [is^=django-][hidden]::-webkit-calendar-picker-indicator{display:none}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
-var Yn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var fe = _l;
+var ar = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) input[is^=django]:invalid+[role=textbox]:not(.focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=regex]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=regex]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=regex]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=regex]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty input[is^=django]:valid+[role=textbox]:not(.focus){border-color:var(--django-formset-color-valid);background-image:var(--django-formset-icon-valid) !important}django-formset [role=group][hidden]{display:none}django-formset [role=group].dj-required>label,django-formset [role=group].dj-required-any>label{font-weight:bolder}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=regex]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=regex]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted input[is^=django]:invalid+[role=textbox]{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted input[is^=django]:focus:invalid+[role=textbox],django-formset [role=group].dj-submitted input[is^=django]:invalid+[role=textbox].focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] input,django-formset [role=group] [role=textbox]{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset [role=group] input[type^=date]{position:relative}django-formset [role=group] input[type^=date]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset [role=group] input[type^=date]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset [role=group] input[type^=date]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset [role=group] select,django-formset [role=group] textarea{background-image:none !important}django-formset [role=group] select.dj-concealed,django-formset [role=group] textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset [role=group] .dj-help-text{font-style:oblique}django-formset [role=group] .dj-form-optgroup{margin-bottom:.5rem}django-formset [role=group] .dj-form-optgroup>em{margin-left:.75rem}django-formset [role=group] .dj-form-inlined{display:inline-block}django-formset [role=group] input[type=file]{width:0 !important;height:0 !important}django-formset [role=group] .dj-control-panel{display:flex}django-formset [role=group] .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset [role=group] .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset [role=group] figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset [role=group] figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset [role=group] figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset [role=group] figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset [role=group] figure.dj-dropbox>figcaption dl dd{margin:0}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset [role=group] .dj-dual-selector{display:flex}django-formset [role=group] .dj-dual-selector .left-column,django-formset [role=group] .dj-dual-selector .right-column,django-formset [role=group] .dj-dual-selector .control-column,django-formset [role=group] .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset [role=group] .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset [role=group] .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset [role=group] .dj-dual-selector select,django-formset [role=group] .dj-dual-selector django-sortable-select{min-width:10rem}django-formset [role=group] .dj-dual-selector select{height:auto}django-formset [role=group] .dj-dual-selector input{z-index:1}django-formset [role=group] .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus){border-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>input,django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>select,django-formset [role=group] .dj-dual-selector.invalid .right-column:has(>input:focus,>select:focus,>django-sortable-select.focus)>django-sortable-select{border-color:var(--django-formset-color-invalid)}django-formset [is^=django-][hidden]{display:block !important;width:0 !important;height:0 !important;padding:0 !important;margin:0 !important;border:none !important;outline:none !important;box-shadow:none !important}django-formset [is^=django-][hidden]::-webkit-calendar-picker-indicator{display:none}django-formset dialog .dialog-header{cursor:pointer}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
+var eo = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<g class="spinner">
 		<path style="stroke-width:0.729" d="m 12.73285,23.212276 -10e-7,-4.393157 A 0.27932072,0.27932072 0 0 0 12.27476,18.604602 l -2.6367848,2.196577 a 0.27932072,0.27932072 0 0 0 -10e-8,0.429037 l 2.6367859,2.196577 a 0.27932072,0.27932072 0 0 0 0.458089,-0.214517 z" />
 		<path style="stroke-width:0.729" d="m 11.298326,5.191792 -10e-7,-4.39315704 a 0.27932072,0.27932072 0 0 1 0.458086,-0.214519 L 14.393193,2.780699 a 0.27932072,0.27932072 0 0 1 2e-6,0.429033 l -2.636785,2.19658 a 0.27932072,0.27932072 0 0 1 -0.458084,-0.21452 z" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="M 12.5,2.9179688 C 12.333705,2.9010187 12.166975,2.8886442 12,2.8808594 6.9635919,2.8807514 2.8807499,6.9635934 2.8808594,12 c 0.00661,2.530252 1.064217,4.944009 2.9199218,6.664062" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="m 11.458261,21.082031 c 0.166295,0.01695 0.333025,0.02933 0.5,0.03711 C 16.994669,21.119249 21.077511,17.036407 21.077402,12 21.070802,9.469748 20.013185,7.055991 18.15748,5.335938" />
 	</g>
 </svg>
 `;
-var Qn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var to = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<polyline class="path check" fill="none" stroke="currentColor" stroke-width="12" stroke-linecap="round" stroke-miterlimit="10" points="100.2,40.2 51.5,88.8 29.8,67.5 " transform="matrix(0.18,0,0,0.18,-0.284,0.544)" />
 </svg>
 `;
-var eo = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var ro = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12533" stroke-linecap="round" stroke-miterlimit="10" x1="6.562665" y1="7.1626649" x2="17.437328" y2="16.79755" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12534" stroke-linecap="round" stroke-miterlimit="10" x1="17.437338" y1="7.1626701" x2="6.5626698" y2="16.762127" />
 </svg>
 `;
-var Il = "__all__",
-    Ml = "_collection_errors_",
-    Pl = "_marked_for_removal_",
-    io = document.createElement("style");
-io.innerText = Zn;
-document.head.appendChild(io);
-var or = class {
+var Ml = "__all__",
+    Pl = "_collection_errors_",
+    Ol = "_marked_for_removal_",
+    ao = document.createElement("style");
+ao.innerText = ar;
+document.head.appendChild(ao);
+var sr = class {
         constructor(e) {
             this.value = e
         }
     },
-    ir = class {
+    lr = class {
         constructor(e, r) {
-            this.form = e, this.element = r, this.errorPlaceholder = r.querySelector(".dj-errorlist > .dj-placeholder"), this.errorMessages = new Ar(r);
+            this.form = e, this.element = r, this.errorPlaceholder = r.querySelector(".dj-errorlist > .dj-placeholder"), this.errorMessages = new _r(r);
             let n = r.classList.contains("dj-required-any"),
-                i = m => m instanceof HTMLInputElement && m.name && m.form === e.element && m.type !== "hidden",
+                i = p => p instanceof HTMLInputElement && p.name && p.form === e.element && p.type !== "hidden",
                 o = Array.from(r.getElementsByTagName("INPUT")).filter(i);
-            for (let m of o) switch (m.type) {
+            for (let p of o) switch (p.type) {
                 case "checkbox":
                 case "radio":
-                    m.addEventListener("input", () => {
+                    p.addEventListener("input", () => {
                         this.touch(), this.inputted()
-                    }), m.addEventListener("change", () => {
+                    }), p.addEventListener("change", () => {
                         n ? this.validateCheckboxSelectMultiple() : this.validate()
                     });
                     break;
                 case "file":
-                    this.fileUploader = new bt(this, m);
+                    this.fileUploader = new jt(this, p);
                     break;
                 default:
-                    m.addEventListener("focus", () => this.touch()), m.addEventListener("input", () => this.inputted()), m.addEventListener("blur", () => this.validate()), m.addEventListener("invalid", () => this.showErrorMessage(m));
+                    p.addEventListener("focus", () => this.touch()), p.addEventListener("input", () => this.inputted()), p.addEventListener("blur", () => this.validate()), p.addEventListener("invalid", () => this.showErrorMessage(p));
                     break
             }
             this.fieldElements = Array(0).concat(o);
-            let l = m => m instanceof HTMLSelectElement && m.name && m.form === e.element,
-                c = Array.from(r.getElementsByTagName("SELECT")).filter(l).at(0);
+            let a = p => p instanceof HTMLSelectElement && p.name && p.form === e.element,
+                c = Array.from(r.getElementsByTagName("SELECT")).filter(a).at(0);
             c instanceof HTMLSelectElement && (c.addEventListener("focus", () => this.touch()), c.addEventListener("change", () => {
                 this.setDirty(), this.clearCustomError(), this.validate()
             }), c.addEventListener("invalid", () => this.showErrorMessage(c)), this.fieldElements.push(c));
-            let u = m => m instanceof HTMLTextAreaElement && m.name && m.form === e.element,
-                a = Array.from(r.getElementsByTagName("TEXTAREA")).filter(u).at(0);
-            a instanceof HTMLTextAreaElement && (a.addEventListener("focus", () => this.touch()), a.addEventListener("input", () => this.inputted()), a.addEventListener("blur", () => this.validate()), a.addEventListener("invalid", () => this.showErrorMessage(a)), this.fieldElements.push(a)), this.name = this.assertUniqueName(), this.initialDisabled = this.fieldElements.map(m => m.disabled), this.initialRequired = this.fieldElements.map(m => m.required), n ? this.validateCheckboxSelectMultiple() : this.validateBoundField(), this.pristineValue = new or(this.aggregateValue()), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), this.untouch(), this.setPristine()
+            let u = p => p instanceof HTMLTextAreaElement && p.name && p.form === e.element,
+                s = Array.from(r.getElementsByTagName("TEXTAREA")).filter(u).at(0);
+            s instanceof HTMLTextAreaElement && (s.addEventListener("focus", () => this.touch()), s.addEventListener("input", () => this.inputted()), s.addEventListener("blur", () => this.validate()), s.addEventListener("invalid", () => this.showErrorMessage(s)), this.fieldElements.push(s)), this.name = this.assertUniqueName(), this.initialDisabled = this.fieldElements.map(p => p.disabled), this.initialRequired = this.fieldElements.map(p => p.required), n ? this.validateCheckboxSelectMultiple() : this.validateBoundField(), this.pristineValue = new sr(this.aggregateValue()), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), this.untouch(), this.setPristine()
         }
         aggregateValue() {
             var e, r;
             if (this.fieldElements.length === 1) {
                 let n = this.fieldElements[0];
                 if (n.type === "checkbox") return n.checked ? n.value : "";
                 if (n.type === "select-multiple") {
@@ -2473,15 +2474,15 @@
                 let n = [];
                 for (let i of this.fieldElements)
                     if (i.type === "checkbox") i.checked && n.push(i.value);
                     else if (i.type === "radio" && i.checked) return i.value;
                 return n
             }
         }
-        updateOperability() {
+        updateOperability(e) {
             this.updateVisibility(), this.updateDisabled()
         }
         disableRequiredConstraint() {
             this.fieldElements.forEach(e => e.required = !1)
         }
         restoreRequiredConstraint() {
             this.fieldElements.forEach((e, r) => e.required = this.initialRequired[r])
@@ -2492,50 +2493,50 @@
                 if (e === "__undefined__") e = r.name;
                 else if (e !== r.name) throw new Error(`Duplicate name '${e}' on multiple input fields on '${r.name}'`);
             return e
         }
         evalVisibility(e, r) {
             var o;
 
-            function n(l) {
-                return Array.isArray(l) ? l.length !== 0 : !!l
+            function n(a) {
+                return Array.isArray(a) ? a.length !== 0 : !!a
             }
             let i = (o = this.fieldElements[0]) == null ? void 0 : o.getAttribute(e);
             if (typeof i != "string") return null;
             try {
-                let l = new Function(`return ${we(i,{startRule:"Expression"})};`);
+                let a = new Function(`return ${fe(i,{startRule:"Expression"})};`);
                 return () => {
-                    let c = r != n(l.call(this));
-                    this.element.hasAttribute("hidden") !== c && (this.fieldElements.forEach((u, a) => u.disabled = c || this.initialDisabled[a]), this.element.toggleAttribute("hidden", c))
+                    let c = r != n(a.call(this));
+                    this.element.hasAttribute("hidden") !== c && (this.fieldElements.forEach((u, s) => u.disabled = c || this.initialDisabled[s]), this.element.toggleAttribute("hidden", c))
                 }
-            } catch (l) {
-                throw new Error(`Error while parsing <... df-show/hide="${i}">: ${l}.`)
+            } catch (a) {
+                throw new Error(`Error while parsing <... df-show/hide="${i}">: ${a}.`)
             }
         }
         evalDisable() {
             var r;
             let e = (r = this.fieldElements[0]) == null ? void 0 : r.getAttribute("df-disable");
             if (typeof e != "string") return () => {};
             try {
-                let n = new Function("return " + we(e, {
+                let n = new Function("return " + fe(e, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let i = n.call(this);
-                    this.fieldElements.forEach((o, l) => o.disabled = i || this.initialDisabled[l])
+                    this.fieldElements.forEach((o, a) => o.disabled = i || this.initialDisabled[a])
                 }
             } catch (n) {
                 throw new Error(`Error while parsing <... df-disable="${e}">: ${n}.`)
             }
         }
         getDataValue(e) {
             return this.form.getDataValue(e)
         }
         inputted() {
-            (0, ro.default)(this.pristineValue, this.aggregateValue()) ? this.setPristine(): this.setDirty(), this.clearCustomError(), this.form.restoreRequiredConstraints()
+            (0, pr.default)(this.pristineValue, this.aggregateValue()) ? this.setPristine(): this.setDirty(), this.clearCustomError(), this.form.restoreRequiredConstraints()
         }
         clearCustomError() {
             this.form.clearCustomErrors(), this.errorPlaceholder && (this.errorPlaceholder.innerHTML = "");
             for (let e of this.fieldElements) e.validity.customError && e.setCustomValidity("")
         }
         resetToInitial() {
             var e;
@@ -2547,15 +2548,15 @@
         reenableAllFields() {
             this.fieldElements.forEach((e, r) => e.disabled = this.initialDisabled[r])
         }
         touch() {
             this.element.classList.remove("dj-untouched", "dj-validated"), this.element.classList.add("dj-touched")
         }
         untouch() {
-            this.element.classList.remove("dj-submitted", "dj-touched"), this.element.classList.add("dj-untouched")
+            this.element.classList.remove("dj-submitted", "dj-touched"), this.element.classList.add("dj-untouched"), this.errorPlaceholder && (this.errorPlaceholder.innerHTML = "")
         }
         setDirty() {
             this.element.classList.remove("dj-submitted", "dj-pristine"), this.element.classList.add("dj-dirty")
         }
         setPristine() {
             this.element.classList.remove("dj-dirty"), this.element.classList.add("dj-pristine")
         }
@@ -2613,33 +2614,34 @@
         reportCustomError(e) {
             this.errorPlaceholder && (this.errorPlaceholder.innerHTML = e), this.fieldElements[0].setCustomValidity(e)
         }
         reportFailedUpload() {
             this.errorPlaceholder && (this.errorPlaceholder.innerHTML = this.errorMessages.get("badInput") ?? "File upload failed")
         }
     },
-    jt = class {
+    yt = class {
         constructor(e, r) {
             this.func = e, this.args = r
         }
     },
-    ar = class {
-        constructor(e, r) {
+    vt = class {
+        constructor(e, r, n) {
             this.successActions = Array(0);
             this.rejectActions = Array(0);
+            this.path = Array();
             this.clicked = () => {
                 let e;
                 for (let [r, n] of this.successActions.entries()) e ? e = e.then(n.func.apply(this, n.args)) : e = n.func.apply(this, n.args)();
                 if (e) {
                     for (let [r, n] of this.rejectActions.entries()) r === 0 ? e = e.catch(n.func.apply(this, n.args)) : e = e.then(n.func.apply(this, n.args));
                     e.finally(this.restore.apply(this))
                 }
             };
-            var n;
-            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (n = this.decoratorElement) == null ? void 0 : n.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = Yn, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = Qn, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = eo, this.parseActionsQueue(r.getAttribute("df-click")), r.addEventListener("click", this.clicked)
+            var i;
+            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (i = this.decoratorElement) == null ? void 0 : i.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = eo, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = to, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = ro, this.path = n, this.parseActionsQueue(r.getAttribute("df-click")), r.addEventListener("click", this.clicked)
         }
         autoDisable(e) {
             this.isAutoDisabled && (this.element.disabled = !e)
         }
         disable() {
             return e => (this.element.disabled = !0, Promise.resolve(e))
         }
@@ -2728,14 +2730,17 @@
         confirm(e) {
             if (typeof e != "string") throw new Error("The confirm() action requires a message.");
             return r => window.confirm(e) ? Promise.resolve(r) : Promise.reject({})
         }
         alertOnError() {
             return e => (e.status !== 422 && window.alert(e.statusText), Promise.resolve(e))
         }
+        activate(e) {
+            return r => (this.formset.updateOperability(e), Promise.resolve(r))
+        }
         noop() {
             return e => Promise.resolve(e)
         }
         restore() {
             return () => window.setTimeout(() => this.restoreToInitial())
         }
         decorate(e, r) {
@@ -2746,22 +2751,22 @@
                 }, r))
             }
         }
         parseActionsQueue(e) {
             if (!e) return;
             let r = (n, i) => {
                 for (let o of i) {
-                    let l = this[o.funcname];
-                    if (typeof l != "function") throw new Error(`Unknown function '${o.funcname}'.`);
-                    n.push(new jt(l, o.args))
+                    let a = this[o.funcname];
+                    if (typeof a != "function") throw new Error(`Unknown function '${o.funcname}'.`);
+                    n.push(new yt(a, o.args))
                 }
-                n.length === 0 && n.push(new jt(this.noop, []))
+                n.length === 0 && n.push(new yt(this.noop, []))
             };
             try {
-                let n = we(e, {
+                let n = fe(e, {
                     startRule: "Actions"
                 });
                 r(this.successActions, n.successChain), r(this.rejectActions, n.rejectChain)
             } catch (n) {
                 throw new Error(`Error while parsing <button df-click="${e}">: ${n}.`)
             }
         }
@@ -2769,128 +2774,205 @@
             var e;
             this.element.disabled = !1, this.element.setAttribute("class", this.initialClass), this.originalDecorator && ((e = this.decoratorElement) == null || e.replaceChildren(...this.originalDecorator.cloneNode(!0).childNodes))
         }
         abortAction() {
             this.timeoutHandler && (clearTimeout(this.timeoutHandler), this.timeoutHandler = void 0)
         }
     },
-    sr = class {
+    dr = class {
         constructor(e, r) {
             this.form = e, this.element = r, this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable()
         }
         evalVisibility(e, r) {
             let n = this.element.getAttribute(e);
             if (n === null) return null;
             try {
-                let i = new Function(`return ${we(n,{startRule:"Expression"})}`);
+                let i = new Function(`return ${fe(n,{startRule:"Expression"})}`);
                 return () => {
                     let o = r != !!i.call(this);
                     this.element.hasAttribute("hidden") !== o && this.element.toggleAttribute("hidden", o)
                 }
             } catch (i) {
                 throw new Error(`Error while parsing <fieldset df-show/hide="${n}">: ${i}.`)
             }
         }
         evalDisable() {
             let e = this.element.getAttribute("df-disable");
             if (typeof e != "string") return () => {};
             try {
-                let r = new Function(`return ${we(e,{startRule:"Expression"})}`);
+                let r = new Function(`return ${fe(e,{startRule:"Expression"})}`);
                 return () => this.element.disabled = r.call(this)
             } catch (r) {
                 throw new Error(`Error while parsing <fieldset df-disable="${e}">: ${r}.`)
             }
         }
         getDataValue(e) {
             return this.form.getDataValue(e)
         }
-        updateOperability() {
+        updateOperability(e) {
             this.updateVisibility(), this.updateDisabled()
         }
     },
-    lr = class {
+    cr = class {
+        constructor(e, r) {
+            this.baseSelector = 'dialog[is="django-dialog-form"]';
+            this.dialogRect = null;
+            this.dialogOffsetX = 0;
+            this.dialogOffsetY = 0;
+            this.openDialog = () => {
+                this.element.open || (this.form.setPristine(), this.form.untouch(), this.element.show(), this.dialogHeaderElement && !this.dialogRect && (this.dialogRect = this.element.getBoundingClientRect(), this.dialogHeaderElement.addEventListener("pointerdown", this.handlePointerDown), this.dialogHeaderElement.addEventListener("touchstart", this.handlePointerDown)))
+            };
+            this.closeDialog = e => {
+                switch (e) {
+                    case "apply":
+                        this.form.isValid() && this.element.close(e);
+                        break;
+                    case "close":
+                        this.element.close(e);
+                        break;
+                    case "reset":
+                        this.form.resetToInitial();
+                        break;
+                    default:
+                        break
+                }
+            };
+            this.handlePointerDown = e => {
+                let r = window.visualViewport,
+                    n, i, o = (p, j) => {
+                        this.dialogOffsetX = Math.max(p - n, -this.dialogRect.left), this.dialogOffsetY = Math.max(j - i, -this.dialogRect.top), this.dialogOffsetX = Math.min(this.dialogOffsetX, r.width - this.dialogRect.right), this.dialogOffsetY = Math.min(this.dialogOffsetY, r.height - this.dialogRect.bottom), this.element.style.transform = `translate(${this.dialogOffsetX}px, ${this.dialogOffsetY}px)`
+                    },
+                    a = p => {
+                        o(p.clientX, p.clientY)
+                    },
+                    c = p => {
+                        p.preventDefault(), o(p.touches[0].clientX, p.touches[0].clientY)
+                    },
+                    u = p => {
+                        this.dialogHeaderElement.releasePointerCapture(p.pointerId), this.dialogHeaderElement.removeEventListener("pointermove", a)
+                    },
+                    s = p => {
+                        this.dialogHeaderElement.removeEventListener("touchmove", c)
+                    };
+                e instanceof PointerEvent ? (n = e.clientX - this.dialogOffsetX, i = e.clientY - this.dialogOffsetY, this.dialogHeaderElement.setPointerCapture(e.pointerId), this.dialogHeaderElement.addEventListener("pointermove", a), this.dialogHeaderElement.addEventListener("pointerup", u, {
+                    once: !0
+                })) : (n = e.touches[0].clientX - this.dialogOffsetX, i = e.touches[0].clientY - this.dialogOffsetY, this.dialogHeaderElement.addEventListener("touchmove", c), this.dialogHeaderElement.addEventListener("touchend", s, {
+                    once: !0
+                }))
+            };
+            if (this.form = e, this.element = r, this.formElement = this.element.querySelector('form[method="dialog"]'), !this.formElement) throw new Error(`${this} requires child <form method="dialog">`);
+            this.dialogHeaderElement = this.element.querySelector(".dialog-header"), Ze.stylesAreInstalled(this.baseSelector) || this.transferStyles(), this.induceOpen = this.evalInducer("df-induce-open", this.openDialog), this.induceClose = this.evalInducer("df-induce-close", this.closeDialog)
+        }
+        evalInducer(e, r) {
+            var i;
+            let n = (i = this.element) == null ? void 0 : i.getAttribute(e);
+            if (typeof n != "string") return () => {};
+            try {
+                let o = new Function(`return ${fe(n,{startRule:"InduceExpression"})}`);
+                return a => {
+                    o.call(this) && r(a)
+                }
+            } catch (o) {
+                throw new Error(`Error while parsing <dialog ${e}="${n}">: ${o}.`)
+            }
+        }
+        transferStyles() {
+            let e = document.createElement("style");
+            if (e.innerText = ar, document.head.appendChild(e), !e.sheet) throw new Error("Could not create <style> element")
+        }
+        getDataValue(e) {
+            return this.form.getDataValue(e)
+        }
+        isButtonActive(e, r) {
+            let n = this.form.formset.buttons.find(i => (0, pr.default)(i.path, e));
+            return r === "active" && (n == null ? void 0 : n.element) === document.activeElement
+        }
+        updateOperability(e) {
+            this.induceOpen(e), this.induceClose(e)
+        }
+    },
+    ur = class {
         constructor(e, r) {
             this.errorList = null;
             this.errorPlaceholder = null;
             this.fieldGroups = Array(0);
             this.hiddenInputFields = Array(0);
             this.markedForRemoval = !1;
             this.handleSubmit = e => {
                 e.target instanceof HTMLFormElement && e.target.method === "dialog" || e.preventDefault()
             };
             this.handleReset = () => {
                 for (let e of this.fieldGroups) e.resetToInitial()
             };
-            var o, l;
-            this.formset = e, this.element = r, this.path = ((o = this.name) == null ? void 0 : o.split(".")) ?? [];
+            var a, c;
+            this.formset = e, this.element = r, this.path = ((a = this.name) == null ? void 0 : a.split(".")) ?? [];
             let n = r.nextSibling;
-            this.fieldset = n instanceof HTMLFieldSetElement && n.form === r ? new sr(this, n) : null;
-            let i = (l = r.nextElementSibling) == null ? void 0 : l.querySelector(".dj-form-errors > .dj-errorlist > .dj-placeholder");
-            i && (this.errorList = i.parentElement, this.errorPlaceholder = this.errorList.removeChild(i)), this.element.addEventListener("submit", this.handleSubmit), this.element.addEventListener("reset", this.handleReset)
+            this.fieldset = n instanceof HTMLFieldSetElement && n.form === r ? new dr(this, n) : null;
+            let i = (c = r.nextElementSibling) == null ? void 0 : c.querySelector(".dj-form-errors > .dj-errorlist > .dj-placeholder");
+            i && (this.errorList = i.parentElement, this.errorPlaceholder = this.errorList.removeChild(i));
+            let o = r.closest("dialog");
+            this.parentDialog = o ? new cr(this, o) : null, this.isTransient = this.element.getAttribute("df-transient") === "true", this.element.addEventListener("submit", this.handleSubmit), this.element.addEventListener("reset", this.handleReset)
         }
         aggregateValues() {
             let e = new Map;
             for (let r of this.fieldGroups) e.set(r.name, r.aggregateValue());
             for (let r of this.hiddenInputFields.filter(n => n.type === "hidden")) e.set(r.name, r.value);
             return e
         }
         get name() {
             return this.element.getAttribute("name")
         }
         get formId() {
             return this.element.getAttribute("id")
         }
-        get provideData() {
-            return this.element.method !== "dialog"
-        }
         getAbsPath() {
             return ["formset_data", ...this.path]
         }
         getDataValue(e) {
             if (e[0] !== "") return this.formset.getDataValue(e);
             let r = [...this.path],
                 n = e.filter(o => o !== ""),
                 i = e.length - n.length;
             return r.splice(r.length - i + 1), r.push(...n), this.formset.getDataValue(r)
         }
-        updateOperability() {
-            var e;
-            (e = this.fieldset) == null || e.updateOperability(), this.fieldGroups.forEach(r => r.updateOperability())
+        updateOperability(e) {
+            var r, n;
+            (r = this.fieldset) == null || r.updateOperability(e), this.fieldGroups.forEach(i => i.updateOperability(e)), (n = this.parentDialog) == null || n.updateOperability(e)
         }
         setSubmitted() {
             this.fieldGroups.forEach(e => e.setSubmitted())
         }
         validate() {
             this.formset.validate()
         }
         isValid() {
-            if (this.element.noValidate || !this.provideData) return !0;
+            if (this.element.noValidate || this.isTransient) return !0;
             let e = !0;
             for (let r of this.fieldGroups) e = r.setValidationError() && e;
             return e
         }
         checkValidity() {
-            return this.element.noValidate || !this.provideData ? !0 : this.element.checkValidity()
+            return this.element.noValidate || this.isTransient ? !0 : this.element.checkValidity()
         }
         reportValidity() {
-            this.element.noValidate || !this.provideData || this.element.reportValidity()
+            this.element.noValidate || this.isTransient || this.element.reportValidity()
         }
         clearCustomErrors() {
             for (; this.errorList && this.errorList.lastChild;) this.errorList.removeChild(this.errorList.lastChild)
         }
         resetToInitial() {
             this.element.reset()
         }
         toggleForRemoval(e) {
             this.markedForRemoval = e;
             for (let r of this.fieldGroups) e ? (r.resetToInitial(), r.disableAllFields()) : r.reenableAllFields()
         }
         reportCustomErrors(e) {
             this.clearCustomErrors();
-            let r = e.get(Il);
+            let r = e.get(Ml);
             if (this.errorList && r instanceof Array && this.errorPlaceholder)
                 for (let n of r) {
                     let i = this.errorPlaceholder.cloneNode();
                     i.innerHTML = n, this.errorList.appendChild(i)
                 }
             for (let n of this.fieldGroups) {
                 let i = e.get(n.name);
@@ -2900,36 +2982,42 @@
         findFirstErrorReport() {
             var e, r;
             if ((e = this.errorList) != null && e.textContent) return this.element;
             for (let n of this.fieldGroups)
                 if ((r = n.errorPlaceholder) != null && r.textContent) return n.element;
             return null
         }
+        untouch() {
+            this.fieldGroups.forEach(e => e.untouch())
+        }
+        setPristine() {
+            this.fieldGroups.forEach(e => e.setPristine())
+        }
         get isPristine() {
             return this.fieldGroups.every(e => e.isPristine)
         }
         disableRequiredConstraints() {
             this.fieldGroups.forEach(e => e.disableRequiredConstraint())
         }
         restoreRequiredConstraints() {
             this.fieldGroups.forEach(e => e.restoreRequiredConstraint())
         }
     },
-    fe = class t {
+    pe = class t {
         constructor(e, r, n) {
             this.forms = Array(0);
             this.children = Array(0);
             this.markedForRemoval = !1;
             this.formset = e, this.element = r, this.parent = n, this.findFormCollections()
         }
         findFormCollections() {
             for (let e of t.getChildCollections(this.element)) this.children.push(new t(this.formset, e, this));
-            for (let [e, r] of t.getChildSiblingsCollections(this.element).entries()) this.children.push(new K(this.formset, r, e, this));
+            for (let [e, r] of t.getChildSiblingsCollections(this.element).entries()) this.children.push(new X(this.formset, r, e, this));
             for (let e of this.children) e.updateRemoveButtonAttrs();
-            this.formCollectionTemplate = yt.findFormCollectionTemplate(this.formset, this.element, this)
+            this.formCollectionTemplate = xt.findFormCollectionTemplate(this.formset, this.element, this)
         }
         assignForms(e) {
             this.forms = e.filter(r => {
                 var n;
                 return (n = r.element.parentElement) == null ? void 0 : n.isEqualNode(this.element)
             });
             for (let r of this.children) r.assignForms(e)
@@ -2981,43 +3069,43 @@
             let r = (n = e.querySelector("django-form-collection")) == null ? void 0 : n.parentElement;
             return r ? r.querySelectorAll(":scope > django-form-collection[sibling-position]") : []
         }
         static resetCollectionsToInitial(e) {
             var i;
             let r = Array(0);
             for (let o of e) o.resetToInitial() && r.push(o);
-            r.forEach(o => e.splice(e.indexOf(o), 1)), e.sort((o, l) => o instanceof K && l instanceof K ? o.initialPosition - l.initialPosition : 0);
+            r.forEach(o => e.splice(e.indexOf(o), 1)), e.sort((o, a) => o instanceof X && a instanceof X ? o.initialPosition - a.initialPosition : 0);
             let n = null;
-            for (let o of e) o instanceof K && (o.initialPosition === 0 ? (i = o.element.parentElement) == null || i.insertAdjacentElement("afterbegin", o.element) : n == null || n.insertAdjacentElement("afterend", o.element), n = o.element);
+            for (let o of e) o instanceof X && (o.initialPosition === 0 ? (i = o.element.parentElement) == null || i.insertAdjacentElement("afterbegin", o.element) : n == null || n.insertAdjacentElement("afterend", o.element), n = o.element);
             e.forEach(o => o.repositionSiblings())
         }
     },
-    K = class t extends fe {
+    X = class t extends pe {
         constructor(r, n, i, o) {
             super(r, n, o);
             this.siblingId = 0;
             this.minSiblings = 0;
             this.maxSiblings = null;
             this.justAdded = !1;
             this.removeCollection = () => {
                 var i, o;
                 let r = ((i = this.parent) == null ? void 0 : i.children) ?? this.formset.formCollections;
-                this.justAdded ? (this.disconnect(), r.splice(r.indexOf(this), 1), this.repositionSiblings()) : (this.toggleForRemoval(!this.markedForRemoval), this.removeButton.disabled = !this.markedForRemoval), r.forEach(l => l.updateRemoveButtonAttrs()), (((o = this.parent) == null ? void 0 : o.formCollectionTemplate) ?? this.formset.formCollectionTemplate).updateAddButtonAttrs()
+                this.justAdded ? (this.disconnect(), r.splice(r.indexOf(this), 1), this.repositionSiblings()) : (this.toggleForRemoval(!this.markedForRemoval), this.removeButton.disabled = !this.markedForRemoval), r.forEach(a => a.updateRemoveButtonAttrs()), (((o = this.parent) == null ? void 0 : o.formCollectionTemplate) ?? this.formset.formCollectionTemplate).updateAddButtonAttrs()
             };
-            let l = n.getAttribute("sibling-position");
-            if (!l) throw new Error("Missing argument 'sibling-position' in <django-form-collection>");
-            this.position = this.initialPosition = parseInt(l), this.siblingId = i;
+            let a = n.getAttribute("sibling-position");
+            if (!a) throw new Error("Missing argument 'sibling-position' in <django-form-collection>");
+            this.position = this.initialPosition = parseInt(a), this.siblingId = i;
             let c = n.getAttribute("min-siblings");
             if (!c) throw new Error("Missing argument 'min-siblings' in <django-form-collection>");
             this.minSiblings = parseInt(c);
             let u = n.getAttribute("max-siblings");
             u && (this.maxSiblings = parseInt(u));
-            let a = n.querySelector(":scope > button.remove-collection");
-            if (!a) throw new Error('<django-form-collection> with siblings requires child element <button class="remove-collection">');
-            this.removeButton = a, this.removeButton.addEventListener("click", this.removeCollection)
+            let s = n.querySelector(":scope > button.remove-collection");
+            if (!s) throw new Error('<django-form-collection> with siblings requires child element <button class="remove-collection">');
+            this.removeButton = s, this.removeButton.addEventListener("click", this.removeCollection)
         }
         disconnect() {
             this.removeButton.removeEventListener("click", this.removeCollection), super.disconnect()
         }
         repositionSiblings() {
             var n;
             (((n = this.parent) == null ? void 0 : n.children) ?? this.formset.formCollections).forEach((i, o) => {
@@ -3036,72 +3124,72 @@
         get isFreshAndEmpty() {
             return this.justAdded && super.isFreshAndEmpty
         }
         removeFreshAndEmpty() {
             !this.removeButton.disabled && this.isFreshAndEmpty ? this.removeCollection() : super.removeFreshAndEmpty()
         }
         resetToInitial() {
-            return this.justAdded ? (this.disconnect(), !0) : (super.resetToInitial(), !1)
+            return this.justAdded && !this.element.hasAttribute("fresh-and-empty") ? (this.disconnect(), !0) : (super.resetToInitial(), !1)
         }
     },
-    yt = class t {
+    xt = class t {
         constructor(e, r, n) {
             this.maxSiblings = null;
             this.baseContext = new Map;
             this.markedForRemoval = !1;
             this.resortSiblings = e => {
                 var o;
                 let r = e.oldDraggableIndex ?? NaN,
                     n = e.newDraggableIndex ?? NaN;
                 if (!isFinite(r) || !isFinite(n) || r === n) return;
                 let i = ((o = this.parent) == null ? void 0 : o.children) ?? this.formset.formCollections;
-                if (i.at(r) instanceof K) {
-                    let l = i.splice(r, 1);
-                    i.splice(n, 0, ...l), l.at(0).repositionSiblings();
+                if (i.at(r) instanceof X) {
+                    let a = i.splice(r, 1);
+                    i.splice(n, 0, ...a), a.at(0).repositionSiblings();
                     let c = this.prefix === "0" ? 0 : this.prefix.split(".").length;
-                    i.forEach((u, a) => u.repositionForms(c, a)), this.formset.validate()
+                    i.forEach((u, s) => u.repositionForms(c, s)), this.formset.validate()
                 }
             };
             this.appendFormCollectionSibling = () => {
                 var u;
                 let e = Object.fromEntries(this.baseContext),
                     [r, n] = this.getNextPositionAndSiblingId();
                 e.position = r.toString(), e.siblingId = n.toString(), e.position_1 = "${position}", e.siblingId_1 = "${siblingId}";
-                for (let a = 1; a < 10; ++a) e[`position_${a+1}`] = `\${position_${a}}`, e[`siblingId_${a+1}`] = `\${siblingId_${a}}`;
+                for (let s = 1; s < 10; ++s) e[`position_${s+1}`] = `\${position_${s}}`, e[`siblingId_${s+1}`] = `\${siblingId_${s}}`;
                 let i = this.renderEmptyCollection(e);
                 this.element.insertAdjacentHTML("beforebegin", i);
                 let o = this.element.previousElementSibling;
                 if (!(o instanceof HTMLElement)) throw new Error("Unable to insert empty <django-form-collection> element.");
-                let l = ((u = this.parent) == null ? void 0 : u.children) ?? this.formset.formCollections,
-                    c = new K(this.formset, o, n, this.parent);
-                l.push(c), this.formset.findForms(o), this.formset.assignFieldsToForms(o), this.formset.assignFormsToCollections(), this.formset.findCollectionErrorsList(), c.markAsFreshAndEmpty(!0), this.formset.validate(), l.forEach(a => a.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
+                let a = ((u = this.parent) == null ? void 0 : u.children) ?? this.formset.formCollections,
+                    c = new X(this.formset, o, n, this.parent);
+                a.push(c), this.formset.findForms(o), this.formset.assignFieldsToForms(o), this.formset.assignFormsToCollections(), this.formset.findCollectionErrorsList(), c.markAsFreshAndEmpty(!0), this.formset.validate(), a.forEach(s => s.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
             };
             var u;
             this.formset = e, this.element = r, this.parent = n;
             let i = r.innerHTML.matchAll(/\$\{([^} ]+)\}/g);
-            for (let a of i) this.baseContext.set(a[1], a[0]);
+            for (let s of i) this.baseContext.set(s[1], s[0]);
             let o = r.getAttribute("prefix");
             if (!o) throw new Error('<template class="empty-collection" ...> requires attribute "prefix"');
-            this.prefix = o, e.pushTemplatePrefix(this.prefix), this.renderEmptyCollection = (0, oo.default)(r.innerHTML), (u = r.nextElementSibling) != null && u.matches("button.add-collection") && (this.addButton = r.nextElementSibling, this.addButton.addEventListener("click", this.appendFormCollectionSibling));
-            let l = this.element.content.querySelector("django-form-collection"),
-                c = l == null ? void 0 : l.getAttribute("max-siblings");
-            c && (this.maxSiblings = parseInt(c)), r.hasAttribute("sortable") && new kr(r.parentElement, {
+            this.prefix = o, e.pushTemplatePrefix(this.prefix), this.renderEmptyCollection = (0, io.default)(r.innerHTML), (u = r.nextElementSibling) != null && u.matches("button.add-collection") && (this.addButton = r.nextElementSibling, this.addButton.addEventListener("click", this.appendFormCollectionSibling));
+            let a = this.element.content.querySelector("django-form-collection"),
+                c = a == null ? void 0 : a.getAttribute("max-siblings");
+            c && (this.maxSiblings = parseInt(c)), r.hasAttribute("sortable") && new Fr(r.parentElement, {
                 animation: 150,
                 handle: "django-form-collection[sibling-position]:not(.dj-marked-for-removal) > .collection-drag-handle",
                 draggable: "django-form-collection[sibling-position]",
                 selectedClass: "selected",
                 ghostClass: "dj-ghost-collection",
                 onEnd: this.resortSiblings
             })
         }
         getNextPositionAndSiblingId() {
             let e = -1,
                 r = -1,
                 n = this.parent ? this.parent.children : this.formset.formCollections;
-            for (let i of n.filter(o => o instanceof K)) e = Math.max(e, i.position), r = Math.max(r, i.siblingId);
+            for (let i of n.filter(o => o instanceof X)) e = Math.max(e, i.position), r = Math.max(r, i.siblingId);
             return [e + 1, r + 1]
         }
         disconnect() {
             var e;
             this.formset.popTemplatePrefix(this.prefix), (e = this.addButton) == null || e.removeEventListener("click", this.appendFormCollectionSibling)
         }
         updateAddButtonAttrs() {
@@ -3118,27 +3206,27 @@
             let i = r.querySelector(":scope > .collection-siblings > template.empty-collection");
             if (i) {
                 let o = new t(e, i, n);
                 return o.updateAddButtonAttrs(), o
             }
         }
     },
-    dr = class {
+    fr = class {
         constructor(e) {
             this.buttons = Array(0);
             this.forms = Array(0);
             this.formCollections = Array(0);
             this.collectionErrorsList = new Map;
             this.abortController = new AbortController;
             this.emptyCollectionPrefixes = Array(0);
             this.data = {};
             this.element = e, this.showFeedbackMessages = this.parseWithholdFeedback(), this.CSRFToken = this.element.getAttribute("csrf-token")
         }
         connectedCallback() {
-            this.findButtons(), this.findForms(), this.findFormCollections(), this.findCollectionErrorsList(), this.assignFieldsToForms(), this.assignFormsToCollections(), this.formCollections.forEach(e => e.markAsFreshAndEmpty()), window.setTimeout(() => this.validate(), 0)
+            this.findForms(), this.findFormCollections(), this.findCollectionErrorsList(), this.assignFieldsToForms(), this.assignFormsToCollections(), this.findDetachedButtons(), this.formCollections.forEach(e => e.markAsFreshAndEmpty()), window.setTimeout(() => this.validate(), 0)
         }
         get endpoint() {
             return this.element.getAttribute("endpoint") ?? ""
         }
         get forceSubmission() {
             return this.element.hasAttribute("force-submission")
         }
@@ -3170,114 +3258,132 @@
         }
         popTemplatePrefix(e) {
             let r = this.emptyCollectionPrefixes.indexOf(e);
             r >= 0 && this.emptyCollectionPrefixes.splice(r, 1)
         }
         assignFieldsToForms(e) {
             e = e ?? this.element;
-            for (let r of e.querySelectorAll("INPUT, SELECT, TEXTAREA")) {
+            for (let r of e.querySelectorAll("INPUT, SELECT, TEXTAREA, BUTTON")) {
                 let n = r.getAttribute("form");
                 if (!n) continue;
-                let i = this.forms.filter(c => c.formId && c.formId === n);
+                let i = this.forms.filter(a => a.formId && a.formId === n);
                 if (i.length < 1) continue;
                 if (i.length > 1) throw new Error(`More than one form has id="${n}"`);
-                let o = i[0],
-                    l = r.closest('[role="group"]');
-                l ? o.fieldGroups.filter(c => c.element === l).length === 0 && o.fieldGroups.push(new ir(o, l)) : r instanceof HTMLInputElement && r.type === "hidden" && (o.hiddenInputFields.includes(r) || o.hiddenInputFields.push(r))
+                let o = i[0];
+                if (r instanceof HTMLInputElement && r.type === "hidden") o.hiddenInputFields.includes(r) || o.hiddenInputFields.push(r);
+                else if (r instanceof HTMLButtonElement) {
+                    if (r.hasAttribute("df-click") && r.form === o.element) {
+                        let a = new vt(o.formset, r, [...o.path, r.name]);
+                        this.buttons.push(a)
+                    }
+                } else {
+                    let a = r.closest('[role="group"]');
+                    a && !o.fieldGroups.find(c => c.element === a) && o.fieldGroups.push(new lr(o, a))
+                }
             }
         }
         findForms(e) {
             e = e ?? this.element;
             for (let r of e.getElementsByTagName("FORM")) {
-                let n = new lr(this, r);
+                let n = new ur(this, r);
                 this.forms.push(n)
             }
             this.checkForUniqueness()
         }
         checkForUniqueness() {
-            let e = this.forms.filter(n => n.provideData);
+            let e = this.forms.filter(n => !n.isTransient);
             if (e.length === 1) return;
             let r = Array();
             e.forEach(n => {
                 if (!n.name) throw new Error("Multiple <form>-elements in a <django-formset> require a unique name each.");
                 if (n.name in r) throw new Error(`Duplicate name "${n.name}" used in multiple forms of same <django-formset>.`);
                 r.push(n.name)
             })
         }
         findFormCollections() {
-            for (let e of fe.getChildCollections(this.element)) this.formCollections.push(new fe(this, e));
-            for (let [e, r] of fe.getChildSiblingsCollections(this.element).entries()) this.formCollections.push(new K(this, r, e));
-            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = yt.findFormCollectionTemplate(this, this.element)
+            for (let e of pe.getChildCollections(this.element)) this.formCollections.push(new pe(this, e));
+            for (let [e, r] of pe.getChildSiblingsCollections(this.element).entries()) this.formCollections.push(new X(this, r, e));
+            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = xt.findFormCollectionTemplate(this, this.element)
         }
         findCollectionErrorsList() {
             this.collectionErrorsList.clear();
             for (let e of this.element.getElementsByClassName("dj-collection-errors")) {
                 let r = e.getAttribute("prefix") ?? "",
                     n = e.querySelector("ul.dj-errorlist");
                 this.collectionErrorsList.set(r, n)
             }
         }
-        findButtons() {
-            this.buttons.length = 0;
-            for (let e of this.element.getElementsByTagName("BUTTON")) e.hasAttribute("df-click") && this.buttons.push(new ar(this, e))
+        findDetachedButtons() {
+            for (let e of this.element.getElementsByTagName("BUTTON"))
+                if (e.hasAttribute("df-click")) {
+                    let r = e;
+                    if (!this.buttons.find(n => n.element === r)) {
+                        let n = r.name ? [r.name] : [];
+                        this.buttons.push(new vt(this, r, n))
+                    }
+                }
         }
         assignFormsToCollections() {
             this.formCollections.forEach(e => e.assignForms(this.forms))
         }
         removeForm(e) {
             this.forms.splice(this.forms.indexOf(e), 1)
         }
         removeFreshCollections() {
             Array.from(this.formCollections).reverse().forEach(r => r.removeFreshAndEmpty())
         }
         aggregateValues() {
             this.data = {};
-            for (let e of this.forms) e.provideData && (0, to.default)(this.data, e.getAbsPath(), Object.fromEntries(e.aggregateValues()));
-            for (let e of this.forms) e.markedForRemoval || e.updateOperability()
+            for (let e of this.forms) e.isTransient || (0, no.default)(this.data, e.getAbsPath(), Object.fromEntries(e.aggregateValues()));
+            this.updateOperability()
+        }
+        updateOperability(e) {
+            for (let r of this.forms) r.markedForRemoval || r.updateOperability(e)
         }
         validate() {
             let e = !0;
             for (let r of this.forms) e = (r.markedForRemoval || r.checkValidity()) && e;
             for (let r of this.buttons) r.autoDisable(e);
             return this.aggregateValues(), e
         }
         buildBody(e) {
             let r;
 
-            function n(o, l) {
-                if (l.length === 1) {
-                    Array.isArray(o) ? r && !o.includes(r) && o.push(r) : o[l[0]] = r ?? [];
+            function n(o, a) {
+                if (a.length === 1) {
+                    Array.isArray(o) ? r && !o.includes(r) && o.push(r) : o[a[0]] = r ?? [];
                     return
                 }
-                if (isNaN(parseInt(l[1]))) {
-                    let c = o[l[0]] ?? {};
-                    n(c, l.slice(1));
-                    let u = parseInt(l[0]);
-                    isNaN(u) ? o[l[0]] = c : o[u] = {
+                if (isNaN(parseInt(a[1]))) {
+                    let c = o[a[0]] ?? {};
+                    n(c, a.slice(1));
+                    let u = parseInt(a[0]);
+                    isNaN(u) ? o[a[0]] = c : o[u] = {
                         ...o[u],
                         ...c
                     }
                 } else {
                     if (Array.isArray(o)) throw new Error("Invalid form structure: Contains nested arrays.");
-                    let c = o[l[0]] ?? [];
+                    let c = o[a[0]] ?? [];
                     if (!Array.isArray(c)) throw new Error("Invalid form structure: Inner array is missing.");
-                    n(c, l.slice(1)), o[l[0]] = c
+                    n(c, a.slice(1)), o[a[0]] = c
                 }
             }
             let i = {};
             for (let o of this.emptyCollectionPrefixes) {
-                let l = ["formset_data", ...o.split(".")];
-                r = (0, Ae.default)(i, l), n(i, l)
+                let a = ["formset_data", ...o.split(".")];
+                r = (0, Ae.default)(i, a), n(i, a)
             }
             for (let o of this.forms) {
                 if (!o.name) return Object.assign({}, this.data, {
                     _extra: e
                 });
-                let l = o.getAbsPath();
-                r = (0, Ae.default)(this.data, l), o.markedForRemoval && (r[Pl] = !0), n(i, l)
+                if (o.isTransient) continue;
+                let a = o.getAbsPath();
+                r = (0, Ae.default)(this.data, a), o.markedForRemoval && (r[Ol] = !0), n(i, a)
             }
             return Object.assign({}, i, {
                 _extra: e
             })
         }
         async submit(e) {
             let r = !0;
@@ -3299,44 +3405,44 @@
                     switch (o.status) {
                         case 200:
                             this.clearErrors();
                             for (let c of this.forms) c.element.dispatchEvent(new Event("submitted"));
                             return o;
                         case 422:
                             this.clearErrors();
-                            let l = await o.clone().json();
-                            return this.reportErrors(l), o;
+                            let a = await o.clone().json();
+                            return this.reportErrors(a), o;
                         default:
                             return console.warn(`Unknown response status: ${o.status}`), this.clearErrors(), this.buttons.forEach(c => c.restoreToInitial()), o
                     }
                 } catch (i) {
                     this.clearErrors(), this.buttons.forEach(o => o.restoreToInitial()), alert(i)
                 }
             } else {
                 this.clearErrors();
                 for (let n of this.forms) n.reportValidity()
             }
         }
         reportErrors(e) {
             for (let r of this.forms) {
                 let n = r.name ? (0, Ae.default)(e, r.name.split("."), null) : e;
-                (0, no.default)(n) ? r.clearCustomErrors(): (r.reportCustomErrors(new Map(Object.entries(n))), r.reportValidity())
+                (0, oo.default)(n) ? r.clearCustomErrors(): (r.reportCustomErrors(new Map(Object.entries(n))), r.reportValidity())
             }
             for (let [r, n] of this.collectionErrorsList) {
                 let i = r ? r.split(".") : [];
-                i = [...i, "0", Ml];
+                i = [...i, "0", Pl];
                 for (let o of (0, Ae.default)(e, i, [])) {
-                    let l = document.createElement("li");
-                    l.classList.add("dj-placeholder"), l.innerText = o, n.appendChild(l)
+                    let a = document.createElement("li");
+                    a.classList.add("dj-placeholder"), a.innerText = o, n.appendChild(a)
                 }
             }
         }
         resetToInitial() {
             var e;
-            fe.resetCollectionsToInitial(this.formCollections), (e = this.formCollectionTemplate) == null || e.updateAddButtonAttrs(), this.forms.forEach(r => r.resetToInitial()), this.validate()
+            pe.resetCollectionsToInitial(this.formCollections), (e = this.formCollectionTemplate) == null || e.updateAddButtonAttrs(), this.forms.forEach(r => r.resetToInitial()), this.validate()
         }
         abort() {
             for (let e of this.buttons) e.abortAction();
             this.abortController.abort()
         }
         setSubmitted() {
             for (let e of this.forms) e.setSubmitted()
@@ -3355,18 +3461,18 @@
         clearErrors() {
             for (let e of this.forms) e.clearCustomErrors();
             for (let e of this.collectionErrorsList.values())
                 for (; e.firstElementChild;) e.removeChild(e.firstElementChild)
         }
     },
     ke = Symbol("DjangoFormset"),
-    vt = class extends HTMLElement {
+    Et = class extends HTMLElement {
         constructor() {
             super();
-            this[ke] = new dr(this)
+            this[ke] = new fr(this)
         }
         static get observedAttributes() {
             return ["endpoint", "withhold-feedback", "force-submission"]
         }
         connectedCallback() {
             this[ke].connectedCallback()
         }
@@ -3378,193 +3484,193 @@
         }
         async reset() {
             return this[ke].resetToInitial()
         }
     };
 ke;
 window.addEventListener("DOMContentLoaded", t => {
-    let e = Cr.convertPseudoClasses(),
+    let e = Ze.convertPseudoClasses(),
         r = Array();
 
-    function n(l, c, u, a = void 0) {
-        customElements.get(c) instanceof Function ? l() : (window.customElements.define(c, u, a), window.customElements.whenDefined(c).then(() => l()))
+    function n(a, c, u, s = void 0) {
+        customElements.get(c) instanceof Function ? a() : (window.customElements.define(c, u, s), window.customElements.whenDefined(c).then(() => a()))
     }
 
-    function i(l) {
-        l.querySelector('select[is="django-selectize"]') && r.push(new Promise((c, u) => {
-            import("./DjangoSelectize-ALXOS5DF.js").then(({
-                DjangoSelectizeElement: a
+    function i(a) {
+        a.querySelector('select[is="django-selectize"]') && r.push(new Promise((c, u) => {
+            import("./DjangoSelectize-R66DE3UZ.js").then(({
+                DjangoSelectizeElement: s
             }) => {
-                n(c, "django-selectize", a, {
+                n(c, "django-selectize", s, {
                     extends: "select"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('select[is="django-country-selectize"]') && r.push(new Promise((c, u) => {
-            import("./CountrySelectize-OY7UUXBC.js").then(({
-                CountrySelectizeElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('select[is="django-country-selectize"]') && r.push(new Promise((c, u) => {
+            import("./CountrySelectize-NOGU4FDW.js").then(({
+                CountrySelectizeElement: s
             }) => {
-                n(c, "django-country-selectize", a, {
+                n(c, "django-country-selectize", s, {
                     extends: "select"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector("django-sortable-select") ? r.push(new Promise((c, u) => {
-            import("./SortableSelect-MET5DDXS.js").then(({
-                SortableSelectElement: a
+            }).catch(s => u(s))
+        })), a.querySelector("django-sortable-select") ? r.push(new Promise((c, u) => {
+            import("./SortableSelect-XTYK7VPU.js").then(({
+                SortableSelectElement: s
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? c() : window.customElements.define("django-sortable-select", a), import("./DualSelector-QBPMDGUD.js").then(({
-                    DualSelectorElement: m
+                customElements.get("django-sortable-select") instanceof Function ? c() : window.customElements.define("django-sortable-select", s), import("./DualSelector-RRDODSQ4.js").then(({
+                    DualSelectorElement: p
                 }) => {
-                    customElements.get("django-dual-selector") instanceof Function ? c() : (window.customElements.define("django-dual-selector", m, {
+                    customElements.get("django-dual-selector") instanceof Function ? c() : (window.customElements.define("django-dual-selector", p, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => c()))
-                }).catch(m => u(m))
-            }).catch(a => u(a))
-        })) : l.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((c, u) => {
-            import("./DualSelector-QBPMDGUD.js").then(({
-                DualSelectorElement: a
+                }).catch(p => u(p))
+            }).catch(s => u(s))
+        })) : a.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((c, u) => {
+            import("./DualSelector-RRDODSQ4.js").then(({
+                DualSelectorElement: s
             }) => {
-                n(c, "django-dual-selector", a, {
+                n(c, "django-dual-selector", s, {
                     extends: "select"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-phone-number"]') && r.push(new Promise((c, u) => {
-            import("./PhoneNumber-W7FUG5CI.js").then(({
-                PhoneNumberElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-phone-number"]') && r.push(new Promise((c, u) => {
+            import("./PhoneNumber-SS26COAZ.js").then(({
+                PhoneNumberElement: s
             }) => {
-                n(c, "django-phone-number", a, {
+                n(c, "django-phone-number", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((c, u) => {
-            import("./RichtextArea-7F64YF45.js").then(({
-                RichTextAreaElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((c, u) => {
+            import("./RichtextArea-X76JZ5BK.js").then(({
+                RichTextAreaElement: s
             }) => {
-                n(c, "django-richtext", a, {
+                n(c, "django-richtext", s, {
                     extends: "textarea"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-slug"]') && r.push(new Promise((c, u) => {
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-slug"]') && r.push(new Promise((c, u) => {
             import("./DjangoSlug-SHZN726V.js").then(({
-                DjangoSlugElement: a
+                DjangoSlugElement: s
             }) => {
-                n(c, "django-slug", a, {
+                n(c, "django-slug", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datefield"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateFieldElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datefield"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateFieldElement: s
             }) => {
-                n(c, "django-datefield", a, {
+                n(c, "django-datefield", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datecalendar"]') && r.push(new Promise((c, u) => {
-            import("./Calendar-3E4D43HW.js").then(({
-                DateCalendarElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datecalendar"]') && r.push(new Promise((c, u) => {
+            import("./Calendar-OQTG3ONX.js").then(({
+                DateCalendarElement: s
             }) => {
-                n(c, "django-datecalendar", a, {
+                n(c, "django-datecalendar", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datepicker"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DatePickerElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datepicker"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DatePickerElement: s
             }) => {
-                n(c, "django-datepicker", a, {
+                n(c, "django-datepicker", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimefield"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateTimeFieldElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimefield"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateTimeFieldElement: s
             }) => {
-                n(c, "django-datetimefield", a, {
+                n(c, "django-datetimefield", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimecalendar"]') && r.push(new Promise((c, u) => {
-            import("./Calendar-3E4D43HW.js").then(({
-                DateCalendarElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimecalendar"]') && r.push(new Promise((c, u) => {
+            import("./Calendar-OQTG3ONX.js").then(({
+                DateCalendarElement: s
             }) => {
-                n(c, "django-datetimecalendar", a, {
+                n(c, "django-datetimecalendar", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateTimePickerElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateTimePickerElement: s
             }) => {
-                n(c, "django-datetimepicker", a, {
+                n(c, "django-datetimepicker", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-daterangefield"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateRangeFieldElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-daterangefield"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateRangeFieldElement: s
             }) => {
-                n(c, "django-daterangefield", a, {
+                n(c, "django-daterangefield", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-daterangecalendar"]') && r.push(new Promise((c, u) => {
-            import("./Calendar-3E4D43HW.js").then(({
-                DateCalendarElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-daterangecalendar"]') && r.push(new Promise((c, u) => {
+            import("./Calendar-OQTG3ONX.js").then(({
+                DateCalendarElement: s
             }) => {
-                n(c, "django-daterangecalendar", a, {
+                n(c, "django-daterangecalendar", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-daterangepicker"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateRangePickerElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-daterangepicker"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateRangePickerElement: s
             }) => {
-                n(c, "django-daterangepicker", a, {
+                n(c, "django-daterangepicker", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimerangefield"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateTimeRangeFieldElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimerangefield"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateTimeRangeFieldElement: s
             }) => {
-                n(c, "django-datetimerangefield", a, {
+                n(c, "django-datetimerangefield", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimerangecalendar"]') && r.push(new Promise((c, u) => {
-            import("./Calendar-3E4D43HW.js").then(({
-                DateCalendarElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimerangecalendar"]') && r.push(new Promise((c, u) => {
+            import("./Calendar-OQTG3ONX.js").then(({
+                DateCalendarElement: s
             }) => {
-                n(c, "django-datetimerangecalendar", a, {
+                n(c, "django-datetimerangecalendar", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
-        })), l.querySelector('input[is="django-datetimerangepicker"]') && r.push(new Promise((c, u) => {
-            import("./DateTime-2CEEHEI3.js").then(({
-                DateTimeRangePickerElement: a
+            }).catch(s => u(s))
+        })), a.querySelector('input[is="django-datetimerangepicker"]') && r.push(new Promise((c, u) => {
+            import("./DateTime-WMTYZZNN.js").then(({
+                DateTimeRangePickerElement: s
             }) => {
-                n(c, "django-datetimerangepicker", a, {
+                n(c, "django-datetimerangepicker", s, {
                     extends: "input"
                 })
-            }).catch(a => u(a))
+            }).catch(s => u(s))
         }))
     }
-    document.querySelectorAll("template.empty-collection").forEach(l => {
-        l instanceof HTMLTemplateElement && l.content instanceof DocumentFragment && i(l.content)
+    document.querySelectorAll("template.empty-collection").forEach(a => {
+        a instanceof HTMLTemplateElement && a.content instanceof DocumentFragment && i(a.content)
     }), i(document);
     let o = new Set;
-    document.querySelectorAll("django-formset [id]").forEach(l => {
-        let c = l.getAttribute("id");
+    document.querySelectorAll("django-formset [id]").forEach(a => {
+        let c = a.getAttribute("id");
         if (o.has(c)) throw new Error(`There are at least two elements with attribute id="${c}"`);
         o.add(c)
     }), Promise.all(r).then(() => {
-        window.customElements.define("django-formset", vt), window.customElements.whenDefined("django-formset").then(() => {
+        window.customElements.define("django-formset", Et), window.customElements.whenDefined("django-formset").then(() => {
             e.remove()
         })
-    }).catch(l => console.error(`Failed to initialize django-formset: ${l}`))
+    }).catch(a => console.error(`Failed to initialize django-formset: ${a}`))
 });
 /*! Bundled license information:
 
 @ungap/custom-elements/index.js:
   (*! (c) Andrea Giammarchi @webreflection ISC *)
   (*! (c) Andrea Giammarchi - ISC *)
 */
```

### Comparing `django-formset-1.3.8/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.3.9/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files 4% similar despite different names*

```diff
@@ -45,27 +45,29 @@
 	dialog {
 		padding: 0;
 		word-wrap: break-word;
 		color: $modal-content-color;
 		background-color: $modal-content-bg;
 		border: $modal-content-border-width solid $modal-content-border-color;
 		border-radius: $modal-content-border-radius;
+		box-shadow: $box-shadow;
+		z-index: 1;
+
 		.dialog-header {
 			display: flex;
 			flex-shrink: 0;
 			align-items: center;
 			justify-content: space-between;
 			padding: $modal-header-padding;
 			border-bottom: $modal-header-border-width solid $modal-header-border-color;
 			border-top-left-radius: $modal-content-inner-border-radius;
 			border-top-right-radius: $modal-content-inner-border-radius;
-			.modal-title {
-				line-height: $modal-title-line-height;
-				font-weight: bolder;
-				font-size: larger;
+
+			h3 {
+				margin: 0;
 			}
 		}
 		.dialog-body {
 			position: relative;
 			flex: 1 1 auto;
 			padding: $modal-inner-padding;
 		}
```

### Comparing `django-formset-1.3.8/formset/static/formset/scss/collections.scss` & `django-formset-1.3.9/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/calendar/hours.html` & `django-formset-1.3.9/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/calendar/months.html` & `django-formset-1.3.9/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/calendar/weeks.html` & `django-formset-1.3.9/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/calendar/years.html` & `django-formset-1.3.9/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.3.9/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.3.9/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/collection.html` & `django-formset-1.3.9/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/dialog_form.html` & `django-formset-1.3.9/formset/templates/formset/default/dialog_form.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% spaceless %}
-<form{% include "formset/form_attrs.html" %}></form>
+<form{% include "formset/form_attrs.html" %} df-transient="true"></form>
 {% if form.modal_title %}
 <div class="dialog-header">
 	<div class="modal-title">{{ form.modal_title }}</div>
 </div>
 {% endif %}
 {% if form.fields %}
 <div class="dialog-body">
```

### Comparing `django-formset-1.3.8/formset/templates/formset/default/fieldset.html` & `django-formset-1.3.9/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.3.9/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.3.9/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.3.9/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.3.9/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/calendar-today.svg` & `django-formset-1.3.9/formset/templates/formset/icons/calendar-today.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/letters.svg` & `django-formset-1.3.9/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.3.9/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.3.9/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/subscript.svg` & `django-formset-1.3.9/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/icons/unlink.svg` & `django-formset-1.3.9/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.3.9/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.3.9/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templatetags/formsetify.py` & `django-formset-1.3.9/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templatetags/phonenumber.py` & `django-formset-1.3.9/formset/templatetags/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/templatetags/richtext.py` & `django-formset-1.3.9/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/upload.py` & `django-formset-1.3.9/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/utils.py` & `django-formset-1.3.9/formset/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
-from django.forms.utils import ErrorDict, ErrorList
+from django.forms.utils import ErrorDict, ErrorList, RenderableMixin
 from django.utils.functional import cached_property
+from django.utils.safestring import mark_safe
 
-from formset.boundfield import BoundField
 from formset.renderers.default import FormRenderer
 
 MARKED_FOR_REMOVAL = '_marked_for_removal_'
 
 
 class FormsetErrorList(ErrorList):
     template_name = 'formset/default/field_errors.html'
@@ -113,14 +113,16 @@
 class FormDecoratorMixin:
     def __init__(self, error_class=FormsetErrorList, **kwargs):
         kwargs['error_class'] = error_class
         super().__init__(**kwargs)
 
     def __getitem__(self, name):
         "Returns a modified BoundField for the given field."
+        from formset.boundfield import BoundField
+
         try:
             field = self.fields[name]
         except KeyError:
             raise KeyError(f"Key {name} not found in Form")
         return BoundField(self, field, name)
 
     @cached_property
@@ -153,7 +155,57 @@
         """
         return {
             'form': self,
         }
 
     def get_field(self, field_name):
         return self.fields[field_name]
+
+
+class RenderableDetachedFieldMixin(RenderableMixin):
+    """
+    Mixin class to be added to detached fields, if used outside a native Django Form.
+    This is required to render a field without converting it to a `BoundField`.
+    """
+
+    def get_context(self):
+        return {
+            'field': self,
+        }
+
+    def as_widget(self, widget=None, attrs=None, only_initial=False):
+        """
+        Render the field by rendering the passed widget, adding any HTML
+        attributes passed as attrs. If a widget isn't specified, use the
+        field's default widget.
+        """
+        widget = widget or self.widget
+        attrs = attrs or {}
+        if self.disabled:
+            attrs['disabled'] = True
+        if '%s' in str(self.auto_id):
+            auto_id = self.auto_id % self._name
+        elif self.auto_id:
+            auto_id = self.auto_id
+        else:
+            auto_id = ''
+        if auto_id:
+            attrs['id'] = auto_id
+            if self.help_text:
+                attrs['aria-describedby'] = f'{auto_id}_help_text'
+        attrs['label'] = self._name.replace('_', ' ').title() if self.label is None else self.label
+        return widget.render(
+            name=self._name,
+            value=None,
+            attrs=attrs,
+            renderer=self.renderer,
+        )
+
+    def render(self, template_name=None, context=None, renderer=None):
+        """Render this detached field as HTML widget."""
+        renderer = renderer or self.renderer
+        template_name = template_name or 'formset/default/detached_field.html'
+        context = context or self.get_context()
+        return mark_safe(renderer.render(template_name, context))
+
+    __str__ = render
+    __html__ = render
```

### Comparing `django-formset-1.3.8/formset/views.py` & `django-formset-1.3.9/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.3.8/formset/widgets.py` & `django-formset-1.3.9/formset/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,48 @@
 
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
 from django.core.files.storage import default_storage
 from django.core.files.uploadedfile import UploadedFile
 from django.core.signing import get_cookie_signer
 from django.db.models.query_utils import Q
 from django.forms.models import ModelChoiceIterator, ModelChoiceIteratorValue
-from django.forms.widgets import DateTimeBaseInput, FileInput, Select, SelectMultiple, TextInput
+from django.forms.widgets import DateTimeBaseInput, FileInput, Select, SelectMultiple, TextInput, Widget
+from django.utils.encoding import uri_to_iri
 from django.utils.timezone import datetime, now
 from django.utils.translation import gettext_lazy as _
 
 from formset.calendar import CalendarRenderer
 
 
+class Button(Widget):
+    template_name = 'formset/default/widgets/button.html'
+    button_type = 'button'
+    action = None
+    button_variant = None
+
+    def __init__(self, attrs=None, action=None, button_variant=None):
+        if action:
+            self.action = action
+        if button_variant:
+            self.button_variant = button_variant
+        super().__init__(attrs)
+
+    def build_attrs(self, base_attrs, extra_attrs=None):
+        attrs = super().build_attrs(base_attrs, extra_attrs)
+        attrs['df-click'] = self.action if self.action else 'activate'
+        return attrs
+
+    def get_context(self, name, value, attrs):
+        context = super().get_context(name, value, attrs)
+        context['label'] = context['widget']['attrs'].pop('label', None)  # for buttons, the label is the value
+        context['widget']['type'] = self.button_type
+        context['widget']['variant'] = self.button_variant
+        return context
+
+
 class SimpleModelChoiceIterator(ModelChoiceIterator):
     def __iter__(self):
         queryset = self.queryset
         # Can't use iterator() when queryset uses prefetch_related()
         if not queryset._prefetch_related_lookups:
             queryset = queryset.iterator()
         for obj in queryset:
@@ -78,14 +105,15 @@
                 queries.append(Q(**{lookup: filtervalue}))
         try:
             return reduce(and_, queries, Q())
         except TypeError:
             raise ImproperlyConfigured(f"Invalid attribute 'filter_by' in {self.__class__}.")
 
     def build_search_query(self, search_term):
+        search_term = uri_to_iri(search_term)
         try:
             return reduce(or_, (Q(**{sl: search_term}) for sl in self.search_lookup))
         except TypeError:
             raise ImproperlyConfigured(f"Invalid attribute 'search_lookup' in {self.__class__}.")
 
     def format_value(self, value):
         if value is None:
```

### Comparing `django-formset-1.3.8/setup.py` & `django-formset-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
 ]
 
 setup(
     name='django-formset',
     version=__version__,
-    description='Prevalidate Django Forms in the browser',
+    description='The missing widgets and form manipulation library for Django',
     author='Jacob Rief',
     author_email='jacob.rief@gmail.com',
     url='https://github.com/jrief/django-formset',
     packages=find_packages(include=['formset', 'formset.*']),
     install_requires=[
         'django>=4.0',
     ],
```

