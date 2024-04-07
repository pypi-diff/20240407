# Comparing `tmp/django-diary-4.2.7.1.tar.gz` & `tmp/django-diary-4.2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-diary-4.2.7.1.tar", last modified: Tue Nov 21 13:25:29 2023, max compression
+gzip compressed data, was "django-diary-4.2.7.2.tar", last modified: Fri Nov 24 14:23:09 2023, max compression
```

## Comparing `django-diary-4.2.7.1.tar` & `django-diary-4.2.7.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/
--rw-r--r--   0 bob       (1000) bob       (1000)     6128 2023-11-21 13:17:57.000000 django-diary-4.2.7.1/CHANGES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)     1105 2015-09-09 10:52:23.000000 django-diary-4.2.7.1/LICENSE.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      105 2015-09-26 10:31:45.000000 django-diary-4.2.7.1/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)    27025 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)    25959 2023-11-03 09:35:48.000000 django-diary-4.2.7.1/README.rst
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.676793 django-diary-4.2.7.1/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)       24 2023-11-21 13:20:14.000000 django-diary-4.2.7.1/diary/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)     6340 2023-11-20 19:29:08.000000 django-diary-4.2.7.1/diary/admin.py
--rw-r--r--   0 bob       (1000) bob       (1000)      691 2020-07-01 15:24:38.000000 django-diary-4.2.7.1/diary/backends.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.676793 django-diary-4.2.7.1/diary/formats/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-08-31 15:32:46.000000 django-diary-4.2.7.1/diary/formats/__init__.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.676793 django-diary-4.2.7.1/diary/formats/en/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-08-31 15:33:20.000000 django-diary-4.2.7.1/diary/formats/en/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)      220 2023-08-31 15:35:17.000000 django-diary-4.2.7.1/diary/formats/en/formats.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2581 2023-11-20 21:24:53.000000 django-diary-4.2.7.1/diary/forms.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.676793 django-diary-4.2.7.1/diary/management/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-4.2.7.1/diary/management/__init__.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.676793 django-diary-4.2.7.1/diary/management/commands/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-4.2.7.1/diary/management/commands/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1927 2020-07-02 10:27:30.000000 django-diary-4.2.7.1/diary/management/commands/clean_entries.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2949 2023-09-15 12:49:34.000000 django-diary-4.2.7.1/diary/management/commands/email_reminder.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.680793 django-diary-4.2.7.1/diary/migrations/
--rw-r--r--   0 bob       (1000) bob       (1000)     3547 2020-07-01 15:24:38.000000 django-diary-4.2.7.1/diary/migrations/0001_initial.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1103 2023-09-09 16:34:34.000000 django-diary-4.2.7.1/diary/migrations/0002_auto_20151010_1324.py
--rw-r--r--   0 bob       (1000) bob       (1000)      640 2015-10-11 12:07:14.000000 django-diary-4.2.7.1/diary/migrations/0003_auto_20151010_1331.py
--rw-r--r--   0 bob       (1000) bob       (1000)      533 2015-10-19 13:04:03.000000 django-diary-4.2.7.1/diary/migrations/0004_customer_title.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1332 2015-10-19 13:04:04.000000 django-diary-4.2.7.1/diary/migrations/0005_auto_20151017_1119.py
--rw-r--r--   0 bob       (1000) bob       (1000)      557 2015-10-19 13:04:04.000000 django-diary-4.2.7.1/diary/migrations/0006_auto_20151017_1347.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1033 2015-10-19 13:04:04.000000 django-diary-4.2.7.1/diary/migrations/0007_auto_20151017_1348.py
--rw-r--r--   0 bob       (1000) bob       (1000)      585 2023-09-15 12:23:45.000000 django-diary-4.2.7.1/diary/migrations/0008_customer_opt_out_entry_change_email_and_more.py
--rw-r--r--   0 bob       (1000) bob       (1000)      889 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/migrations/0009_resource_bg_color_resource_fg_color.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2670 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/migrations/0010_resource_enabled_alter_resource_bg_color_and_more.py
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-09-09 10:52:23.000000 django-diary-4.2.7.1/diary/migrations/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)    17755 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/models.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1954 2023-08-25 16:53:34.000000 django-diary-4.2.7.1/diary/settings.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.680793 django-diary-4.2.7.1/diary/static/
--rw-r--r--   0 bob       (1000) bob       (1000)      702 2015-09-23 12:09:00.000000 django-diary-4.2.7.1/diary/static/ajax_csrf.js
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.680793 django-diary-4.2.7.1/diary/static/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)     2547 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/static/diary/base.css
--rw-r--r--   0 bob       (1000) bob       (1000)     3296 2015-10-19 13:04:04.000000 django-diary-4.2.7.1/diary/static/diary/entry_ajax_dnd.js
--rw-r--r--   0 bob       (1000) bob       (1000)     1880 2015-10-11 12:07:14.000000 django-diary-4.2.7.1/diary/static/diary/entry_ajax_modal.js
--rw-r--r--   0 bob       (1000) bob       (1000)     3897 2020-07-03 15:15:23.000000 django-diary-4.2.7.1/diary/static/diary/multi_col.css
--rw-r--r--   0 bob       (1000) bob       (1000)     3285 2015-09-09 10:52:23.000000 django-diary-4.2.7.1/diary/static/js.cookie.js
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.672793 django-diary-4.2.7.1/diary/templates/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/diary/templates/diary/
--rw-r--r--   0 bob       (1000) bob       (1000)      714 2020-06-23 11:55:46.000000 django-diary-4.2.7.1/diary/templates/diary/base.html
--rw-r--r--   0 bob       (1000) bob       (1000)      504 2015-09-23 12:09:00.000000 django-diary-4.2.7.1/diary/templates/diary/customer_add.html
--rw-r--r--   0 bob       (1000) bob       (1000)      325 2015-09-23 12:09:00.000000 django-diary-4.2.7.1/diary/templates/diary/customer_change.html
--rw-r--r--   0 bob       (1000) bob       (1000)     5293 2023-09-22 17:12:02.000000 django-diary-4.2.7.1/diary/templates/diary/day.html
--rw-r--r--   0 bob       (1000) bob       (1000)      268 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/templates/diary/day_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2047 2015-09-09 10:52:23.000000 django-diary-4.2.7.1/diary/templates/diary/day_list.html
--rw-r--r--   0 bob       (1000) bob       (1000)      140 2023-09-15 14:04:12.000000 django-diary-4.2.7.1/diary/templates/diary/email_notify_entry_change.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      110 2023-09-15 14:04:35.000000 django-diary-4.2.7.1/diary/templates/diary/email_notify_entry_status_change.txt
--rw-r--r--   0 bob       (1000) bob       (1000)       86 2023-09-15 14:04:54.000000 django-diary-4.2.7.1/diary/templates/diary/email_notify_new_entry.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      394 2015-11-05 11:33:50.000000 django-diary-4.2.7.1/diary/templates/diary/email_reminder.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      459 2015-10-11 12:07:14.000000 django-diary-4.2.7.1/diary/templates/diary/entry.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2810 2015-10-11 12:07:14.000000 django-diary-4.2.7.1/diary/templates/diary/form_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2822 2015-10-25 11:07:28.000000 django-diary-4.2.7.1/diary/templates/diary/history.html
--rw-r--r--   0 bob       (1000) bob       (1000)     6425 2020-06-23 11:55:46.000000 django-diary-4.2.7.1/diary/templates/diary/main_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     1336 2020-07-01 15:30:36.000000 django-diary-4.2.7.1/diary/templates/diary/modal_base.html
--rw-r--r--   0 bob       (1000) bob       (1000)     5091 2020-06-11 11:12:17.000000 django-diary-4.2.7.1/diary/templates/diary/modal_entry.html
--rw-r--r--   0 bob       (1000) bob       (1000)     2730 2020-06-23 11:55:46.000000 django-diary-4.2.7.1/diary/templates/diary/month.html
--rw-r--r--   0 bob       (1000) bob       (1000)     6950 2023-09-22 17:00:26.000000 django-diary-4.2.7.1/diary/templates/diary/multi_day.html
--rw-r--r--   0 bob       (1000) bob       (1000)      590 2015-10-26 11:18:31.000000 django-diary-4.2.7.1/diary/templates/diary/reminders.html
--rw-r--r--   0 bob       (1000) bob       (1000)     1247 2015-09-19 16:38:13.000000 django-diary-4.2.7.1/diary/templates/diary/year.html
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/diary/templatetags/
--rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/templatetags/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)      338 2023-09-22 16:52:34.000000 django-diary-4.2.7.1/diary/templatetags/diary_tags.py
--rw-r--r--   0 bob       (1000) bob       (1000)    29880 2020-07-02 09:46:14.000000 django-diary-4.2.7.1/diary/tests.py
--rw-r--r--   0 bob       (1000) bob       (1000)     3612 2023-09-07 15:56:55.000000 django-diary-4.2.7.1/diary/urls.py
--rw-r--r--   0 bob       (1000) bob       (1000)    26978 2023-11-20 21:25:14.000000 django-diary-4.2.7.1/diary/views.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1857 2023-08-31 15:56:01.000000 django-diary-4.2.7.1/diary/widgets.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/django_diary.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)    27025 2023-11-21 13:25:29.000000 django-diary-4.2.7.1/django_diary.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     3004 2023-11-21 13:25:29.000000 django-diary-4.2.7.1/django_diary.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-11-21 13:25:29.000000 django-diary-4.2.7.1/django_diary.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2015-09-26 10:24:06.000000 django-diary-4.2.7.1/django_diary.egg-info/not-zip-safe
--rw-r--r--   0 bob       (1000) bob       (1000)       62 2023-11-21 13:25:29.000000 django-diary-4.2.7.1/django_diary.egg-info/requires.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        6 2023-11-21 13:25:29.000000 django-diary-4.2.7.1/django_diary.egg-info/top_level.txt
--rwxr-xr-x   0 bob       (1000) bob       (1000)    11434 2015-09-25 15:18:27.000000 django-diary-4.2.7.1/ez_setup.py
--rw-r--r--   0 bob       (1000) bob       (1000)       38 2023-11-21 13:25:29.684793 django-diary-4.2.7.1/setup.cfg
--rwxr-xr-x   0 bob       (1000) bob       (1000)     3326 2023-09-22 18:49:34.000000 django-diary-4.2.7.1/setup.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/
+-rw-r--r--   0 bob       (1000) bob       (1000)     6128 2023-11-21 13:17:57.000000 django-diary-4.2.7.2/CHANGES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)     1105 2015-09-09 10:52:23.000000 django-diary-4.2.7.2/LICENSE.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      105 2015-09-26 10:31:45.000000 django-diary-4.2.7.2/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)    27372 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)    26306 2023-11-24 14:04:27.000000 django-diary-4.2.7.2/README.rst
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.238046 django-diary-4.2.7.2/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)       24 2023-11-24 14:17:41.000000 django-diary-4.2.7.2/diary/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8885 2023-11-24 13:41:14.000000 django-diary-4.2.7.2/diary/admin.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      691 2020-07-01 15:24:38.000000 django-diary-4.2.7.2/diary/backends.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.238046 django-diary-4.2.7.2/diary/formats/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-08-31 15:32:46.000000 django-diary-4.2.7.2/diary/formats/__init__.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.238046 django-diary-4.2.7.2/diary/formats/en/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-08-31 15:33:20.000000 django-diary-4.2.7.2/diary/formats/en/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      220 2023-08-31 15:35:17.000000 django-diary-4.2.7.2/diary/formats/en/formats.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2581 2023-11-20 21:24:53.000000 django-diary-4.2.7.2/diary/forms.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.242046 django-diary-4.2.7.2/diary/management/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-4.2.7.2/diary/management/__init__.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.242046 django-diary-4.2.7.2/diary/management/commands/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-10-30 14:06:59.000000 django-diary-4.2.7.2/diary/management/commands/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1927 2020-07-02 10:27:30.000000 django-diary-4.2.7.2/diary/management/commands/clean_entries.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2949 2023-09-15 12:49:34.000000 django-diary-4.2.7.2/diary/management/commands/email_reminder.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.242046 django-diary-4.2.7.2/diary/migrations/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3547 2020-07-01 15:24:38.000000 django-diary-4.2.7.2/diary/migrations/0001_initial.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1103 2023-09-09 16:34:34.000000 django-diary-4.2.7.2/diary/migrations/0002_auto_20151010_1324.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      640 2015-10-11 12:07:14.000000 django-diary-4.2.7.2/diary/migrations/0003_auto_20151010_1331.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      533 2015-10-19 13:04:03.000000 django-diary-4.2.7.2/diary/migrations/0004_customer_title.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1332 2015-10-19 13:04:04.000000 django-diary-4.2.7.2/diary/migrations/0005_auto_20151017_1119.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      557 2015-10-19 13:04:04.000000 django-diary-4.2.7.2/diary/migrations/0006_auto_20151017_1347.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1033 2015-10-19 13:04:04.000000 django-diary-4.2.7.2/diary/migrations/0007_auto_20151017_1348.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      585 2023-09-15 12:23:45.000000 django-diary-4.2.7.2/diary/migrations/0008_customer_opt_out_entry_change_email_and_more.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      889 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/migrations/0009_resource_bg_color_resource_fg_color.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2670 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/migrations/0010_resource_enabled_alter_resource_bg_color_and_more.py
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2015-09-09 10:52:23.000000 django-diary-4.2.7.2/diary/migrations/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)    17755 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/models.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1954 2023-08-25 16:53:34.000000 django-diary-4.2.7.2/diary/settings.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.242046 django-diary-4.2.7.2/diary/static/
+-rw-r--r--   0 bob       (1000) bob       (1000)      702 2015-09-23 12:09:00.000000 django-diary-4.2.7.2/diary/static/ajax_csrf.js
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.246046 django-diary-4.2.7.2/diary/static/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2547 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/static/diary/base.css
+-rw-r--r--   0 bob       (1000) bob       (1000)     3296 2015-10-19 13:04:04.000000 django-diary-4.2.7.2/diary/static/diary/entry_ajax_dnd.js
+-rw-r--r--   0 bob       (1000) bob       (1000)     1880 2015-10-11 12:07:14.000000 django-diary-4.2.7.2/diary/static/diary/entry_ajax_modal.js
+-rw-r--r--   0 bob       (1000) bob       (1000)     3897 2020-07-03 15:15:23.000000 django-diary-4.2.7.2/diary/static/diary/multi_col.css
+-rw-r--r--   0 bob       (1000) bob       (1000)     3285 2015-09-09 10:52:23.000000 django-diary-4.2.7.2/diary/static/js.cookie.js
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.234046 django-diary-4.2.7.2/diary/templates/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/diary/templates/diary/
+-rw-r--r--   0 bob       (1000) bob       (1000)      714 2020-06-23 11:55:46.000000 django-diary-4.2.7.2/diary/templates/diary/base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      599 2023-11-24 13:41:14.000000 django-diary-4.2.7.2/diary/templates/diary/customer_add.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      420 2023-11-24 13:41:14.000000 django-diary-4.2.7.2/diary/templates/diary/customer_change.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     5293 2023-09-22 17:12:02.000000 django-diary-4.2.7.2/diary/templates/diary/day.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      268 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/templates/diary/day_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2047 2015-09-09 10:52:23.000000 django-diary-4.2.7.2/diary/templates/diary/day_list.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      140 2023-09-15 14:04:12.000000 django-diary-4.2.7.2/diary/templates/diary/email_notify_entry_change.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      110 2023-09-15 14:04:35.000000 django-diary-4.2.7.2/diary/templates/diary/email_notify_entry_status_change.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)       86 2023-09-15 14:04:54.000000 django-diary-4.2.7.2/diary/templates/diary/email_notify_new_entry.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      394 2015-11-05 11:33:50.000000 django-diary-4.2.7.2/diary/templates/diary/email_reminder.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)      459 2015-10-11 12:07:14.000000 django-diary-4.2.7.2/diary/templates/diary/entry.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2795 2023-11-24 13:41:14.000000 django-diary-4.2.7.2/diary/templates/diary/form_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2822 2015-10-25 11:07:28.000000 django-diary-4.2.7.2/diary/templates/diary/history.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     6425 2020-06-23 11:55:46.000000 django-diary-4.2.7.2/diary/templates/diary/main_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     1336 2020-07-01 15:30:36.000000 django-diary-4.2.7.2/diary/templates/diary/modal_base.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     5091 2020-06-11 11:12:17.000000 django-diary-4.2.7.2/diary/templates/diary/modal_entry.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     2730 2020-06-23 11:55:46.000000 django-diary-4.2.7.2/diary/templates/diary/month.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     6950 2023-09-22 17:00:26.000000 django-diary-4.2.7.2/diary/templates/diary/multi_day.html
+-rw-r--r--   0 bob       (1000) bob       (1000)      590 2015-10-26 11:18:31.000000 django-diary-4.2.7.2/diary/templates/diary/reminders.html
+-rw-r--r--   0 bob       (1000) bob       (1000)     1247 2015-09-19 16:38:13.000000 django-diary-4.2.7.2/diary/templates/diary/year.html
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/diary/templatetags/
+-rw-r--r--   0 bob       (1000) bob       (1000)        0 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/templatetags/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      338 2023-09-22 16:52:34.000000 django-diary-4.2.7.2/diary/templatetags/diary_tags.py
+-rw-r--r--   0 bob       (1000) bob       (1000)    29880 2020-07-02 09:46:14.000000 django-diary-4.2.7.2/diary/tests.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     3612 2023-09-07 15:56:55.000000 django-diary-4.2.7.2/diary/urls.py
+-rw-r--r--   0 bob       (1000) bob       (1000)    26978 2023-11-20 21:25:14.000000 django-diary-4.2.7.2/diary/views.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1857 2023-08-31 15:56:01.000000 django-diary-4.2.7.2/diary/widgets.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/django_diary.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)    27372 2023-11-24 14:23:09.000000 django-diary-4.2.7.2/django_diary.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     3004 2023-11-24 14:23:09.000000 django-diary-4.2.7.2/django_diary.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-11-24 14:23:09.000000 django-diary-4.2.7.2/django_diary.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2015-09-26 10:24:06.000000 django-diary-4.2.7.2/django_diary.egg-info/not-zip-safe
+-rw-r--r--   0 bob       (1000) bob       (1000)       62 2023-11-24 14:23:09.000000 django-diary-4.2.7.2/django_diary.egg-info/requires.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        6 2023-11-24 14:23:09.000000 django-diary-4.2.7.2/django_diary.egg-info/top_level.txt
+-rwxr-xr-x   0 bob       (1000) bob       (1000)    11434 2015-09-25 15:18:27.000000 django-diary-4.2.7.2/ez_setup.py
+-rw-r--r--   0 bob       (1000) bob       (1000)       38 2023-11-24 14:23:09.250046 django-diary-4.2.7.2/setup.cfg
+-rwxr-xr-x   0 bob       (1000) bob       (1000)     3326 2023-09-22 18:49:34.000000 django-diary-4.2.7.2/setup.py
```

### Comparing `django-diary-4.2.7.1/CHANGES.txt` & `django-diary-4.2.7.2/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/LICENSE.txt` & `django-diary-4.2.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/PKG-INFO` & `django-diary-4.2.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-diary
-Version: 4.2.7.1
+Version: 4.2.7.2
 Summary: A pluggable diary app for use in the Django framework.
 Home-page: http://pypi.python.org/pypi/django-diary/
 Author: Bob Bowles
 Author-email: bobjohnbowles@gmail.com
 License: MIT License
 Keywords: Diary,Django
 Classifier: Programming Language :: Python
