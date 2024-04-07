# Comparing `tmp/wagtail_fedit-1.3.9.tar.gz` & `tmp/wagtail_fedit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.9.tar", last modified: Sat Apr  6 20:47:37 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.0.tar", last modified: Sun Apr  7 05:16:03 2024, max compression
```

## Comparing `wagtail_fedit-1.3.9.tar` & `wagtail_fedit-1.4.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.562050 wagtail_fedit-1.3.9/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     7566 2024-04-06 20:47:37.562050 wagtail_fedit-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     6573 2024-04-05 22:53:31.000000 wagtail_fedit-1.3.9/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-06 20:47:37.574974 wagtail_fedit-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.314624 wagtail_fedit-1.3.9/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.9/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.9/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.9/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.361668 wagtail_fedit-1.3.9/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.9/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.9/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.9/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      729 2024-04-06 18:37:05.000000 wagtail_fedit-1.3.9/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.362667 wagtail_fedit-1.3.9/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.9/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.364667 wagtail_fedit-1.3.9/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.3.9/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.274834 wagtail_fedit-1.3.9/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.274834 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.399180 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.400180 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.277304 wagtail_fedit-1.3.9/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.279308 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.413660 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.425829 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-05 20:57:10.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.455849 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.475457 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.484762 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.517409 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.519380 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.522389 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    18943 2024-04-05 22:57:30.000000 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    15195 2024-04-05 22:39:28.000000 wagtail_fedit-1.3.9/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.524387 wagtail_fedit-1.3.9/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.528391 wagtail_fedit-1.3.9/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.533331 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3529 2024-04-05 23:35:47.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.539908 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.547822 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.9/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.3.9/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11238 2024-04-06 18:35:33.000000 wagtail_fedit-1.3.9/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.553295 wagtail_fedit-1.3.9/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.9/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.9/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.3.9/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.3.9/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.3.9/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.561297 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:47:37.357667 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7566 2024-04-06 20:47:37.000000 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3542 2024-04-06 20:47:37.000000 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 20:47:37.000000 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-06 20:47:37.000000 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 20:47:37.000000 wagtail_fedit-1.3.9/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.708273 wagtail_fedit-1.4.0/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12872 2024-04-07 05:16:03.706847 wagtail_fedit-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11822 2024-04-06 22:25:03.000000 wagtail_fedit-1.4.0/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-07 05:16:03.718055 wagtail_fedit-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.260854 wagtail_fedit-1.4.0/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.0/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.0/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.0/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.301674 wagtail_fedit-1.4.0/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.0/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.0/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.0/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3356 2024-04-06 21:44:51.000000 wagtail_fedit-1.4.0/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.302675 wagtail_fedit-1.4.0/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.0/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.303675 wagtail_fedit-1.4.0/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.0/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.205561 wagtail_fedit-1.4.0/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.206559 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.316988 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.335462 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.206559 wagtail_fedit-1.4.0/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.207644 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.339819 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.349987 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.407444 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.419673 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.428865 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.434891 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1285 2024-04-06 18:43:26.000000 wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.447905 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.451371 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    18951 2024-04-06 22:02:41.000000 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15092 2024-04-07 05:12:36.000000 wagtail_fedit-1.4.0/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.461416 wagtail_fedit-1.4.0/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.488894 wagtail_fedit-1.4.0/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.531962 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3529 2024-04-05 23:35:47.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.590893 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7039 2024-04-05 23:57:48.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     4339 2024-04-06 00:03:48.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.636891 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.0/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      916 2024-04-06 20:43:13.000000 wagtail_fedit-1.4.0/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11238 2024-04-06 18:35:33.000000 wagtail_fedit-1.4.0/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.675622 wagtail_fedit-1.4.0/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.0/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.4.0/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14621 2024-04-05 23:51:10.000000 wagtail_fedit-1.4.0/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12225 2024-04-06 19:48:05.000000 wagtail_fedit-1.4.0/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.0/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.704471 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      160 2024-04-06 18:20:48.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6061 2024-04-06 18:49:36.000000 wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:16:03.706847 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12872 2024-04-07 05:16:02.000000 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3542 2024-04-07 05:16:03.000000 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 05:16:02.000000 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-07 05:16:02.000000 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 05:16:02.000000 wagtail_fedit-1.4.0/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.9/LICENSE` & `wagtail_fedit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/setup.cfg` & `wagtail_fedit-1.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
+00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.0/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.0/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/models.py` & `wagtail_fedit-1.4.0/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa07d1066 (Fri Apr  5 22:39:28 2024 UTC)
-files sz: 15195
+moddate:  0x76c61166 (Sat Apr  6 22:02:30 2024 UTC)
+files sz: 15073
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -20,16 +20,16 @@
       0300000000000000005a296524a02a000000000000000000000000000000
       00000000006416ac17a6010000ab01000000000000000064186507641965
       086604641a8404a6000000ab0000000000000000005a2b02004700641b84
       00641c6502a6030000ab0300000000000000005a2c6524a02a0000000000
       000000000000000000000000000000641dac17a6010000ab010000000000
       00000064186507641965086604641e8404a6000000ab0000000000000000
       005a2d641f84005a2e641865076420652f65301900000000000000000064
-      21652f653019000000000000000000642265316608642384045a32642484
-      005a33640d5300
+      21652f653019000000000000000000642265316608642384045a32642465
+      116a3300000000000000006602642584045a34642684005a35640d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library', 'Node', 'NodeList'))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
@@ -160,106 +160,114 @@
     29         244 PUSH_NULL
                246 LOAD_NAME               15 (signing)
                248 LOAD_ATTR               37 (TimestampSigner)
                258 PRECALL                  0
                262 CALL                     0
                272 STORE_NAME              38 (url_value_signer)
    
-    32         274 LOAD_CONST              18 ('Field name is not available in the context for field %(field)s.')
+    32         274 LOAD_CONST              18 ('Field name is not available in the context for %(object)s.')
                276 STORE_NAME              39 (WARNING_FIELD_NAME_NOT_AVAILABLE)
    
-    33         278 LOAD_CONST              19 ('Model instance is not available in the context for block %(block)s.')
+    33         278 LOAD_CONST              19 ('Model instance is not available in the context for %(object)s.')
                280 STORE_NAME              40 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
    
     36         282 PUSH_NULL
                284 LOAD_BUILD_CLASS
                286 LOAD_CONST              20 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 36>)
                288 MAKE_FUNCTION            0
                290 LOAD_CONST              21 ('BlockEditNode')
                292 LOAD_NAME                2 (Node)
                294 PRECALL                  3
                298 CALL                     3
                308 STORE_NAME              41 (BlockEditNode)
    
-   229         310 LOAD_NAME               36 (register)
+   228         310 LOAD_NAME               36 (register)
                312 LOAD_METHOD             42 (tag)
                334 LOAD_CONST              22 ('fedit_block')
                336 KW_NAMES                23
                338 PRECALL                  1
                342 CALL                     1
    
-   230         352 LOAD_CONST              24 ('parser')
+   229         352 LOAD_CONST              24 ('parser')
                354 LOAD_NAME                7 (Parser)
                356 LOAD_CONST              25 ('token')
                358 LOAD_NAME                8 (Token)
                360 BUILD_TUPLE              4
-               362 LOAD_CONST              26 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 229>)
+               362 LOAD_CONST              26 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 228>)
                364 MAKE_FUNCTION            4 (annotations)
    
-   229         366 PRECALL                  0
+   228         366 PRECALL                  0
                370 CALL                     0
    
-   230         380 STORE_NAME              43 (do_render_fedit_block)
+   229         380 STORE_NAME              43 (do_render_fedit_block)
    
-   289         382 PUSH_NULL
+   288         382 PUSH_NULL
                384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              27 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 289>)
+               386 LOAD_CONST              27 (<code object FieldEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 288>)
                388 MAKE_FUNCTION            0
                390 LOAD_CONST              28 ('FieldEditNode')
                392 LOAD_NAME                2 (Node)
                394 PRECALL                  3
                398 CALL                     3
                408 STORE_NAME              44 (FieldEditNode)
    
-   345         410 LOAD_NAME               36 (register)
+   338         410 LOAD_NAME               36 (register)
                412 LOAD_METHOD             42 (tag)
                434 LOAD_CONST              29 ('fedit_field')
                436 KW_NAMES                23
                438 PRECALL                  1
                442 CALL                     1
    
-   346         452 LOAD_CONST              24 ('parser')
+   339         452 LOAD_CONST              24 ('parser')
                454 LOAD_NAME                7 (Parser)
                456 LOAD_CONST              25 ('token')
                458 LOAD_NAME                8 (Token)
                460 BUILD_TUPLE              4
-               462 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 345>)
+               462 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 338>)
                464 MAKE_FUNCTION            4 (annotations)
    
-   345         466 PRECALL                  0
+   338         466 PRECALL                  0
                470 CALL                     0
    
-   346         480 STORE_NAME              45 (do_render_fedit_field)
+   339         480 STORE_NAME              45 (do_render_fedit_field)
    
-   388         482 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 388>)
+   381         482 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 381>)
                484 MAKE_FUNCTION            0
                486 STORE_NAME              46 (render_editable_field)
    
-   427         488 LOAD_CONST              24 ('parser')
+   420         488 LOAD_CONST              24 ('parser')
                490 LOAD_NAME                7 (Parser)
                492 LOAD_CONST              32 ('kwarg_list')
                494 LOAD_NAME               47 (list)
                496 LOAD_NAME               48 (str)
                498 BINARY_SUBSCR
                508 LOAD_CONST              33 ('tokens')
                510 LOAD_NAME               47 (list)
                512 LOAD_NAME               48 (str)
                514 BINARY_SUBSCR
                524 LOAD_CONST              34 ('return')
                526 LOAD_NAME               49 (dict)
                528 BUILD_TUPLE              8
-               530 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 427>)
+               530 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 420>)
                532 MAKE_FUNCTION            4 (annotations)
                534 STORE_NAME              50 (get_kwargs)
    
-   454         536 LOAD_CONST              36 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 454>)
-               538 MAKE_FUNCTION            0
-               540 STORE_NAME              51 (_get_from_context_or_set)
-               542 LOAD_CONST              13 (None)
-               544 RETURN_VALUE
+   445         536 LOAD_CONST              36 ('obj')
+               538 LOAD_NAME               17 (models)
+               540 LOAD_ATTR               51 (Model)
+               550 BUILD_TUPLE              2
+               552 LOAD_CONST              37 (<code object _can_edit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 445>)
+               554 MAKE_FUNCTION            4 (annotations)
+               556 STORE_NAME              52 (_can_edit)
+   
+   457         558 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 457>)
+               560 MAKE_FUNCTION            0
+               562 STORE_NAME              53 (_get_from_context_or_set)
+               564 LOAD_CONST              13 (None)
+               566 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
       ('render_to_string',)
       ('Parser', 'Token')
       ('FilterExpression',)
       ('mark_safe',)
@@ -271,16 +279,16 @@
       ('hooks',)
       ('urlencode',)
       None
       2
       ('FeditBlockEditButton', 'FeditFieldEditButton')
       ('FEDIT_PREVIEW_VAR', 'get_field_content')
       ('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR')
-      'Field name is not available in the context for field %(field)s.'
-      'Model instance is not available in the context for block %(block)s.'
+      'Field name is not available in the context for %(object)s.'
+      'Model instance is not available in the context for %(object)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a02020047006401840064026503a6030000ab0300
@@ -344,64 +352,64 @@
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
           56          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 56>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
-         180          94 LOAD_NAME               12 (staticmethod)
+         179          94 LOAD_NAME               12 (staticmethod)
          
-         181          96 LOAD_CONST              11 ('return')
+         180          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 180>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 179>)
                      104 MAKE_FUNCTION            4 (annotations)
          
-         180         106 PRECALL                  0
+         179         106 PRECALL                  0
                      110 CALL                     0
          
-         181         120 STORE_NAME              14 (pack)
+         180         120 STORE_NAME              14 (pack)
          
-         189         122 LOAD_NAME               15 (classmethod)
+         188         122 LOAD_NAME               15 (classmethod)
          
-         190         124 LOAD_CONST               3 (None)
+         189         124 LOAD_CONST               3 (None)
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 189>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 188>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-         189         144 PRECALL                  0
+         188         144 PRECALL                  0
                      148 CALL                     0
          
-         190         158 STORE_NAME              16 (unpack)
+         189         158 STORE_NAME              16 (unpack)
          
-         212         160 LOAD_NAME               12 (staticmethod)
+         211         160 LOAD_NAME               12 (staticmethod)
          
-         213         162 LOAD_CONST               6 ('block_id')
+         212         162 LOAD_CONST               6 ('block_id')
                      164 LOAD_NAME                7 (str)
                      166 LOAD_CONST               7 ('field_name')
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 212>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 211>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         212         194 PRECALL                  0
+         211         194 PRECALL                  0
                      198 CALL                     0
          