@@ -26,19 +26,14 @@
 Requires-Dist: django-datetime-widget2>=0.9.5
 Requires-Dist: DateTime>=5.2
 
 ============
 Django Diary
 ============
 
-.. image:: https://pypip.in/v/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-.. image:: https://pypip.in/d/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-
 
 Description
 -----------
 
 Django-Diary is a project to create an easy-to-use desk diary and scheduling tool for use in a fast-paced retail environment. The aim is to be able to schedule and manage client bookings with available resources as quickly and easily as possible with no fuss.
 
 While the data model is very simple, some effort has been put into making the UI slick and intuitive, with ``ajax`` enabling drag-and-drop and updates of modal displays on the diary grid, and ``Bootstrap``-compatible widgets used on the forms.
@@ -75,22 +70,38 @@
 
     For versions >= 2 this may need to be a two-stage process due to references to package forks not in Pypi (TBA)::
 
         pip install django-diary --no-deps  # installs the app by itself
         pip install django-diary            # installs the dependencies
 
 
-#.  Add ``diary`` and ``datetimewidget`` to your ``INSTALLED_APPS`` in ``settings.py`` underneath your main project app:
+#.  Add ``diary`` and ``datetimewidget`` underneath your main project app in
+        ``settings.py``
 
     ::
 
+        INSTALLED_APPS = [
         ...
             'diary',
             'datetimewidget',
         ...
+        ]
+
+
+#.  For better forms layouts add ``crispy_forms`` and its template pack for ``Bootstrap 3`` to your ``INSTALLED_APPS`` in ``settings.py``
+
+    ::
+
+        INSTALLED_APPS = [
+        ...
+            'crispy_forms',
+            'crispy-bootstrap3'
+        ...
+        ]
+        CRISPY_TEMPLATE_PACK = 'bootstrap3'
 
 
 #.  Add the following to your ``settings.py`` for Django >= 3.2
 
     ::
 
         ...
@@ -371,22 +382,33 @@
 
 ::
 
     Django==3.2.20
     django-datetime-widget2>=0.9.5
     pytz>=2023.3
 
-Version 4.2 < 5 (Django 4 Maintenance)
---------------------------------------
+Version 4.2 <= 4.2.7 (Django 4 Maintenance)
+-------------------------------------------
+
+::
+
+    Django==4.2.7, <5
+    django-datetime-widget2>=0.9.5
+    DateTime>=5.2
+
+Version 4.2.7.2 <5 (Django 4 Maintenance)
+-----------------------------------------
 
 ::
 
     Django==4.2.7, <5
     django-datetime-widget2>=0.9.5
     DateTime>=5.2