-         213         208 STORE_NAME              17 (get_edit_url)
+         212         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
                      212 RETURN_VALUE
          consts
             'BlockEditNode'
             code
                argcount  : 0
                nlocals   : 0
@@ -479,85 +487,80 @@
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
                firstlineno 40
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
-               nlocals   : 12
+               nlocals   : 13
                stacksize : 14
                flags     : 3
                code
-                  0x870c870d97007c006a0000000000000000007d027c006a010000000000
+                  0x870d870e97007c006a0000000000000000007d027c006a010000000000
                   0000007d037c006a0200000000000000007d047c006a0300000000000000
-                  008a0c7c006a0400000000000000007d057c05a005000000000000000000
+                  008a0d7c006a0400000000000000007d057c05a005000000000000000000
                   0000000000000000000000a6000000ab00000000000000000044005d325c
                   0200007d067d07740d000000000000000000007c07740e00000000000000
                   000000a6020000ab02000000000000000072187c07a00800000000000000
                   000000000000000000000000007c01a6010000ab0100000000000000007c
                   057c063c0000008c337c04730c64017c01760072087c0164011900000000
                   00000000007d04740d000000000000000000007c02740e00000000000000
                   000000a6020000ab02000000000000000072157c02a00800000000000000
                   000000000000000000000000007c01a6010000ab0100000000000000007d
                   02740d000000000000000000007c03740e00000000000000000000a60200
                   00ab02000000000000000072157c03a00800000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d03740d000000
                   000000000000007c04740e00000000000000000000a6020000ab02000000
                   000000000072157c04a00800000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d04740d000000000000000000
-                  00890c740e00000000000000000000a6020000ab02000000000000000072
-                  15890ca00800000000000000000000000000000000000000007c01a60100
-                  00ab0100000000000000008a0c7c03731564027c01760172117c02730f74
+                  00890d740e00000000000000000000a6020000ab02000000000000000072
+                  15890da00800000000000000000000000000000000000000007c01a60100
+                  00ab0100000000000000008a0d7c03731564027c01760172117c02730f74
                   13000000000000000000006403a6010000ab010000000000000000820189
-                  0c70147c01a00a00000000000000000000000000000000000000006404a6
-                  010000ab0100000000000000008a0c7c047c0164013c000000890c7c0164
+                  0d70147c01a00a00000000000000000000000000000000000000006404a6
+                  010000ab0100000000000000008a0d7c047c0164013c000000890d7c0164
                   043c0000007c02725809007c01a00b000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d016e1023007418000000
-                  0000000000000024007203010059006e0477007803590077017c01a00d00
+                  0000000000a6000000ab0000000000000000007d086e1023007418000000
+                  0000000000000024007203010059006e0477007803590077017c08a00d00
                   000000000000000000000000000000000000007c05a6010000ab01000000
                   000000000001007c02a00e00000000000000000000000000000000000000
-                  007c01a6010000ab0100000000000000007d0864057c005f0f0000000000
+                  007c08a6010000ab0100000000000000007d0964057c005f0f0000000000
                   0000006e387c006a10000000000000000072227c006a1000000000000000
                   00a01100000000000000000000000000000000000000007c01a6010000ab
-                  0100000000000000007d0864067c005f0f00000000000000006e0f741300
+                  0100000000000000007d0964067c005f0f00000000000000006e0f741300
                   0000000000000000006407a6010000ab01000000000000000082017c0473
-                  207425000000000000000000006a13000000000000000074280000000000
-                  000000000064087c0469017a060000a6010000ab01000000000000000001
-                  007c085300890c73257425000000000000000000006a1300000000000000
-                  00742a0000000000000000000064097c026a16000000000000000069017a
-                  060000a6010000ab01000000000000000001007c0853007c03730d64027c
+                  257425000000000000000000006a13000000000000000074280000000000
+                  000000000064087c016a15000000000000000069017a060000a6010000ab
+                  01000000000000000001007c095300890d732f7425000000000000000000
+                  006a130000000000000000742c0000000000000000000064087c026a0000
+                  000000000000006a1700000000000000006a18000000000000000069017a
+                  060000a6010000ab01000000000000000001007c0953007c03730d64027c
                   01760072097c016402190000000000000000007d036e2d7c03731a7c0272
-                  18742f000000000000000000007c02640aa6020000ab0200000000000000
-                  0072087c026a1800000000000000007d036e117c03730f74130000000000
+                  187433000000000000000000007c026409a6020000ab0200000000000000
+                  0072087c026a1a00000000000000007d036e117c03730f74130000000000
                   00000000006403a6010000ab01000000000000000082017c01a00a000000
-                  0000000000000000000000000000000000640ba6010000ab010000000000
-                  0000008a0d890d7271890d6a1900000000000000006a1a00000000000000
-                  007263890d6a190000000000000000a01b00000000000000000000000000
-                  00000000000000640ca6010000ab0100000000000000007249890d6a1900
-                  00000000000000a01b000000000000000000000000000000000000000089
-                  0c6a1c00000000000000006a1d00000000000000009b00640d890c6a1c00
-                  000000000000006a1e00000000000000009b009d03a6010000ab01000000
-                  00000000007216743f00000000000000000000890d744000000000000000
-                  0000006406a6030000ab03000000000000000073027c085300740d000000
-                  00000000000000890c744200000000000000000000a6020000ab02000000
-                  0000000000721d7445000000000000000000007c01640e880c6601640f84
-                  08a6030000ab0300000000000000007d097c099b0064107c039b0064119d
-                  047d096e0264007d097c006a0f00000000000000007c0564123c00000074
-                  4700000000000000000000a6000000ab00000000000000000067017d0a74
-                  49000000000000000000006a250000000000000000744c00000000000000
-                  000000a6010000ab01000000000000000044005d127d0b02007c0b890d7c
-                  0a890c7c037c04ac13a6050000ab05000000000000000001008c13880d66
-                  01641484087c0a4400a6000000ab0000000000000000007d0a744f000000
-                  0000000000000074510000000000000000000064007c0aa6020000ab0200
-                  00000000000000a6010000ab0100000000000000007d0a74530000000000
-                  0000000000641502007c006a2a00000000000000007c037c046602641689
-                  0c69017c05a4018e017c097c03890c7c087c047c017c04890c7c0a64179c
-                  0aa6020000ab0200000000000000005300
-                             0 MAKE_CELL               12 (model)
-                             2 MAKE_CELL               13 (request)
+                  0000000000000000000000000000000000640aa6010000ab010000000000
+                  0000008a0e743700000000000000000000890e890da6020000ab02000000
+                  000000000073027c095300740d00000000000000000000890d7438000000
+                  00000000000000a6020000ab020000000000000000721d743b0000000000
+                  00000000007c01640b880d6601640c8408a6030000ab0300000000000000
+                  007d0a7c0a9b00640d7c039b00640e9d047d0a6e0264007d0a7c006a0f00
+                  000000000000007c05640f3c000000743d00000000000000000000a60000
+                  00ab00000000000000000067017d0b743f000000000000000000006a2000
+                  00000000000000744200000000000000000000a6010000ab010000000000
+                  00000044005d127d0c02007c0c890e7c0b890d7c037c04ac10a6050000ab
+                  05000000000000000001008c13880e6601641184087c0b4400a6000000ab
+                  0000000000000000007d0b74450000000000000000000074470000000000
+                  000000000064007c0ba6020000ab020000000000000000a6010000ab0100
+                  000000000000007d0b744900000000000000000000641202007c006a2500
+                  000000000000007c037c0466026413890d69017c05a4018e017c0a7c0389
+                  0d7c097c047c017c04890d7c0b64149c0aa6020000ab0200000000000000
+                  005300
+                             0 MAKE_CELL               13 (model)
+                             2 MAKE_CELL               14 (request)
                
                 56           4 RESUME                   0
                
                 57           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (block)
                             18 STORE_FAST               2 (block)
                
@@ -567,15 +570,15 @@
                
                 59          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (field_name)
                             46 STORE_FAST               4 (field_name)
                
                 60          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                3 (model)
-                            60 STORE_DEREF             12 (model)
+                            60 STORE_DEREF             13 (model)
                
                 61          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                4 (extra)
                             74 STORE_FAST               5 (extra)
                
                 64          76 LOAD_FAST                5 (extra)
                             78 LOAD_METHOD              5 (items)
@@ -655,26 +658,26 @@
                            458 LOAD_METHOD              8 (resolve)
                            480 LOAD_FAST                1 (context)
                            482 PRECALL                  1
                            486 CALL                     1
                            496 STORE_FAST               4 (field_name)
                
                 77     >>  498 LOAD_GLOBAL             13 (NULL + isinstance)
-                           510 LOAD_DEREF              12 (model)
+                           510 LOAD_DEREF              13 (model)
                            512 LOAD_GLOBAL             14 (FilterExpression)
                            524 PRECALL                  2
                            528 CALL                     2
                            538 POP_JUMP_FORWARD_IF_FALSE    21 (to 582)
                
-                78         540 LOAD_DEREF              12 (model)
+                78         540 LOAD_DEREF              13 (model)
                            542 LOAD_METHOD              8 (resolve)
                            564 LOAD_FAST                1 (context)
                            566 PRECALL                  1
                            570 CALL                     1
-                           580 STORE_DEREF             12 (model)
+                           580 STORE_DEREF             13 (model)
                
                 80     >>  582 LOAD_FAST                3 (block_id)
                            584 POP_JUMP_FORWARD_IF_TRUE    21 (to 628)
                            586 LOAD_CONST               2 ('block_id')
                            588 LOAD_FAST                1 (context)
                            590 CONTAINS_OP              1
                            592 POP_JUMP_FORWARD_IF_FALSE    17 (to 628)
@@ -683,43 +686,43 @@
                
                 81         598 LOAD_GLOBAL             19 (NULL + ValueError)
                            610 LOAD_CONST               3 ('Block ID is required')
                            612 PRECALL                  1
                            616 CALL                     1
                            626 RAISE_VARARGS            1
                
-                86     >>  628 LOAD_DEREF              12 (model)
+                86     >>  628 LOAD_DEREF              13 (model)
                            630 JUMP_IF_TRUE_OR_POP     20 (to 672)
                            632 LOAD_FAST                1 (context)
                            634 LOAD_METHOD             10 (get)
                            656 LOAD_CONST               4 ('wagtail_fedit_instance')
                            658 PRECALL                  1
                            662 CALL                     1
-                       >>  672 STORE_DEREF             12 (model)
+                       >>  672 STORE_DEREF             13 (model)
                
                 87         674 LOAD_FAST                4 (field_name)
                            676 LOAD_FAST                1 (context)
                            678 LOAD_CONST               1 ('wagtail_fedit_field_name')
                            680 STORE_SUBSCR
                
-                88         684 LOAD_DEREF              12 (model)
+                88         684 LOAD_DEREF              13 (model)
                            686 LOAD_FAST                1 (context)
                            688 LOAD_CONST               4 ('wagtail_fedit_instance')
                            690 STORE_SUBSCR
                
                 92         694 LOAD_FAST                2 (block)
                            696 POP_JUMP_FORWARD_IF_FALSE    88 (to 874)
                
                 93         698 NOP
                
                 94         700 LOAD_FAST                1 (context)
                            702 LOAD_METHOD             11 (flatten)
                            724 PRECALL                  0
                            728 CALL                     0
-                           738 STORE_FAST               1 (context)
+                           738 STORE_FAST               8 (block_context)
                            740 JUMP_FORWARD            16 (to 774)
                        >>  742 PUSH_EXC_INFO
                
                 95         744 LOAD_GLOBAL             24 (AttributeError)
                            756 CHECK_EXC_MATCH
                            758 POP_JUMP_FORWARD_IF_FALSE     3 (to 766)
                            760 POP_TOP
@@ -728,27 +731,27 @@
                            764 JUMP_FORWARD             4 (to 774)
                
                 95     >>  766 RERAISE                  0
                        >>  768 COPY                     3
                            770 POP_EXCEPT
                            772 RERAISE                  1
                
-                97     >>  774 LOAD_FAST                1 (context)
+                97     >>  774 LOAD_FAST                8 (block_context)
                            776 LOAD_METHOD             13 (update)
                            798 LOAD_FAST                5 (extra)
                            800 PRECALL                  1
                            804 CALL                     1
                            814 POP_TOP
                
                 98         816 LOAD_FAST                2 (block)
                            818 LOAD_METHOD             14 (render_as_block)
-                           840 LOAD_FAST                1 (context)
+                           840 LOAD_FAST                8 (block_context)
                            842 PRECALL                  1
                            846 CALL                     1
-                           856 STORE_FAST               8 (rendered)
+                           856 STORE_FAST               9 (rendered)
                
                 99         858 LOAD_CONST               5 (True)
                            860 LOAD_FAST                0 (self)
                            862 STORE_ATTR              15 (has_block)
                            872 JUMP_FORWARD            56 (to 986)
                
                100     >>  874 LOAD_FAST                0 (self)