+    crispy_forms>=2.1
+    crispy-bootstrap3>=2022.1
 
 Version 5+ (Django 5 Development - TBA)
 ---------------------------------------
 
 ::
 
     Django>=5.0, <6
```

### Comparing `django-diary-4.2.7.1/README.rst` & `django-diary-4.2.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 ============
 Django Diary
 ============
 
-.. image:: https://pypip.in/v/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-.. image:: https://pypip.in/d/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-
 
 Description
 -----------
 
 Django-Diary is a project to create an easy-to-use desk diary and scheduling tool for use in a fast-paced retail environment. The aim is to be able to schedule and manage client bookings with available resources as quickly and easily as possible with no fuss.
 
 While the data model is very simple, some effort has been put into making the UI slick and intuitive, with ``ajax`` enabling drag-and-drop and updates of modal displays on the diary grid, and ``Bootstrap``-compatible widgets used on the forms.
@@ -47,22 +42,38 @@
 
     For versions >= 2 this may need to be a two-stage process due to references to package forks not in Pypi (TBA)::
 
         pip install django-diary --no-deps  # installs the app by itself
         pip install django-diary            # installs the dependencies
 
 
-#.  Add ``diary`` and ``datetimewidget`` to your ``INSTALLED_APPS`` in ``settings.py`` underneath your main project app:
+#.  Add ``diary`` and ``datetimewidget`` underneath your main project app in
+        ``settings.py``
 
     ::
 