@@ -757,345 +760,315 @@
                
                101         888 LOAD_FAST                0 (self)
                            890 LOAD_ATTR               16 (nl)
                            900 LOAD_METHOD             17 (render)
                            922 LOAD_FAST                1 (context)
                            924 PRECALL                  1
                            928 CALL                     1
-                           938 STORE_FAST               8 (rendered)
+                           938 STORE_FAST               9 (rendered)
                
                102         940 LOAD_CONST               6 (False)
                            942 LOAD_FAST                0 (self)
                            944 STORE_ATTR              15 (has_block)
                            954 JUMP_FORWARD            15 (to 986)
                
                104     >>  956 LOAD_GLOBAL             19 (NULL + ValueError)
                            968 LOAD_CONST               7 ('Block or nodelist is required')
                            970 PRECALL                  1
                            974 CALL                     1
                            984 RAISE_VARARGS            1
                
                106     >>  986 LOAD_FAST                4 (field_name)
-                           988 POP_JUMP_FORWARD_IF_TRUE    32 (to 1054)
+                           988 POP_JUMP_FORWARD_IF_TRUE    37 (to 1064)
                
                107         990 LOAD_GLOBAL             37 (NULL + warnings)
                           1002 LOAD_ATTR               19 (warn)
-                          1012 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-                          1024 LOAD_CONST               8 ('field')
-                          1026 LOAD_FAST                4 (field_name)
-                          1028 BUILD_MAP                1
-                          1030 BINARY_OP                6 (%)
-                          1034 PRECALL                  1
-                          1038 CALL                     1
-                          1048 POP_TOP
-               
-               108        1050 LOAD_FAST                8 (rendered)
-                          1052 RETURN_VALUE
-               
-               110     >> 1054 LOAD_DEREF              12 (model)
-                          1056 POP_JUMP_FORWARD_IF_TRUE    37 (to 1132)
-               
-               111        1058 LOAD_GLOBAL             37 (NULL + warnings)
-                          1070 LOAD_ATTR               19 (warn)
-                          1080 LOAD_GLOBAL             42 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-                          1092 LOAD_CONST               9 ('block')
-                          1094 LOAD_FAST                2 (block)
-                          1096 LOAD_ATTR               22 (label)
-                          1106 BUILD_MAP                1
-                          1108 BINARY_OP                6 (%)
-                          1112 PRECALL                  1
-                          1116 CALL                     1
-                          1126 POP_TOP
-               
-               112        1128 LOAD_FAST                8 (rendered)
-                          1130 RETURN_VALUE
-               
-               115     >> 1132 LOAD_FAST                3 (block_id)
-                          1134 POP_JUMP_FORWARD_IF_TRUE    13 (to 1162)
-                          1136 LOAD_CONST               2 ('block_id')
-                          1138 LOAD_FAST                1 (context)
-                          1140 CONTAINS_OP              0
-                          1142 POP_JUMP_FORWARD_IF_FALSE     9 (to 1162)
-               
-               116        1144 LOAD_FAST                1 (context)
-                          1146 LOAD_CONST               2 ('block_id')
-                          1148 BINARY_SUBSCR
-                          1158 STORE_FAST               3 (block_id)
-                          1160 JUMP_FORWARD            45 (to 1252)
-               
-               117     >> 1162 LOAD_FAST                3 (block_id)
-                          1164 POP_JUMP_FORWARD_IF_TRUE    26 (to 1218)
-                          1166 LOAD_FAST                2 (block)
-                          1168 POP_JUMP_FORWARD_IF_FALSE    24 (to 1218)
-                          1170 LOAD_GLOBAL             47 (NULL + hasattr)
-                          1182 LOAD_FAST                2 (block)
-                          1184 LOAD_CONST              10 ('id')
-                          1186 PRECALL                  2
-                          1190 CALL                     2
-                          1200 POP_JUMP_FORWARD_IF_FALSE     8 (to 1218)
-               
-               118        1202 LOAD_FAST                2 (block)
-                          1204 LOAD_ATTR               24 (id)
-                          1214 STORE_FAST               3 (block_id)
-                          1216 JUMP_FORWARD            17 (to 1252)
-               
-               119     >> 1218 LOAD_FAST                3 (block_id)
-                          1220 POP_JUMP_FORWARD_IF_TRUE    15 (to 1252)
-               
-               120        1222 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1234 LOAD_CONST               3 ('Block ID is required')
-                          1236 PRECALL                  1
-                          1240 CALL                     1
-                          1250 RAISE_VARARGS            1
-               
-               123     >> 1252 LOAD_FAST                1 (context)
-                          1254 LOAD_METHOD             10 (get)
-                          1276 LOAD_CONST              11 ('request')
-                          1278 PRECALL                  1
-                          1282 CALL                     1
-                          1292 STORE_DEREF             13 (request)
-               
-               124        1294 LOAD_DEREF              13 (request)
-                          1296 POP_JUMP_FORWARD_IF_FALSE   113 (to 1524)
-               
-               126        1298 LOAD_DEREF              13 (request)
-                          1300 LOAD_ATTR               25 (user)
-                          1310 LOAD_ATTR               26 (is_authenticated)
-               
-               125        1320 POP_JUMP_FORWARD_IF_FALSE    99 (to 1520)
-               
-               127        1322 LOAD_DEREF              13 (request)
-                          1324 LOAD_ATTR               25 (user)
-                          1334 LOAD_METHOD             27 (has_perm)
-                          1356 LOAD_CONST              12 ('wagtailadmin.access_admin')
-                          1358 PRECALL                  1
-                          1362 CALL                     1
-               
-               125        1372 POP_JUMP_FORWARD_IF_FALSE    73 (to 1520)
-               
-               128        1374 LOAD_DEREF              13 (request)
-                          1376 LOAD_ATTR               25 (user)
-                          1386 LOAD_METHOD             27 (has_perm)
-                          1408 LOAD_DEREF              12 (model)
-                          1410 LOAD_ATTR               28 (_meta)
-                          1420 LOAD_ATTR               29 (app_label)
-                          1430 FORMAT_VALUE             0
-                          1432 LOAD_CONST              13 ('.change_')
-                          1434 LOAD_DEREF              12 (model)
-                          1436 LOAD_ATTR               28 (_meta)
-                          1446 LOAD_ATTR               30 (model_name)
-                          1456 FORMAT_VALUE             0
-                          1458 BUILD_STRING             3
-                          1460 PRECALL                  1
-                          1464 CALL                     1
-               
-               125        1474 POP_JUMP_FORWARD_IF_FALSE    22 (to 1520)
-               
-               129        1476 LOAD_GLOBAL             63 (NULL + getattr)
-                          1488 LOAD_DEREF              13 (request)
-                          1490 LOAD_GLOBAL             64 (FEDIT_PREVIEW_VAR)
-                          1502 LOAD_CONST               6 (False)
-                          1504 PRECALL                  3
-                          1508 CALL                     3
-               
-               125        1518 POP_JUMP_FORWARD_IF_TRUE     2 (to 1524)
-               
-               132     >> 1520 LOAD_FAST                8 (rendered)
-                          1522 RETURN_VALUE
-               
-               136     >> 1524 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1536 LOAD_DEREF              12 (model)
-                          1538 LOAD_GLOBAL             66 (Page)
-                          1550 PRECALL                  2
-                          1554 CALL                     2
-                          1564 POP_JUMP_FORWARD_IF_FALSE    29 (to 1624)
-               
-               137        1566 LOAD_GLOBAL             69 (NULL + _get_from_context_or_set)
-               
-               138        1578 LOAD_FAST                1 (context)
-                          1580 LOAD_CONST              14 ('page_base_edit_url')
-               
-               139        1582 LOAD_CLOSURE            12 (model)
-                          1584 BUILD_TUPLE              1
-                          1586 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 139>)
-                          1588 MAKE_FUNCTION            8 (closure)
-               
-               137        1590 PRECALL                  3
-                          1594 CALL                     3
-                          1604 STORE_FAST               9 (admin_edit_url)
-               
-               144        1606 LOAD_FAST                9 (admin_edit_url)
-                          1608 FORMAT_VALUE             0
-                          1610 LOAD_CONST              16 ('#block-')
-                          1612 LOAD_FAST                3 (block_id)
-                          1614 FORMAT_VALUE             0
-                          1616 LOAD_CONST              17 ('-section')
-                          1618 BUILD_STRING             4
-                          1620 STORE_FAST               9 (admin_edit_url)
-                          1622 JUMP_FORWARD             2 (to 1628)
-               
-               146     >> 1624 LOAD_CONST               0 (None)
-                          1626 STORE_FAST               9 (admin_edit_url)
-               
-               148     >> 1628 LOAD_FAST                0 (self)
-                          1630 LOAD_ATTR               15 (has_block)
-                          1640 LOAD_FAST                5 (extra)
-                          1642 LOAD_CONST              18 ('has_block')
-                          1644 STORE_SUBSCR
-               
-               151        1648 LOAD_GLOBAL             71 (NULL + FeditBlockEditButton)
-                          1660 PRECALL                  0
-                          1664 CALL                     0
-               
-               150        1674 BUILD_LIST               1
-                          1676 STORE_FAST              10 (items)
-               
-               154        1678 LOAD_GLOBAL             73 (NULL + hooks)
-                          1690 LOAD_ATTR               37 (get_hooks)
-                          1700 LOAD_GLOBAL             76 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1712 PRECALL                  1
-                          1716 CALL                     1
-                          1726 GET_ITER
-                       >> 1728 FOR_ITER                18 (to 1766)
-                          1730 STORE_FAST              11 (hook)
-               
-               155        1732 PUSH_NULL
-                          1734 LOAD_FAST               11 (hook)
-                          1736 LOAD_DEREF              13 (request)
-                          1738 LOAD_FAST               10 (items)
-                          1740 LOAD_DEREF              12 (model)
-                          1742 LOAD_FAST                3 (block_id)
-                          1744 LOAD_FAST                4 (field_name)
-                          1746 KW_NAMES                19
-                          1748 PRECALL                  5
-                          1752 CALL                     5
-                          1762 POP_TOP
-                          1764 JUMP_BACKWARD           19 (to 1728)
-               
-               157     >> 1766 LOAD_CLOSURE            13 (request)
-                          1768 BUILD_TUPLE              1
-                          1770 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 157>)
-                          1772 MAKE_FUNCTION            8 (closure)
-                          1774 LOAD_FAST               10 (items)
-                          1776 GET_ITER
-                          1778 PRECALL                  0
-                          1782 CALL                     0
-                          1792 STORE_FAST              10 (items)
-               
-               158        1794 LOAD_GLOBAL             79 (NULL + list)
-                          1806 LOAD_GLOBAL             81 (NULL + filter)
-                          1818 LOAD_CONST               0 (None)
-                          1820 LOAD_FAST               10 (items)
-                          1822 PRECALL                  2
-                          1826 CALL                     2
-                          1836 PRECALL                  1
-                          1840 CALL                     1
-                          1850 STORE_FAST              10 (items)
-               
-               160        1852 LOAD_GLOBAL             83 (NULL + render_to_string)
-               
-               161        1864 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
-               
-               163        1866 PUSH_NULL
-                          1868 LOAD_FAST                0 (self)
-                          1870 LOAD_ATTR               42 (get_edit_url)
-               
-               164        1880 LOAD_FAST                3 (block_id)
-                          1882 LOAD_FAST                4 (field_name)
-               
-               163        1884 BUILD_TUPLE              2
-                          1886 LOAD_CONST              22 ('instance')
-               
-               165        1888 LOAD_DEREF              12 (model)
-               
-               163        1890 BUILD_MAP                1
-               
-               166        1892 LOAD_FAST                5 (extra)
-               
-               163        1894 DICT_MERGE               1
-                          1896 CALL_FUNCTION_EX         1
-               
-               168        1898 LOAD_FAST                9 (admin_edit_url)
-               
-               169        1900 LOAD_FAST                3 (block_id)
-               
-               170        1902 LOAD_DEREF              12 (model)
-               
-               171        1904 LOAD_FAST                8 (rendered)
-               
-               172        1906 LOAD_FAST                4 (field_name)
-               
-               173        1908 LOAD_FAST                1 (context)
-               
-               174        1910 LOAD_FAST                4 (field_name)
-               
-               175        1912 LOAD_DEREF              12 (model)
-               
-               176        1914 LOAD_FAST               10 (items)
-               
-               162        1916 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
-                          1918 BUILD_CONST_KEY_MAP     10
-               
-               160        1920 PRECALL                  2
-                          1924 CALL                     2
-                          1934 RETURN_VALUE
+               
+               108        1012 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+               
+               109        1024 LOAD_CONST               8 ('object')
+                          1026 LOAD_FAST                1 (context)
+                          1028 LOAD_ATTR               21 (template_name)
+                          1038 BUILD_MAP                1
+               
+               108        1040 BINARY_OP                6 (%)
+               
+               107        1044 PRECALL                  1
+                          1048 CALL                     1
+                          1058 POP_TOP
+               
+               111        1060 LOAD_FAST                9 (rendered)
+                          1062 RETURN_VALUE
+               
+               113     >> 1064 LOAD_DEREF              13 (model)
+                          1066 POP_JUMP_FORWARD_IF_TRUE    47 (to 1162)
+               
+               114        1068 LOAD_GLOBAL             37 (NULL + warnings)
+                          1080 LOAD_ATTR               19 (warn)
+               
+               115        1090 LOAD_GLOBAL             44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+               116        1102 LOAD_CONST               8 ('object')
+                          1104 LOAD_FAST                2 (block)
+                          1106 LOAD_ATTR                0 (block)
+                          1116 LOAD_ATTR               23 (__class__)
+                          1126 LOAD_ATTR               24 (__name__)
+                          1136 BUILD_MAP                1
+               
+               115        1138 BINARY_OP                6 (%)
+               
+               114        1142 PRECALL                  1
+                          1146 CALL                     1
+                          1156 POP_TOP
+               
+               118        1158 LOAD_FAST                9 (rendered)
+                          1160 RETURN_VALUE
+               
+               121     >> 1162 LOAD_FAST                3 (block_id)
+                          1164 POP_JUMP_FORWARD_IF_TRUE    13 (to 1192)
+                          1166 LOAD_CONST               2 ('block_id')
+                          1168 LOAD_FAST                1 (context)
+                          1170 CONTAINS_OP              0
+                          1172 POP_JUMP_FORWARD_IF_FALSE     9 (to 1192)
+               
+               122        1174 LOAD_FAST                1 (context)
+                          1176 LOAD_CONST               2 ('block_id')
+                          1178 BINARY_SUBSCR
+                          1188 STORE_FAST               3 (block_id)
+                          1190 JUMP_FORWARD            45 (to 1282)
+               
+               123     >> 1192 LOAD_FAST                3 (block_id)
+                          1194 POP_JUMP_FORWARD_IF_TRUE    26 (to 1248)
+                          1196 LOAD_FAST                2 (block)
+                          1198 POP_JUMP_FORWARD_IF_FALSE    24 (to 1248)
+                          1200 LOAD_GLOBAL             51 (NULL + hasattr)
+                          1212 LOAD_FAST                2 (block)
+                          1214 LOAD_CONST               9 ('id')
+                          1216 PRECALL                  2
+                          1220 CALL                     2
+                          1230 POP_JUMP_FORWARD_IF_FALSE     8 (to 1248)
+               
+               124        1232 LOAD_FAST                2 (block)
+                          1234 LOAD_ATTR               26 (id)
+                          1244 STORE_FAST               3 (block_id)
+                          1246 JUMP_FORWARD            17 (to 1282)
+               
+               125     >> 1248 LOAD_FAST                3 (block_id)
+                          1250 POP_JUMP_FORWARD_IF_TRUE    15 (to 1282)
+               
+               126        1252 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1264 LOAD_CONST               3 ('Block ID is required')
+                          1266 PRECALL                  1
+                          1270 CALL                     1
+                          1280 RAISE_VARARGS            1
+               
+               129     >> 1282 LOAD_FAST                1 (context)
+                          1284 LOAD_METHOD             10 (get)
+                          1306 LOAD_CONST              10 ('request')
+                          1308 PRECALL                  1
+                          1312 CALL                     1
+                          1322 STORE_DEREF             14 (request)
+               
+               130        1324 LOAD_GLOBAL             55 (NULL + _can_edit)
+                          1336 LOAD_DEREF              14 (request)
+                          1338 LOAD_DEREF              13 (model)
+                          1340 PRECALL                  2
+                          1344 CALL                     2
+                          1354 POP_JUMP_FORWARD_IF_TRUE     2 (to 1360)
+               
+               131        1356 LOAD_FAST                9 (rendered)
+                          1358 RETURN_VALUE
+               
+               135     >> 1360 LOAD_GLOBAL             13 (NULL + isinstance)
+                          1372 LOAD_DEREF              13 (model)
+                          1374 LOAD_GLOBAL             56 (Page)
+                          1386 PRECALL                  2
+                          1390 CALL                     2
+                          1400 POP_JUMP_FORWARD_IF_FALSE    29 (to 1460)
+               
+               136        1402 LOAD_GLOBAL             59 (NULL + _get_from_context_or_set)
+               
+               137        1414 LOAD_FAST                1 (context)
+                          1416 LOAD_CONST              11 ('page_base_edit_url')
+               
+               138        1418 LOAD_CLOSURE            13 (model)
+                          1420 BUILD_TUPLE              1
+                          1422 LOAD_CONST              12 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 138>)
+                          1424 MAKE_FUNCTION            8 (closure)
+               
+               136        1426 PRECALL                  3
+                          1430 CALL                     3
+                          1440 STORE_FAST              10 (admin_edit_url)
+               
+               143        1442 LOAD_FAST               10 (admin_edit_url)
+                          1444 FORMAT_VALUE             0
+                          1446 LOAD_CONST              13 ('#block-')
+                          1448 LOAD_FAST                3 (block_id)
+                          1450 FORMAT_VALUE             0
+                          1452 LOAD_CONST              14 ('-section')
+                          1454 BUILD_STRING             4
+                          1456 STORE_FAST              10 (admin_edit_url)
+                          1458 JUMP_FORWARD             2 (to 1464)
+               
+               145     >> 1460 LOAD_CONST               0 (None)
+                          1462 STORE_FAST              10 (admin_edit_url)
+               
+               147     >> 1464 LOAD_FAST                0 (self)
+                          1466 LOAD_ATTR               15 (has_block)
+                          1476 LOAD_FAST                5 (extra)
+                          1478 LOAD_CONST              15 ('has_block')
+                          1480 STORE_SUBSCR
+               
+               150        1484 LOAD_GLOBAL             61 (NULL + FeditBlockEditButton)
+                          1496 PRECALL                  0
+                          1500 CALL                     0
+               
+               149        1510 BUILD_LIST               1
+                          1512 STORE_FAST              11 (items)
+               
+               153        1514 LOAD_GLOBAL             63 (NULL + hooks)
+                          1526 LOAD_ATTR               32 (get_hooks)
+                          1536 LOAD_GLOBAL             66 (CONSTRUCT_BLOCK_TOOLBAR)
+                          1548 PRECALL                  1
+                          1552 CALL                     1
+                          1562 GET_ITER
+                       >> 1564 FOR_ITER                18 (to 1602)
+                          1566 STORE_FAST              12 (hook)
+               
+               154        1568 PUSH_NULL
+                          1570 LOAD_FAST               12 (hook)
+                          1572 LOAD_DEREF              14 (request)
+                          1574 LOAD_FAST               11 (items)
+                          1576 LOAD_DEREF              13 (model)
+                          1578 LOAD_FAST                3 (block_id)
+                          1580 LOAD_FAST                4 (field_name)
+                          1582 KW_NAMES                16
+                          1584 PRECALL                  5
+                          1588 CALL                     5
+                          1598 POP_TOP
+                          1600 JUMP_BACKWARD           19 (to 1564)
+               
+               156     >> 1602 LOAD_CLOSURE            14 (request)
+                          1604 BUILD_TUPLE              1
+                          1606 LOAD_CONST              17 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 156>)
+                          1608 MAKE_FUNCTION            8 (closure)
+                          1610 LOAD_FAST               11 (items)
+                          1612 GET_ITER
+                          1614 PRECALL                  0
+                          1618 CALL                     0
+                          1628 STORE_FAST              11 (items)
+               
+               157        1630 LOAD_GLOBAL             69 (NULL + list)
+                          1642 LOAD_GLOBAL             71 (NULL + filter)
+                          1654 LOAD_CONST               0 (None)
+                          1656 LOAD_FAST               11 (items)
+                          1658 PRECALL                  2
+                          1662 CALL                     2
+                          1672 PRECALL                  1
+                          1676 CALL                     1
+                          1686 STORE_FAST              11 (items)
+               
+               159        1688 LOAD_GLOBAL             73 (NULL + render_to_string)
+               
+               160        1700 LOAD_CONST              18 ('wagtail_fedit/content/editable_block.html')
+               
+               162        1702 PUSH_NULL
+                          1704 LOAD_FAST                0 (self)
+                          1706 LOAD_ATTR               37 (get_edit_url)
+               
+               163        1716 LOAD_FAST                3 (block_id)
+                          1718 LOAD_FAST                4 (field_name)
+               
+               162        1720 BUILD_TUPLE              2
+                          1722 LOAD_CONST              19 ('instance')
+               
+               164        1724 LOAD_DEREF              13 (model)
+               
+               162        1726 BUILD_MAP                1
+               
+               165        1728 LOAD_FAST                5 (extra)
+               
+               162        1730 DICT_MERGE               1
+                          1732 CALL_FUNCTION_EX         1
+               
+               167        1734 LOAD_FAST               10 (admin_edit_url)
+               
+               168        1736 LOAD_FAST                3 (block_id)
+               
+               169        1738 LOAD_DEREF              13 (model)
+               
+               170        1740 LOAD_FAST                9 (rendered)
+               
+               171        1742 LOAD_FAST                4 (field_name)
+               
+               172        1744 LOAD_FAST                1 (context)
+               
+               173        1746 LOAD_FAST                4 (field_name)
+               
+               174        1748 LOAD_DEREF              13 (model)
+               
+               175        1750 LOAD_FAST               11 (items)
+               
+               161        1752 LOAD_CONST              20 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
+                          1754 BUILD_CONST_KEY_MAP     10
+               
+               159        1756 PRECALL                  2
+                          1760 CALL                     2
+                          1770 RETURN_VALUE
                ExceptionTable:
                  700 to 738 -> 742 [0]
                  742 to 760 -> 768 [1] lasti
                  766 to 766 -> 768 [1] lasti
                consts
                   None
                   'wagtail_fedit_field_name'
                   'block_id'
                   'Block ID is required'
                   'wagtail_fedit_instance'
                   True
                   False
                   'Block or nodelist is required'