+        INSTALLED_APPS = [
         ...
             'diary',
             'datetimewidget',
         ...
+        ]
+
+
+#.  For better forms layouts add ``crispy_forms`` and its template pack for ``Bootstrap 3`` to your ``INSTALLED_APPS`` in ``settings.py``
+
+    ::
+
+        INSTALLED_APPS = [
+        ...
+            'crispy_forms',
+            'crispy-bootstrap3'
+        ...
+        ]
+        CRISPY_TEMPLATE_PACK = 'bootstrap3'
 
 
 #.  Add the following to your ``settings.py`` for Django >= 3.2
 
     ::
 
         ...
@@ -343,22 +354,33 @@
 
 ::
 
     Django==3.2.20
     django-datetime-widget2>=0.9.5
     pytz>=2023.3
 
-Version 4.2 < 5 (Django 4 Maintenance)
---------------------------------------
+Version 4.2 <= 4.2.7 (Django 4 Maintenance)
+-------------------------------------------
+
+::
+
+    Django==4.2.7, <5
+    django-datetime-widget2>=0.9.5
+    DateTime>=5.2
+
+Version 4.2.7.2 <5 (Django 4 Maintenance)
+-----------------------------------------
 
 ::
 
     Django==4.2.7, <5
     django-datetime-widget2>=0.9.5
     DateTime>=5.2
+    crispy_forms>=2.1
+    crispy-bootstrap3>=2022.1
 
 Version 5+ (Django 5 Development - TBA)
 ---------------------------------------
 
 ::
 
     Django>=5.0, <6
```

### Comparing `django-diary-4.2.7.1/diary/backends.py` & `django-diary-4.2.7.2/diary/backends.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/forms.py` & `django-diary-4.2.7.2/diary/forms.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/management/commands/clean_entries.py` & `django-diary-4.2.7.2/diary/management/commands/clean_entries.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/management/commands/email_reminder.py` & `django-diary-4.2.7.2/diary/management/commands/email_reminder.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0001_initial.py` & `django-diary-4.2.7.2/diary/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0002_auto_20151010_1324.py` & `django-diary-4.2.7.2/diary/migrations/0002_auto_20151010_1324.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0003_auto_20151010_1331.py` & `django-diary-4.2.7.2/diary/migrations/0003_auto_20151010_1331.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0004_customer_title.py` & `django-diary-4.2.7.2/diary/migrations/0004_customer_title.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0005_auto_20151017_1119.py` & `django-diary-4.2.7.2/diary/migrations/0005_auto_20151017_1119.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0006_auto_20151017_1347.py` & `django-diary-4.2.7.2/diary/migrations/0006_auto_20151017_1347.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0007_auto_20151017_1348.py` & `django-diary-4.2.7.2/diary/migrations/0007_auto_20151017_1348.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0008_customer_opt_out_entry_change_email_and_more.py` & `django-diary-4.2.7.2/diary/migrations/0008_customer_opt_out_entry_change_email_and_more.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0009_resource_bg_color_resource_fg_color.py` & `django-diary-4.2.7.2/diary/migrations/0009_resource_bg_color_resource_fg_color.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/migrations/0010_resource_enabled_alter_resource_bg_color_and_more.py` & `django-diary-4.2.7.2/diary/migrations/0010_resource_enabled_alter_resource_bg_color_and_more.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/models.py` & `django-diary-4.2.7.2/diary/models.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/settings.py` & `django-diary-4.2.7.2/diary/settings.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/ajax_csrf.js` & `django-diary-4.2.7.2/diary/static/ajax_csrf.js`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/diary/base.css` & `django-diary-4.2.7.2/diary/static/diary/base.css`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/diary/entry_ajax_dnd.js` & `django-diary-4.2.7.2/diary/static/diary/entry_ajax_dnd.js`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/diary/entry_ajax_modal.js` & `django-diary-4.2.7.2/diary/static/diary/entry_ajax_modal.js`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/diary/multi_col.css` & `django-diary-4.2.7.2/diary/static/diary/multi_col.css`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/static/js.cookie.js` & `django-diary-4.2.7.2/diary/static/js.cookie.js`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/base.html` & `django-diary-4.2.7.2/diary/templates/diary/base.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/day.html` & `django-diary-4.2.7.2/diary/templates/diary/day.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/day_list.html` & `django-diary-4.2.7.2/diary/templates/diary/day_list.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/form_base.html` & `django-diary-4.2.7.2/diary/templates/diary/form_base.html`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,23 @@
                                         </p>
                                     {% endif %}
                                 </div>
                             </div>
                         {% endfor %}
                         <div class="row">
                             <div class="col-md-12">
-                                <button 
-                                    class="save btn btn-default diarybutton" 
-                                    type="{{ button_type }}"
+                                <button
+                        class="save btn btn-default diarybutton btn-primary"
+                        type="{{ button_type }}"
                                     >
                                     {{ button_label }}
                                 </button>
                             </div>
                         </div>
                     </form>
                 {% endblock diary_form_content %}
             </div>
         </div>
     </div>
 
 {% endwith %}
 {% endblock diary_content %}
-
```