-                  'field'
-                  'block'
+                  'object'
                   'id'
                   'request'
-                  'wagtailadmin.access_admin'
-                  '.change_'
                   'page_base_edit_url'
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 4
                      flags     : 19
                      code
                         0x95019700740100000000000000000000640189006a0100000000000000
                         006701ac02a6020000ab0200000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     139           2 RESUME                   0
+                     138           2 RESUME                   0
                                    4 LOAD_GLOBAL              1 (NULL + reverse)
                      
-                     140          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
+                     139          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
                      
-                     141          18 LOAD_DEREF               0 (model)
+                     140          18 LOAD_DEREF               0 (model)
                                   20 LOAD_ATTR                1 (id)
                                   30 BUILD_LIST               1
                      
-                     139          32 KW_NAMES                 2
+                     138          32 KW_NAMES                 2
                                   34 PRECALL                  2
                                   38 CALL                     2
                                   48 RETURN_VALUE
                      consts
                         None
                         'wagtailadmin_pages:edit'
                         ('args',)
                      names      ('reverse', 'id')
                      varnames   ()
                      freevars   ('model',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<lambda>'
-                     firstlineno 139
+                     firstlineno 138
                      lnotab 0x100102010efe
                   '#block-'
                   '-section'
                   'has_block'
                   ('request', 'items', 'model', 'block_id', 'field_name')
                   code
                      argcount  : 1
@@ -1103,15 +1076,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d017c01a00000000000000000000000000000
                         000000000000008902a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     157           2 RESUME                   0
+                     156           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (item)
                                   12 LOAD_FAST                1 (item)
                                   14 LOAD_METHOD              0 (render)
                                   36 LOAD_DEREF               2 (request)
@@ -1123,31 +1096,31 @@
                      consts
                      names      ('render',)
                      varnames   ('.0', 'item')
                      freevars   ('request',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 157
+                     firstlineno 156
                      lnotab 0x
                   'wagtail_fedit/content/editable_block.html'
                   'instance'
                   ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'label', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
-               varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'rendered', 'admin_edit_url', 'items', 'hook')
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'template_name', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__class__', '__name__', 'hasattr', 'id', '_can_edit', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
+               varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'block_context', 'rendered', 'admin_edit_url', 'items', 'hook')
                freevars   ()
                cellvars   ('model', 'request')
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 56
                lnotab
                   0x06010e010e010e010e010e0332012a0132020c0110022a012a012a012a
                   012a012a012a012a0210011e052e010a010a04040102012c01120104ff08
-                  022a012a0110010e01340110021e0204013c0104020401460104030c0112
-                  012801100104011e032a01040216ff020232fe020364fd02042afc020704
+                  022a012a0110010e01340110021e02040116010c0110ff04ff1004040204
+                  0116010c0124ff04ff100404030c0112012801100104011e032a01200104
                   042a010c01040108fe10071202040214031aff0404360122021c013a020c
                   0102020e0104ff040202fe020302fd040502010201020102010201020102
                   01020102f204fe
             'return'
             code
                argcount  : 0
                nlocals   : 4