### Comparing `django-diary-4.2.7.1/diary/templates/diary/history.html` & `django-diary-4.2.7.2/diary/templates/diary/history.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/main_base.html` & `django-diary-4.2.7.2/diary/templates/diary/main_base.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/modal_base.html` & `django-diary-4.2.7.2/diary/templates/diary/modal_base.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/modal_entry.html` & `django-diary-4.2.7.2/diary/templates/diary/modal_entry.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/month.html` & `django-diary-4.2.7.2/diary/templates/diary/month.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/multi_day.html` & `django-diary-4.2.7.2/diary/templates/diary/multi_day.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/reminders.html` & `django-diary-4.2.7.2/diary/templates/diary/reminders.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/templates/diary/year.html` & `django-diary-4.2.7.2/diary/templates/diary/year.html`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/tests.py` & `django-diary-4.2.7.2/diary/tests.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/urls.py` & `django-diary-4.2.7.2/diary/urls.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/views.py` & `django-diary-4.2.7.2/diary/views.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/diary/widgets.py` & `django-diary-4.2.7.2/diary/widgets.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/django_diary.egg-info/PKG-INFO` & `django-diary-4.2.7.2/django_diary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-diary
-Version: 4.2.7.1
+Version: 4.2.7.2
 Summary: A pluggable diary app for use in the Django framework.
 Home-page: http://pypi.python.org/pypi/django-diary/
 Author: Bob Bowles
 Author-email: bobjohnbowles@gmail.com
 License: MIT License
 Keywords: Diary,Django
 Classifier: Programming Language :: Python