@@ -1155,53 +1128,53 @@
                flags     : 11
                code
                   0x970069007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d2f5c0200007d027d03740200
                   000000000000000000a00200000000000000000000000000000000000000
                   007407000000000000000000007c03a6010000ab010000000000000000a6
                   010000ab0100000000000000007c017c023c0000008c307c015300
-               180           0 RESUME                   0
+               179           0 RESUME                   0
                
-               183           2 BUILD_MAP                0
+               182           2 BUILD_MAP                0
                              4 STORE_FAST               1 (packed)
                
-               184           6 LOAD_FAST                0 (kwargs)
+               183           6 LOAD_FAST                0 (kwargs)
                              8 LOAD_METHOD              0 (items)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                47 (to 142)
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               2 (k)
                             54 STORE_FAST               3 (v)
                
-               185          56 LOAD_GLOBAL              2 (url_value_signer)
+               184          56 LOAD_GLOBAL              2 (url_value_signer)
                             68 LOAD_METHOD              2 (sign)
                             90 LOAD_GLOBAL              7 (NULL + str)
                            102 LOAD_FAST                3 (v)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                1 (packed)
                            134 LOAD_FAST                2 (k)
                            136 STORE_SUBSCR
                            140 JUMP_BACKWARD           48 (to 46)
                
-               187     >>  142 LOAD_FAST                1 (packed)
+               186     >>  142 LOAD_FAST                1 (packed)
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
-               firstlineno 180
+               firstlineno 179
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -1222,130 +1195,130 @@
                   057c039b009d02a6010000ab010000000000000000820177007803590077
                   0174150000000000000000000088046601640684087c024400a6000000ab
                   000000000000000000a6010000ab01000000000000000073187c00a00700
                   0000000000000000000000000000000000000064057c039b009d02a60100
                   00ab010000000000000000820189045300
                              0 MAKE_CELL                4 (unpacked)
                
-               189           2 RESUME                   0
+               188           2 RESUME                   0
                
-               191           4 LOAD_FAST                1 (request)
+               190           4 LOAD_FAST                1 (request)
                              6 POP_JUMP_FORWARD_IF_TRUE    15 (to 38)
                
-               192           8 LOAD_GLOBAL              1 (NULL + ValueError)
+               191           8 LOAD_GLOBAL              1 (NULL + ValueError)
                             20 LOAD_CONST               1 ('Request is required')
                             22 PRECALL                  1
                             26 CALL                     1
                             36 RAISE_VARARGS            1
                
-               194     >>   38 BUILD_MAP                0
+               193     >>   38 BUILD_MAP                0
                             40 STORE_DEREF              4 (unpacked)
                
-               195          42 LOAD_FAST                2 (expected)
+               194          42 LOAD_FAST                2 (expected)
                             44 GET_ITER
                        >>   46 FOR_ITER               171 (to 390)
                             48 STORE_FAST               3 (key)
                
-               196          50 NOP
+               195          50 NOP
                
-               197          52 LOAD_GLOBAL              2 (url_value_signer)
+               196          52 LOAD_GLOBAL              2 (url_value_signer)
                             64 LOAD_METHOD              2 (unsign)
                
-               198          86 LOAD_FAST                1 (request)
+               197          86 LOAD_FAST                1 (request)
                             88 LOAD_ATTR                3 (GET)
                             98 LOAD_METHOD              4 (get)
                            120 LOAD_FAST                3 (key)
                            122 PRECALL                  1
                            126 CALL                     1
                
-               197         136 PRECALL                  1
+               196         136 PRECALL                  1
                            140 CALL                     1
                            150 LOAD_DEREF               4 (unpacked)
                            152 LOAD_FAST                3 (key)
                            154 STORE_SUBSCR
                            158 JUMP_BACKWARD           57 (to 46)
                        >>  160 PUSH_EXC_INFO
                
-               200         162 LOAD_GLOBAL             10 (signing)
+               199         162 LOAD_GLOBAL             10 (signing)
                            174 LOAD_ATTR                6 (SignatureExpired)
                            184 CHECK_EXC_MATCH
                            186 POP_JUMP_FORWARD_IF_FALSE    26 (to 240)
                            188 POP_TOP
                
-               201         190 LOAD_FAST                0 (cls)
+               200         190 LOAD_FAST                0 (cls)
                            192 LOAD_METHOD              7 (UnpackError)
                            214 LOAD_CONST               2 ('Value for ')
                            216 LOAD_FAST                3 (key)
                            218 FORMAT_VALUE             0
                            220 LOAD_CONST               3 (' has expired')
                            222 BUILD_STRING             3
                            224 PRECALL                  1
                            228 CALL                     1
                            238 RAISE_VARARGS            1
                
-               202     >>  240 LOAD_GLOBAL             10 (signing)
+               201     >>  240 LOAD_GLOBAL             10 (signing)
                            252 LOAD_ATTR                8 (BadSignature)
                            262 CHECK_EXC_MATCH
                            264 POP_JUMP_FORWARD_IF_FALSE    25 (to 316)
                            266 POP_TOP
                
-               203         268 LOAD_FAST                0 (cls)
+               202         268 LOAD_FAST                0 (cls)
                            270 LOAD_METHOD              7 (UnpackError)
                            292 LOAD_CONST               4 ('Invalid value for ')
                            294 LOAD_FAST                3 (key)
                            296 FORMAT_VALUE             0
                            298 BUILD_STRING             2
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               204     >>  316 LOAD_GLOBAL             18 (TypeError)
+               203     >>  316 LOAD_GLOBAL             18 (TypeError)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    25 (to 382)
                            332 POP_TOP
                
-               205         334 LOAD_FAST                0 (cls)
+               204         334 LOAD_FAST                0 (cls)
                            336 LOAD_METHOD              7 (UnpackError)
                            358 LOAD_CONST               5 ('Missing value for ')
                            360 LOAD_FAST                3 (key)
                            362 FORMAT_VALUE             0
                            364 BUILD_STRING             2
                            366 PRECALL                  1
                            370 CALL                     1
                            380 RAISE_VARARGS            1
                
-               204     >>  382 RERAISE                  0
+               203     >>  382 RERAISE                  0
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
-               207     >>  390 LOAD_GLOBAL             21 (NULL + all)
+               206     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 207>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 206>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
                            442 POP_JUMP_FORWARD_IF_TRUE    24 (to 492)
                
-               208         444 LOAD_FAST                0 (cls)
+               207         444 LOAD_FAST                0 (cls)
                            446 LOAD_METHOD              7 (UnpackError)
                            468 LOAD_CONST               5 ('Missing value for ')
                            470 LOAD_FAST                3 (key)
                            472 FORMAT_VALUE             0
                            474 BUILD_STRING             2
                            476 PRECALL                  1
                            480 CALL                     1
                            490 RAISE_VARARGS            1
                
-               210     >>  492 LOAD_DEREF               4 (unpacked)
+               209     >>  492 LOAD_DEREF               4 (unpacked)
                            494 RETURN_VALUE
                ExceptionTable:
                  52 to 156 -> 160 [1]
                  160 to 382 -> 384 [2] lasti
                consts
                   None
                   'Request is required'
@@ -1359,15 +1332,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     207           2 RESUME                   0
+                     206           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (key)
                                   12 LOAD_DEREF               2 (unpacked)
                                   14 LOAD_METHOD              0 (get)
                                   36 LOAD_FAST                1 (key)
@@ -1379,23 +1352,23 @@
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 207
+                     firstlineno 206
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
-               firstlineno 189
+               firstlineno 188
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
                argcount  : 3
                nlocals   : 6
@@ -1404,58 +1377,58 @@
                code
                   0x970074010000000000000000000064017c007c017c026a010000000000
                   0000006a0200000000000000007c026a0100000000000000006a03000000
                   00000000007c026a0400000000000000006705ac02a6020000ab02000000
                   00000000007d047c0373027c045300740b00000000000000000000740d00
                   0000000000000000006a070000000000000000640469007c03a4018e01a6
                   010000ab0100000000000000007d057c049b0064037c059b009d035300
-               212           0 RESUME                   0
+               211           0 RESUME                   0
                
-               214           2 LOAD_GLOBAL              1 (NULL + reverse)
+               213           2 LOAD_GLOBAL              1 (NULL + reverse)
                
-               215          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
+               214          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
                
-               216          16 LOAD_FAST                0 (block_id)
+               215          16 LOAD_FAST                0 (block_id)
                             18 LOAD_FAST                1 (field_name)
                             20 LOAD_FAST                2 (instance)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (app_label)
                             42 LOAD_FAST                2 (instance)
                             44 LOAD_ATTR                1 (_meta)
                             54 LOAD_ATTR                3 (model_name)
                             64 LOAD_FAST                2 (instance)
                             66 LOAD_ATTR                4 (pk)
                             76 BUILD_LIST               5
                
-               214          78 KW_NAMES                 2
+               213          78 KW_NAMES                 2
                             80 PRECALL                  2
                             84 CALL                     2
                             94 STORE_FAST               4 (base_url)
                
-               219          96 LOAD_FAST                3 (kwargs)
+               218          96 LOAD_FAST                3 (kwargs)
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-               220         100 LOAD_FAST                4 (base_url)
+               219         100 LOAD_FAST                4 (base_url)
                            102 RETURN_VALUE
                
-               222     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
+               221     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
                
-               223         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+               222         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                            128 LOAD_ATTR                7 (pack)
                            138 LOAD_CONST               4 (())
                            140 BUILD_MAP                0
                            142 LOAD_FAST                3 (kwargs)
                            144 DICT_MERGE               1
                            146 CALL_FUNCTION_EX         1
                
-               222         148 PRECALL                  1
+               221         148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               5 (packed)
                
-               225         164 LOAD_FAST                4 (base_url)
+               224         164 LOAD_FAST                4 (base_url)
                            166 FORMAT_VALUE             0
                            168 LOAD_CONST               3 ('?')
                            170 LOAD_FAST                5 (packed)
                            172 FORMAT_VALUE             0
                            174 BUILD_STRING             3
                            176 RETURN_VALUE
                consts
@@ -1466,27 +1439,27 @@
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
-               firstlineno 212
+               firstlineno 211
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
          firstlineno 36
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
-            fc02050cfb0810067c02010aff0e010208020114ff0e010216020120ff0e
+            fc02050cfb0810067b02010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
       'fedit_block'
       ('name',)
       'parser'
       'token'
       code
@@ -1508,123 +1481,123 @@
             000000000000000000640a7c067c05a00700000000000000000000000000
             000000000000006403a6010000ab0100000000000000007c05a007000000
             00000000000000000000000000000000006406a6010000ab010000000000
             0000007c05a00700000000000000000000000000000000000000006407a6
             010000ab0100000000000000007c05a00700000000000000000000000000
             000000000000006408a6010000ab01000000000000000064099c057c07a4
             018e015300
-         229           0 RESUME                   0
+         228           0 RESUME                   0
          
-         259           2 LOAD_FAST                1 (token)
+         258           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         260          42 LOAD_FAST                2 (tokens)
+         259          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         261          84 BUILD_LIST               0
+         260          84 BUILD_LIST               0
                       86 LOAD_CONST               2 (('block', 'block_id', 'field_name', 'model'))
                       88 LIST_EXTEND              1
                       90 STORE_FAST               4 (kwargs_names)
          
-         266          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
+         265          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
                      104 LOAD_FAST                0 (parser)
                      106 LOAD_FAST                4 (kwargs_names)
                      108 LOAD_FAST                2 (tokens)
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_FAST               5 (kwargs)
          
-         268         126 LOAD_CONST               3 ('block')
+         267         126 LOAD_CONST               3 ('block')
                      128 LOAD_FAST                5 (kwargs)
                      130 CONTAINS_OP              1
                      132 POP_JUMP_FORWARD_IF_FALSE    42 (to 218)
          
-         269         134 LOAD_FAST                0 (parser)
+         268         134 LOAD_FAST                0 (parser)
                      136 LOAD_METHOD              3 (parse)
                      158 LOAD_CONST               4 (('unfedit_block',))
                      160 PRECALL                  1
                      164 CALL                     1
                      174 STORE_FAST               6 (nodelist)
          
-         270         176 LOAD_FAST                0 (parser)
+         269         176 LOAD_FAST                0 (parser)
                      178 LOAD_METHOD              4 (delete_first_token)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
                      216 JUMP_FORWARD             2 (to 222)
          
-         272     >>  218 LOAD_CONST               5 (None)
+         271     >>  218 LOAD_CONST               5 (None)
                      220 STORE_FAST               6 (nodelist)
          
-         274     >>  222 BUILD_MAP                0
+         273     >>  222 BUILD_MAP                0
                      224 STORE_FAST               7 (extra)
          
-         275         226 LOAD_FAST                5 (kwargs)
+         274         226 LOAD_FAST                5 (kwargs)
                      228 LOAD_METHOD              5 (items)
                      250 PRECALL                  0
                      254 CALL                     0
                      264 GET_ITER
                  >>  266 FOR_ITER                14 (to 296)
                      268 UNPACK_SEQUENCE          2
                      272 STORE_FAST               8 (key)
                      274 STORE_FAST               9 (value)
          
-         276         276 LOAD_FAST                8 (key)
+         275         276 LOAD_FAST                8 (key)
                      278 LOAD_FAST                4 (kwargs_names)
                      280 CONTAINS_OP              1
                      282 POP_JUMP_FORWARD_IF_FALSE     5 (to 294)
          
-         277         284 LOAD_FAST                9 (value)
+         276         284 LOAD_FAST                9 (value)
                      286 LOAD_FAST                7 (extra)
                      288 LOAD_FAST                8 (key)
                      290 STORE_SUBSCR
                  >>  294 JUMP_BACKWARD           15 (to 266)
          
-         279     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         278     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      308 LOAD_CONST              10 (())
          
-         280         310 LOAD_FAST                6 (nodelist)
+         279         310 LOAD_FAST                6 (nodelist)
          
-         281         312 LOAD_FAST                5 (kwargs)
+         280         312 LOAD_FAST                5 (kwargs)
                      314 LOAD_METHOD              7 (get)
                      336 LOAD_CONST               3 ('block')
                      338 PRECALL                  1
                      342 CALL                     1
          
-         282         352 LOAD_FAST                5 (kwargs)
+         281         352 LOAD_FAST                5 (kwargs)
                      354 LOAD_METHOD              7 (get)
                      376 LOAD_CONST               6 ('block_id')
                      378 PRECALL                  1
                      382 CALL                     1
          
-         283         392 LOAD_FAST                5 (kwargs)
+         282         392 LOAD_FAST                5 (kwargs)
                      394 LOAD_METHOD              7 (get)
                      416 LOAD_CONST               7 ('field_name')
                      418 PRECALL                  1
                      422 CALL                     1
          
-         284         432 LOAD_FAST                5 (kwargs)
+         283         432 LOAD_FAST                5 (kwargs)
                      434 LOAD_METHOD              7 (get)
                      456 LOAD_CONST               8 ('model')
                      458 PRECALL                  1
                      462 CALL                     1
          
-         279         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
+         278         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
                      474 BUILD_CONST_KEY_MAP      5
          
-         285         476 LOAD_FAST                7 (extra)
+         284         476 LOAD_FAST                7 (extra)
          
-         279         478 DICT_MERGE               1
+         278         478 DICT_MERGE               1
                      480 CALL_FUNCTION_EX         1
                      482 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable block.\n\n    This block will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the block_id and field_name of the streamfield this block belongs to.\n\n    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.\n    \n    Usage example 1:\n        ```python\n        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}\n        ```\n\n    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.\n\n    This will allow you to use the block as a block tag.\n\n    Usage example 2:\n        ```python\n        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}\n            <p>Some content before block</p>\n            {% include_block my_block %}\n            <p>Some content after block</p>\n        {% unfedit_block %}\n        ```\n    '
             0
             ('block', 'block_id', 'field_name', 'model')
             'block'
@@ -1637,49 +1610,49 @@
             ()
          names      ('split_contents', 'pop', 'get_kwargs', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
-         firstlineno 229
+         firstlineno 228
          lnotab
             0x021e28012a010805220208012a012a0204020401320108010c020e0102
             0128012801280128fb040602fa
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a026408640265036a040000000000000000640365
             05650619000000000000000000640465076606640584055a08640684005a
             0964075300
-         289           0 RESUME                   0
+         288           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FieldEditNode')
                        8 STORE_NAME               2 (__qualname__)
          
-         290          10 LOAD_CONST               8 ((False,))
+         289          10 LOAD_CONST               8 ((False,))
                       12 LOAD_CONST               2 ('model')
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (Model)
                       26 LOAD_CONST               3 ('getters')
                       28 LOAD_NAME                5 (list)
                       30 LOAD_NAME                6 (str)
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               4 ('inline')
                       44 LOAD_NAME                7 (bool)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 290>)
+                      48 LOAD_CONST               5 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 289>)
                       50 MAKE_FUNCTION            5 (defaults, annotations)
                       52 STORE_NAME               8 (__init__)
          
-         297          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 297>)
+         296          54 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 296>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (render)
                       60 LOAD_CONST               7 (None)
                       62 RETURN_VALUE
          consts
             'FieldEditNode'
             False
@@ -1693,54 +1666,54 @@
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027403000000000000000000
                   007c02a6010000ab01000000000000000064017a0a000019000000000000
                   0000007c005f0200000000000000007c027c005f0300000000000000007c
                   037c005f0400000000000000007c047c005f050000000000000000640053
                   00
-               290           0 RESUME                   0
+               289           0 RESUME                   0
                
-               291           2 LOAD_FAST                1 (model)
+               290           2 LOAD_FAST                1 (model)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (model)
                
-               292          16 LOAD_FAST                2 (getters)
+               291          16 LOAD_FAST                2 (getters)
                             18 LOAD_GLOBAL              3 (NULL + len)
                             30 LOAD_FAST                2 (getters)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               1 (1)
                             48 BINARY_OP               10 (-)
                             52 BINARY_SUBSCR
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (field)
                
-               293          74 LOAD_FAST                2 (getters)
+               292          74 LOAD_FAST                2 (getters)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (getters)
                
-               294          88 LOAD_FAST                3 (inline)
+               293          88 LOAD_FAST                3 (inline)
                             90 LOAD_FAST                0 (self)
                             92 STORE_ATTR               4 (inline)
                