@@ -26,19 +26,14 @@
 Requires-Dist: django-datetime-widget2>=0.9.5
 Requires-Dist: DateTime>=5.2
 
 ============
 Django Diary
 ============
 
-.. image:: https://pypip.in/v/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-.. image:: https://pypip.in/d/django-diary/badge.png
-    :target: https://crate.io/packages/django-diary
-
 
 Description
 -----------
 
 Django-Diary is a project to create an easy-to-use desk diary and scheduling tool for use in a fast-paced retail environment. The aim is to be able to schedule and manage client bookings with available resources as quickly and easily as possible with no fuss.
 
 While the data model is very simple, some effort has been put into making the UI slick and intuitive, with ``ajax`` enabling drag-and-drop and updates of modal displays on the diary grid, and ``Bootstrap``-compatible widgets used on the forms.
@@ -75,22 +70,38 @@
 
     For versions >= 2 this may need to be a two-stage process due to references to package forks not in Pypi (TBA)::
 
         pip install django-diary --no-deps  # installs the app by itself
         pip install django-diary            # installs the dependencies
 
 
-#.  Add ``diary`` and ``datetimewidget`` to your ``INSTALLED_APPS`` in ``settings.py`` underneath your main project app:
+#.  Add ``diary`` and ``datetimewidget`` underneath your main project app in
+        ``settings.py``
 
     ::
 
+        INSTALLED_APPS = [
         ...
             'diary',
             'datetimewidget',
         ...
+        ]
+
+
+#.  For better forms layouts add ``crispy_forms`` and its template pack for ``Bootstrap 3`` to your ``INSTALLED_APPS`` in ``settings.py``
+
+    ::
+
+        INSTALLED_APPS = [
+        ...
+            'crispy_forms',
+            'crispy-bootstrap3'
+        ...
+        ]
+        CRISPY_TEMPLATE_PACK = 'bootstrap3'
 
 
 #.  Add the following to your ``settings.py`` for Django >= 3.2
 
     ::
 
         ...
@@ -371,22 +382,33 @@
 
 ::
 
     Django==3.2.20
     django-datetime-widget2>=0.9.5
     pytz>=2023.3
 
-Version 4.2 < 5 (Django 4 Maintenance)
---------------------------------------
+Version 4.2 <= 4.2.7 (Django 4 Maintenance)
+-------------------------------------------
+
+::
+
+    Django==4.2.7, <5
+    django-datetime-widget2>=0.9.5
+    DateTime>=5.2
+
+Version 4.2.7.2 <5 (Django 4 Maintenance)
+-----------------------------------------
 
 ::
 
     Django==4.2.7, <5
     django-datetime-widget2>=0.9.5
     DateTime>=5.2
+    crispy_forms>=2.1
+    crispy-bootstrap3>=2022.1
 
 Version 5+ (Django 5 Development - TBA)
 ---------------------------------------
 
 ::
 
     Django>=5.0, <6
```

### Comparing `django-diary-4.2.7.1/django_diary.egg-info/SOURCES.txt` & `django-diary-4.2.7.2/django_diary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/ez_setup.py` & `django-diary-4.2.7.2/ez_setup.py`

 * *Files identical despite different names*

### Comparing `django-diary-4.2.7.1/setup.py` & `django-diary-4.2.7.2/setup.py`

 * *Files identical despite different names*