-               295         102 LOAD_FAST                4 (kwargs)
+               294         102 LOAD_FAST                4 (kwargs)
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (kwargs)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                consts
                   None
                   1
                names      ('model', 'len', 'field', 'getters', 'inline', 'kwargs')
                varnames   ('self', 'model', 'getters', 'inline', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 290
+               firstlineno 289
                lnotab 0x02010e013a010e010e01
             code
                argcount  : 2
                nlocals   : 10
                stacksize : 10
                flags     : 3
                code
@@ -1758,257 +1731,209 @@
                   007d058c1c23007412000000000000000000002400722001007413000000
                   0000000000000064027c036a0a00000000000000006a0b00000000000000
                   009b0064037c079b009d04a6010000ab0100000000000000008201770078
                   03590077017c01a00c000000000000000000000000000000000000000064
                   04a6010000ab0100000000000000007d08741b000000000000000000007c
                   087c057c056a0e0000000000000000a00f00000000000000000000000000
                   000000000000007c006a100000000000000000a6010000ab010000000000
-                  0000007c01a6040000ab0400000000000000007d097c0872717c086a1100
-                  000000000000006a12000000000000000072637c086a1100000000000000
-                  00a01300000000000000000000000000000000000000006405a6010000ab
-                  01000000000000000072497c086a110000000000000000a0130000000000
-                  0000000000000000000000000000007c056a0e00000000000000006a1400
-                  000000000000009b0064067c056a0e00000000000000006a150000000000
-                  0000009b009d03a6010000ab010000000000000000721674110000000000
-                  00000000007c08742c000000000000000000006407a6030000ab03000000
-                  000000000073027c095300742f0000000000000000000064097c087c097c
-                  006a1000000000000000007c057c017c0464089c067c006a180000000000
-                  000000a4018e015300
-               297           0 RESUME                   0
+                  0000007c01a6040000ab0400000000000000007d09742300000000000000
+                  0000007c087c05a6020000ab02000000000000000073027c095300742500
+                  00000000000000000064067c087c097c006a1000000000000000007c057c
+                  017c0464059c067c006a130000000000000000a4018e015300
+               296           0 RESUME                   0
                
-               298           2 LOAD_FAST                0 (self)
+               297           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (getters)
                             14 STORE_FAST               2 (getters)
                
-               299          16 LOAD_FAST                0 (self)
+               298          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (model)
                             28 STORE_FAST               3 (model)
                
-               300          30 LOAD_FAST                0 (self)
+               299          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (inline)
                             42 STORE_FAST               4 (inline)
                
-               302          44 LOAD_GLOBAL              7 (NULL + isinstance)
+               301          44 LOAD_GLOBAL              7 (NULL + isinstance)
                             56 LOAD_FAST                3 (model)
                             58 LOAD_GLOBAL              8 (FilterExpression)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 POP_JUMP_FORWARD_IF_FALSE    21 (to 128)
                
-               303          86 LOAD_FAST                3 (model)
+               302          86 LOAD_FAST                3 (model)
                             88 LOAD_METHOD              5 (resolve)
                            110 LOAD_FAST                1 (context)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               3 (model)
                
-               305     >>  128 LOAD_GLOBAL              7 (NULL + isinstance)
+               304     >>  128 LOAD_GLOBAL              7 (NULL + isinstance)
                            140 LOAD_FAST                4 (inline)
                            142 LOAD_GLOBAL              8 (FilterExpression)
                            154 PRECALL                  2
                            158 CALL                     2
                            168 POP_JUMP_FORWARD_IF_FALSE    21 (to 212)
                
-               306         170 LOAD_FAST                4 (inline)
+               305         170 LOAD_FAST                4 (inline)
                            172 LOAD_METHOD              5 (resolve)
                            194 LOAD_FAST                1 (context)
                            196 PRECALL                  1
                            200 CALL                     1
                            210 STORE_FAST               4 (inline)
                
-               308     >>  212 LOAD_FAST                3 (model)
+               307     >>  212 LOAD_FAST                3 (model)
                            214 STORE_FAST               5 (obj)
                
-               309         216 LOAD_GLOBAL             13 (NULL + range)
+               308         216 LOAD_GLOBAL             13 (NULL + range)
                            228 LOAD_GLOBAL             15 (NULL + len)
                            240 LOAD_FAST                2 (getters)
                            242 PRECALL                  1
                            246 CALL                     1
                            256 LOAD_CONST               1 (1)
                            258 BINARY_OP               10 (-)
                            262 PRECALL                  1
                            266 CALL                     1
                            276 GET_ITER
                        >>  278 FOR_ITER                72 (to 424)
                            280 STORE_FAST               6 (i)
                
-               310         282 LOAD_FAST                2 (getters)
+               309         282 LOAD_FAST                2 (getters)
                            284 LOAD_FAST                6 (i)
                            286 BINARY_SUBSCR
                            296 STORE_FAST               7 (getter)
                
-               311         298 NOP
+               310         298 NOP
                
-               312         300 LOAD_GLOBAL             17 (NULL + getattr)
+               311         300 LOAD_GLOBAL             17 (NULL + getattr)
                            312 LOAD_FAST                5 (obj)
                            314 LOAD_FAST                7 (getter)
                            316 PRECALL                  2
                            320 CALL                     2
                            330 STORE_FAST               5 (obj)
                            332 JUMP_BACKWARD           28 (to 278)
                        >>  334 PUSH_EXC_INFO
                
-               313         336 LOAD_GLOBAL             18 (AttributeError)
+               312         336 LOAD_GLOBAL             18 (AttributeError)
                            348 CHECK_EXC_MATCH
                            350 POP_JUMP_FORWARD_IF_FALSE    32 (to 416)
                            352 POP_TOP
                
-               314         354 LOAD_GLOBAL             19 (NULL + AttributeError)
+               313         354 LOAD_GLOBAL             19 (NULL + AttributeError)
                            366 LOAD_CONST               2 ('Object ')
                            368 LOAD_FAST                3 (model)
                            370 LOAD_ATTR               10 (__class__)
                            380 LOAD_ATTR               11 (__name__)
                            390 FORMAT_VALUE             0
                            392 LOAD_CONST               3 (' does not have attribute ')
                            394 LOAD_FAST                7 (getter)
                            396 FORMAT_VALUE             0
                            398 BUILD_STRING             4
                            400 PRECALL                  1
                            404 CALL                     1
                            414 RAISE_VARARGS            1
                
-               313     >>  416 RERAISE                  0
+               312     >>  416 RERAISE                  0
                        >>  418 COPY                     3
                            420 POP_EXCEPT
                            422 RERAISE                  1
                
-               316     >>  424 LOAD_FAST                1 (context)
+               315     >>  424 LOAD_FAST                1 (context)
                            426 LOAD_METHOD             12 (get)
                            448 LOAD_CONST               4 ('request')
                            450 PRECALL                  1
                            454 CALL                     1
                            464 STORE_FAST               8 (request)
                
-               317         466 LOAD_GLOBAL             27 (NULL + get_field_content)
+               316         466 LOAD_GLOBAL             27 (NULL + get_field_content)
                
-               318         478 LOAD_FAST                8 (request)
+               317         478 LOAD_FAST                8 (request)
                
-               319         480 LOAD_FAST                5 (obj)
+               318         480 LOAD_FAST                5 (obj)
                
-               320         482 LOAD_FAST                5 (obj)
+               319         482 LOAD_FAST                5 (obj)
                            484 LOAD_ATTR               14 (_meta)
                            494 LOAD_METHOD             15 (get_field)
                            516 LOAD_FAST                0 (self)
                            518 LOAD_ATTR               16 (field)
                            528 PRECALL                  1
                            532 CALL                     1
                
-               321         542 LOAD_FAST                1 (context)
+               320         542 LOAD_FAST                1 (context)
                
-               317         544 PRECALL                  4
+               316         544 PRECALL                  4
                            548 CALL                     4
                            558 STORE_FAST               9 (content)
                
-               324         560 LOAD_FAST                8 (request)
-                           562 POP_JUMP_FORWARD_IF_FALSE   113 (to 790)
-               
-               326         564 LOAD_FAST                8 (request)
-                           566 LOAD_ATTR               17 (user)
-                           576 LOAD_ATTR               18 (is_authenticated)
-               
-               325         586 POP_JUMP_FORWARD_IF_FALSE    99 (to 786)
-               
-               327         588 LOAD_FAST                8 (request)
-                           590 LOAD_ATTR               17 (user)
-                           600 LOAD_METHOD             19 (has_perm)
-                           622 LOAD_CONST               5 ('wagtailadmin.access_admin')
-                           624 PRECALL                  1
-                           628 CALL                     1
-               
-               325         638 POP_JUMP_FORWARD_IF_FALSE    73 (to 786)
-               
-               328         640 LOAD_FAST                8 (request)
-                           642 LOAD_ATTR               17 (user)
-                           652 LOAD_METHOD             19 (has_perm)
-                           674 LOAD_FAST                5 (obj)
-                           676 LOAD_ATTR               14 (_meta)
-                           686 LOAD_ATTR               20 (app_label)
-                           696 FORMAT_VALUE             0
-                           698 LOAD_CONST               6 ('.change_')
-                           700 LOAD_FAST                5 (obj)
-                           702 LOAD_ATTR               14 (_meta)
-                           712 LOAD_ATTR               21 (model_name)
-                           722 FORMAT_VALUE             0
-                           724 BUILD_STRING             3
-                           726 PRECALL                  1
-                           730 CALL                     1
+               323         560 LOAD_GLOBAL             35 (NULL + _can_edit)
+                           572 LOAD_FAST                8 (request)
+                           574 LOAD_FAST                5 (obj)
+                           576 PRECALL                  2
+                           580 CALL                     2
+                           590 POP_JUMP_FORWARD_IF_TRUE     2 (to 596)
                
-               325         740 POP_JUMP_FORWARD_IF_FALSE    22 (to 786)
+               324         592 LOAD_FAST                9 (content)
+                           594 RETURN_VALUE
                
-               329         742 LOAD_GLOBAL             17 (NULL + getattr)
-                           754 LOAD_FAST                8 (request)
-                           756 LOAD_GLOBAL             44 (FEDIT_PREVIEW_VAR)
-                           768 LOAD_CONST               7 (False)
-                           770 PRECALL                  3
-                           774 CALL                     3
+               326     >>  596 LOAD_GLOBAL             37 (NULL + render_editable_field)
+                           608 LOAD_CONST               6 (())
                
-               325         784 POP_JUMP_FORWARD_IF_TRUE     2 (to 790)
+               327         610 LOAD_FAST                8 (request)
                
-               331     >>  786 LOAD_FAST                9 (content)
-                           788 RETURN_VALUE
+               328         612 LOAD_FAST                9 (content)
                
-               333     >>  790 LOAD_GLOBAL             47 (NULL + render_editable_field)
-                           802 LOAD_CONST               9 (())
+               329         614 LOAD_FAST                0 (self)
+                           616 LOAD_ATTR               16 (field)
                
-               334         804 LOAD_FAST                8 (request)
+               330         626 LOAD_FAST                5 (obj)
                
-               335         806 LOAD_FAST                9 (content)
+               331         628 LOAD_FAST                1 (context)
                
-               336         808 LOAD_FAST                0 (self)
-                           810 LOAD_ATTR               16 (field)
+               332         630 LOAD_FAST                4 (inline)
                
-               337         820 LOAD_FAST                5 (obj)
+               326         632 LOAD_CONST               5 (('request', 'content', 'field_name', 'model', 'context', 'inline'))
+                           634 BUILD_CONST_KEY_MAP      6
                
-               338         822 LOAD_FAST                1 (context)
+               333         636 LOAD_FAST                0 (self)
+                           638 LOAD_ATTR               19 (kwargs)
                
-               339         824 LOAD_FAST                4 (inline)
-               
-               333         826 LOAD_CONST               8 (('request', 'content', 'field_name', 'model', 'context', 'inline'))
-                           828 BUILD_CONST_KEY_MAP      6
-               
-               340         830 LOAD_FAST                0 (self)
-                           832 LOAD_ATTR               24 (kwargs)
-               
-               333         842 DICT_MERGE               1
-                           844 CALL_FUNCTION_EX         1
-                           846 RETURN_VALUE
+               326         648 DICT_MERGE               1
+                           650 CALL_FUNCTION_EX         1
+                           652 RETURN_VALUE
                ExceptionTable:
                  300 to 330 -> 334 [1]
                  334 to 416 -> 418 [2] lasti
                consts
                   None
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
-                  'wagtailadmin.access_admin'
-                  '.change_'
-                  False
                   ('request', 'content', 'field_name', 'model', 'context', 'inline')
                   ()
-               names      ('getters', 'model', 'inline', 'isinstance', 'FilterExpression', 'resolve', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', 'user', 'is_authenticated', 'has_perm', 'app_label', 'model_name', 'FEDIT_PREVIEW_VAR', 'render_editable_field', 'kwargs')
+               names      ('getters', 'model', 'inline', 'isinstance', 'FilterExpression', 'resolve', 'range', 'len', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'get_field_content', '_meta', 'get_field', 'field', '_can_edit', 'render_editable_field', 'kwargs')
                varnames   ('self', 'context', 'getters', 'model', 'inline', 'obj', 'i', 'getter', 'request', 'content')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 297
+               firstlineno 296
                lnotab
                   0x02010e010e010e022a012a022a012a020401420110010201240112013e
-                  ff08032a010c01020102013c0102fc1007040216ff020232fe020364fd02
-                  042afc020604020e01020102010c010201020102fa04070cf9
+                  ff08032a010c01020102013c0102fc1007200104020e01020102010c0102
+                  01020102fa04070cf9
             None
             (False,)
          names      ('__name__', '__module__', '__qualname__', 'models', 'Model', 'list', 'str', 'bool', '__init__', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'FieldEditNode'
-         firstlineno 289
+         firstlineno 288
          lnotab 0x0a012c07
       'FieldEditNode'
       'fedit_field'
       code
          argcount  : 2
          nlocals   : 9
          stacksize : 6
@@ -2024,101 +1949,101 @@
             0000000000000000006404a6010000ab01000000000000000082017c00a0
             0500000000000000000000000000000000000000007c05a0010000000000
             0000000000000000000000000000006401a6010000ab0100000000000000
             00a6010000ab0100000000000000007d067c027215640567017d07740d00
             0000000000000000007c007c077c02a6030000ab0300000000000000007d
             086e0269007d08740f0000000000000000000064077c067c0564069c027c
             08a4018e015300
-         345           0 RESUME                   0
+         338           0 RESUME                   0
          
-         360           2 LOAD_FAST                1 (token)
+         353           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         361          42 LOAD_FAST                2 (tokens)
+         354          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         362          84 LOAD_FAST                2 (tokens)
+         355          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (model__field)
          
-         363         126 LOAD_FAST                4 (model__field)
+         356         126 LOAD_FAST                4 (model__field)
                      128 LOAD_METHOD              2 (split)
                      150 LOAD_CONST               2 ('.')
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               5 (model_tokens)
          
-         365         168 LOAD_GLOBAL              7 (NULL + len)
+         358         168 LOAD_GLOBAL              7 (NULL + len)
                      180 LOAD_FAST                5 (model_tokens)
                      182 PRECALL                  1
                      186 CALL                     1
                      196 LOAD_CONST               3 (2)
                      198 COMPARE_OP               0 (<)
                      204 POP_JUMP_FORWARD_IF_FALSE    15 (to 236)
          
-         366         206 LOAD_GLOBAL              9 (NULL + ValueError)
+         359         206 LOAD_GLOBAL              9 (NULL + ValueError)
                      218 LOAD_CONST               4 ('Model and field name are required')
                      220 PRECALL                  1
                      224 CALL                     1
                      234 RAISE_VARARGS            1
          
-         370     >>  236 LOAD_FAST                0 (parser)
+         363     >>  236 LOAD_FAST                0 (parser)
                      238 LOAD_METHOD              5 (compile_filter)
                      260 LOAD_FAST                5 (model_tokens)
                      262 LOAD_METHOD              1 (pop)
                      284 LOAD_CONST               1 (0)
                      286 PRECALL                  1
                      290 CALL                     1
                      300 PRECALL                  1
                      304 CALL                     1
                      314 STORE_FAST               6 (model)
          
-         372         316 LOAD_FAST                2 (tokens)
+         365         316 LOAD_FAST                2 (tokens)
                      318 POP_JUMP_FORWARD_IF_FALSE    21 (to 362)
          
-         374         320 LOAD_CONST               5 ('inline')
+         367         320 LOAD_CONST               5 ('inline')
          
-         373         322 BUILD_LIST               1
+         366         322 BUILD_LIST               1
                      324 STORE_FAST               7 (kwargs_names)
          
-         377         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
+         370         326 LOAD_GLOBAL             13 (NULL + get_kwargs)
                      338 LOAD_FAST                0 (parser)
                      340 LOAD_FAST                7 (kwargs_names)
                      342 LOAD_FAST                2 (tokens)
                      344 PRECALL                  3
                      348 CALL                     3
                      358 STORE_FAST               8 (kwargs)
                      360 JUMP_FORWARD             2 (to 366)
          
-         379     >>  362 BUILD_MAP                0
+         372     >>  362 BUILD_MAP                0
                      364 STORE_FAST               8 (kwargs)
          
-         381     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
+         374     >>  366 LOAD_GLOBAL             15 (NULL + FieldEditNode)
                      378 LOAD_CONST               7 (())
          
-         382         380 LOAD_FAST                6 (model)
+         375         380 LOAD_FAST                6 (model)
          
-         383         382 LOAD_FAST                5 (model_tokens)
+         376         382 LOAD_FAST                5 (model_tokens)
          
-         381         384 LOAD_CONST               6 (('model', 'getters'))
+         374         384 LOAD_CONST               6 (('model', 'getters'))
                      386 BUILD_CONST_KEY_MAP      2
          
-         384         388 LOAD_FAST                8 (kwargs)
+         377         388 LOAD_FAST                8 (kwargs)
          
-         381         390 DICT_MERGE               1
+         374         390 DICT_MERGE               1
                      392 CALL_FUNCTION_EX         1
                      394 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    Usage example:\n        ```python\n        {% fedit_field mymodel.myfield inline=(default: False) key1=value1 key2=value2 %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             0
             '.'
             2
@@ -2128,15 +2053,15 @@
             ()
          names      ('split_contents', 'pop', 'split', 'len', 'ValueError', 'compile_filter', 'get_kwargs', 'FieldEditNode')
          varnames   ('parser', 'token', 'tokens', '_', 'model__field', 'model_tokens', 'model', 'kwargs_names', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
-         firstlineno 345
+         firstlineno 338
          lnotab
             0x020f28012a012a012a0226011e045002040202ff0404240204020e0102
             0102fe040302fd
       code
          argcount  : 5
          nlocals   : 10
          stacksize : 10
@@ -2160,120 +2085,120 @@
             00a6010000ab010000000000000000a01000000000000000000000000000
             00000000000000a6000000ab000000000000000000640a6b02000000007c
             0564083c000000742300000000000000000000640b7c067c027c037c017c
             047c08640c9c067c05a5018900ac0da6030000ab03000000000000000053
             00
                        0 MAKE_CELL                0 (request)
          
-         388           2 RESUME                   0
+         381           2 RESUME                   0
          
-         389           4 LOAD_GLOBAL              1 (NULL + reverse)
+         382           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         390          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         383          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         391          18 LOAD_FAST                2 (field_name)
+         384          18 LOAD_FAST                2 (field_name)
                       20 LOAD_FAST                3 (model)
                       22 LOAD_ATTR                1 (_meta)
                       32 LOAD_ATTR                2 (app_label)
                       42 LOAD_FAST                3 (model)
                       44 LOAD_ATTR                1 (_meta)
                       54 LOAD_ATTR                3 (model_name)
                       64 LOAD_FAST                3 (model)
                       66 LOAD_ATTR                4 (pk)
                       76 BUILD_LIST               4
          
-         389          78 KW_NAMES                 2
+         382          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         394          96 LOAD_FAST                5 (kwargs)
+         387          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         395         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         388         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         396         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         389         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
                      134 LOAD_CONST              14 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         395         144 PRECALL                  1
+         388         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         398         160 LOAD_FAST                6 (edit_url)
+         391         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         401     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         394     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         400         200 BUILD_LIST               1
+         393         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         404         204 LOAD_GLOBAL             19 (NULL + hooks)
+         397         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         405         258 PUSH_NULL
+         398         258 PUSH_NULL
                      260 LOAD_FAST                9 (hook)
                      262 LOAD_DEREF               0 (request)
                      264 LOAD_FAST                8 (items)
                      266 LOAD_FAST                3 (model)
                      268 LOAD_FAST                2 (field_name)
                      270 KW_NAMES                 4
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
-         407     >>  290 LOAD_CLOSURE             0 (request)
+         400     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 407>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 400>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         408         318 LOAD_GLOBAL             25 (NULL + list)
+         401         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         410         376 LOAD_FAST                2 (field_name)
+         403         376 LOAD_FAST                2 (field_name)
                      378 LOAD_FAST                5 (kwargs)
                      380 LOAD_CONST               6 ('wagtail_fedit_field_name')
                      382 STORE_SUBSCR
          
-         411         386 LOAD_FAST                3 (model)
+         404         386 LOAD_FAST                3 (model)
                      388 LOAD_FAST                5 (kwargs)
                      390 LOAD_CONST               7 ('wagtail_fedit_instance')
                      392 STORE_SUBSCR
          
-         412         396 LOAD_GLOBAL             29 (NULL + str)
+         405         396 LOAD_GLOBAL             29 (NULL + str)
                      408 LOAD_FAST                5 (kwargs)
                      410 LOAD_METHOD             15 (get)
                      432 LOAD_CONST               8 ('inline')
                      434 LOAD_CONST               9 (False)
                      436 PRECALL                  2
                      440 CALL                     2
                      450 PRECALL                  1
@@ -2283,40 +2208,40 @@
                      490 CALL                     0
                      500 LOAD_CONST              10 ('true')
                      502 COMPARE_OP               2 (==)
                      508 LOAD_FAST                5 (kwargs)
                      510 LOAD_CONST               8 ('inline')
                      512 STORE_SUBSCR
          
-         413         516 LOAD_GLOBAL             35 (NULL + render_to_string)
+         406         516 LOAD_GLOBAL             35 (NULL + render_to_string)
          
-         414         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
+         407         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
          
-         416         530 LOAD_FAST                6 (edit_url)
+         409         530 LOAD_FAST                6 (edit_url)
          
-         417         532 LOAD_FAST                2 (field_name)
+         410         532 LOAD_FAST                2 (field_name)
          
-         418         534 LOAD_FAST                3 (model)
+         411         534 LOAD_FAST                3 (model)
          
-         419         536 LOAD_FAST                1 (content)
+         412         536 LOAD_FAST                1 (content)
          
-         420         538 LOAD_FAST                4 (context)
+         413         538 LOAD_FAST                4 (context)
          
-         421         540 LOAD_FAST                8 (items)
+         414         540 LOAD_FAST                8 (items)
          
-         415         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+         408         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
                      544 BUILD_CONST_KEY_MAP      6
          
-         422         546 LOAD_FAST                5 (kwargs)
+         415         546 LOAD_FAST                5 (kwargs)
          
-         415         548 DICT_UPDATE              1
+         408         548 DICT_UPDATE              1
          
-         424         550 LOAD_DEREF               0 (request)
+         417         550 LOAD_DEREF               0 (request)
          
-         413         552 KW_NAMES                13
+         406         552 KW_NAMES                13
                      554 PRECALL                  3
                      558 CALL                     3
                      568 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
@@ -2328,15 +2253,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               407           2 RESUME                   0
+               400           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2348,15 +2273,15 @@
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 407
+               firstlineno 400
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
             'inline'
             False
             'true'
             'wagtail_fedit/content/editable_field.html'
@@ -2365,15 +2290,15 @@
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'str', 'get', 'lower', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 388
+         firstlineno 381
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020a010a0178010c0102020201020102010201020102fa040702f902
             0902f5
       'kwarg_list'
       'tokens'
       'return'
@@ -2390,89 +2315,89 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         427           0 RESUME                   0
+         420           0 RESUME                   0
          
-         428           2 LOAD_CONST               1 (False)
+         421           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         429           6 BUILD_MAP                0
+         422           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         434          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         427          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         435          50 LOAD_FAST                6 (token)
+         428          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         436          92 LOAD_GLOBAL              5 (NULL + len)
+         429          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         437         130 LOAD_FAST                3 (had_kwargs)
+         430         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         438         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         431         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         440     >>  164 LOAD_FAST                0 (parser)
+         433     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         442     >>  226 LOAD_FAST                7 (split)
+         435     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         446         242 LOAD_FAST                0 (parser)
+         439         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         447         302 LOAD_CONST               6 (True)
+         440         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         449     >>  308 LOAD_FAST                4 (kwargs)
+         442     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -2480,73 +2405,157 @@
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 427
+         firstlineno 420
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
+      'obj'
+      code
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 5
+         flags     : 3
+         code
+            0x97007c0072027c017302640153007c006a0000000000000000006a0100
+            000000000000000c0070657c006a000000000000000000a0020000000000
+            0000000000000000000000000000006402a6010000ab0100000000000000
+            000c00704a7c006a000000000000000000a0020000000000000000000000
+            0000000000000000007c016a0300000000000000006a0400000000000000
+            009b0064037c016a0300000000000000006a0500000000000000009b009d
+            03a6010000ab0100000000000000000c007016740d000000000000000000
+            007c00740e000000000000000000006401a6030000ab0300000000000000
+            000c000c005300
+         445           0 RESUME                   0
+         
+         446           2 LOAD_FAST                0 (request)
+                       4 POP_JUMP_FORWARD_IF_FALSE     2 (to 10)
+                       6 LOAD_FAST                1 (obj)
+                       8 POP_JUMP_FORWARD_IF_TRUE     2 (to 14)
+         
+         447     >>   10 LOAD_CONST               1 (False)
+                      12 RETURN_VALUE
+         
+         450     >>   14 LOAD_FAST                0 (request)
+                      16 LOAD_ATTR                0 (user)
+                      26 LOAD_ATTR                1 (is_authenticated)
+                      36 UNARY_NOT
+                      38 JUMP_IF_TRUE_OR_POP    101 (to 242)
+         
+         451          40 LOAD_FAST                0 (request)
+                      42 LOAD_ATTR                0 (user)
+                      52 LOAD_METHOD              2 (has_perm)
+                      74 LOAD_CONST               2 ('wagtailadmin.access_admin')
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 UNARY_NOT
+         
+         450          92 JUMP_IF_TRUE_OR_POP     74 (to 242)
+         
+         452          94 LOAD_FAST                0 (request)
+                      96 LOAD_ATTR                0 (user)
+                     106 LOAD_METHOD              2 (has_perm)
+                     128 LOAD_FAST                1 (obj)
+                     130 LOAD_ATTR                3 (_meta)
+                     140 LOAD_ATTR                4 (app_label)
+                     150 FORMAT_VALUE             0
+                     152 LOAD_CONST               3 ('.change_')
+                     154 LOAD_FAST                1 (obj)
+                     156 LOAD_ATTR                3 (_meta)
+                     166 LOAD_ATTR                5 (model_name)
+                     176 FORMAT_VALUE             0
+                     178 BUILD_STRING             3
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 UNARY_NOT
+         
+         450         196 JUMP_IF_TRUE_OR_POP     22 (to 242)
+         
+         453         198 LOAD_GLOBAL             13 (NULL + getattr)
+                     210 LOAD_FAST                0 (request)
+                     212 LOAD_GLOBAL             14 (FEDIT_PREVIEW_VAR)
+                     224 LOAD_CONST               1 (False)
+                     226 PRECALL                  3
+                     230 CALL                     3
+                     240 UNARY_NOT
+         
+         449     >>  242 UNARY_NOT
+                     244 RETURN_VALUE
+         consts
+            None
+            False
+            'wagtailadmin.access_admin'
+            '.change_'
+         names      ('user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR')
+         varnames   ('request', 'obj')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         name       '_can_edit'
+         firstlineno 445
+         lnotab 0x0201080104031a0134ff020266fe02032cfc
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 15
          code
             0x97007c017c00760072087c007c01190000000000000000005300740100
             0000000000000000007c02a6010000ab010000000000000000720802007c
             027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         454           0 RESUME                   0
+         457           0 RESUME                   0
          
-         455           2 LOAD_FAST                1 (key)
+         458           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         456          10 LOAD_FAST                0 (context)
+         459          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         458     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         461     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         459          56 PUSH_NULL
+         462          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         461     >>   72 LOAD_FAST                2 (value)
+         464     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         462          82 LOAD_FAST                2 (value)
+         465          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 454
+         firstlineno 457
          lnotab 0x0201080110021e0110020a01
-   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
+   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'FieldEditNode', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', 'Model', '_can_edit', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0110010c010c010c010c010c020c010c010c010c0208
-      021004100110061e011e03040104031c7f00422a010eff0e01023b1c382a
-      010eff0e01022a0627301b
+      021004100110061e011e03040104031c7f00412a010eff0e01023b1c322a
+      010eff0e01022a06273019160c
```

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.0/wagtail_fedit/templatetags/fedit.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 )
 
 
 register = library.Library()
 url_value_signer = signing.TimestampSigner()
 
 
-WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for field %(field)s."
-WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for block %(block)s."
+WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for %(object)s."
+WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for %(object)s."
 
 
 class BlockEditNode(Node):
     class UnpackError(Exception):
         pass
 
     def __init__(self,
@@ -87,53 +87,52 @@
         context["wagtail_fedit_field_name"] = field_name
         context["wagtail_fedit_instance"] = model
         
         # Render the block or nodelist
         # This allows us to use the block as a block tag or as a simple tag.
         if block:
             try:
-                context = context.flatten()
+                block_context = context.flatten()
             except AttributeError:
-                pass
-            context.update(extra)
-            rendered = block.render_as_block(context)
+                block_context = context
+            block_context.update(extra)
+            rendered = block.render_as_block(block_context)
             self.has_block = True
         elif self.nl:
             rendered = self.nl.render(context)
             self.has_block = False
         else:
             raise ValueError("Block or nodelist is required")
         
         if not field_name:
-            warnings.warn(WARNING_FIELD_NAME_NOT_AVAILABLE % {"field": field_name})
+            warnings.warn(
+                WARNING_FIELD_NAME_NOT_AVAILABLE
+                % {"object": context.template_name}
+            )
             return rendered
         
         if not model:
-            warnings.warn(WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {"block": block.label})
+            warnings.warn(
+                WARNING_MODEL_INSTANCE_NOT_AVAILABLE
+                % {"object": block.block.__class__.__name__}
+            )
             return rendered
         
         # Get block id from block if bound or context.
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
         elif not block_id:
             raise ValueError("Block ID is required")
 
         # Check if the user has permission to edit the block.
         request = context.get("request")
-        if request:
-            if (
-                not request.user.is_authenticated\
-                or not request.user.has_perm("wagtailadmin.access_admin")\
-                or not request.user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")    
-                or not getattr(request, FEDIT_PREVIEW_VAR, False)
-            ):
-                
-                return rendered
+        if not _can_edit(request, model):
+            return rendered
 
         # If the model is a page, we can redirect the user to the page editor.
         # This will act as a shortcut; jumping to the block inside of the admin.
         if isinstance(model, Page):
             admin_edit_url = _get_from_context_or_set(
                 context, "page_base_edit_url",
                 lambda: reverse(
@@ -317,22 +316,16 @@
         content = get_field_content(
             request,
             obj,
             obj._meta.get_field(self.field),
             context,
         )
 
-        if request:
-            if (
-                not request.user.is_authenticated\
-                or not request.user.has_perm("wagtailadmin.access_admin")\
-                or not request.user.has_perm(f"{obj._meta.app_label}.change_{obj._meta.model_name}")\
-                or not getattr(request, FEDIT_PREVIEW_VAR, False)
-            ):
-                return content
+        if not _can_edit(request, obj):
+            return content
             
         return render_editable_field(
             request=request, 
             content=content,
             field_name=self.field, 
             model=obj,
             context=context,
@@ -445,14 +438,24 @@
             
             kwargs[key] = parser.compile_filter(split[1])
             had_kwargs = True
 
     return kwargs
 
 
+def _can_edit(request, obj: models.Model):
+    if not request or not obj:
+        return False
+    
+    return not (
+        not request.user.is_authenticated\
+        or not request.user.has_perm("wagtailadmin.access_admin")\
+        or not request.user.has_perm(f"{obj._meta.app_label}.change_{obj._meta.model_name}")\
+        or not getattr(request, FEDIT_PREVIEW_VAR, False)
+    )
 
 
 def _get_from_context_or_set(context, key, value, *args, **kwargs):
     if key in context:
         return context[key]
     
     if callable(value):
```

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     BaseFEditTest,
 )
 
 import json
 
 class TestBlockEdit(BaseFEditTest):
     def test_block_edited(self):
+
         self.client.force_login(self.admin_user)
         
         for i, model in enumerate(self.models):
             
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 0)
             else:
```

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.0/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.0/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.0/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.0/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.4.0/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.0/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.4.0/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.0/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.0/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.9/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.0/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

