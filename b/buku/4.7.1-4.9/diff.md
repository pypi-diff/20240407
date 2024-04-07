# Comparing `tmp/buku-4.7.1.tar.gz` & `tmp/buku-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buku-4.7.1.tar", last modified: Fri Jul  1 22:38:36 2022, max compression
+gzip compressed data, was "buku-4.9.tar", last modified: Sun Apr  7 05:37:14 2024, max compression
```

## Comparing `buku-4.7.1.tar` & `buku-4.9.tar`

### file list

```diff
@@ -1,66 +1,78 @@
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.550615 buku-4.7.1/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    19686 2022-07-01 22:29:19.000000 buku-4.7.1/CHANGELOG
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    35142 2022-07-01 22:29:19.000000 buku-4.7.1/LICENSE
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      283 2022-07-01 22:29:19.000000 buku-4.7.1/MANIFEST.in
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    25840 2022-07-01 22:38:36.550615 buku-4.7.1/PKG-INFO
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    24661 2022-07-01 22:29:19.000000 buku-4.7.1/README.md
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.542615 buku-4.7.1/auto-completion/
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/auto-completion/bash/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1630 2022-07-01 22:29:19.000000 buku-4.7.1/auto-completion/bash/buku-completion.bash
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/auto-completion/fish/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     3105 2022-07-01 22:29:19.000000 buku-4.7.1/auto-completion/fish/buku.fish
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/auto-completion/zsh/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     2484 2022-07-01 22:29:19.000000 buku-4.7.1/auto-completion/zsh/_buku
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    27131 2022-07-01 22:29:19.000000 buku-4.7.1/buku.1
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/buku.egg-info/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    25840 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/PKG-INFO
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1463 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/SOURCES.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)        1 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/dependency_links.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)       71 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/entry_points.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1405 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/requires.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)       16 2022-07-01 22:38:36.000000 buku-4.7.1/buku.egg-info/top_level.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)   195941 2022-07-01 22:38:36.000000 buku-4.7.1/buku.py
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/bukuserver/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/__init__.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      130 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/__main__.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     7778 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/filters.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      703 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/forms.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      127 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/response.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    25579 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/server.py
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.542615 buku-4.7.1/bukuserver/static/
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.542615 buku-4.7.1/bukuserver/static/bukuserver/
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.546615 buku-4.7.1/bukuserver/static/bukuserver/js/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)   403942 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/static/bukuserver/js/Chart.js
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      177 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/static/bukuserver/js/bookmark.js
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.542615 buku-4.7.1/bukuserver/templates/
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.550615 buku-4.7.1/bukuserver/templates/bukuserver/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     3914 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/base.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      177 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/bookmark_create.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      184 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/bookmark_create_modal.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      175 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/bookmark_edit.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      182 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/bookmark_edit_modal.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1313 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/bookmarks.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     2292 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/home.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      719 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/index.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    10257 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/statistic.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1542 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/templates/bukuserver/tags.html
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    26988 2022-07-01 22:29:19.000000 buku-4.7.1/bukuserver/views.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      173 2022-07-01 22:29:19.000000 buku-4.7.1/requirements.txt
--rw-rw-r--   0 r3r       (1000) r3r       (1000)       38 2022-07-01 22:38:36.550615 buku-4.7.1/setup.cfg
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     3299 2022-07-01 22:29:19.000000 buku-4.7.1/setup.py
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.550615 buku-4.7.1/tests/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:29:19.000000 buku-4.7.1/tests/__init__.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1393 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_BukuCrypt.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1089 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_ExtendedArgumentParser.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    29537 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_buku.py
-drwxrwxr-x   0 r3r       (1000) r3r       (1000)        0 2022-07-01 22:38:36.550615 buku-4.7.1/tests/test_bukuDb/
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     2284 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb/25491522_res.yaml
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1636 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb/25491522_res_nopt.yaml
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    11351 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb/Bookmarks
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     2388 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb/firefox_res.yaml
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     1912 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb/firefox_res_nopt.yaml
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    50439 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_bukuDb.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)    10000 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_import_firefox_json.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     9335 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_server.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)      420 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_setup.py
--rw-rw-r--   0 r3r       (1000) r3r       (1000)     3410 2022-07-01 22:29:19.000000 buku-4.7.1/tests/test_views.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.933868 buku-4.9/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    21581 2024-04-07 05:35:20.000000 buku-4.9/CHANGELOG
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    35142 2024-04-07 05:35:20.000000 buku-4.9/LICENSE
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      283 2024-04-07 05:35:20.000000 buku-4.9/MANIFEST.in
+-rw-r--r--   0 vaio      (1000) vaio      (1000)    31555 2024-04-07 05:37:14.933868 buku-4.9/PKG-INFO
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    28037 2024-04-07 05:35:20.000000 buku-4.9/README.md
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.921867 buku-4.9/auto-completion/
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/auto-completion/bash/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1754 2024-04-07 05:35:20.000000 buku-4.9/auto-completion/bash/buku-completion.bash
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/auto-completion/fish/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     3621 2024-04-07 05:35:20.000000 buku-4.9/auto-completion/fish/buku.fish
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/auto-completion/zsh/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2935 2024-04-07 05:35:20.000000 buku-4.9/auto-completion/zsh/_buku
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    29743 2024-04-07 05:35:20.000000 buku-4.9/buku.1
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.929868 buku-4.9/buku.egg-info/
+-rw-r--r--   0 vaio      (1000) vaio      (1000)    31555 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/PKG-INFO
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1883 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/SOURCES.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)        1 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/dependency_links.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)       70 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/entry_points.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      807 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/requires.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)       16 2024-04-07 05:37:14.000000 buku-4.9/buku.egg-info/top_level.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)   213443 2024-04-07 05:37:14.000000 buku-4.9/buku.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/__init__.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      130 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/__main__.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    10503 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/api.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     7483 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/filters.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2865 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/forms.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/middleware/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)       96 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/middleware/__init__.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2563 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/middleware/flask_reverse_proxy_fix.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1673 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/response.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     7969 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/server.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.921867 buku-4.9/bukuserver/static/
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/static/bukuserver/
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/static/bukuserver/css/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      229 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/css/bookmark.css
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      121 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/favicon.svg
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/static/bukuserver/js/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)   403942 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/js/Chart.js
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      177 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/js/bookmark.js
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      217 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/js/last_page.js
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1004 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/static/bukuserver/js/page_size.js
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.921867 buku-4.9/bukuserver/templates/
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.925868 buku-4.9/bukuserver/templates/bukuserver/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      277 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_create.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      438 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_create_modal.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      247 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_details.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      195 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_details_modal.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      984 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_edit.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      185 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmark_edit_modal.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      637 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmarklet.url
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      248 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/bookmarks_list.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     3189 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/home.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2377 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/lib.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    10333 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/statistic.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      408 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/templates/bukuserver/tags_list.html
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    27567 2024-04-07 05:35:20.000000 buku-4.9/bukuserver/views.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      216 2024-04-07 05:35:20.000000 buku-4.9/requirements.txt
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)       38 2024-04-07 05:37:14.933868 buku-4.9/setup.cfg
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     3299 2024-04-07 05:35:20.000000 buku-4.9/setup.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.929868 buku-4.9/tests/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:35:20.000000 buku-4.9/tests/__init__.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1411 2024-04-07 05:35:20.000000 buku-4.9/tests/test_BukuCrypt.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1089 2024-04-07 05:35:20.000000 buku-4.9/tests/test_ExtendedArgumentParser.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    30722 2024-04-07 05:35:20.000000 buku-4.9/tests/test_buku.py
+drwxrwxr-x   0 vaio      (1000) vaio      (1000)        0 2024-04-07 05:37:14.929868 buku-4.9/tests/test_bukuDb/
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2491 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb/25491522_res.yaml
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1636 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb/25491522_res_nopt.yaml
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    11374 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb/Bookmarks
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     2393 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb/firefox_res.yaml
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)     1912 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb/firefox_res_nopt.yaml
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    65499 2024-04-07 05:35:20.000000 buku-4.9/tests/test_bukuDb.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    10000 2024-04-07 05:35:20.000000 buku-4.9/tests/test_import_firefox_json.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    13484 2024-04-07 05:35:20.000000 buku-4.9/tests/test_server.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      821 2024-04-07 05:35:20.000000 buku-4.9/tests/test_setup.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)    16574 2024-04-07 05:35:20.000000 buku-4.9/tests/test_views.py
+-rw-rw-r--   0 vaio      (1000) vaio      (1000)      859 2024-04-07 05:35:20.000000 buku-4.9/tests/util.py
```

### Comparing `buku-4.7.1/CHANGELOG` & `buku-4.9/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,49 @@
+buku v4.9
+2024-04-07
+
+- fixed profile detection for multiple Firefox installs (#711)
+- added option `--offline` to add a bookmark without web connection
+- added a mini-guide for quick keyboard access to the bookmarklet
+- support environment variable `NO_COLOR`
+- fixed HTML encoding detection (#713)
+- fixed Windows profile detection (#683)
+- support python 3.11 (support for python 3.7 removed)
+- fixed readline internal error on Windows (#704)
+
+-------------------------------------------------------------------------------
+
+buku v4.8
+2023-02-18
+
+- support Vivaldi browser
+- better XBEL compatibility
+- check for empty search results in piped operations
+- remove python 3.6 support, add 3.10
+- API changes in bukudb (#660):
+  - bookmark data tuples returned from methods `get_rec_all()`
+    & `get_rec_by_id()`, now have user-friendly properties
+    (`id`, `url`, `title`, `desc`, `tags`/`taglist`, `immutable`;
+    as well as for raw DB fields – `tags_raw`, `flags`)
+  - methods `get_rec_all()`, `list_using_id()`, `searchdb()`, `search_by_tag()`,
+    `search_keywords_and_filter_by_tags()` & `exclude_results_from_search()`
+    are now guaranteed to return a list (empty if no data is found)
+  - methods `get_rec_id()`, `get_max_id()` & `add_rec()` now return `None` as
+    the "no ID" value
+  - methods `add_rec()`, `update_rec()` & `edit_update_rec()` now treat the
+    value of `immutable` parameter as a boolean (the default/noop value for
+    update calls is `None`)
+  - a `FIELD_FILTER` dictionary is introduced that contains fields formatting
+    description; also, in `format_json()` (and `print_json_safe()`), the output
+    format now matches the one described in CLI help
+- IMPACT: If you have a local repo clone, remove .tox/ subfolder if it's there
+    before you run tests for the first time
+
+-------------------------------------------------------------------------------
+
 buku v4.7
 2022-07-01
 
 - support XBEL export/import (#569)
 - support for Microsoft Edge bookmarks (#585)
 - block web fetch on import
 - many bukuserver fixes (#543, #545, #547, #548, #553, #554, #559)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buku-4.7.1/LICENSE` & `buku-4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `buku-4.7.1/PKG-INFO` & `buku-4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,15 @@
-Metadata-Version: 2.1
-Name: buku
-Version: 4.7.1
-Summary: Bookmark manager like a text-based mini-web.
-Home-page: https://github.com/jarun/buku
-Author: Arun Prakash Jana
-Author-email: engineerarun@gmail.com
-License: GPLv3
-Keywords: cli bookmarks tag utility
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: ca-certificates
-Provides-Extra: tests
-Provides-Extra: server
-Provides-Extra: docs
-Provides-Extra: packaging
-License-File: LICENSE
-
 <h1 align="center">buku</h1>
 
 <p align="center">
 <a href="https://github.com/jarun/buku/releases/latest"><img src="https://img.shields.io/github/release/jarun/buku.svg?maxAge=600" alt="Latest release" /></a>
 <a href="https://repology.org/project/buku/versions"><img src="https://repology.org/badge/tiny-repos/buku.svg?header=repos" alt="Availability"></a>
 <a href="https://pypi.org/project/buku/"><img src="https://img.shields.io/pypi/v/buku.svg?maxAge=600" alt="PyPI" /></a>
 <a href="https://circleci.com/gh/jarun/workflows/buku"><img src="https://img.shields.io/circleci/project/github/jarun/buku.svg" alt="Build Status" /></a>
-<a href="http://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
+<a href="https://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
 <a href="https://en.wikipedia.org/wiki/Privacy-invasive_software"><img src="https://img.shields.io/badge/privacy-✓-crimson" alt="Privacy Awareness" /></a>
 <a href="https://github.com/jarun/buku/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-GPLv3-yellowgreen.svg?maxAge=2592000" alt="License" /></a>
 </p>
 
 <p align="center">
 <a href="https://asciinema.org/a/137065"><img src="https://asciinema.org/a/137065.svg" alt="buku in action!" width="734"/></a>
 </p>
@@ -55,15 +22,15 @@
 
 For those who prefer the GUI, [bukuserver](https://github.com/jarun/buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local web host server.
 
 When I started writing it, I couldn't find a flexible command-line solution with a private, portable, merge-able database along with seamless GUI integration. Hence, `buku`.
 
 `buku` can import bookmarks from browser(s) or fetch the title, tags and description of a URL from the web. Use your favourite editor to add, compose and update bookmarks. Search bookmarks instantly with multiple search options, including regex and a deep scan mode (handy with URLs).
 
-It can look up broken links on Wayback Machine. There's an Easter Egg to revisit random bookmarks.
+It can look up broken links on the Wayback Machine. There's an Easter Egg to revisit random bookmarks.
 
 There's no tracking, hidden history, obsolete records, usage analytics or homing.
 
 To get started right away, jump to the [Quickstart](#quickstart) section. `buku` has one of the best documentation around. The man page comes with examples. For internal details, please refer to the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 
 `buku` is a library too! There are several related projects, including a browser plug-in.
 
@@ -91,33 +58,35 @@
 - [In the Press](#in-the-press)
 
 ### Features
 
 - Store bookmarks with auto-fetched title, tags and description
 - Auto-import from Firefox, Google Chrome, Chromium and MS Edge
 - Open bookmarks and search results in browser
-- Shorten, expand URLs, browse cached page from Wayback Machine
+- Shorten, expand URLs
+- Browse cached page from the Wayback Machine
 - Text editor integration
 - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...)
 - Continuous search with on the fly mode switch
 - Portable, merge-able database to sync between systems
 - Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile
 - Smart tag management using redirection (>>, >, <<)
-- Multi-threaded full DB refresh, manual encryption support
+- Multi-threaded full DB refresh
+- Manual encryption support
 - Shell completion scripts, man page with examples
 - Privacy-aware (no unconfirmed user data collection)
 
 ### Installation
 
 #### Dependencies
 
 | Feature | Dependency |
 | --- | --- |
-| Lang, SQLite | Python 3.6+ |
+| Lang, SQLite | Python 3.8+ |
 | HTTPS | certifi, urllib3 |
 | Encryption | cryptography |
 | HTML | beautifulsoup4, html5lib |
 
 To copy URL to clipboard `buku` uses `xsel` (or `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default installed) on Windows, `termux-clipboard` on Termux (terminal emulation for Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-paste buffers are recognized.
 
 #### From a package manager
@@ -240,25 +209,26 @@
       -x, --exclude [...]  omit records matching specified keywords
 
 ENCRYPTION OPTIONS:
       -l, --lock [N]       encrypt DB in N (default 8) # iterations
       -k, --unlock [N]     decrypt DB in N (default 8) # iterations
 
 POWER TOYS:
-      --ai                 auto-import (Firefox/Chrome/Chromium/Edge)
+      --ai                 auto-import bookmarks from web browsers
+                           Firefox, Chrome, Chromium, Vivaldi, Edge
       -e, --export file    export bookmarks to Firefox format HTML
                            export XBEL, if file ends with '.xbel'
                            export Markdown, if file ends with '.md'
                            format: [title](url) <!-- TAGS -->
                            export Orgfile, if file ends with '.org'
                            format: *[[url][title]] :tags:
                            export buku DB, if file ends with '.db'
                            combines with search results, if opted
-      -i, --import file    import bookmarks based on file extension
-                           supports 'html', 'xbel', 'json', 'md', 'org', 'db'
+      -i, --import file    import bookmarks from file
+                           supports .html .xbel .json .md .org .db
       -p, --print [...]    show record details by indices, ranges
                            print all bookmarks, if no arguments
                            -n shows the last n results (like tail)
       -f, --format N       limit fields in -p or JSON search output
                            N=1: URL; N=2: URL, tag; N=3: title;
                            N=4: URL, title, tag; N=5: title, tag;
                            N0 (10, 20, 30, 40, 50) omits DB index
@@ -270,17 +240,34 @@
       -n, --count N        show N results per page (default 10)
       --np                 do not show the subprompt, run and exit
       -o, --open [...]     browse bookmarks by indices and ranges
                            open a random bookmark, if no arguments
       --oa                 browse all search results immediately
       --replace old new    replace old tag with new tag everywhere
                            delete old tag, if new tag not specified
+      --url-redirect       when fetching an URL, use the resulting
+                           URL from following *permanent* redirects
+                           (when combined with --export, the old URL
+                           is included as additional metadata)
+      --tag-redirect [tag] when fetching an URL that causes permanent
+                           redirect, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --tag-error [tag]    when fetching an URL that causes an HTTP
+                           error, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --del-error [...]    when fetching an URL causes any (given)
+                           HTTP error, delete/do not add it
+      --export-on [...]    export records affected by the above
+                           options, including removed info
+                           (requires --update and --export; specific
+                           HTTP response filter can be provided)
       --shorten index|URL  fetch shortened url from tny.im service
       --expand index|URL   expand a tny.im shortened url
       --cached index|URL   browse a cached page from Wayback Machine
+      --offline            add a bookmark without connecting to web
       --suggest            show similar tags when adding bookmarks
       --tacit              reduce verbosity, skip some confirmations
       --nostdin            do not wait for input (must be first arg)
       --threads N          max network connections in full refresh
                            default N=4, min N=1, max N=10
       -V                   check latest upstream version available
       -g, --debug          show debug information and verbose logs
@@ -353,162 +340,192 @@
 
 1. **Edit and add** a bookmark from editor:
 
        $ buku -w
        $ buku -w 'gedit -w'
        $ buku -w 'macvim -f' -a https://ddg.gg search engine, privacy
     The first command picks editor from the environment variable `EDITOR`. The second command opens gedit in blocking mode. The third command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
+2. **Add** a simple bookmark:
+
+       $ buku --nostdin -a https://github.com/
+       2648. GitHub: Let’s build from here · GitHub
+       > https://github.com/
+       + GitHub is where over 94 million developers shape the future of software, together. Contribute to the open source community, manage your Git repositories, review code like a pro, track bugs
+        and features, power your CI/CD and DevOps workflows, and secure code before you commit it.
+
+       $ buku --nostdin -a https://github.com/
+       [ERROR] URL [https://github.com/] already exists at index 2648
+
+      `>`: URL, `+`: comment, `#`: tags
+
+      Title, description and tags will be fetched from site. Buku only stores unique URLs and will raise error if the URL already present in the database:
+3. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
 
        $ buku -a https://ddg.gg search engine, privacy -c Search engine with perks
        336. DuckDuckGo
        > https://ddg.gg
        + Alternative search engine with perks
        # privacy,search engine
-    where, >: URL, +: comment, #: tags
-3. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
+    where, `>`: URL, `+`: comment, `#`: tags
+4. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
 
        $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --immutable 1
        336. DDG (L)
        > https://ddg.gg
        # privacy,search engine
     Note that URL must precede tags.
-4. **Add** a bookmark **without a title** (works for update too):
+5. **Add** a bookmark **without a title** (works for update too):
 
        $ buku -a https://ddg.gg search engine, privacy --title
-5. **Edit and update** a bookmark from editor:
+6. **Edit and update** a bookmark from editor:
 
        $ buku -w 15012014
     This will open the existing bookmark's details in the editor for modifications. Environment variable `EDITOR` must be set.
-6. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
+7. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
 
        $ buku -u 15012014 --url http://ddg.gg/ --tag web search, utilities -c Private search engine
-7. **Fetch and update only title** for bookmark at 15012014:
+8. **Fetch and update only title** for bookmark at 15012014:
 
        $ buku -u 15012014
-8. **Update only comment** for bookmark at 15012014:
+9. **Update only comment** for bookmark at 15012014:
 
        $ buku -u 15012014 -c this is a new comment
     Applies to --url, --title and --tag too.
-9. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
+10. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
 
        $ buku -e bookmarks.html --stag tag 1, tag 2
        $ buku -e bookmarks.xbel --stag tag 1, tag 2
        $ buku -e bookmarks.md --stag tag 1, tag 2
        $ buku -e bookmarks.org --stag tag 1, tag 2
        $ buku -e bookmarks.db --stag tag 1, tag 2
     All bookmarks are exported if search is not opted.
-10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
+11. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
 
         $ buku -i bookmarks.html
         $ buku -i bookmarks.xbel
         $ buku -i bookmarks.md
         $ buku -i bookmarks.org
         $ buku -i bookmarks.db
-11. **Delete only comment** for bookmark at 15012014:
+12. **Delete only comment** for bookmark at 15012014:
 
         $ buku -u 15012014 -c
     Applies to --title and --tag too. URL cannot be deleted without deleting the bookmark.
-12. **Update** or refresh **full DB** with page titles from the web:
+13. **Update** or refresh **full DB** with page titles from the web:
 
         $ buku -u
         $ buku -u --tacit (show only failures and exceptions)
     This operation can update the title or description fields of non-immutable bookmarks by parsing the fetched page. Fields are updated only if the fetched fields are non-empty. Tags remain untouched.
-13. **Delete** bookmark at index 15012014:
+14. **Delete** bookmark at index 15012014:
 
         $ buku -d 15012014
         Index 15012020 moved to 15012014
     The last index is moved to the deleted index to keep the DB compact. Add `--tacit` to delete without confirmation.
-14. **Delete all** bookmarks:
+15. **Delete all** bookmarks:
 
         $ buku -d
-15. **Delete** a **range or list** of bookmarks:
+16. **Delete** a **range or list** of bookmarks:
 
         $ buku -d 100-200
         $ buku -d 100 15 200
-16. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
+17. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku kernel debugging
         $ buku -s kernel debugging
-17. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
+18. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku -S kernel debugging
-18. **Search** bookmarks **tagged** `general kernel concepts`:
+19. **Search** bookmarks **tagged** `general kernel concepts`:
 
         $ buku --stag general kernel concepts
-19. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+20. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel, debugging, general kernel concepts
-20. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
+21. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel + debugging + general kernel concepts
-21. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+22. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
 
         $ buku hello world --exclude real life --stag 'kernel + debugging - general kernel concepts, books'
-22. List **all unique tags** alphabetically:
+23. List **all unique tags** alphabetically:
 
         $ buku --stag
-23. Run a **search and update** the results:
+24. Run a **search and update** the results:
 
         $ buku -s kernel debugging -u --tag + linux kernel
-24. Run a **search and delete** the results:
+25. Run a **search and delete** the results:
 
         $ buku -s kernel debugging -d
-25. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
+26. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
 
         $ buku -l 15
         $ buku -k 15
     The same number of iterations must be specified for one lock & unlock instance. Default is 8, if omitted.
-26. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
+27. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
 
         $ buku -p 20-30 15012014 40-50
-27. Show details of the **last 10 bookmarks**:
+28. Show details of the **last 10 bookmarks**:
 
         $ buku -p -10
-28. **Show all** bookmarks with real index from database:
+29. **Show all** bookmarks with real index from database:
 
         $ buku -p
         $ buku -p | more
-29. **Replace tag** 'old tag' with 'new tag':
+30. **Replace tag** 'old tag' with 'new tag':
 
         $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB:
+31. **Delete tag** 'old tag' from DB:
 
         $ buku --replace 'old tag'
-31. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
+32. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
 
         $ buku -u 15012014 --tag + tag 1, tag 2
         $ buku -u 15012014 --tag - tag 1, tag 2
-32. **Open URL** at index 15012014 in browser:
+33. **Open URL** at index 15012014 in browser:
 
         $ buku -o 15012014
-33. List bookmarks with **no title or tags** for bookkeeping:
+34. List bookmarks with **no title or tags** for bookkeeping:
 
         $ buku -S blank
-34. List bookmarks with **immutable title**:
+35. List bookmarks with **immutable title**:
 
         $ buku -S immutable
-35. **Shorten URL** www.google.com and the URL at index 20:
+36. **Shorten URL** www.google.com and the URL at index 20:
 
         $ buku --shorten www.google.com
         $ buku --shorten 20
-36. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
+37. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
 
         // append tags at taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 >> 5 3-2
         // set tags at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 > 5 3-2
         // remove all tags from bookmarks at indices 5 and 2-3
         buku (? for help) g > 5 3-2
         // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 << 5 3-2
-37. List bookmarks with **colored output**:
+38. List bookmarks with **colored output**:
 
         $ buku --colors oKlxm -p
-38. More **help**:
+39. Add a bookmark after following all permanent redirects, but only if the server doesn't respond with an error (and there's no network failure)
+
+        $ buku --add http://wikipedia.net --url-redirect --del-error
+        2. Wikipedia
+           > https://www.wikipedia.org/
+           + Wikipedia is a free online encyclopedia, created and edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a permanent redirect, or tag shaped like `http 404` on an error response:
+
+        $ buku --add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error 'http {}'
+        [ERROR] [404] Not Found
+        3. Not Found
+           > http://wikipedia.net/notfound
+           # http 404,http redirect
+41. Update all bookmarks matching the search by updating the URL if the server responds with a permanent redirect, deleting the bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500, or adding a tag shaped like `http:{}` in case of any other HTTP error; then export those affected by such changes into an HTML file, marking deleted records as well as old URLs for those replaced by redirect.
+
+        $ buku -S ://wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on --export backup.html
+42. More **help**:
 
         $ buku -h
         $ man buku
 
 ### Automation
 
 Interactive workflows can be automated using expect. Issue [#368](https://github.com/jarun/buku/issues/368) has a working example on automating auto-import.
@@ -518,38 +535,40 @@
 #### Editor integration
 
 You may encounter issues with GUI editors which maintain only one instance by default and return immediately from other instances. Use the appropriate editor option to block the caller when a new document is opened. See issue [#210](https://github.com/jarun/buku/issues/210) for gedit.
 
 ### Collaborators
 
 - [Arun Prakash Jana](https://github.com/jarun)
+- [Alexey Gulenko](https://github.com/LeXofLeviafan)
 - [Rachmadani Haryono](https://github.com/rachmadaniHaryono)
 - [Johnathan Jenkins](https://github.com/shaggytwodope)
 - [SZ Lin](https://github.com/szlin)
 
-Copyright © 2015-2022 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
+Copyright © 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 <br>
 <p><a href="https://gitter.im/jarun/buku"><img src="https://img.shields.io/gitter/room/jarun/buku.svg?maxAge=2592000" alt="gitter chat" /></a></p>
 
 ### Contributions
 
 Missing a feature? There's a rolling [ToDo List](https://github.com/jarun/buku/issues/484) with identified tasks. Contributions are welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/PR-guidelines).
 
+See also our documentation here <a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
+
 ### Related projects
 
 - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for browser integration
 - [oil](https://github.com/AndreiUlmeyda/oil), search-as-you-type cli front-end
 - [buku_run](https://github.com/carnager/buku_run), rofi front-end
 - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku import utility
 - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper
 - [poku](https://github.com/shanedabes/poku), sync between Pocket and buku
 - [Ebuku](https://github.com/flexibeast/ebuku), Emacs interface to buku
 - [diigoku](https://github.com/dppdppd/diigoku), buku importer for Diigo
 
-<a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
 
 ### Videos
 
 - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/embed/9HzEHrUBQXE)
 - [Buku is a great open-source bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8)
 
 ### In the Press
@@ -559,9 +578,7 @@
 - [It's F.O.S.S.](https://itsfoss.com/buku-command-line-bookmark-manager-linux/)
 - [LinOxide](https://linoxide.com/linux-how-to/buku-browser-bookmarks-linux/)
 - [LinuxUser Magazine 01/2017 Issue](http://www.linux-community.de/LU/2017/01/Das-Beste-aus-zwei-Welten)
 - [Make Tech Easier](https://www.maketecheasier.com/manage-browser-bookmarks-ubuntu-command-line/)
 - [One Thing Well](http://onethingwell.org/post/144952807044/buku)
 - [Open Source For You](https://opensourceforu.com/2018/05/buku-a-bookmark-manager-in-the-command-line/)
 - [ulno.net](https://ulno.net/blog/2017-07-19/of-bookmarks-tags-and-browsers/)
-
-
```

#### html2text {}

```diff
@@ -1,39 +1,23 @@
-Metadata-Version: 2.1 Name: buku Version: 4.7.1 Summary: Bookmark manager like
-a text-based mini-web. Home-page: https://github.com/jarun/buku Author: Arun
-Prakash Jana Author-email: engineerarun@gmail.com License: GPLv3 Keywords: cli
-bookmarks tag utility Platform: any Classifier: Development Status :: 5 -
-Production/Stable Classifier: Environment :: Console Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Internet :: WWW/HTTP
-:: Indexing/Search Classifier: Topic :: Utilities Requires-Python: >=3.6
-Description-Content-Type: text/markdown Provides-Extra: ca-certificates
-Provides-Extra: tests Provides-Extra: server Provides-Extra: docs Provides-
-Extra: packaging License-File: LICENSE
                               ************ bbuukkuu ************
     _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_A_v_a_i_l_a_b_i_l_i_t_y_]_[_P_y_P_I_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_s_ _S_t_a_t_u_s_]_[_P_r_i_v_a_c_y
                               _A_w_a_r_e_n_e_s_s_]_[_L_i_c_e_n_s_e_]
                                _[_b_u_k_u_ _i_n_ _a_c_t_i_o_n_!_]
                                 buku in action!
 ### Introduction `buku` is a powerful bookmark manager and a personal textual
 mini-web. For those who prefer the GUI, [bukuserver](https://github.com/jarun/
 buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local
 web host server. When I started writing it, I couldn't find a flexible command-
 line solution with a private, portable, merge-able database along with seamless
 GUI integration. Hence, `buku`. `buku` can import bookmarks from browser(s) or
 fetch the title, tags and description of a URL from the web. Use your favourite
 editor to add, compose and update bookmarks. Search bookmarks instantly with
 multiple search options, including regex and a deep scan mode (handy with
-URLs). It can look up broken links on Wayback Machine. There's an Easter Egg to
-revisit random bookmarks. There's no tracking, hidden history, obsolete
+URLs). It can look up broken links on the Wayback Machine. There's an Easter
+Egg to revisit random bookmarks. There's no tracking, hidden history, obsolete
 records, usage analytics or homing. To get started right away, jump to the
 [Quickstart](#quickstart) section. `buku` has one of the best documentation
 around. The man page comes with examples. For internal details, please refer to
 the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 `buku` is a library too! There are several related projects, including a
 browser plug-in. ### Table of Contents - [Features](#features) - [Installation]
 (#installation) - [Dependencies](#dependencies) - [From a package manager]
@@ -43,24 +27,24 @@
 (#command-line-options) - [Colors](#colors) - [Quickstart](#quickstart) -
 [Examples](#examples) - [Automation](#automation) - [Troubleshooting]
 (#troubleshooting) - [Editor integration](#editor-integration) -
 [Collaborators](#collaborators) - [Contributions](#contributions) - [Related
 projects](#related-projects) - [In the Press](#in-the-press) ### Features -
 Store bookmarks with auto-fetched title, tags and description - Auto-import
 from Firefox, Google Chrome, Chromium and MS Edge - Open bookmarks and search
-results in browser - Shorten, expand URLs, browse cached page from Wayback
+results in browser - Shorten, expand URLs - Browse cached page from the Wayback
 Machine - Text editor integration - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...) - Continuous search with on the
 fly mode switch - Portable, merge-able database to sync between systems -
 Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile - Smart tag
-management using redirection (>>, >, <<) - Multi-threaded full DB refresh,
-manual encryption support - Shell completion scripts, man page with examples -
+management using redirection (>>, >, <<) - Multi-threaded full DB refresh -
+Manual encryption support - Shell completion scripts, man page with examples -
 Privacy-aware (no unconfirmed user data collection) ### Installation ####
 Dependencies | Feature | Dependency | | --- | --- | | Lang, SQLite | Python
-3.6+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
+3.8+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
 beautifulsoup4, html5lib | To copy URL to clipboard `buku` uses `xsel` (or
 `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default
 installed) on Windows, `termux-clipboard` on Termux (terminal emulation for
 Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-
 paste buffers are recognized. #### From a package manager To install buku with
 all its dependencies from PyPI, run: # pip3 install buku You can also install
 `buku` from your package manager. If the version available is dated try an
@@ -111,54 +95,64 @@
 tag "immutable": entries with locked title --deep match substrings ('pen'
 matches 'opens') -r, --sreg expr run a regex search -t, --stag [tag [,|+] ...]
 [- tag, ...] search bookmarks by tags use ',' to find entries matching ANY tag
 use '+' to find entries matching ALL tags excludes entries with tags after ' -
 ' list all tags, if no search keywords -x, --exclude [...] omit records
 matching specified keywords ENCRYPTION OPTIONS: -l, --lock [N] encrypt DB in N
 (default 8) # iterations -k, --unlock [N] decrypt DB in N (default 8) #
-iterations POWER TOYS: --ai auto-import (Firefox/Chrome/Chromium/Edge) -e, --
-export file export bookmarks to Firefox format HTML export XBEL, if file ends
-with '.xbel' export Markdown, if file ends with '.md' format: [title](url)
-export Orgfile, if file ends with '.org' format: *[[url][title]] :tags: export
-buku DB, if file ends with '.db' combines with search results, if opted -i, --
-import file import bookmarks based on file extension supports 'html', 'xbel',
-'json', 'md', 'org', 'db' -p, --print [...] show record details by indices,
-ranges print all bookmarks, if no arguments -n shows the last n results (like
-tail) -f, --format N limit fields in -p or JSON search output N=1: URL; N=2:
-URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0 (10, 20, 30,
-40, 50) omits DB index -j, --json [file] JSON formatted output for -p and
-search. prints to stdout if argument missing. otherwise writes to given file --
-colors COLORS set output colors in five-letter string --nc disable color output
--n, --count N show N results per page (default 10) --np do not show the
+iterations POWER TOYS: --ai auto-import bookmarks from web browsers Firefox,
+Chrome, Chromium, Vivaldi, Edge -e, --export file export bookmarks to Firefox
+format HTML export XBEL, if file ends with '.xbel' export Markdown, if file
+ends with '.md' format: [title](url) export Orgfile, if file ends with '.org'
+format: *[[url][title]] :tags: export buku DB, if file ends with '.db' combines
+with search results, if opted -i, --import file import bookmarks from file
+supports .html .xbel .json .md .org .db -p, --print [...] show record details
+by indices, ranges print all bookmarks, if no arguments -n shows the last n
+results (like tail) -f, --format N limit fields in -p or JSON search output
+N=1: URL; N=2: URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0
+(10, 20, 30, 40, 50) omits DB index -j, --json [file] JSON formatted output for
+-p and search. prints to stdout if argument missing. otherwise writes to given
+file --colors COLORS set output colors in five-letter string --nc disable color
+output -n, --count N show N results per page (default 10) --np do not show the
 subprompt, run and exit -o, --open [...] browse bookmarks by indices and ranges
 open a random bookmark, if no arguments --oa browse all search results
 immediately --replace old new replace old tag with new tag everywhere delete
-old tag, if new tag not specified --shorten index|URL fetch shortened url from
-tny.im service --expand index|URL expand a tny.im shortened url --cached
-index|URL browse a cached page from Wayback Machine --suggest show similar tags
-when adding bookmarks --tacit reduce verbosity, skip some confirmations --
-nostdin do not wait for input (must be first arg) --threads N max network
-connections in full refresh default N=4, min N=1, max N=10 -V check latest
-upstream version available -g, --debug show debug information and verbose logs
-SYMBOLS: > url + comment # tags PROMPT KEYS: 1-N browse search result indices
-and/or ranges O [id|range [...]] open search results/indices in GUI browser
-toggle try GUI browser if no arguments a open all results in browser s keyword
-[...] search for records with ANY keyword S keyword [...] search for records
-with ALL keywords d match substrings ('pen' matches 'opened') r expression run
-a regex search t [tag, ...] search by tags; show taglist, if no args g taglist
-id|range [...] [>>|>|<<] [record id|range ...] append, set, remove (all or
-specific) tags search by taglist id(s) if records are omitted n show next page
-of search results o id|range [...] browse bookmarks by indices and/or ranges p
-id|range [...] print bookmarks by indices and/or ranges w [editor|id] edit and
-add or update a bookmark c id copy URL at search result index to clipboard ?
-show this help q, ^D, double Enter exit buku ``` #### Colors `buku` supports
-custom colors. Visit the wiki page on how to [customize colors](https://
-github.com/jarun/buku/wiki/Customize-colors) for more details. ### Quickstart
-1. Export `VISUAL` or `EDITOR` to point to your favourite editor. Note that
-`VISUAL` takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
+old tag, if new tag not specified --url-redirect when fetching an URL, use the
+resulting URL from following *permanent* redirects (when combined with --
+export, the old URL is included as additional metadata) --tag-redirect [tag]
+when fetching an URL that causes permanent redirect, add a tag in specified
+pattern (using 'http:{}' if not specified) --tag-error [tag] when fetching an
+URL that causes an HTTP error, add a tag in specified pattern (using 'http:{}'
+if not specified) --del-error [...] when fetching an URL causes any (given)
+HTTP error, delete/do not add it --export-on [...] export records affected by
+the above options, including removed info (requires --update and --export;
+specific HTTP response filter can be provided) --shorten index|URL fetch
+shortened url from tny.im service --expand index|URL expand a tny.im shortened
+url --cached index|URL browse a cached page from Wayback Machine --offline add
+a bookmark without connecting to web --suggest show similar tags when adding
+bookmarks --tacit reduce verbosity, skip some confirmations --nostdin do not
+wait for input (must be first arg) --threads N max network connections in full
+refresh default N=4, min N=1, max N=10 -V check latest upstream version
+available -g, --debug show debug information and verbose logs SYMBOLS: > url +
+comment # tags PROMPT KEYS: 1-N browse search result indices and/or ranges O
+[id|range [...]] open search results/indices in GUI browser toggle try GUI
+browser if no arguments a open all results in browser s keyword [...] search
+for records with ANY keyword S keyword [...] search for records with ALL
+keywords d match substrings ('pen' matches 'opened') r expression run a regex
+search t [tag, ...] search by tags; show taglist, if no args g taglist id|range
+[...] [>>|>|<<] [record id|range ...] append, set, remove (all or specific)
+tags search by taglist id(s) if records are omitted n show next page of search
+results o id|range [...] browse bookmarks by indices and/or ranges p id|range
+[...] print bookmarks by indices and/or ranges w [editor|id] edit and add or
+update a bookmark c id copy URL at search result index to clipboard ? show this
+help q, ^D, double Enter exit buku ``` #### Colors `buku` supports custom
+colors. Visit the wiki page on how to [customize colors](https://github.com/
+jarun/buku/wiki/Customize-colors) for more details. ### Quickstart 1. Export
+`VISUAL` or `EDITOR` to point to your favourite editor. Note that `VISUAL`
+takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
 convenience. alias b='buku --suggest' 3. Auto-import bookmarks from your
 browser(s). Please quit the relevant browsers beforehand to ensure the
 databases are not locked. b --ai 4. Manually add a bookmark (for hands-on). b -
 w 5. List your bookmarks with DB index. b -p 6. For GUI and browser integration
 (or to sync bookmarks with your favourite bookmark management service) refer to
 the wiki page on [System integration](https://github.com/jarun/buku/wiki/
 System-integration). 7. Quick (bash/zsh) commands to fuzzy search with fzf and
@@ -167,120 +161,146 @@
 well: ```sh #!/usr/bin/env sh url=$(buku -p -f4 | fzf -m --reverse --preview
 "buku -p {1}" --preview-window=wrap | cut -f2) if [ -n "$url" ]; then echo
 "$url" | xargs firefox fi ``` ### Examples 1. **Edit and add** a bookmark from
 editor: $ buku -w $ buku -w 'gedit -w' $ buku -w 'macvim -f' -a https://ddg.gg
 search engine, privacy The first command picks editor from the environment
 variable `EDITOR`. The second command opens gedit in blocking mode. The third
 command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment**
-`Search engine with perks`, **fetch page title** from the web: $ buku -a https:
-//ddg.gg search engine, privacy -c Search engine with perks 336. DuckDuckGo >
-https://ddg.gg + Alternative search engine with perks # privacy,search engine
-where, >: URL, +: comment, #: tags 3. **Add** a bookmark with tags `search
-engine` & `privacy` and **immutable custom title** `DDG`: $ buku -a https://
-ddg.gg search engine, privacy --title 'DDG' --immutable 1 336. DDG (L) > https:
-//ddg.gg # privacy,search engine Note that URL must precede tags. 4. **Add** a
-bookmark **without a title** (works for update too): $ buku -a https://ddg.gg
-search engine, privacy --title 5. **Edit and update** a bookmark from editor: $
-buku -w 15012014 This will open the existing bookmark's details in the editor
-for modifications. Environment variable `EDITOR` must be set. 6. **Update**
-existing bookmark at index 15012014 with new URL, tags and comments, fetch
-title from the web: $ buku -u 15012014 --url http://ddg.gg/ --tag web search,
-utilities -c Private search engine 7. **Fetch and update only title** for
-bookmark at 15012014: $ buku -u 15012014 8. **Update only comment** for
-bookmark at 15012014: $ buku -u 15012014 -c this is a new comment Applies to --
-url, --title and --tag too. 9. **Export** bookmarks tagged `tag 1` or `tag 2`
-to HTML, XBEL, Markdown, Orgfile or a new database: $ buku -e bookmarks.html --
-stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag 1, tag 2 $ buku -
-e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --stag tag 1, tag 2
-$ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are exported if search
-is not opted. 10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile: $
-buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -i bookmarks.md $ buku -
-i bookmarks.org $ buku -i bookmarks.db 11. **Delete only comment** for bookmark
-at 15012014: $ buku -u 15012014 -c Applies to --title and --tag too. URL cannot
-be deleted without deleting the bookmark. 12. **Update** or refresh **full DB**
-with page titles from the web: $ buku -u $ buku -u --tacit (show only failures
-and exceptions) This operation can update the title or description fields of
-non-immutable bookmarks by parsing the fetched page. Fields are updated only if
-the fetched fields are non-empty. Tags remain untouched. 13. **Delete**
-bookmark at index 15012014: $ buku -d 15012014 Index 15012020 moved to 15012014
-The last index is moved to the deleted index to keep the DB compact. Add `--
-tacit` to delete without confirmation. 14. **Delete all** bookmarks: $ buku -
-d 15. **Delete** a **range or list** of bookmarks: $ buku -d 100-200 $ buku -
-d 100 15 200 16. **Search** bookmarks for **ANY** of the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku kernel debugging $ buku -s kernel
-debugging 17. **Search** bookmarks with **ALL** the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku -S kernel debugging 18. **Search**
-bookmarks **tagged** `general kernel concepts`: $ buku --stag general kernel
-concepts 19. **Search** for bookmarks matching **ANY** of the tags `kernel`,
-`debugging`, `general kernel concepts`: $ buku --stag kernel, debugging,
-general kernel concepts 20. **Search** for bookmarks matching **ALL** of the
-tags `kernel`, `debugging`, `general kernel concepts`: $ buku --stag kernel +
-debugging + general kernel concepts 21. **Search** for bookmarks matching any
-of the keywords `hello` or `world`, excluding the keywords `real` and `life`,
-matching both the tags `kernel` and `debugging`, but **excluding** the tags
-`general kernel concepts` and `books`: $ buku hello world --exclude real life -
--stag 'kernel + debugging - general kernel concepts, books' 22. List **all
-unique tags** alphabetically: $ buku --stag 23. Run a **search and update** the
-results: $ buku -s kernel debugging -u --tag + linux kernel 24. Run a **search
-and delete** the results: $ buku -s kernel debugging -d 25. **Encrypt or
-decrypt** DB with **custom number of iterations** (15) to generate key: $ buku
--l 15 $ buku -k 15 The same number of iterations must be specified for one lock
-& unlock instance. Default is 8, if omitted. 26. **Show details** of bookmarks
-at index 15012014 and ranges 20-30, 40-50: $ buku -p 20-30 15012014 40-50 27.
-Show details of the **last 10 bookmarks**: $ buku -p -10 28. **Show all**
-bookmarks with real index from database: $ buku -p $ buku -p | more 29.
-**Replace tag** 'old tag' with 'new tag': $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB: $ buku --replace 'old tag' 31. **Append
-(or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at
-index 15012014: $ buku -u 15012014 --tag + tag 1, tag 2 $ buku -u 15012014 --
-tag - tag 1, tag 2 32. **Open URL** at index 15012014 in browser: $ buku -
-o 15012014 33. List bookmarks with **no title or tags** for bookkeeping: $ buku
--S blank 34. List bookmarks with **immutable title**: $ buku -S immutable 35.
-**Shorten URL** www.google.com and the URL at index 20: $ buku --shorten
-www.google.com $ buku --shorten 20 36. **Append, remove tags at prompt**
-(taglist index to the left, bookmark index to the right): // append tags at
-taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-
-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags at taglist indices 4 and 6-
-9 as tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 > 5 3-2 /
-/ remove all tags from bookmarks at indices 5 and 2-3 buku (? for help) g > 5
-3-2 // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at
-indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 37. List bookmarks with
-**colored output**: $ buku --colors oKlxm -p 38. More **help**: $ buku -h $ man
-buku ### Automation Interactive workflows can be automated using expect. Issue
-[#368](https://github.com/jarun/buku/issues/368) has a working example on
-automating auto-import. ### Troubleshooting #### Editor integration You may
-encounter issues with GUI editors which maintain only one instance by default
-and return immediately from other instances. Use the appropriate editor option
-to block the caller when a new document is opened. See issue [#210](https://
-github.com/jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash
-Jana](https://github.com/jarun) - [Rachmadani Haryono](https://github.com/
-rachmadaniHaryono) - [Johnathan Jenkins](https://github.com/shaggytwodope) -
-[SZ Lin](https://github.com/szlin) Copyright Â© 2015-2022 [Arun Prakash Jana]
-(mailto:engineerarun@gmail.com)
+2. **Add** a simple bookmark: $ buku --nostdin -a https://github.com/ 2648.
+GitHub: Letâs build from here Â· GitHub > https://github.com/ + GitHub is
+where over 94 million developers shape the future of software, together.
+Contribute to the open source community, manage your Git repositories, review
+code like a pro, track bugs and features, power your CI/CD and DevOps
+workflows, and secure code before you commit it. $ buku --nostdin -a https://
+github.com/ [ERROR] URL [https://github.com/] already exists at index 2648 `>`:
+URL, `+`: comment, `#`: tags Title, description and tags will be fetched from
+site. Buku only stores unique URLs and will raise error if the URL already
+present in the database: 3. **Add** a bookmark with **tags** `search engine`
+and `privacy`, **comment** `Search engine with perks`, **fetch page title**
+from the web: $ buku -a https://ddg.gg search engine, privacy -c Search engine
+with perks 336. DuckDuckGo > https://ddg.gg + Alternative search engine with
+perks # privacy,search engine where, `>`: URL, `+`: comment, `#`: tags 4.
+**Add** a bookmark with tags `search engine` & `privacy` and **immutable custom
+title** `DDG`: $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --
+immutable 1 336. DDG (L) > https://ddg.gg # privacy,search engine Note that URL
+must precede tags. 5. **Add** a bookmark **without a title** (works for update
+too): $ buku -a https://ddg.gg search engine, privacy --title 6. **Edit and
+update** a bookmark from editor: $ buku -w 15012014 This will open the existing
+bookmark's details in the editor for modifications. Environment variable
+`EDITOR` must be set. 7. **Update** existing bookmark at index 15012014 with
+new URL, tags and comments, fetch title from the web: $ buku -u 15012014 --url
+http://ddg.gg/ --tag web search, utilities -c Private search engine 8. **Fetch
+and update only title** for bookmark at 15012014: $ buku -u 15012014 9.
+**Update only comment** for bookmark at 15012014: $ buku -u 15012014 -c this is
+a new comment Applies to --url, --title and --tag too. 10. **Export** bookmarks
+tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database: $
+buku -e bookmarks.html --stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag
+1, tag 2 $ buku -e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --
+stag tag 1, tag 2 $ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are
+exported if search is not opted. 11. **Import** bookmarks from HTML, XBEL,
+Markdown or Orgfile: $ buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -
+i bookmarks.md $ buku -i bookmarks.org $ buku -i bookmarks.db 12. **Delete only
+comment** for bookmark at 15012014: $ buku -u 15012014 -c Applies to --title
+and --tag too. URL cannot be deleted without deleting the bookmark. 13.
+**Update** or refresh **full DB** with page titles from the web: $ buku -u $
+buku -u --tacit (show only failures and exceptions) This operation can update
+the title or description fields of non-immutable bookmarks by parsing the
+fetched page. Fields are updated only if the fetched fields are non-empty. Tags
+remain untouched. 14. **Delete** bookmark at index 15012014: $ buku -d 15012014
+Index 15012020 moved to 15012014 The last index is moved to the deleted index
+to keep the DB compact. Add `--tacit` to delete without confirmation. 15.
+**Delete all** bookmarks: $ buku -d 16. **Delete** a **range or list** of
+bookmarks: $ buku -d 100-200 $ buku -d 100 15 200 17. **Search** bookmarks for
+**ANY** of the keywords `kernel` and `debugging` in URL, title or tags: $ buku
+kernel debugging $ buku -s kernel debugging 18. **Search** bookmarks with
+**ALL** the keywords `kernel` and `debugging` in URL, title or tags: $ buku -
+S kernel debugging 19. **Search** bookmarks **tagged** `general kernel
+concepts`: $ buku --stag general kernel concepts 20. **Search** for bookmarks
+matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+$ buku --stag kernel, debugging, general kernel concepts 21. **Search** for
+bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel
+concepts`: $ buku --stag kernel + debugging + general kernel concepts 22.
+**Search** for bookmarks matching any of the keywords `hello` or `world`,
+excluding the keywords `real` and `life`, matching both the tags `kernel` and
+`debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+$ buku hello world --exclude real life --stag 'kernel + debugging - general
+kernel concepts, books' 23. List **all unique tags** alphabetically: $ buku --
+stag 24. Run a **search and update** the results: $ buku -s kernel debugging -
+u --tag + linux kernel 25. Run a **search and delete** the results: $ buku -
+s kernel debugging -d 26. **Encrypt or decrypt** DB with **custom number of
+iterations** (15) to generate key: $ buku -l 15 $ buku -k 15 The same number of
+iterations must be specified for one lock & unlock instance. Default is 8, if
+omitted. 27. **Show details** of bookmarks at index 15012014 and ranges 20-30,
+40-50: $ buku -p 20-30 15012014 40-50 28. Show details of the **last 10
+bookmarks**: $ buku -p -10 29. **Show all** bookmarks with real index from
+database: $ buku -p $ buku -p | more 30. **Replace tag** 'old tag' with 'new
+tag': $ buku --replace 'old tag' 'new tag' 31. **Delete tag** 'old tag' from
+DB: $ buku --replace 'old tag' 32. **Append (or delete) tags** 'tag 1', 'tag 2'
+to (or from) existing tags of bookmark at index 15012014: $ buku -u 15012014 --
+tag + tag 1, tag 2 $ buku -u 15012014 --tag - tag 1, tag 2 33. **Open URL** at
+index 15012014 in browser: $ buku -o 15012014 34. List bookmarks with **no
+title or tags** for bookkeeping: $ buku -S blank 35. List bookmarks with
+**immutable title**: $ buku -S immutable 36. **Shorten URL** www.google.com and
+the URL at index 20: $ buku --shorten www.google.com $ buku --shorten 20 37.
+**Append, remove tags at prompt** (taglist index to the left, bookmark index to
+the right): // append tags at taglist indices 4 and 6-9 to existing tags in
+bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags
+at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3 buku (?
+for help) g 4 9-6 > 5 3-2 // remove all tags from bookmarks at indices 5 and 2-
+3 buku (? for help) g > 5 3-2 // remove tags at taglist indices 4 and 6-9 from
+tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 38.
+List bookmarks with **colored output**: $ buku --colors oKlxm -p 39. Add a
+bookmark after following all permanent redirects, but only if the server
+doesn't respond with an error (and there's no network failure) $ buku --add
+http://wikipedia.net --url-redirect --del-error 2. Wikipedia > https://
+www.wikipedia.org/ + Wikipedia is a free online encyclopedia, created and
+edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a
+permanent redirect, or tag shaped like `http 404` on an error response: $ buku
+--add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error
+'http {}' [ERROR] [404] Not Found 3. Not Found > http://wikipedia.net/notfound
+# http 404,http redirect 41. Update all bookmarks matching the search by
+updating the URL if the server responds with a permanent redirect, deleting the
+bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500,
+or adding a tag shaped like `http:{}` in case of any other HTTP error; then
+export those affected by such changes into an HTML file, marking deleted
+records as well as old URLs for those replaced by redirect. $ buku -S ://
+wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on
+--export backup.html 42. More **help**: $ buku -h $ man buku ### Automation
+Interactive workflows can be automated using expect. Issue [#368](https://
+github.com/jarun/buku/issues/368) has a working example on automating auto-
+import. ### Troubleshooting #### Editor integration You may encounter issues
+with GUI editors which maintain only one instance by default and return
+immediately from other instances. Use the appropriate editor option to block
+the caller when a new document is opened. See issue [#210](https://github.com/
+jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash Jana]
+(https://github.com/jarun) - [Alexey Gulenko](https://github.com/LeXofLeviafan)
+- [Rachmadani Haryono](https://github.com/rachmadaniHaryono) - [Johnathan
+Jenkins](https://github.com/shaggytwodope) - [SZ Lin](https://github.com/szlin)
+Copyright Â© 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 _[_g_i_t_t_e_r_ _c_h_a_t_]
 ### Contributions Missing a feature? There's a rolling [ToDo List](https://
 github.com/jarun/buku/issues/484) with identified tasks. Contributions are
 welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/
-PR-guidelines). ### Related projects - [bukubrow](https://github.com/SamHH/
-bukubrow), WebExtension for browser integration - [oil](https://github.com/
-AndreiUlmeyda/oil), search-as-you-type cli front-end - [buku_run](https://
-github.com/carnager/buku_run), rofi front-end - [pinku](https://github.com/
-mosegontar/pinku), a Pinboard-to-buku import utility - [buku-dmenu](https://
-gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper - [poku]
-(https://github.com/shanedabes/poku), sync between Pocket and buku - [Ebuku]
-(https://github.com/flexibeast/ebuku), Emacs interface to buku - [diigoku]
-(https://github.com/dppdppd/diigoku), buku importer for Diigo _[_S_t_a_b_l_e_ _D_o_c_s_]###
-Videos - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/
-embed/9HzEHrUBQXE) - [Buku is a great open-source bookmark manager](https://
-www.youtube.com/embed/7VxgKMWm-J8) ### In the Press - [2daygeek](http://
-www.2daygeek.com/buku-command-line-bookmark-manager-linux/) - [Hacker Milk]
-(https://hackermilk.blogspot.com/2020/01/how-to-manage-your-browsers-
-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-line-
-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/buku-
-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
+PR-guidelines). See also our documentation here _[_S_t_a_b_l_e_ _D_o_c_s_]### Related
+projects - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for
+browser integration - [oil](https://github.com/AndreiUlmeyda/oil), search-as-
+you-type cli front-end - [buku_run](https://github.com/carnager/buku_run), rofi
+front-end - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku
+import utility - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a
+simple bash dmenu wrapper - [poku](https://github.com/shanedabes/poku), sync
+between Pocket and buku - [Ebuku](https://github.com/flexibeast/ebuku), Emacs
+interface to buku - [diigoku](https://github.com/dppdppd/diigoku), buku
+importer for Diigo ### Videos - [Buku: Take Your Bookmarks Everywhere You Go]
+(https://www.youtube.com/embed/9HzEHrUBQXE) - [Buku is a great open-source
+bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8) ### In the Press -
+[2daygeek](http://www.2daygeek.com/buku-command-line-bookmark-manager-linux/) -
+[Hacker Milk](https://hackermilk.blogspot.com/2020/01/how-to-manage-your-
+browsers-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-
+line-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/
+buku-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
 www.linux-community.de/LU/2017/01/Das-Beste-aus-zwei-Welten) - [Make Tech
 Easier](https://www.maketecheasier.com/manage-browser-bookmarks-ubuntu-command-
 line/) - [One Thing Well](http://onethingwell.org/post/144952807044/buku) -
 [Open Source For You](https://opensourceforu.com/2018/05/buku-a-bookmark-
 manager-in-the-command-line/) - [ulno.net](https://ulno.net/blog/2017-07-19/of-
 bookmarks-tags-and-browsers/)
```

### Comparing `buku-4.7.1/README.md` & `buku-4.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,95 @@
+Metadata-Version: 2.1
+Name: buku
+Version: 4.9
+Summary: Bookmark manager like a text-based mini-web.
+Home-page: https://github.com/jarun/buku
+Author: Arun Prakash Jana
+Author-email: engineerarun@gmail.com
+License: GPLv3
+Project-URL: Documentation, https://buku.readthedocs.io/en/latest
+Project-URL: Funding, https://github.com/sponsors/jarun
+Project-URL: Source, https://github.com/jarun/buku
+Project-URL: Tracker, https://github.com/jarun/buku/issues
+Keywords: cli bookmarks tag utility
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: certifi
+Requires-Dist: cryptography>=1.2.3
+Requires-Dist: html5lib>=1.0.1
+Requires-Dist: urllib3<2,>=1.23
+Requires-Dist: pyreadline3; sys_platform == "win32"
+Requires-Dist: colorama>=0.4.6; sys_platform == "win32"
+Provides-Extra: tests
+Requires-Dist: attrs>=17.4.0; extra == "tests"
+Requires-Dist: beautifulsoup4>=4.6.0; extra == "tests"
+Requires-Dist: Click>=7.0; extra == "tests"
+Requires-Dist: flake8>=3.4.1; extra == "tests"
+Requires-Dist: hypothesis>=6.0.0; extra == "tests"
+Requires-Dist: mypy-extensions==0.4.1; extra == "tests"
+Requires-Dist: py>=1.5.0; extra == "tests"
+Requires-Dist: pylint>=1.7.2; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-recording>=0.12.1; extra == "tests"
+Requires-Dist: pytest>=6.2.1; extra == "tests"
+Requires-Dist: PyYAML>=4.2b1; extra == "tests"
+Requires-Dist: setuptools>=41.0.1; extra == "tests"
+Requires-Dist: vcrpy>=1.13.0; extra == "tests"
+Requires-Dist: lxml; extra == "tests"
+Requires-Dist: flask_babel; extra == "tests"
+Requires-Dist: arrow>=1.2.2; extra == "tests"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "tests"
+Requires-Dist: Flask-API>=3.0.post1; extra == "tests"
+Requires-Dist: Flask-Bootstrap>=3.3.7.1; extra == "tests"
+Requires-Dist: flask-paginate>=2022.1.8; extra == "tests"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "tests"
+Requires-Dist: Flask<2.3,>=2.2.2; extra == "tests"
+Requires-Dist: werkzeug<2.4; extra == "tests"
+Provides-Extra: server
+Requires-Dist: arrow>=1.2.2; extra == "server"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "server"
+Requires-Dist: Flask-API>=3.0.post1; extra == "server"
+Requires-Dist: Flask-Bootstrap>=3.3.7.1; extra == "server"
+Requires-Dist: flask-paginate>=2022.1.8; extra == "server"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "server"
+Requires-Dist: Flask<2.3,>=2.2.2; extra == "server"
+Requires-Dist: werkzeug<2.4; extra == "server"
+Provides-Extra: docs
+Requires-Dist: myst-parser>=0.17.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
+Provides-Extra: packaging
+Requires-Dist: twine>=1.11.0; extra == "packaging"
+
 <h1 align="center">buku</h1>
 
 <p align="center">
 <a href="https://github.com/jarun/buku/releases/latest"><img src="https://img.shields.io/github/release/jarun/buku.svg?maxAge=600" alt="Latest release" /></a>
 <a href="https://repology.org/project/buku/versions"><img src="https://repology.org/badge/tiny-repos/buku.svg?header=repos" alt="Availability"></a>
 <a href="https://pypi.org/project/buku/"><img src="https://img.shields.io/pypi/v/buku.svg?maxAge=600" alt="PyPI" /></a>
 <a href="https://circleci.com/gh/jarun/workflows/buku"><img src="https://img.shields.io/circleci/project/github/jarun/buku.svg" alt="Build Status" /></a>
-<a href="http://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
+<a href="https://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
 <a href="https://en.wikipedia.org/wiki/Privacy-invasive_software"><img src="https://img.shields.io/badge/privacy-✓-crimson" alt="Privacy Awareness" /></a>
 <a href="https://github.com/jarun/buku/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-GPLv3-yellowgreen.svg?maxAge=2592000" alt="License" /></a>
 </p>
 
 <p align="center">
 <a href="https://asciinema.org/a/137065"><img src="https://asciinema.org/a/137065.svg" alt="buku in action!" width="734"/></a>
 </p>
@@ -22,15 +102,15 @@
 
 For those who prefer the GUI, [bukuserver](https://github.com/jarun/buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local web host server.
 
 When I started writing it, I couldn't find a flexible command-line solution with a private, portable, merge-able database along with seamless GUI integration. Hence, `buku`.
 
 `buku` can import bookmarks from browser(s) or fetch the title, tags and description of a URL from the web. Use your favourite editor to add, compose and update bookmarks. Search bookmarks instantly with multiple search options, including regex and a deep scan mode (handy with URLs).
 
-It can look up broken links on Wayback Machine. There's an Easter Egg to revisit random bookmarks.
+It can look up broken links on the Wayback Machine. There's an Easter Egg to revisit random bookmarks.
 
 There's no tracking, hidden history, obsolete records, usage analytics or homing.
 
 To get started right away, jump to the [Quickstart](#quickstart) section. `buku` has one of the best documentation around. The man page comes with examples. For internal details, please refer to the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 
 `buku` is a library too! There are several related projects, including a browser plug-in.
 
@@ -58,33 +138,35 @@
 - [In the Press](#in-the-press)
 
 ### Features
 
 - Store bookmarks with auto-fetched title, tags and description
 - Auto-import from Firefox, Google Chrome, Chromium and MS Edge
 - Open bookmarks and search results in browser
-- Shorten, expand URLs, browse cached page from Wayback Machine
+- Shorten, expand URLs
+- Browse cached page from the Wayback Machine
 - Text editor integration
 - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...)
 - Continuous search with on the fly mode switch
 - Portable, merge-able database to sync between systems
 - Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile
 - Smart tag management using redirection (>>, >, <<)
-- Multi-threaded full DB refresh, manual encryption support
+- Multi-threaded full DB refresh
+- Manual encryption support
 - Shell completion scripts, man page with examples
 - Privacy-aware (no unconfirmed user data collection)
 
 ### Installation
 
 #### Dependencies
 
 | Feature | Dependency |
 | --- | --- |
-| Lang, SQLite | Python 3.6+ |
+| Lang, SQLite | Python 3.8+ |
 | HTTPS | certifi, urllib3 |
 | Encryption | cryptography |
 | HTML | beautifulsoup4, html5lib |
 
 To copy URL to clipboard `buku` uses `xsel` (or `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default installed) on Windows, `termux-clipboard` on Termux (terminal emulation for Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-paste buffers are recognized.
 
 #### From a package manager
@@ -207,25 +289,26 @@
       -x, --exclude [...]  omit records matching specified keywords
 
 ENCRYPTION OPTIONS:
       -l, --lock [N]       encrypt DB in N (default 8) # iterations
       -k, --unlock [N]     decrypt DB in N (default 8) # iterations
 
 POWER TOYS:
-      --ai                 auto-import (Firefox/Chrome/Chromium/Edge)
+      --ai                 auto-import bookmarks from web browsers
+                           Firefox, Chrome, Chromium, Vivaldi, Edge
       -e, --export file    export bookmarks to Firefox format HTML
                            export XBEL, if file ends with '.xbel'
                            export Markdown, if file ends with '.md'
                            format: [title](url) <!-- TAGS -->
                            export Orgfile, if file ends with '.org'
                            format: *[[url][title]] :tags:
                            export buku DB, if file ends with '.db'
                            combines with search results, if opted
-      -i, --import file    import bookmarks based on file extension
-                           supports 'html', 'xbel', 'json', 'md', 'org', 'db'
+      -i, --import file    import bookmarks from file
+                           supports .html .xbel .json .md .org .db
       -p, --print [...]    show record details by indices, ranges
                            print all bookmarks, if no arguments
                            -n shows the last n results (like tail)
       -f, --format N       limit fields in -p or JSON search output
                            N=1: URL; N=2: URL, tag; N=3: title;
                            N=4: URL, title, tag; N=5: title, tag;
                            N0 (10, 20, 30, 40, 50) omits DB index
@@ -237,17 +320,34 @@
       -n, --count N        show N results per page (default 10)
       --np                 do not show the subprompt, run and exit
       -o, --open [...]     browse bookmarks by indices and ranges
                            open a random bookmark, if no arguments
       --oa                 browse all search results immediately
       --replace old new    replace old tag with new tag everywhere
                            delete old tag, if new tag not specified
+      --url-redirect       when fetching an URL, use the resulting
+                           URL from following *permanent* redirects
+                           (when combined with --export, the old URL
+                           is included as additional metadata)
+      --tag-redirect [tag] when fetching an URL that causes permanent
+                           redirect, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --tag-error [tag]    when fetching an URL that causes an HTTP
+                           error, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --del-error [...]    when fetching an URL causes any (given)
+                           HTTP error, delete/do not add it
+      --export-on [...]    export records affected by the above
+                           options, including removed info
+                           (requires --update and --export; specific
+                           HTTP response filter can be provided)
       --shorten index|URL  fetch shortened url from tny.im service
       --expand index|URL   expand a tny.im shortened url
       --cached index|URL   browse a cached page from Wayback Machine
+      --offline            add a bookmark without connecting to web
       --suggest            show similar tags when adding bookmarks
       --tacit              reduce verbosity, skip some confirmations
       --nostdin            do not wait for input (must be first arg)
       --threads N          max network connections in full refresh
                            default N=4, min N=1, max N=10
       -V                   check latest upstream version available
       -g, --debug          show debug information and verbose logs
@@ -320,162 +420,192 @@
 
 1. **Edit and add** a bookmark from editor:
 
        $ buku -w
        $ buku -w 'gedit -w'
        $ buku -w 'macvim -f' -a https://ddg.gg search engine, privacy
     The first command picks editor from the environment variable `EDITOR`. The second command opens gedit in blocking mode. The third command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
+2. **Add** a simple bookmark:
+
+       $ buku --nostdin -a https://github.com/
+       2648. GitHub: Let’s build from here · GitHub
+       > https://github.com/
+       + GitHub is where over 94 million developers shape the future of software, together. Contribute to the open source community, manage your Git repositories, review code like a pro, track bugs
+        and features, power your CI/CD and DevOps workflows, and secure code before you commit it.
+
+       $ buku --nostdin -a https://github.com/
+       [ERROR] URL [https://github.com/] already exists at index 2648
+
+      `>`: URL, `+`: comment, `#`: tags
+
+      Title, description and tags will be fetched from site. Buku only stores unique URLs and will raise error if the URL already present in the database:
+3. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
 
        $ buku -a https://ddg.gg search engine, privacy -c Search engine with perks
        336. DuckDuckGo
        > https://ddg.gg
        + Alternative search engine with perks
        # privacy,search engine
-    where, >: URL, +: comment, #: tags
-3. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
+    where, `>`: URL, `+`: comment, `#`: tags
+4. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
 
        $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --immutable 1
        336. DDG (L)
        > https://ddg.gg
        # privacy,search engine
     Note that URL must precede tags.
-4. **Add** a bookmark **without a title** (works for update too):
+5. **Add** a bookmark **without a title** (works for update too):
 
        $ buku -a https://ddg.gg search engine, privacy --title
-5. **Edit and update** a bookmark from editor:
+6. **Edit and update** a bookmark from editor:
 
        $ buku -w 15012014
     This will open the existing bookmark's details in the editor for modifications. Environment variable `EDITOR` must be set.
-6. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
+7. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
 
        $ buku -u 15012014 --url http://ddg.gg/ --tag web search, utilities -c Private search engine
-7. **Fetch and update only title** for bookmark at 15012014:
+8. **Fetch and update only title** for bookmark at 15012014:
 
        $ buku -u 15012014
-8. **Update only comment** for bookmark at 15012014:
+9. **Update only comment** for bookmark at 15012014:
 
        $ buku -u 15012014 -c this is a new comment
     Applies to --url, --title and --tag too.
-9. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
+10. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
 
        $ buku -e bookmarks.html --stag tag 1, tag 2
        $ buku -e bookmarks.xbel --stag tag 1, tag 2
        $ buku -e bookmarks.md --stag tag 1, tag 2
        $ buku -e bookmarks.org --stag tag 1, tag 2
        $ buku -e bookmarks.db --stag tag 1, tag 2
     All bookmarks are exported if search is not opted.
-10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
+11. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
 
         $ buku -i bookmarks.html
         $ buku -i bookmarks.xbel
         $ buku -i bookmarks.md
         $ buku -i bookmarks.org
         $ buku -i bookmarks.db
-11. **Delete only comment** for bookmark at 15012014:
+12. **Delete only comment** for bookmark at 15012014:
 
         $ buku -u 15012014 -c
     Applies to --title and --tag too. URL cannot be deleted without deleting the bookmark.
-12. **Update** or refresh **full DB** with page titles from the web:
+13. **Update** or refresh **full DB** with page titles from the web:
 
         $ buku -u
         $ buku -u --tacit (show only failures and exceptions)
     This operation can update the title or description fields of non-immutable bookmarks by parsing the fetched page. Fields are updated only if the fetched fields are non-empty. Tags remain untouched.
-13. **Delete** bookmark at index 15012014:
+14. **Delete** bookmark at index 15012014:
 
         $ buku -d 15012014
         Index 15012020 moved to 15012014
     The last index is moved to the deleted index to keep the DB compact. Add `--tacit` to delete without confirmation.
-14. **Delete all** bookmarks:
+15. **Delete all** bookmarks:
 
         $ buku -d
-15. **Delete** a **range or list** of bookmarks:
+16. **Delete** a **range or list** of bookmarks:
 
         $ buku -d 100-200
         $ buku -d 100 15 200
-16. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
+17. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku kernel debugging
         $ buku -s kernel debugging
-17. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
+18. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku -S kernel debugging
-18. **Search** bookmarks **tagged** `general kernel concepts`:
+19. **Search** bookmarks **tagged** `general kernel concepts`:
 
         $ buku --stag general kernel concepts
-19. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+20. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel, debugging, general kernel concepts
-20. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
+21. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel + debugging + general kernel concepts
-21. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+22. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
 
         $ buku hello world --exclude real life --stag 'kernel + debugging - general kernel concepts, books'
-22. List **all unique tags** alphabetically:
+23. List **all unique tags** alphabetically:
 
         $ buku --stag
-23. Run a **search and update** the results:
+24. Run a **search and update** the results:
 
         $ buku -s kernel debugging -u --tag + linux kernel
-24. Run a **search and delete** the results:
+25. Run a **search and delete** the results:
 
         $ buku -s kernel debugging -d
-25. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
+26. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
 
         $ buku -l 15
         $ buku -k 15
     The same number of iterations must be specified for one lock & unlock instance. Default is 8, if omitted.
-26. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
+27. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
 
         $ buku -p 20-30 15012014 40-50
-27. Show details of the **last 10 bookmarks**:
+28. Show details of the **last 10 bookmarks**:
 
         $ buku -p -10
-28. **Show all** bookmarks with real index from database:
+29. **Show all** bookmarks with real index from database:
 
         $ buku -p
         $ buku -p | more
-29. **Replace tag** 'old tag' with 'new tag':
+30. **Replace tag** 'old tag' with 'new tag':
 
         $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB:
+31. **Delete tag** 'old tag' from DB:
 
         $ buku --replace 'old tag'
-31. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
+32. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
 
         $ buku -u 15012014 --tag + tag 1, tag 2
         $ buku -u 15012014 --tag - tag 1, tag 2
-32. **Open URL** at index 15012014 in browser:
+33. **Open URL** at index 15012014 in browser:
 
         $ buku -o 15012014
-33. List bookmarks with **no title or tags** for bookkeeping:
+34. List bookmarks with **no title or tags** for bookkeeping:
 
         $ buku -S blank
-34. List bookmarks with **immutable title**:
+35. List bookmarks with **immutable title**:
 
         $ buku -S immutable
-35. **Shorten URL** www.google.com and the URL at index 20:
+36. **Shorten URL** www.google.com and the URL at index 20:
 
         $ buku --shorten www.google.com
         $ buku --shorten 20
-36. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
+37. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
 
         // append tags at taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 >> 5 3-2
         // set tags at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 > 5 3-2
         // remove all tags from bookmarks at indices 5 and 2-3
         buku (? for help) g > 5 3-2
         // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 << 5 3-2
-37. List bookmarks with **colored output**:
+38. List bookmarks with **colored output**:
 
         $ buku --colors oKlxm -p
-38. More **help**:
+39. Add a bookmark after following all permanent redirects, but only if the server doesn't respond with an error (and there's no network failure)
+
+        $ buku --add http://wikipedia.net --url-redirect --del-error
+        2. Wikipedia
+           > https://www.wikipedia.org/
+           + Wikipedia is a free online encyclopedia, created and edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a permanent redirect, or tag shaped like `http 404` on an error response:
+
+        $ buku --add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error 'http {}'
+        [ERROR] [404] Not Found
+        3. Not Found
+           > http://wikipedia.net/notfound
+           # http 404,http redirect
+41. Update all bookmarks matching the search by updating the URL if the server responds with a permanent redirect, deleting the bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500, or adding a tag shaped like `http:{}` in case of any other HTTP error; then export those affected by such changes into an HTML file, marking deleted records as well as old URLs for those replaced by redirect.
+
+        $ buku -S ://wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on --export backup.html
+42. More **help**:
 
         $ buku -h
         $ man buku
 
 ### Automation
 
 Interactive workflows can be automated using expect. Issue [#368](https://github.com/jarun/buku/issues/368) has a working example on automating auto-import.
@@ -485,38 +615,40 @@
 #### Editor integration
 
 You may encounter issues with GUI editors which maintain only one instance by default and return immediately from other instances. Use the appropriate editor option to block the caller when a new document is opened. See issue [#210](https://github.com/jarun/buku/issues/210) for gedit.
 
 ### Collaborators
 
 - [Arun Prakash Jana](https://github.com/jarun)
+- [Alexey Gulenko](https://github.com/LeXofLeviafan)
 - [Rachmadani Haryono](https://github.com/rachmadaniHaryono)
 - [Johnathan Jenkins](https://github.com/shaggytwodope)
 - [SZ Lin](https://github.com/szlin)
 
-Copyright © 2015-2022 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
+Copyright © 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 <br>
 <p><a href="https://gitter.im/jarun/buku"><img src="https://img.shields.io/gitter/room/jarun/buku.svg?maxAge=2592000" alt="gitter chat" /></a></p>
 
 ### Contributions
 
 Missing a feature? There's a rolling [ToDo List](https://github.com/jarun/buku/issues/484) with identified tasks. Contributions are welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/PR-guidelines).
 
+See also our documentation here <a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
+
 ### Related projects
 
 - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for browser integration
 - [oil](https://github.com/AndreiUlmeyda/oil), search-as-you-type cli front-end
 - [buku_run](https://github.com/carnager/buku_run), rofi front-end
 - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku import utility
 - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper
 - [poku](https://github.com/shanedabes/poku), sync between Pocket and buku
 - [Ebuku](https://github.com/flexibeast/ebuku), Emacs interface to buku
 - [diigoku](https://github.com/dppdppd/diigoku), buku importer for Diigo
 
-<a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
 
 ### Videos
 
 - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/embed/9HzEHrUBQXE)
 - [Buku is a great open-source bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8)
 
 ### In the Press
```

#### html2text {}

```diff
@@ -1,23 +1,70 @@
+Metadata-Version: 2.1 Name: buku Version: 4.9 Summary: Bookmark manager like a
+text-based mini-web. Home-page: https://github.com/jarun/buku Author: Arun
+Prakash Jana Author-email: engineerarun@gmail.com License: GPLv3 Project-URL:
+Documentation, https://buku.readthedocs.io/en/latest Project-URL: Funding,
+https://github.com/sponsors/jarun Project-URL: Source, https://github.com/
+jarun/buku Project-URL: Tracker, https://github.com/jarun/buku/issues Keywords:
+cli bookmarks tag utility Platform: any Classifier: Development Status :: 5 -
+Production/Stable Classifier: Environment :: Console Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: certifi Requires-Dist: cryptography>=1.2.3 Requires-Dist:
+html5lib>=1.0.1 Requires-Dist: urllib3<2,>=1.23 Requires-Dist: pyreadline3;
+sys_platform == "win32" Requires-Dist: colorama>=0.4.6; sys_platform == "win32"
+Provides-Extra: tests Requires-Dist: attrs>=17.4.0; extra == "tests" Requires-
+Dist: beautifulsoup4>=4.6.0; extra == "tests" Requires-Dist: Click>=7.0; extra
+== "tests" Requires-Dist: flake8>=3.4.1; extra == "tests" Requires-Dist:
+hypothesis>=6.0.0; extra == "tests" Requires-Dist: mypy-extensions==0.4.1;
+extra == "tests" Requires-Dist: py>=1.5.0; extra == "tests" Requires-Dist:
+pylint>=1.7.2; extra == "tests" Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-recording>=0.12.1; extra == "tests" Requires-Dist:
+pytest>=6.2.1; extra == "tests" Requires-Dist: PyYAML>=4.2b1; extra == "tests"
+Requires-Dist: setuptools>=41.0.1; extra == "tests" Requires-Dist:
+vcrpy>=1.13.0; extra == "tests" Requires-Dist: lxml; extra == "tests" Requires-
+Dist: flask_babel; extra == "tests" Requires-Dist: arrow>=1.2.2; extra ==
+"tests" Requires-Dist: Flask-Admin>=1.6.1; extra == "tests" Requires-Dist:
+Flask-API>=3.0.post1; extra == "tests" Requires-Dist: Flask-Bootstrap>=3.3.7.1;
+extra == "tests" Requires-Dist: flask-paginate>=2022.1.8; extra == "tests"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "tests" Requires-Dist:
+Flask<2.3,>=2.2.2; extra == "tests" Requires-Dist: werkzeug<2.4; extra ==
+"tests" Provides-Extra: server Requires-Dist: arrow>=1.2.2; extra == "server"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "server" Requires-Dist: Flask-
+API>=3.0.post1; extra == "server" Requires-Dist: Flask-Bootstrap>=3.3.7.1;
+extra == "server" Requires-Dist: flask-paginate>=2022.1.8; extra == "server"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "server" Requires-Dist:
+Flask<2.3,>=2.2.2; extra == "server" Requires-Dist: werkzeug<2.4; extra ==
+"server" Provides-Extra: docs Requires-Dist: myst-parser>=0.17.0; extra ==
+"docs" Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "docs" Requires-Dist:
+sphinx-autobuild>=2021.3.14; extra == "docs" Provides-Extra: packaging
+Requires-Dist: twine>=1.11.0; extra == "packaging"
                               ************ bbuukkuu ************
     _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_A_v_a_i_l_a_b_i_l_i_t_y_]_[_P_y_P_I_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_s_ _S_t_a_t_u_s_]_[_P_r_i_v_a_c_y
                               _A_w_a_r_e_n_e_s_s_]_[_L_i_c_e_n_s_e_]
                                _[_b_u_k_u_ _i_n_ _a_c_t_i_o_n_!_]
                                 buku in action!
 ### Introduction `buku` is a powerful bookmark manager and a personal textual
 mini-web. For those who prefer the GUI, [bukuserver](https://github.com/jarun/
 buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local
 web host server. When I started writing it, I couldn't find a flexible command-
 line solution with a private, portable, merge-able database along with seamless
 GUI integration. Hence, `buku`. `buku` can import bookmarks from browser(s) or
 fetch the title, tags and description of a URL from the web. Use your favourite
 editor to add, compose and update bookmarks. Search bookmarks instantly with
 multiple search options, including regex and a deep scan mode (handy with
-URLs). It can look up broken links on Wayback Machine. There's an Easter Egg to
-revisit random bookmarks. There's no tracking, hidden history, obsolete
+URLs). It can look up broken links on the Wayback Machine. There's an Easter
+Egg to revisit random bookmarks. There's no tracking, hidden history, obsolete
 records, usage analytics or homing. To get started right away, jump to the
 [Quickstart](#quickstart) section. `buku` has one of the best documentation
 around. The man page comes with examples. For internal details, please refer to
 the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 `buku` is a library too! There are several related projects, including a
 browser plug-in. ### Table of Contents - [Features](#features) - [Installation]
 (#installation) - [Dependencies](#dependencies) - [From a package manager]
@@ -27,24 +74,24 @@
 (#command-line-options) - [Colors](#colors) - [Quickstart](#quickstart) -
 [Examples](#examples) - [Automation](#automation) - [Troubleshooting]
 (#troubleshooting) - [Editor integration](#editor-integration) -
 [Collaborators](#collaborators) - [Contributions](#contributions) - [Related
 projects](#related-projects) - [In the Press](#in-the-press) ### Features -
 Store bookmarks with auto-fetched title, tags and description - Auto-import
 from Firefox, Google Chrome, Chromium and MS Edge - Open bookmarks and search
-results in browser - Shorten, expand URLs, browse cached page from Wayback
+results in browser - Shorten, expand URLs - Browse cached page from the Wayback
 Machine - Text editor integration - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...) - Continuous search with on the
 fly mode switch - Portable, merge-able database to sync between systems -
 Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile - Smart tag
-management using redirection (>>, >, <<) - Multi-threaded full DB refresh,
-manual encryption support - Shell completion scripts, man page with examples -
+management using redirection (>>, >, <<) - Multi-threaded full DB refresh -
+Manual encryption support - Shell completion scripts, man page with examples -
 Privacy-aware (no unconfirmed user data collection) ### Installation ####
 Dependencies | Feature | Dependency | | --- | --- | | Lang, SQLite | Python
-3.6+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
+3.8+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
 beautifulsoup4, html5lib | To copy URL to clipboard `buku` uses `xsel` (or
 `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default
 installed) on Windows, `termux-clipboard` on Termux (terminal emulation for
 Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-
 paste buffers are recognized. #### From a package manager To install buku with
 all its dependencies from PyPI, run: # pip3 install buku You can also install
 `buku` from your package manager. If the version available is dated try an
@@ -95,54 +142,64 @@
 tag "immutable": entries with locked title --deep match substrings ('pen'
 matches 'opens') -r, --sreg expr run a regex search -t, --stag [tag [,|+] ...]
 [- tag, ...] search bookmarks by tags use ',' to find entries matching ANY tag
 use '+' to find entries matching ALL tags excludes entries with tags after ' -
 ' list all tags, if no search keywords -x, --exclude [...] omit records
 matching specified keywords ENCRYPTION OPTIONS: -l, --lock [N] encrypt DB in N
 (default 8) # iterations -k, --unlock [N] decrypt DB in N (default 8) #
-iterations POWER TOYS: --ai auto-import (Firefox/Chrome/Chromium/Edge) -e, --
-export file export bookmarks to Firefox format HTML export XBEL, if file ends
-with '.xbel' export Markdown, if file ends with '.md' format: [title](url)
-export Orgfile, if file ends with '.org' format: *[[url][title]] :tags: export
-buku DB, if file ends with '.db' combines with search results, if opted -i, --
-import file import bookmarks based on file extension supports 'html', 'xbel',
-'json', 'md', 'org', 'db' -p, --print [...] show record details by indices,
-ranges print all bookmarks, if no arguments -n shows the last n results (like
-tail) -f, --format N limit fields in -p or JSON search output N=1: URL; N=2:
-URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0 (10, 20, 30,
-40, 50) omits DB index -j, --json [file] JSON formatted output for -p and
-search. prints to stdout if argument missing. otherwise writes to given file --
-colors COLORS set output colors in five-letter string --nc disable color output
--n, --count N show N results per page (default 10) --np do not show the
+iterations POWER TOYS: --ai auto-import bookmarks from web browsers Firefox,
+Chrome, Chromium, Vivaldi, Edge -e, --export file export bookmarks to Firefox
+format HTML export XBEL, if file ends with '.xbel' export Markdown, if file
+ends with '.md' format: [title](url) export Orgfile, if file ends with '.org'
+format: *[[url][title]] :tags: export buku DB, if file ends with '.db' combines
+with search results, if opted -i, --import file import bookmarks from file
+supports .html .xbel .json .md .org .db -p, --print [...] show record details
+by indices, ranges print all bookmarks, if no arguments -n shows the last n
+results (like tail) -f, --format N limit fields in -p or JSON search output
+N=1: URL; N=2: URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0
+(10, 20, 30, 40, 50) omits DB index -j, --json [file] JSON formatted output for
+-p and search. prints to stdout if argument missing. otherwise writes to given
+file --colors COLORS set output colors in five-letter string --nc disable color
+output -n, --count N show N results per page (default 10) --np do not show the
 subprompt, run and exit -o, --open [...] browse bookmarks by indices and ranges
 open a random bookmark, if no arguments --oa browse all search results
 immediately --replace old new replace old tag with new tag everywhere delete
-old tag, if new tag not specified --shorten index|URL fetch shortened url from
-tny.im service --expand index|URL expand a tny.im shortened url --cached
-index|URL browse a cached page from Wayback Machine --suggest show similar tags
-when adding bookmarks --tacit reduce verbosity, skip some confirmations --
-nostdin do not wait for input (must be first arg) --threads N max network
-connections in full refresh default N=4, min N=1, max N=10 -V check latest
-upstream version available -g, --debug show debug information and verbose logs
-SYMBOLS: > url + comment # tags PROMPT KEYS: 1-N browse search result indices
-and/or ranges O [id|range [...]] open search results/indices in GUI browser
-toggle try GUI browser if no arguments a open all results in browser s keyword
-[...] search for records with ANY keyword S keyword [...] search for records
-with ALL keywords d match substrings ('pen' matches 'opened') r expression run
-a regex search t [tag, ...] search by tags; show taglist, if no args g taglist
-id|range [...] [>>|>|<<] [record id|range ...] append, set, remove (all or
-specific) tags search by taglist id(s) if records are omitted n show next page
-of search results o id|range [...] browse bookmarks by indices and/or ranges p
-id|range [...] print bookmarks by indices and/or ranges w [editor|id] edit and
-add or update a bookmark c id copy URL at search result index to clipboard ?
-show this help q, ^D, double Enter exit buku ``` #### Colors `buku` supports
-custom colors. Visit the wiki page on how to [customize colors](https://
-github.com/jarun/buku/wiki/Customize-colors) for more details. ### Quickstart
-1. Export `VISUAL` or `EDITOR` to point to your favourite editor. Note that
-`VISUAL` takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
+old tag, if new tag not specified --url-redirect when fetching an URL, use the
+resulting URL from following *permanent* redirects (when combined with --
+export, the old URL is included as additional metadata) --tag-redirect [tag]
+when fetching an URL that causes permanent redirect, add a tag in specified
+pattern (using 'http:{}' if not specified) --tag-error [tag] when fetching an
+URL that causes an HTTP error, add a tag in specified pattern (using 'http:{}'
+if not specified) --del-error [...] when fetching an URL causes any (given)
+HTTP error, delete/do not add it --export-on [...] export records affected by
+the above options, including removed info (requires --update and --export;
+specific HTTP response filter can be provided) --shorten index|URL fetch
+shortened url from tny.im service --expand index|URL expand a tny.im shortened
+url --cached index|URL browse a cached page from Wayback Machine --offline add
+a bookmark without connecting to web --suggest show similar tags when adding
+bookmarks --tacit reduce verbosity, skip some confirmations --nostdin do not
+wait for input (must be first arg) --threads N max network connections in full
+refresh default N=4, min N=1, max N=10 -V check latest upstream version
+available -g, --debug show debug information and verbose logs SYMBOLS: > url +
+comment # tags PROMPT KEYS: 1-N browse search result indices and/or ranges O
+[id|range [...]] open search results/indices in GUI browser toggle try GUI
+browser if no arguments a open all results in browser s keyword [...] search
+for records with ANY keyword S keyword [...] search for records with ALL
+keywords d match substrings ('pen' matches 'opened') r expression run a regex
+search t [tag, ...] search by tags; show taglist, if no args g taglist id|range
+[...] [>>|>|<<] [record id|range ...] append, set, remove (all or specific)
+tags search by taglist id(s) if records are omitted n show next page of search
+results o id|range [...] browse bookmarks by indices and/or ranges p id|range
+[...] print bookmarks by indices and/or ranges w [editor|id] edit and add or
+update a bookmark c id copy URL at search result index to clipboard ? show this
+help q, ^D, double Enter exit buku ``` #### Colors `buku` supports custom
+colors. Visit the wiki page on how to [customize colors](https://github.com/
+jarun/buku/wiki/Customize-colors) for more details. ### Quickstart 1. Export
+`VISUAL` or `EDITOR` to point to your favourite editor. Note that `VISUAL`
+takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
 convenience. alias b='buku --suggest' 3. Auto-import bookmarks from your
 browser(s). Please quit the relevant browsers beforehand to ensure the
 databases are not locked. b --ai 4. Manually add a bookmark (for hands-on). b -
 w 5. List your bookmarks with DB index. b -p 6. For GUI and browser integration
 (or to sync bookmarks with your favourite bookmark management service) refer to
 the wiki page on [System integration](https://github.com/jarun/buku/wiki/
 System-integration). 7. Quick (bash/zsh) commands to fuzzy search with fzf and
@@ -151,120 +208,146 @@
 well: ```sh #!/usr/bin/env sh url=$(buku -p -f4 | fzf -m --reverse --preview
 "buku -p {1}" --preview-window=wrap | cut -f2) if [ -n "$url" ]; then echo
 "$url" | xargs firefox fi ``` ### Examples 1. **Edit and add** a bookmark from
 editor: $ buku -w $ buku -w 'gedit -w' $ buku -w 'macvim -f' -a https://ddg.gg
 search engine, privacy The first command picks editor from the environment
 variable `EDITOR`. The second command opens gedit in blocking mode. The third
 command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment**
-`Search engine with perks`, **fetch page title** from the web: $ buku -a https:
-//ddg.gg search engine, privacy -c Search engine with perks 336. DuckDuckGo >
-https://ddg.gg + Alternative search engine with perks # privacy,search engine
-where, >: URL, +: comment, #: tags 3. **Add** a bookmark with tags `search
-engine` & `privacy` and **immutable custom title** `DDG`: $ buku -a https://
-ddg.gg search engine, privacy --title 'DDG' --immutable 1 336. DDG (L) > https:
-//ddg.gg # privacy,search engine Note that URL must precede tags. 4. **Add** a
-bookmark **without a title** (works for update too): $ buku -a https://ddg.gg
-search engine, privacy --title 5. **Edit and update** a bookmark from editor: $
-buku -w 15012014 This will open the existing bookmark's details in the editor
-for modifications. Environment variable `EDITOR` must be set. 6. **Update**
-existing bookmark at index 15012014 with new URL, tags and comments, fetch
-title from the web: $ buku -u 15012014 --url http://ddg.gg/ --tag web search,
-utilities -c Private search engine 7. **Fetch and update only title** for
-bookmark at 15012014: $ buku -u 15012014 8. **Update only comment** for
-bookmark at 15012014: $ buku -u 15012014 -c this is a new comment Applies to --
-url, --title and --tag too. 9. **Export** bookmarks tagged `tag 1` or `tag 2`
-to HTML, XBEL, Markdown, Orgfile or a new database: $ buku -e bookmarks.html --
-stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag 1, tag 2 $ buku -
-e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --stag tag 1, tag 2
-$ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are exported if search
-is not opted. 10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile: $
-buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -i bookmarks.md $ buku -
-i bookmarks.org $ buku -i bookmarks.db 11. **Delete only comment** for bookmark
-at 15012014: $ buku -u 15012014 -c Applies to --title and --tag too. URL cannot
-be deleted without deleting the bookmark. 12. **Update** or refresh **full DB**
-with page titles from the web: $ buku -u $ buku -u --tacit (show only failures
-and exceptions) This operation can update the title or description fields of
-non-immutable bookmarks by parsing the fetched page. Fields are updated only if
-the fetched fields are non-empty. Tags remain untouched. 13. **Delete**
-bookmark at index 15012014: $ buku -d 15012014 Index 15012020 moved to 15012014
-The last index is moved to the deleted index to keep the DB compact. Add `--
-tacit` to delete without confirmation. 14. **Delete all** bookmarks: $ buku -
-d 15. **Delete** a **range or list** of bookmarks: $ buku -d 100-200 $ buku -
-d 100 15 200 16. **Search** bookmarks for **ANY** of the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku kernel debugging $ buku -s kernel
-debugging 17. **Search** bookmarks with **ALL** the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku -S kernel debugging 18. **Search**
-bookmarks **tagged** `general kernel concepts`: $ buku --stag general kernel
-concepts 19. **Search** for bookmarks matching **ANY** of the tags `kernel`,
-`debugging`, `general kernel concepts`: $ buku --stag kernel, debugging,
-general kernel concepts 20. **Search** for bookmarks matching **ALL** of the
-tags `kernel`, `debugging`, `general kernel concepts`: $ buku --stag kernel +
-debugging + general kernel concepts 21. **Search** for bookmarks matching any
-of the keywords `hello` or `world`, excluding the keywords `real` and `life`,
-matching both the tags `kernel` and `debugging`, but **excluding** the tags
-`general kernel concepts` and `books`: $ buku hello world --exclude real life -
--stag 'kernel + debugging - general kernel concepts, books' 22. List **all
-unique tags** alphabetically: $ buku --stag 23. Run a **search and update** the
-results: $ buku -s kernel debugging -u --tag + linux kernel 24. Run a **search
-and delete** the results: $ buku -s kernel debugging -d 25. **Encrypt or
-decrypt** DB with **custom number of iterations** (15) to generate key: $ buku
--l 15 $ buku -k 15 The same number of iterations must be specified for one lock
-& unlock instance. Default is 8, if omitted. 26. **Show details** of bookmarks
-at index 15012014 and ranges 20-30, 40-50: $ buku -p 20-30 15012014 40-50 27.
-Show details of the **last 10 bookmarks**: $ buku -p -10 28. **Show all**
-bookmarks with real index from database: $ buku -p $ buku -p | more 29.
-**Replace tag** 'old tag' with 'new tag': $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB: $ buku --replace 'old tag' 31. **Append
-(or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at
-index 15012014: $ buku -u 15012014 --tag + tag 1, tag 2 $ buku -u 15012014 --
-tag - tag 1, tag 2 32. **Open URL** at index 15012014 in browser: $ buku -
-o 15012014 33. List bookmarks with **no title or tags** for bookkeeping: $ buku
--S blank 34. List bookmarks with **immutable title**: $ buku -S immutable 35.
-**Shorten URL** www.google.com and the URL at index 20: $ buku --shorten
-www.google.com $ buku --shorten 20 36. **Append, remove tags at prompt**
-(taglist index to the left, bookmark index to the right): // append tags at
-taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-
-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags at taglist indices 4 and 6-
-9 as tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 > 5 3-2 /
-/ remove all tags from bookmarks at indices 5 and 2-3 buku (? for help) g > 5
-3-2 // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at
-indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 37. List bookmarks with
-**colored output**: $ buku --colors oKlxm -p 38. More **help**: $ buku -h $ man
-buku ### Automation Interactive workflows can be automated using expect. Issue
-[#368](https://github.com/jarun/buku/issues/368) has a working example on
-automating auto-import. ### Troubleshooting #### Editor integration You may
-encounter issues with GUI editors which maintain only one instance by default
-and return immediately from other instances. Use the appropriate editor option
-to block the caller when a new document is opened. See issue [#210](https://
-github.com/jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash
-Jana](https://github.com/jarun) - [Rachmadani Haryono](https://github.com/
-rachmadaniHaryono) - [Johnathan Jenkins](https://github.com/shaggytwodope) -
-[SZ Lin](https://github.com/szlin) Copyright Â© 2015-2022 [Arun Prakash Jana]
-(mailto:engineerarun@gmail.com)
+2. **Add** a simple bookmark: $ buku --nostdin -a https://github.com/ 2648.
+GitHub: Letâs build from here Â· GitHub > https://github.com/ + GitHub is
+where over 94 million developers shape the future of software, together.
+Contribute to the open source community, manage your Git repositories, review
+code like a pro, track bugs and features, power your CI/CD and DevOps
+workflows, and secure code before you commit it. $ buku --nostdin -a https://
+github.com/ [ERROR] URL [https://github.com/] already exists at index 2648 `>`:
+URL, `+`: comment, `#`: tags Title, description and tags will be fetched from
+site. Buku only stores unique URLs and will raise error if the URL already
+present in the database: 3. **Add** a bookmark with **tags** `search engine`
+and `privacy`, **comment** `Search engine with perks`, **fetch page title**
+from the web: $ buku -a https://ddg.gg search engine, privacy -c Search engine
+with perks 336. DuckDuckGo > https://ddg.gg + Alternative search engine with
+perks # privacy,search engine where, `>`: URL, `+`: comment, `#`: tags 4.
+**Add** a bookmark with tags `search engine` & `privacy` and **immutable custom
+title** `DDG`: $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --
+immutable 1 336. DDG (L) > https://ddg.gg # privacy,search engine Note that URL
+must precede tags. 5. **Add** a bookmark **without a title** (works for update
+too): $ buku -a https://ddg.gg search engine, privacy --title 6. **Edit and
+update** a bookmark from editor: $ buku -w 15012014 This will open the existing
+bookmark's details in the editor for modifications. Environment variable
+`EDITOR` must be set. 7. **Update** existing bookmark at index 15012014 with
+new URL, tags and comments, fetch title from the web: $ buku -u 15012014 --url
+http://ddg.gg/ --tag web search, utilities -c Private search engine 8. **Fetch
+and update only title** for bookmark at 15012014: $ buku -u 15012014 9.
+**Update only comment** for bookmark at 15012014: $ buku -u 15012014 -c this is
+a new comment Applies to --url, --title and --tag too. 10. **Export** bookmarks
+tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database: $
+buku -e bookmarks.html --stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag
+1, tag 2 $ buku -e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --
+stag tag 1, tag 2 $ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are
+exported if search is not opted. 11. **Import** bookmarks from HTML, XBEL,
+Markdown or Orgfile: $ buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -
+i bookmarks.md $ buku -i bookmarks.org $ buku -i bookmarks.db 12. **Delete only
+comment** for bookmark at 15012014: $ buku -u 15012014 -c Applies to --title
+and --tag too. URL cannot be deleted without deleting the bookmark. 13.
+**Update** or refresh **full DB** with page titles from the web: $ buku -u $
+buku -u --tacit (show only failures and exceptions) This operation can update
+the title or description fields of non-immutable bookmarks by parsing the
+fetched page. Fields are updated only if the fetched fields are non-empty. Tags
+remain untouched. 14. **Delete** bookmark at index 15012014: $ buku -d 15012014
+Index 15012020 moved to 15012014 The last index is moved to the deleted index
+to keep the DB compact. Add `--tacit` to delete without confirmation. 15.
+**Delete all** bookmarks: $ buku -d 16. **Delete** a **range or list** of
+bookmarks: $ buku -d 100-200 $ buku -d 100 15 200 17. **Search** bookmarks for
+**ANY** of the keywords `kernel` and `debugging` in URL, title or tags: $ buku
+kernel debugging $ buku -s kernel debugging 18. **Search** bookmarks with
+**ALL** the keywords `kernel` and `debugging` in URL, title or tags: $ buku -
+S kernel debugging 19. **Search** bookmarks **tagged** `general kernel
+concepts`: $ buku --stag general kernel concepts 20. **Search** for bookmarks
+matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+$ buku --stag kernel, debugging, general kernel concepts 21. **Search** for
+bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel
+concepts`: $ buku --stag kernel + debugging + general kernel concepts 22.
+**Search** for bookmarks matching any of the keywords `hello` or `world`,
+excluding the keywords `real` and `life`, matching both the tags `kernel` and
+`debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+$ buku hello world --exclude real life --stag 'kernel + debugging - general
+kernel concepts, books' 23. List **all unique tags** alphabetically: $ buku --
+stag 24. Run a **search and update** the results: $ buku -s kernel debugging -
+u --tag + linux kernel 25. Run a **search and delete** the results: $ buku -
+s kernel debugging -d 26. **Encrypt or decrypt** DB with **custom number of
+iterations** (15) to generate key: $ buku -l 15 $ buku -k 15 The same number of
+iterations must be specified for one lock & unlock instance. Default is 8, if
+omitted. 27. **Show details** of bookmarks at index 15012014 and ranges 20-30,
+40-50: $ buku -p 20-30 15012014 40-50 28. Show details of the **last 10
+bookmarks**: $ buku -p -10 29. **Show all** bookmarks with real index from
+database: $ buku -p $ buku -p | more 30. **Replace tag** 'old tag' with 'new
+tag': $ buku --replace 'old tag' 'new tag' 31. **Delete tag** 'old tag' from
+DB: $ buku --replace 'old tag' 32. **Append (or delete) tags** 'tag 1', 'tag 2'
+to (or from) existing tags of bookmark at index 15012014: $ buku -u 15012014 --
+tag + tag 1, tag 2 $ buku -u 15012014 --tag - tag 1, tag 2 33. **Open URL** at
+index 15012014 in browser: $ buku -o 15012014 34. List bookmarks with **no
+title or tags** for bookkeeping: $ buku -S blank 35. List bookmarks with
+**immutable title**: $ buku -S immutable 36. **Shorten URL** www.google.com and
+the URL at index 20: $ buku --shorten www.google.com $ buku --shorten 20 37.
+**Append, remove tags at prompt** (taglist index to the left, bookmark index to
+the right): // append tags at taglist indices 4 and 6-9 to existing tags in
+bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags
+at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3 buku (?
+for help) g 4 9-6 > 5 3-2 // remove all tags from bookmarks at indices 5 and 2-
+3 buku (? for help) g > 5 3-2 // remove tags at taglist indices 4 and 6-9 from
+tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 38.
+List bookmarks with **colored output**: $ buku --colors oKlxm -p 39. Add a
+bookmark after following all permanent redirects, but only if the server
+doesn't respond with an error (and there's no network failure) $ buku --add
+http://wikipedia.net --url-redirect --del-error 2. Wikipedia > https://
+www.wikipedia.org/ + Wikipedia is a free online encyclopedia, created and
+edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a
+permanent redirect, or tag shaped like `http 404` on an error response: $ buku
+--add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error
+'http {}' [ERROR] [404] Not Found 3. Not Found > http://wikipedia.net/notfound
+# http 404,http redirect 41. Update all bookmarks matching the search by
+updating the URL if the server responds with a permanent redirect, deleting the
+bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500,
+or adding a tag shaped like `http:{}` in case of any other HTTP error; then
+export those affected by such changes into an HTML file, marking deleted
+records as well as old URLs for those replaced by redirect. $ buku -S ://
+wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on
+--export backup.html 42. More **help**: $ buku -h $ man buku ### Automation
+Interactive workflows can be automated using expect. Issue [#368](https://
+github.com/jarun/buku/issues/368) has a working example on automating auto-
+import. ### Troubleshooting #### Editor integration You may encounter issues
+with GUI editors which maintain only one instance by default and return
+immediately from other instances. Use the appropriate editor option to block
+the caller when a new document is opened. See issue [#210](https://github.com/
+jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash Jana]
+(https://github.com/jarun) - [Alexey Gulenko](https://github.com/LeXofLeviafan)
+- [Rachmadani Haryono](https://github.com/rachmadaniHaryono) - [Johnathan
+Jenkins](https://github.com/shaggytwodope) - [SZ Lin](https://github.com/szlin)
+Copyright Â© 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 _[_g_i_t_t_e_r_ _c_h_a_t_]
 ### Contributions Missing a feature? There's a rolling [ToDo List](https://
 github.com/jarun/buku/issues/484) with identified tasks. Contributions are
 welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/
-PR-guidelines). ### Related projects - [bukubrow](https://github.com/SamHH/
-bukubrow), WebExtension for browser integration - [oil](https://github.com/
-AndreiUlmeyda/oil), search-as-you-type cli front-end - [buku_run](https://
-github.com/carnager/buku_run), rofi front-end - [pinku](https://github.com/
-mosegontar/pinku), a Pinboard-to-buku import utility - [buku-dmenu](https://
-gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper - [poku]
-(https://github.com/shanedabes/poku), sync between Pocket and buku - [Ebuku]
-(https://github.com/flexibeast/ebuku), Emacs interface to buku - [diigoku]
-(https://github.com/dppdppd/diigoku), buku importer for Diigo _[_S_t_a_b_l_e_ _D_o_c_s_]###
-Videos - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/
-embed/9HzEHrUBQXE) - [Buku is a great open-source bookmark manager](https://
-www.youtube.com/embed/7VxgKMWm-J8) ### In the Press - [2daygeek](http://
-www.2daygeek.com/buku-command-line-bookmark-manager-linux/) - [Hacker Milk]
-(https://hackermilk.blogspot.com/2020/01/how-to-manage-your-browsers-
-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-line-
-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/buku-
-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
+PR-guidelines). See also our documentation here _[_S_t_a_b_l_e_ _D_o_c_s_]### Related
+projects - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for
+browser integration - [oil](https://github.com/AndreiUlmeyda/oil), search-as-
+you-type cli front-end - [buku_run](https://github.com/carnager/buku_run), rofi
+front-end - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku
+import utility - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a
+simple bash dmenu wrapper - [poku](https://github.com/shanedabes/poku), sync
+between Pocket and buku - [Ebuku](https://github.com/flexibeast/ebuku), Emacs
+interface to buku - [diigoku](https://github.com/dppdppd/diigoku), buku
+importer for Diigo ### Videos - [Buku: Take Your Bookmarks Everywhere You Go]
+(https://www.youtube.com/embed/9HzEHrUBQXE) - [Buku is a great open-source
+bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8) ### In the Press -
+[2daygeek](http://www.2daygeek.com/buku-command-line-bookmark-manager-linux/) -
+[Hacker Milk](https://hackermilk.blogspot.com/2020/01/how-to-manage-your-
+browsers-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-
+line-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/
+buku-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
 www.linux-community.de/LU/2017/01/Das-Beste-aus-zwei-Welten) - [Make Tech
 Easier](https://www.maketecheasier.com/manage-browser-bookmarks-ubuntu-command-
 line/) - [One Thing Well](http://onethingwell.org/post/144952807044/buku) -
 [Open Source For You](https://opensourceforu.com/2018/05/buku-a-bookmark-
 manager-in-the-command-line/) - [ulno.net](https://ulno.net/blog/2017-07-19/of-
 bookmarks-tags-and-browsers/)
```

### Comparing `buku-4.7.1/auto-completion/bash/buku-completion.bash` & `buku-4.9/auto-completion/bash/buku-completion.bash`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,21 @@
         -o --open
         --oa
         -p --print
         -r --sreg
         --replace
         -s --sany
         -S --sall
+        --url-redirect
+        --tag-redirect
+        --tag-error
+        --del-error
+        --export-on
         --shorten
+        --offline
         --suggest
         -t --stag
         --tacit
         --tag
         --threads
         --title
         -u --update
```

### Comparing `buku-4.7.1/auto-completion/fish/buku.fish` & `buku-4.9/auto-completion/fish/buku.fish`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,21 @@
 complete -c buku -s o -l open       --description 'open bookmarks in browser'
 complete -c buku -l oa              --description 'browse all search results immediately'
 complete -c buku -s p -l print      --description 'show bookmark details'
 complete -c buku -s r -l sreg    -r --description 'match a regular expression'
 complete -c buku -l replace      -r --description 'replace a tag'
 complete -c buku -s s -l sany    -r --description 'match any keyword'
 complete -c buku -s S -l sall    -r --description 'match all keywords'
+complete -c buku -l url-redirect    --description 'update URL on a permanent redirect'
+complete -c buku -l tag-redirect    --description 'add tag on a permanent redirect'
+complete -c buku -l tag-error       --description 'add tag on an HTTP error'
+complete -c buku -l del-error       --description 'delete bookmark on an HTTP error'
+complete -c buku -l export-on       --description 'export bookmarks based on HTTP status'
 complete -c buku -l shorten      -r --description 'shorten a URL using tny.im'
+complete -c buku -l offline         --description 'add a bookmark without connecting to web'
 complete -c buku -l suggest         --description 'show a list of similar tags'
 complete -c buku -s t -l stag       --description 'search by tag or show tags'
 complete -c buku -l tacit           --description 'reduce verbosity'
 complete -c buku -l tag             --description 'set tags, use + to append, - to remove'
 complete -c buku -l threads      -r --description 'max connections for full refresh'
 complete -c buku -l title           --description 'set custom title'
 complete -c buku -s u -l update     --description 'update bookmark'
```

### Comparing `buku-4.7.1/auto-completion/zsh/_buku` & `buku-4.9/auto-completion/zsh/_buku`

 * *Files 17% similar despite different names*

```diff
@@ -27,19 +27,25 @@
     '(-l --lock)'{-l,--lock}'[encrypt database]'
     '(-n --count)'{-n,--count}'[results per page]:value'
     '(--nc)--nc[disable color output]'
     '(--np)--np[noninteractive mode]'
     '(-o --open)'{-o,--open}'[open bookmarks in browser]'
     '(--oa)--oa[browse all search results immediately]'
     '(-p --print)'{-p,--print}'[show bookmark details]'
-    '(-r --sreg)'{-r,--sreg}'[match a regular exression]:regex'
+    '(-r --sreg)'{-r,--sreg}'[match a regular expression]:regex'
     '(--replace)--replace[replace a tag]:tag to replace'
     '(-s --sany)'{-s,--sany}'[match any keyword]:keyword(s)'
     '(-S --sall)'{-S,--sall}'[match all keywords]:keyword(s)'
+    '(--url-redirect)--url-redirect[update URL on a permanent redirect]'
+    '(--tag-redirect)--tag-redirect[add tag on a permanent redirect]:tag pattern'
+    '(--tag-error)--tag-error[add tag on an HTTP error]:tag pattern'
+    '(--del-error)--del-error[delete bookmark on an HTTP error]:HTTP codes'
+    '(--export-on)--export-on[export bookmarks based on HTTP status]:HTTP codes'
     '(--shorten)--shorten[shorten a URL using tny.im]:index/url'
+    '(--offline)--offline[add a bookmark without connecting to web]'
     '(--suggest)--suggest[show a list of similar tags]'
     '(-t --stag)'{-t,--stag}'[search by tag or show tags]'
     '(--tacit)--tacit[reduce verbosity]'
     '(--tag)--tag[set tags, use + to append, - to remove]'
     '(--threads)--threads[max connections for full refresh]:value'
     '(--title)--title[set custom title]'
     '(-u --update)'{-u,--update}'[update bookmark]'
```

### Comparing `buku-4.7.1/buku.1` & `buku-4.9/buku.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-.TH "BUKU" "1" "1 Jul 2022" "Version 4.7" "User Commands"
+.TH "BUKU" "1" "07 Apr 2024" "Version 4.9" "User Commands"
 .SH NAME
 buku \- Bookmark manager like a text-based mini-web
 .SH SYNOPSIS
 .B buku [OPTIONS] [KEYWORD [KEYWORD ...]]
 .SH DESCRIPTION
 .B buku
 is a command-line utility to store, tag, search and organize bookmarks.
 .PP
 .B Features
 .PP
   * Store bookmarks with auto-fetched title, tags and description
-  * Auto-import from Firefox, Google Chrome, Chromium and MS Edge
+  * Auto-import from Firefox, Google Chrome, Chromium, Vivaldi, and MS Edge
   * Open bookmarks and search results in browser
-  * Shorten, expand URLs, browse cached page from Wayback Machine
+  * Shorten, expand URLs
+  * Browse cached page from the Wayback Machine
   * Text editor integration
   * Lightweight, clean interface, custom colors
   * Powerful search options (regex, substring...)
   * Continuous search with on the fly mode switch
   * Portable, merge-able database to sync between systems
   * Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile
   * Smart tag management using redirection (>>, >, <<)
-  * Multithreaded full DB refresh, manual encryption support
+  * Multithreaded full DB refresh
+  * Manual encryption support
   * Shell completion scripts, man page with handy examples
 .SH OPERATIONAL NOTES
 .PP
 .IP 1. 4
 The database file is stored in:
   - \fI$XDG_DATA_HOME/buku/bookmarks.db\fR, if XDG_DATA_HOME is defined (first preference), or
   - \fI$HOME/.local/share/buku/bookmarks.db\fR, if HOME is defined (second preference), or
@@ -76,14 +78,15 @@
 .PP
 .IP 9. 4
 \fBImport\fR:
   - Auto-import looks in the default installation path and default user profile.
   - URLs starting with `place:`, `file://` and `apt:` are ignored during import.
   - Parent folder (and subfolder) names are automatically imported as tags if --tacit is used.
   - Tags are merged even if bookmark URL exists when --tacit is used.
+  - JSON files exported from browser can be imported. Export to JSON is not supported.
 .PP
 .IP 10. 4
 \fBEncryption\fR is optional and manual. AES256 algorithm is used. To use encryption, the database file should be unlocked (-k) before using \fBbuku\fR and locked (-l) afterwards. Between these 2 operations, the database file lies unencrypted on the disk, and NOT in memory. Also, note that the database file is \fBunencrypted on creation\fR.
 .PP
 .IP 11. 4
 \fBEditor\fR support:
   - A single bookmark can be edited before adding. The editor can be set using the environment variable *EDITOR* or by explicitly specifying the editor. The latter takes precedence. If -a is used along with -w, the details are populated in the editor template.
@@ -187,15 +190,15 @@
 .BI \-k " " \--unlock " [N]"
 Decrypt (unlock) the DB file with
 .I N
 (> 0, default 8) hash passes to generate key.
 .SH POWER OPTIONS
 .TP
 .BI \--ai
-Auto-import bookmarks from Firefox, Google Chrome, Chromium and Edge browsers.
+Auto-import bookmarks from Firefox, Google Chrome, Chromium, Vivaldi, and Edge browsers. (Firefox profile can be specified using environment variable FIREFOX_PROFILE.)
 .TP
 .BI \-e " " \--export " file"
 Export bookmarks to Firefox bookmarks formatted HTML. Works with all search options.
 .br
 XBEL is used if
 .I file
 has extension '.xbel'.
@@ -268,14 +271,33 @@
 .I new
 tag if both are passed; delete
 .I old
 tag if
 .I new
 tag is not specified.
 .TP
+.BI \--url-redirect
+when fetching an URL, use the resulting URL from following \fBpermanent\fR redirects (when combined with --export, the old URL is included as additional metadata).
+.TP
+.BI \--tag-redirect " [tag]"
+when fetching an URL that causes permanent redirect, add a
+.I tag
+in specified pattern (using 'http:{}' if not specified).
+.TP
+.BI \--tag-error " [tag]"
+when fetching an URL that causes an HTTP error, add a
+.I tag
+in specified pattern (using 'http:{}' if not specified).
+.TP
+.BI \--del-error " [...]"
+when fetching an URL causes any (given) HTTP error, delete/do not add it. (Use a parameter like '404' or '400-404,500')
+.TP
+.BI \--export-on " [...]"
+export records affected by the above options, including removed info (requires --update and --export; specific HTTP response filter can be provided).
+.TP
 .BI \--shorten " index|URL"
 Shorten the URL at DB
 .I index
 or an independent
 .I URL
 using the tny.im URL shortener service.
 .TP
@@ -289,14 +311,17 @@
 .BI \--cached " index|URL"
 Browse the latest cached version of the URL at DB
 .I index
 or an independent
 .I URL
 using the Wayback Machine. Useful for viewing the content of bookmarks which are not live any more.
 .TP
+.BI \--offline
+Add a bookmark without connecting to the web.
+.TP
 .BI \--suggest
 Show a list of similar tags to choose from when adding a new bookmark.
 .TP
 .BI \--tacit
 Show lesser output. Reduces the verbosity of certain operations like add, update etc.
 .TP
 .BI \--nostdin
@@ -470,82 +495,93 @@
 .B buku -w 'macvim -f' -a https://ddg.gg search engine, privacy
 .EE
 .PP
 .IP "" 4
 The first command picks editor from the environment variable \fIEDITOR\fR. The second command opens gedit in blocking mode. The third command opens macvim with option -f and the URL and tags populated in template.
 .PP
 .IP 2. 4
+\fBAdd\fR a simple bookmark:
+.PP
+.EX
+.IP
+.B buku --no-stdin -a https://github.com/
+.EE
+.PP
+.IP "" 4
+In the output, >: url, +: comment, #: tags.
+.PP
+.IP 3. 4
 \fBAdd\fR a bookmark with \fBtags\fR 'search engine' and 'privacy', \fBcomment\fR 'Search engine with perks', \fBfetch page title\fR from the web:
 .PP
 .EX
 .IP
 .B buku -a https://ddg.gg search engine, privacy -c Search engine with perks
 .EE
 .PP
 .IP "" 4
 In the output, >: url, +: comment, #: tags.
 .PP
-.IP 3. 4
+.IP 4. 4
 \fBAdd\fR a bookmark with tags 'search engine' & 'privacy' and \fBimmutable custom title\fR 'DDG':
 .PP
 .EX
 .IP
 .B buku -a https://ddg.gg search engine, privacy --title 'DDG' --immutable 1
 .EE
 .PP
 .IP "" 4
 Note that URL must precede tags.
 .PP
-.IP 4. 4
+.IP 5. 4
 \fBAdd\fR a bookmark \fBwithout a title\fR (works for update too):
 .PP
 .EX
 .IP
 .B buku -a https://ddg.gg search engine, privacy --title
 .EE
 .PP
-.IP 5. 4
+.IP 6. 4
 \fBEdit and update\fR a bookmark from editor:
 .PP
 .EX
 .IP
 .B buku -w 15012014
 .EE
 .PP
 .IP "" 4
 This will open the existing bookmark's details in the editor for modifications. Environment variable \fIEDITOR\fR must be set.
 .PP
-.IP 6. 4
+.IP 7. 4
 \fBUpdate\fR existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
 .PP
 .EX
 .IP
 .B buku -u 15012014 --url http://ddg.gg/ --tag web search, utilities -c Private search engine
 .EE
 .PP
-.IP 7. 4
+.IP 8. 4
 \fBFetch and update only title\fR for bookmark at 15012014:
 .PP
 .EX
 .IP
 .B buku -u 15012014
 .EE
 .PP
-.IP 8. 4
+.IP 9. 4
 \fBUpdate only comment\fR for bookmark at 15012014:
 .PP
 .EX
 .IP
 .B buku -u 15012014 -c this is a new comment
 .EE
 .PP
 .IP "" 4
 Applies to --url, --title and --tag too.
 .PP
-.IP 9. 4
+.IP 10. 4
 \fBExport\fR bookmarks tagged 'tag 1' or 'tag 2' to HTML, XBEL, Markdown, Orgfile or a new database:
 .PP
 .EX
 .IP
 .B buku -e bookmarks.html --stag tag 1, tag 2
 .br
 .B buku -e bookmarks.xbel --stag tag 1, tag 2
@@ -556,253 +592,253 @@
 .br
 .B buku -e bookmarks.db --stag tag 1, tag 2
 .EE
 .PP
 .IP "" 4
 All bookmarks are exported if search is not opted.
 .PP
-.IP 10. 4
+.IP 11. 4
 \fBImport\fR bookmarks from HTML, XBEL, Markdown or Orgfile:
 .PP
 .EX
 .IP
 .B buku -i bookmarks.html
 .br
 .B buku -i bookmarks.xbel
 .br
 .B buku -i bookmarks.md
 .br
 .B buku -i bookmarks.db
 .EE
 .PP
-.IP 11. 4
+.IP 12. 4
 \fBDelete only comment\fR for bookmark at 15012014:
 .PP
 .EX
 .IP
 .B buku -u 15012014 -c
 .EE
 .PP
 .IP "" 4
 Applies to --title and --tag too. URL cannot be deleted without deleting the bookmark.
 .PP
-.IP 12. 4
+.IP 13. 4
 \fBUpdate\fR or refresh \fBfull DB\fR with page titles from the web:
 .PP
 .EX
 .IP
 .B buku -u
 .br
 .B buku -u --tacit (show only failures and exceptions)
 .EE
 .PP
 .IP "" 4
 This operation can update the title or description fields of non-immutable bookmarks by parsing the fetched page. Fields are updated only if the fetched fields are non-empty. Tags remain untouched.
 .PP
-.IP 13. 4
+.IP 14. 4
 \fBDelete\fR bookmark at index 15012014:
 .PP
 .EX
 .IP
 .B buku -d 15012014
 .EE
 .PP
 .IP "" 4
 The last index is moved to the deleted index to keep the DB compact. Add --tacit to delete without confirmation.
 .PP
-.IP 14. 4
+.IP 15. 4
 \fBDelete all\fR bookmarks:
 .PP
 .EX
 .IP
 .B buku -d
 .EE
 .PP
-.IP 15. 4
+.IP 16. 4
 \fBDelete\fR a \fBrange or list\fR of bookmarks:
 .PP
 .EX
 .IP
 .B buku -d 100-200
 .br
 .B buku -d 100 15 200
 .EE
 .PP
-.IP 16. 4
+.IP 17. 4
 \fBSearch\fR bookmarks for \fBANY\fR of the keywords 'kernel' and 'debugging' in URL, title or tags:
 .PP
 .EX
 .IP
 .B buku kernel debugging
 .br
 .B buku -s kernel debugging
 .EE
 .PP
-.IP 17. 4
+.IP 18. 4
 \fBSearch\fR bookmarks with \fBALL\fR the keywords 'kernel' and 'debugging' in URL, title or tags:
 .PP
 .EX
 .IP
 .B buku -S kernel debugging
 .EE
 .PP
-.IP 18. 4
+.IP 19. 4
 \fBSearch\fR bookmarks \fBtagged\fR 'general kernel concepts':
 .PP
 .EX
 .IP
 .B buku --stag general kernel concepts
 .EE
 .PP
-.IP 19. 4
+.IP 20. 4
 \fBSearch\fR for bookmarks matching \fBANY\fR of the tags 'kernel', 'debugging', 'general kernel concepts':
 .PP
 .EX
 .IP
 .B buku --stag kernel, debugging, general kernel concepts
 .EE
 .PP
-.IP 20. 4
+.IP 21. 4
 \fBSearch\fR for bookmarks matching \fBALL\fR of the tags 'kernel', 'debugging', 'general kernel concepts':
 .PP
 .EX
 .IP
 .B buku --stag kernel + debugging + general kernel concepts
 .EE
 .PP
-.IP 21. 4
+.IP 22. 4
 \fBSearch\fR for bookmarks matching any of the keywords 'hello' or 'world', excluding the keywords 'real' and 'life', matching both the tags 'kernel' and 'debugging', but \fBexcluding\fR the tags 'general kernel concepts' and 'books':
 .PP
 .EX
 .IP
 .B buku hello world --exclude real life --stag 'kernel + debugging - general kernel concepts, books'
-.IP 22. 4
+.IP 23. 4
 List \fBall unique tags\fR alphabetically:
 .PP
 .EX
 .IP
 .B buku --stag
 .EE
 .PP
-.IP 23. 4
+.IP 24. 4
 Run a \fBsearch and update\fR the results:
 .PP
 .EX
 .IP
 .B buku -s kernel debugging -u --tag + linux kernel
 .EE
 .PP
-.IP 24. 4
+.IP 25. 4
 Run a \fBsearch and delete\fR the results:
 .PP
 .EX
 .IP
 .B buku -s kernel debugging -d
 .EE
 .PP
-.IP 25. 4
+.IP 26. 4
 \fBEncrypt or decrypt\fR DB with \fBcustom number of iterations\fR (15) to generate key:
 .PP
 .EX
 .IP
 .B buku -l 15
 .br
 .B buku -k 15
 .EE
 .PP
 .IP "" 4
 The same number of iterations must be specified for one lock & unlock instance. Default is 8, if omitted.
 .PP
-.IP 26. 4
+.IP 27. 4
 \fBShow details\fR of bookmarks at index 15012014 and ranges 20-30, 40-50:
 .PP
 .EX
 .IP
 .B buku -p 20-30 15012014 40-50
 .EE
 .PP
-.IP 27. 4
+.IP 28. 4
 Show details of the \fBlast 10 bookmarks\fR:
 .PP
 .EX
 .IP
 .B buku -p -10
 .EE
 .PP
-.IP 28. 4
+.IP 29. 4
 \fBShow all\fR bookmarks with real index from database:
 .PP
 .EX
 .IP
 .B buku -p
 .br
 .B buku -p | more
 .EE
 .PP
-.IP 29. 4
+.IP 30. 4
 \fBReplace tag\fR 'old tag' with 'new tag':
 .PP
 .EX
 .IP
 .B buku --replace 'old tag' 'new tag'
 .EE
 .PP
-.IP 30. 4
+.IP 31. 4
 \fBDelete tag\fR 'old tag' from DB:
 .PP
 .EX
 .IP
 .B buku --replace 'old tag'
 .EE
 .PP
-.IP 31. 4
+.IP 32. 4
 \fBAppend (or delete) tags\fR 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
 .PP
 .EX
 .IP
 .B buku -u 15012014 --tag + tag 1, tag 2
 .br
 .B buku -u 15012014 --tag - tag 1, tag 2
 .EE
 .PP
-.IP 32. 4
+.IP 33. 4
 \fBOpen URL\fR at index 15012014 in browser:
 .PP
 .EX
 .IP
 .B buku -o 15012014
 .EE
 .PP
-.IP 33. 4
+.IP 34. 4
 List bookmarks with \fBno title or tags\fR for bookkeeping:
 .PP
 .EX
 .IP
 .B buku -S blank
 .EE
 .PP
-.IP 34. 4
+.IP 35. 4
 List bookmarks with \fBimmutable title\fR:
 .PP
 .EX
 .IP
 .B buku -S immutable
 .EE
 .PP
-.IP 35. 4
+.IP 36. 4
 \fBShorten\fR the URL www.google.com and the URL at index 20:
 .PP
 .EX
 .IP
 .B buku --shorten www.google.com
 .br
 .B buku --shorten 20
 .EE
 .PP
-.IP 36. 4
+.IP 37. 4
 \fBAppend, remove tags at prompt\fR (taglist index to the left, bookmark index to the right):
 .PP
 .EX
 .IP
 // append tags at taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-3
 .br
 .B buku (? for help) g 4 9-6 >> 5 3-2
@@ -816,30 +852,68 @@
 .B buku (? for help) g > 5 3-2
 .br
 // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at indices 5 and 2-3
 .br
 .B buku (? for help) g 4 9-6 << 5 3-2
 .EE
 .PP
-.IP 37. 4
+.IP 38. 4
 List bookmarks with \fBcolored output\fR:
 .PP
 .EX
 .IP
 .B $ buku --colors oKlxm -p
 .EE
 .PP
+.IP 39. 4
+Add a bookmark after following all permanent redirects, but only if the server doesn't respond with an error (and there's no network failure)
+.PP
+.EX
+.IP
+.B buku --add http://wikipedia.net --url-redirect --del-error
+.br
+2. Wikipedia
+.br
+   > https://www.wikipedia.org/
+.br
+   + Wikipedia is a free online encyclopedia, created and edited by volunteers around the world and hosted by the Wikimedia Foundation.
+.EE
+.PP
+.IP 40. 4
+Add a bookmark with tag 'http redirect' if the server responds with a permanent redirect, or tag shaped like 'http 404' on an error response:
+.PP
+.EX
+.IP
+.B buku --add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error 'http {}'
+.br
+[ERROR] [404] Not Found
+.br
+3. Not Found
+.br
+   > http://wikipedia.net/notfound
+.br
+   # http 404,http redirect
+.EE
+.PP
+.IP 41. 4
+Update all bookmarks matching the search by updating the URL if the server responds with a permanent redirect, deleting the bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500, or adding a tag shaped like 'http:{}' in case of any other HTTP error; then export those affected by such changes into an HTML file, marking deleted records as well as old URLs for those replaced by redirect.
+.PP
+.EX
+.IP
+.B buku -S ://wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on --export backup.html
+.EE
+.PP
 
 .SH AUTHOR
 Arun Prakash Jana <engineerarun@gmail.com>
 .SH HOME
 .I https://github.com/jarun/buku
 .SH WIKI
 .I https://github.com/jarun/buku/wiki
 .SH REPORTING BUGS
 .I https://github.com/jarun/buku/issues
 .SH LICENSE
-Copyright \(co 2015-2022 Arun Prakash Jana <engineerarun@gmail.com>.
+Copyright \(co 2015-2024 Arun Prakash Jana <engineerarun@gmail.com>.
 .PP
 License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
 .br
 This is free software: you are free to change and redistribute it. There is NO WARRANTY, to the extent permitted by law.
```

### Comparing `buku-4.7.1/buku.egg-info/PKG-INFO` & `buku-4.9/buku.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,95 @@
 Metadata-Version: 2.1
 Name: buku
-Version: 4.7.1
+Version: 4.9
 Summary: Bookmark manager like a text-based mini-web.
 Home-page: https://github.com/jarun/buku
 Author: Arun Prakash Jana
 Author-email: engineerarun@gmail.com
 License: GPLv3
+Project-URL: Documentation, https://buku.readthedocs.io/en/latest
+Project-URL: Funding, https://github.com/sponsors/jarun
+Project-URL: Source, https://github.com/jarun/buku
+Project-URL: Tracker, https://github.com/jarun/buku/issues
 Keywords: cli bookmarks tag utility
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: ca-certificates
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: certifi
+Requires-Dist: cryptography>=1.2.3
+Requires-Dist: html5lib>=1.0.1
+Requires-Dist: urllib3<2,>=1.23
+Requires-Dist: pyreadline3; sys_platform == "win32"
+Requires-Dist: colorama>=0.4.6; sys_platform == "win32"
 Provides-Extra: tests
+Requires-Dist: attrs>=17.4.0; extra == "tests"
+Requires-Dist: beautifulsoup4>=4.6.0; extra == "tests"
+Requires-Dist: Click>=7.0; extra == "tests"
+Requires-Dist: flake8>=3.4.1; extra == "tests"
+Requires-Dist: hypothesis>=6.0.0; extra == "tests"
+Requires-Dist: mypy-extensions==0.4.1; extra == "tests"
+Requires-Dist: py>=1.5.0; extra == "tests"
+Requires-Dist: pylint>=1.7.2; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-recording>=0.12.1; extra == "tests"
+Requires-Dist: pytest>=6.2.1; extra == "tests"
+Requires-Dist: PyYAML>=4.2b1; extra == "tests"
+Requires-Dist: setuptools>=41.0.1; extra == "tests"
+Requires-Dist: vcrpy>=1.13.0; extra == "tests"
+Requires-Dist: lxml; extra == "tests"
+Requires-Dist: flask_babel; extra == "tests"
+Requires-Dist: arrow>=1.2.2; extra == "tests"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "tests"
+Requires-Dist: Flask-API>=3.0.post1; extra == "tests"
+Requires-Dist: Flask-Bootstrap>=3.3.7.1; extra == "tests"
+Requires-Dist: flask-paginate>=2022.1.8; extra == "tests"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "tests"
+Requires-Dist: Flask<2.3,>=2.2.2; extra == "tests"
+Requires-Dist: werkzeug<2.4; extra == "tests"
 Provides-Extra: server
+Requires-Dist: arrow>=1.2.2; extra == "server"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "server"
+Requires-Dist: Flask-API>=3.0.post1; extra == "server"
+Requires-Dist: Flask-Bootstrap>=3.3.7.1; extra == "server"
+Requires-Dist: flask-paginate>=2022.1.8; extra == "server"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "server"
+Requires-Dist: Flask<2.3,>=2.2.2; extra == "server"
+Requires-Dist: werkzeug<2.4; extra == "server"
 Provides-Extra: docs
+Requires-Dist: myst-parser>=0.17.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Provides-Extra: packaging
-License-File: LICENSE
+Requires-Dist: twine>=1.11.0; extra == "packaging"
 
 <h1 align="center">buku</h1>
 
 <p align="center">
 <a href="https://github.com/jarun/buku/releases/latest"><img src="https://img.shields.io/github/release/jarun/buku.svg?maxAge=600" alt="Latest release" /></a>
 <a href="https://repology.org/project/buku/versions"><img src="https://repology.org/badge/tiny-repos/buku.svg?header=repos" alt="Availability"></a>
 <a href="https://pypi.org/project/buku/"><img src="https://img.shields.io/pypi/v/buku.svg?maxAge=600" alt="PyPI" /></a>
 <a href="https://circleci.com/gh/jarun/workflows/buku"><img src="https://img.shields.io/circleci/project/github/jarun/buku.svg" alt="Build Status" /></a>
-<a href="http://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
+<a href="https://buku.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/buku/badge/?version=latest" alt="Docs Status" /></a>
 <a href="https://en.wikipedia.org/wiki/Privacy-invasive_software"><img src="https://img.shields.io/badge/privacy-✓-crimson" alt="Privacy Awareness" /></a>
 <a href="https://github.com/jarun/buku/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-GPLv3-yellowgreen.svg?maxAge=2592000" alt="License" /></a>
 </p>
 
 <p align="center">
 <a href="https://asciinema.org/a/137065"><img src="https://asciinema.org/a/137065.svg" alt="buku in action!" width="734"/></a>
 </p>
@@ -55,15 +102,15 @@
 
 For those who prefer the GUI, [bukuserver](https://github.com/jarun/buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local web host server.
 
 When I started writing it, I couldn't find a flexible command-line solution with a private, portable, merge-able database along with seamless GUI integration. Hence, `buku`.
 
 `buku` can import bookmarks from browser(s) or fetch the title, tags and description of a URL from the web. Use your favourite editor to add, compose and update bookmarks. Search bookmarks instantly with multiple search options, including regex and a deep scan mode (handy with URLs).
 
-It can look up broken links on Wayback Machine. There's an Easter Egg to revisit random bookmarks.
+It can look up broken links on the Wayback Machine. There's an Easter Egg to revisit random bookmarks.
 
 There's no tracking, hidden history, obsolete records, usage analytics or homing.
 
 To get started right away, jump to the [Quickstart](#quickstart) section. `buku` has one of the best documentation around. The man page comes with examples. For internal details, please refer to the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 
 `buku` is a library too! There are several related projects, including a browser plug-in.
 
@@ -91,33 +138,35 @@
 - [In the Press](#in-the-press)
 
 ### Features
 
 - Store bookmarks with auto-fetched title, tags and description
 - Auto-import from Firefox, Google Chrome, Chromium and MS Edge
 - Open bookmarks and search results in browser
-- Shorten, expand URLs, browse cached page from Wayback Machine
+- Shorten, expand URLs
+- Browse cached page from the Wayback Machine
 - Text editor integration
 - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...)
 - Continuous search with on the fly mode switch
 - Portable, merge-able database to sync between systems
 - Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile
 - Smart tag management using redirection (>>, >, <<)
-- Multi-threaded full DB refresh, manual encryption support
+- Multi-threaded full DB refresh
+- Manual encryption support
 - Shell completion scripts, man page with examples
 - Privacy-aware (no unconfirmed user data collection)
 
 ### Installation
 
 #### Dependencies
 
 | Feature | Dependency |
 | --- | --- |
-| Lang, SQLite | Python 3.6+ |
+| Lang, SQLite | Python 3.8+ |
 | HTTPS | certifi, urllib3 |
 | Encryption | cryptography |
 | HTML | beautifulsoup4, html5lib |
 
 To copy URL to clipboard `buku` uses `xsel` (or `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default installed) on Windows, `termux-clipboard` on Termux (terminal emulation for Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-paste buffers are recognized.
 
 #### From a package manager
@@ -240,25 +289,26 @@
       -x, --exclude [...]  omit records matching specified keywords
 
 ENCRYPTION OPTIONS:
       -l, --lock [N]       encrypt DB in N (default 8) # iterations
       -k, --unlock [N]     decrypt DB in N (default 8) # iterations
 
 POWER TOYS:
-      --ai                 auto-import (Firefox/Chrome/Chromium/Edge)
+      --ai                 auto-import bookmarks from web browsers
+                           Firefox, Chrome, Chromium, Vivaldi, Edge
       -e, --export file    export bookmarks to Firefox format HTML
                            export XBEL, if file ends with '.xbel'
                            export Markdown, if file ends with '.md'
                            format: [title](url) <!-- TAGS -->
                            export Orgfile, if file ends with '.org'
                            format: *[[url][title]] :tags:
                            export buku DB, if file ends with '.db'
                            combines with search results, if opted
-      -i, --import file    import bookmarks based on file extension
-                           supports 'html', 'xbel', 'json', 'md', 'org', 'db'
+      -i, --import file    import bookmarks from file
+                           supports .html .xbel .json .md .org .db
       -p, --print [...]    show record details by indices, ranges
                            print all bookmarks, if no arguments
                            -n shows the last n results (like tail)
       -f, --format N       limit fields in -p or JSON search output
                            N=1: URL; N=2: URL, tag; N=3: title;
                            N=4: URL, title, tag; N=5: title, tag;
                            N0 (10, 20, 30, 40, 50) omits DB index
@@ -270,17 +320,34 @@
       -n, --count N        show N results per page (default 10)
       --np                 do not show the subprompt, run and exit
       -o, --open [...]     browse bookmarks by indices and ranges
                            open a random bookmark, if no arguments
       --oa                 browse all search results immediately
       --replace old new    replace old tag with new tag everywhere
                            delete old tag, if new tag not specified
+      --url-redirect       when fetching an URL, use the resulting
+                           URL from following *permanent* redirects
+                           (when combined with --export, the old URL
+                           is included as additional metadata)
+      --tag-redirect [tag] when fetching an URL that causes permanent
+                           redirect, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --tag-error [tag]    when fetching an URL that causes an HTTP
+                           error, add a tag in specified pattern
+                           (using 'http:{}' if not specified)
+      --del-error [...]    when fetching an URL causes any (given)
+                           HTTP error, delete/do not add it
+      --export-on [...]    export records affected by the above
+                           options, including removed info
+                           (requires --update and --export; specific
+                           HTTP response filter can be provided)
       --shorten index|URL  fetch shortened url from tny.im service
       --expand index|URL   expand a tny.im shortened url
       --cached index|URL   browse a cached page from Wayback Machine
+      --offline            add a bookmark without connecting to web
       --suggest            show similar tags when adding bookmarks
       --tacit              reduce verbosity, skip some confirmations
       --nostdin            do not wait for input (must be first arg)
       --threads N          max network connections in full refresh
                            default N=4, min N=1, max N=10
       -V                   check latest upstream version available
       -g, --debug          show debug information and verbose logs
@@ -353,162 +420,192 @@
 
 1. **Edit and add** a bookmark from editor:
 
        $ buku -w
        $ buku -w 'gedit -w'
        $ buku -w 'macvim -f' -a https://ddg.gg search engine, privacy
     The first command picks editor from the environment variable `EDITOR`. The second command opens gedit in blocking mode. The third command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
+2. **Add** a simple bookmark:
+
+       $ buku --nostdin -a https://github.com/
+       2648. GitHub: Let’s build from here · GitHub
+       > https://github.com/
+       + GitHub is where over 94 million developers shape the future of software, together. Contribute to the open source community, manage your Git repositories, review code like a pro, track bugs
+        and features, power your CI/CD and DevOps workflows, and secure code before you commit it.
+
+       $ buku --nostdin -a https://github.com/
+       [ERROR] URL [https://github.com/] already exists at index 2648
+
+      `>`: URL, `+`: comment, `#`: tags
+
+      Title, description and tags will be fetched from site. Buku only stores unique URLs and will raise error if the URL already present in the database:
+3. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment** `Search engine with perks`, **fetch page title** from the web:
 
        $ buku -a https://ddg.gg search engine, privacy -c Search engine with perks
        336. DuckDuckGo
        > https://ddg.gg
        + Alternative search engine with perks
        # privacy,search engine
-    where, >: URL, +: comment, #: tags
-3. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
+    where, `>`: URL, `+`: comment, `#`: tags
+4. **Add** a bookmark with tags `search engine` & `privacy` and **immutable custom title** `DDG`:
 
        $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --immutable 1
        336. DDG (L)
        > https://ddg.gg
        # privacy,search engine
     Note that URL must precede tags.
-4. **Add** a bookmark **without a title** (works for update too):
+5. **Add** a bookmark **without a title** (works for update too):
 
        $ buku -a https://ddg.gg search engine, privacy --title
-5. **Edit and update** a bookmark from editor:
+6. **Edit and update** a bookmark from editor:
 
        $ buku -w 15012014
     This will open the existing bookmark's details in the editor for modifications. Environment variable `EDITOR` must be set.
-6. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
+7. **Update** existing bookmark at index 15012014 with new URL, tags and comments, fetch title from the web:
 
        $ buku -u 15012014 --url http://ddg.gg/ --tag web search, utilities -c Private search engine
-7. **Fetch and update only title** for bookmark at 15012014:
+8. **Fetch and update only title** for bookmark at 15012014:
 
        $ buku -u 15012014
-8. **Update only comment** for bookmark at 15012014:
+9. **Update only comment** for bookmark at 15012014:
 
        $ buku -u 15012014 -c this is a new comment
     Applies to --url, --title and --tag too.
-9. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
+10. **Export** bookmarks tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database:
 
        $ buku -e bookmarks.html --stag tag 1, tag 2
        $ buku -e bookmarks.xbel --stag tag 1, tag 2
        $ buku -e bookmarks.md --stag tag 1, tag 2
        $ buku -e bookmarks.org --stag tag 1, tag 2
        $ buku -e bookmarks.db --stag tag 1, tag 2
     All bookmarks are exported if search is not opted.
-10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
+11. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile:
 
         $ buku -i bookmarks.html
         $ buku -i bookmarks.xbel
         $ buku -i bookmarks.md
         $ buku -i bookmarks.org
         $ buku -i bookmarks.db
-11. **Delete only comment** for bookmark at 15012014:
+12. **Delete only comment** for bookmark at 15012014:
 
         $ buku -u 15012014 -c
     Applies to --title and --tag too. URL cannot be deleted without deleting the bookmark.
-12. **Update** or refresh **full DB** with page titles from the web:
+13. **Update** or refresh **full DB** with page titles from the web:
 
         $ buku -u
         $ buku -u --tacit (show only failures and exceptions)
     This operation can update the title or description fields of non-immutable bookmarks by parsing the fetched page. Fields are updated only if the fetched fields are non-empty. Tags remain untouched.
-13. **Delete** bookmark at index 15012014:
+14. **Delete** bookmark at index 15012014:
 
         $ buku -d 15012014
         Index 15012020 moved to 15012014
     The last index is moved to the deleted index to keep the DB compact. Add `--tacit` to delete without confirmation.
-14. **Delete all** bookmarks:
+15. **Delete all** bookmarks:
 
         $ buku -d
-15. **Delete** a **range or list** of bookmarks:
+16. **Delete** a **range or list** of bookmarks:
 
         $ buku -d 100-200
         $ buku -d 100 15 200
-16. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
+17. **Search** bookmarks for **ANY** of the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku kernel debugging
         $ buku -s kernel debugging
-17. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
+18. **Search** bookmarks with **ALL** the keywords `kernel` and `debugging` in URL, title or tags:
 
         $ buku -S kernel debugging
-18. **Search** bookmarks **tagged** `general kernel concepts`:
+19. **Search** bookmarks **tagged** `general kernel concepts`:
 
         $ buku --stag general kernel concepts
-19. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+20. **Search** for bookmarks matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel, debugging, general kernel concepts
-20. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
+21. **Search** for bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel concepts`:
 
         $ buku --stag kernel + debugging + general kernel concepts
-21. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+22. **Search** for bookmarks matching any of the keywords `hello` or `world`, excluding the keywords `real` and `life`, matching both the tags `kernel` and `debugging`, but **excluding** the tags `general kernel concepts` and `books`:
 
         $ buku hello world --exclude real life --stag 'kernel + debugging - general kernel concepts, books'
-22. List **all unique tags** alphabetically:
+23. List **all unique tags** alphabetically:
 
         $ buku --stag
-23. Run a **search and update** the results:
+24. Run a **search and update** the results:
 
         $ buku -s kernel debugging -u --tag + linux kernel
-24. Run a **search and delete** the results:
+25. Run a **search and delete** the results:
 
         $ buku -s kernel debugging -d
-25. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
+26. **Encrypt or decrypt** DB with **custom number of iterations** (15) to generate key:
 
         $ buku -l 15
         $ buku -k 15
     The same number of iterations must be specified for one lock & unlock instance. Default is 8, if omitted.
-26. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
+27. **Show details** of bookmarks at index 15012014 and ranges 20-30, 40-50:
 
         $ buku -p 20-30 15012014 40-50
-27. Show details of the **last 10 bookmarks**:
+28. Show details of the **last 10 bookmarks**:
 
         $ buku -p -10
-28. **Show all** bookmarks with real index from database:
+29. **Show all** bookmarks with real index from database:
 
         $ buku -p
         $ buku -p | more
-29. **Replace tag** 'old tag' with 'new tag':
+30. **Replace tag** 'old tag' with 'new tag':
 
         $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB:
+31. **Delete tag** 'old tag' from DB:
 
         $ buku --replace 'old tag'
-31. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
+32. **Append (or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at index 15012014:
 
         $ buku -u 15012014 --tag + tag 1, tag 2
         $ buku -u 15012014 --tag - tag 1, tag 2
-32. **Open URL** at index 15012014 in browser:
+33. **Open URL** at index 15012014 in browser:
 
         $ buku -o 15012014
-33. List bookmarks with **no title or tags** for bookkeeping:
+34. List bookmarks with **no title or tags** for bookkeeping:
 
         $ buku -S blank
-34. List bookmarks with **immutable title**:
+35. List bookmarks with **immutable title**:
 
         $ buku -S immutable
-35. **Shorten URL** www.google.com and the URL at index 20:
+36. **Shorten URL** www.google.com and the URL at index 20:
 
         $ buku --shorten www.google.com
         $ buku --shorten 20
-36. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
+37. **Append, remove tags at prompt** (taglist index to the left, bookmark index to the right):
 
         // append tags at taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 >> 5 3-2
         // set tags at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 > 5 3-2
         // remove all tags from bookmarks at indices 5 and 2-3
         buku (? for help) g > 5 3-2
         // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at indices 5 and 2-3
         buku (? for help) g 4 9-6 << 5 3-2
-37. List bookmarks with **colored output**:
+38. List bookmarks with **colored output**:
 
         $ buku --colors oKlxm -p
-38. More **help**:
+39. Add a bookmark after following all permanent redirects, but only if the server doesn't respond with an error (and there's no network failure)
+
+        $ buku --add http://wikipedia.net --url-redirect --del-error
+        2. Wikipedia
+           > https://www.wikipedia.org/
+           + Wikipedia is a free online encyclopedia, created and edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a permanent redirect, or tag shaped like `http 404` on an error response:
+
+        $ buku --add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error 'http {}'
+        [ERROR] [404] Not Found
+        3. Not Found
+           > http://wikipedia.net/notfound
+           # http 404,http redirect
+41. Update all bookmarks matching the search by updating the URL if the server responds with a permanent redirect, deleting the bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500, or adding a tag shaped like `http:{}` in case of any other HTTP error; then export those affected by such changes into an HTML file, marking deleted records as well as old URLs for those replaced by redirect.
+
+        $ buku -S ://wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on --export backup.html
+42. More **help**:
 
         $ buku -h
         $ man buku
 
 ### Automation
 
 Interactive workflows can be automated using expect. Issue [#368](https://github.com/jarun/buku/issues/368) has a working example on automating auto-import.
@@ -518,38 +615,40 @@
 #### Editor integration
 
 You may encounter issues with GUI editors which maintain only one instance by default and return immediately from other instances. Use the appropriate editor option to block the caller when a new document is opened. See issue [#210](https://github.com/jarun/buku/issues/210) for gedit.
 
 ### Collaborators
 
 - [Arun Prakash Jana](https://github.com/jarun)
+- [Alexey Gulenko](https://github.com/LeXofLeviafan)
 - [Rachmadani Haryono](https://github.com/rachmadaniHaryono)
 - [Johnathan Jenkins](https://github.com/shaggytwodope)
 - [SZ Lin](https://github.com/szlin)
 
-Copyright © 2015-2022 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
+Copyright © 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 <br>
 <p><a href="https://gitter.im/jarun/buku"><img src="https://img.shields.io/gitter/room/jarun/buku.svg?maxAge=2592000" alt="gitter chat" /></a></p>
 
 ### Contributions
 
 Missing a feature? There's a rolling [ToDo List](https://github.com/jarun/buku/issues/484) with identified tasks. Contributions are welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/PR-guidelines).
 
+See also our documentation here <a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
+
 ### Related projects
 
 - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for browser integration
 - [oil](https://github.com/AndreiUlmeyda/oil), search-as-you-type cli front-end
 - [buku_run](https://github.com/carnager/buku_run), rofi front-end
 - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku import utility
 - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper
 - [poku](https://github.com/shanedabes/poku), sync between Pocket and buku
 - [Ebuku](https://github.com/flexibeast/ebuku), Emacs interface to buku
 - [diigoku](https://github.com/dppdppd/diigoku), buku importer for Diigo
 
-<a href="http://buku.readthedocs.io/en/stable/?badge=stable"><img src="https://img.shields.io/badge/docs-stable-brightgreen.svg?maxAge=2592000" alt="Stable Docs" /></a>
 
 ### Videos
 
 - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/embed/9HzEHrUBQXE)
 - [Buku is a great open-source bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8)
 
 ### In the Press
@@ -559,9 +658,7 @@
 - [It's F.O.S.S.](https://itsfoss.com/buku-command-line-bookmark-manager-linux/)
 - [LinOxide](https://linoxide.com/linux-how-to/buku-browser-bookmarks-linux/)
 - [LinuxUser Magazine 01/2017 Issue](http://www.linux-community.de/LU/2017/01/Das-Beste-aus-zwei-Welten)
 - [Make Tech Easier](https://www.maketecheasier.com/manage-browser-bookmarks-ubuntu-command-line/)
 - [One Thing Well](http://onethingwell.org/post/144952807044/buku)
 - [Open Source For You](https://opensourceforu.com/2018/05/buku-a-bookmark-manager-in-the-command-line/)
 - [ulno.net](https://ulno.net/blog/2017-07-19/of-bookmarks-tags-and-browsers/)
-
-
```

#### html2text {}

```diff
@@ -1,39 +1,70 @@
-Metadata-Version: 2.1 Name: buku Version: 4.7.1 Summary: Bookmark manager like
-a text-based mini-web. Home-page: https://github.com/jarun/buku Author: Arun
-Prakash Jana Author-email: engineerarun@gmail.com License: GPLv3 Keywords: cli
-bookmarks tag utility Platform: any Classifier: Development Status :: 5 -
+Metadata-Version: 2.1 Name: buku Version: 4.9 Summary: Bookmark manager like a
+text-based mini-web. Home-page: https://github.com/jarun/buku Author: Arun
+Prakash Jana Author-email: engineerarun@gmail.com License: GPLv3 Project-URL:
+Documentation, https://buku.readthedocs.io/en/latest Project-URL: Funding,
+https://github.com/sponsors/jarun Project-URL: Source, https://github.com/
+jarun/buku Project-URL: Tracker, https://github.com/jarun/buku/issues Keywords:
+cli bookmarks tag utility Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Internet :: WWW/HTTP
-:: Indexing/Search Classifier: Topic :: Utilities Requires-Python: >=3.6
-Description-Content-Type: text/markdown Provides-Extra: ca-certificates
-Provides-Extra: tests Provides-Extra: server Provides-Extra: docs Provides-
-Extra: packaging License-File: LICENSE
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: certifi Requires-Dist: cryptography>=1.2.3 Requires-Dist:
+html5lib>=1.0.1 Requires-Dist: urllib3<2,>=1.23 Requires-Dist: pyreadline3;
+sys_platform == "win32" Requires-Dist: colorama>=0.4.6; sys_platform == "win32"
+Provides-Extra: tests Requires-Dist: attrs>=17.4.0; extra == "tests" Requires-
+Dist: beautifulsoup4>=4.6.0; extra == "tests" Requires-Dist: Click>=7.0; extra
+== "tests" Requires-Dist: flake8>=3.4.1; extra == "tests" Requires-Dist:
+hypothesis>=6.0.0; extra == "tests" Requires-Dist: mypy-extensions==0.4.1;
+extra == "tests" Requires-Dist: py>=1.5.0; extra == "tests" Requires-Dist:
+pylint>=1.7.2; extra == "tests" Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-recording>=0.12.1; extra == "tests" Requires-Dist:
+pytest>=6.2.1; extra == "tests" Requires-Dist: PyYAML>=4.2b1; extra == "tests"
+Requires-Dist: setuptools>=41.0.1; extra == "tests" Requires-Dist:
+vcrpy>=1.13.0; extra == "tests" Requires-Dist: lxml; extra == "tests" Requires-
+Dist: flask_babel; extra == "tests" Requires-Dist: arrow>=1.2.2; extra ==
+"tests" Requires-Dist: Flask-Admin>=1.6.1; extra == "tests" Requires-Dist:
+Flask-API>=3.0.post1; extra == "tests" Requires-Dist: Flask-Bootstrap>=3.3.7.1;
+extra == "tests" Requires-Dist: flask-paginate>=2022.1.8; extra == "tests"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "tests" Requires-Dist:
+Flask<2.3,>=2.2.2; extra == "tests" Requires-Dist: werkzeug<2.4; extra ==
+"tests" Provides-Extra: server Requires-Dist: arrow>=1.2.2; extra == "server"
+Requires-Dist: Flask-Admin>=1.6.1; extra == "server" Requires-Dist: Flask-
+API>=3.0.post1; extra == "server" Requires-Dist: Flask-Bootstrap>=3.3.7.1;
+extra == "server" Requires-Dist: flask-paginate>=2022.1.8; extra == "server"
+Requires-Dist: Flask-WTF>=1.0.1; extra == "server" Requires-Dist:
+Flask<2.3,>=2.2.2; extra == "server" Requires-Dist: werkzeug<2.4; extra ==
+"server" Provides-Extra: docs Requires-Dist: myst-parser>=0.17.0; extra ==
+"docs" Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "docs" Requires-Dist:
+sphinx-autobuild>=2021.3.14; extra == "docs" Provides-Extra: packaging
+Requires-Dist: twine>=1.11.0; extra == "packaging"
                               ************ bbuukkuu ************
     _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_A_v_a_i_l_a_b_i_l_i_t_y_]_[_P_y_P_I_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_s_ _S_t_a_t_u_s_]_[_P_r_i_v_a_c_y
                               _A_w_a_r_e_n_e_s_s_]_[_L_i_c_e_n_s_e_]
                                _[_b_u_k_u_ _i_n_ _a_c_t_i_o_n_!_]
                                 buku in action!
 ### Introduction `buku` is a powerful bookmark manager and a personal textual
 mini-web. For those who prefer the GUI, [bukuserver](https://github.com/jarun/
 buku/tree/master/bukuserver#readme) exposes a browsable front-end on a local
 web host server. When I started writing it, I couldn't find a flexible command-
 line solution with a private, portable, merge-able database along with seamless
 GUI integration. Hence, `buku`. `buku` can import bookmarks from browser(s) or
 fetch the title, tags and description of a URL from the web. Use your favourite
 editor to add, compose and update bookmarks. Search bookmarks instantly with
 multiple search options, including regex and a deep scan mode (handy with
-URLs). It can look up broken links on Wayback Machine. There's an Easter Egg to
-revisit random bookmarks. There's no tracking, hidden history, obsolete
+URLs). It can look up broken links on the Wayback Machine. There's an Easter
+Egg to revisit random bookmarks. There's no tracking, hidden history, obsolete
 records, usage analytics or homing. To get started right away, jump to the
 [Quickstart](#quickstart) section. `buku` has one of the best documentation
 around. The man page comes with examples. For internal details, please refer to
 the [operational notes](https://github.com/jarun/buku/wiki/Operational-notes).
 `buku` is a library too! There are several related projects, including a
 browser plug-in. ### Table of Contents - [Features](#features) - [Installation]
 (#installation) - [Dependencies](#dependencies) - [From a package manager]
@@ -43,24 +74,24 @@
 (#command-line-options) - [Colors](#colors) - [Quickstart](#quickstart) -
 [Examples](#examples) - [Automation](#automation) - [Troubleshooting]
 (#troubleshooting) - [Editor integration](#editor-integration) -
 [Collaborators](#collaborators) - [Contributions](#contributions) - [Related
 projects](#related-projects) - [In the Press](#in-the-press) ### Features -
 Store bookmarks with auto-fetched title, tags and description - Auto-import
 from Firefox, Google Chrome, Chromium and MS Edge - Open bookmarks and search
-results in browser - Shorten, expand URLs, browse cached page from Wayback
+results in browser - Shorten, expand URLs - Browse cached page from the Wayback
 Machine - Text editor integration - Lightweight, clean interface, custom colors
 - Powerful search options (regex, substring...) - Continuous search with on the
 fly mode switch - Portable, merge-able database to sync between systems -
 Import/export bookmarks from/to HTML, XBEL, Markdown or Orgfile - Smart tag
-management using redirection (>>, >, <<) - Multi-threaded full DB refresh,
-manual encryption support - Shell completion scripts, man page with examples -
+management using redirection (>>, >, <<) - Multi-threaded full DB refresh -
+Manual encryption support - Shell completion scripts, man page with examples -
 Privacy-aware (no unconfirmed user data collection) ### Installation ####
 Dependencies | Feature | Dependency | | --- | --- | | Lang, SQLite | Python
-3.6+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
+3.8+ | | HTTPS | certifi, urllib3 | | Encryption | cryptography | | HTML |
 beautifulsoup4, html5lib | To copy URL to clipboard `buku` uses `xsel` (or
 `xclip`) on Linux, `pbcopy` (default installed) on OS X, `clip` (default
 installed) on Windows, `termux-clipboard` on Termux (terminal emulation for
 Android), `wl-copy` on Wayland. If X11 is missing, GNU Screen or tmux copy-
 paste buffers are recognized. #### From a package manager To install buku with
 all its dependencies from PyPI, run: # pip3 install buku You can also install
 `buku` from your package manager. If the version available is dated try an
@@ -111,54 +142,64 @@
 tag "immutable": entries with locked title --deep match substrings ('pen'
 matches 'opens') -r, --sreg expr run a regex search -t, --stag [tag [,|+] ...]
 [- tag, ...] search bookmarks by tags use ',' to find entries matching ANY tag
 use '+' to find entries matching ALL tags excludes entries with tags after ' -
 ' list all tags, if no search keywords -x, --exclude [...] omit records
 matching specified keywords ENCRYPTION OPTIONS: -l, --lock [N] encrypt DB in N
 (default 8) # iterations -k, --unlock [N] decrypt DB in N (default 8) #
-iterations POWER TOYS: --ai auto-import (Firefox/Chrome/Chromium/Edge) -e, --
-export file export bookmarks to Firefox format HTML export XBEL, if file ends
-with '.xbel' export Markdown, if file ends with '.md' format: [title](url)
-export Orgfile, if file ends with '.org' format: *[[url][title]] :tags: export
-buku DB, if file ends with '.db' combines with search results, if opted -i, --
-import file import bookmarks based on file extension supports 'html', 'xbel',
-'json', 'md', 'org', 'db' -p, --print [...] show record details by indices,
-ranges print all bookmarks, if no arguments -n shows the last n results (like
-tail) -f, --format N limit fields in -p or JSON search output N=1: URL; N=2:
-URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0 (10, 20, 30,
-40, 50) omits DB index -j, --json [file] JSON formatted output for -p and
-search. prints to stdout if argument missing. otherwise writes to given file --
-colors COLORS set output colors in five-letter string --nc disable color output
--n, --count N show N results per page (default 10) --np do not show the
+iterations POWER TOYS: --ai auto-import bookmarks from web browsers Firefox,
+Chrome, Chromium, Vivaldi, Edge -e, --export file export bookmarks to Firefox
+format HTML export XBEL, if file ends with '.xbel' export Markdown, if file
+ends with '.md' format: [title](url) export Orgfile, if file ends with '.org'
+format: *[[url][title]] :tags: export buku DB, if file ends with '.db' combines
+with search results, if opted -i, --import file import bookmarks from file
+supports .html .xbel .json .md .org .db -p, --print [...] show record details
+by indices, ranges print all bookmarks, if no arguments -n shows the last n
+results (like tail) -f, --format N limit fields in -p or JSON search output
+N=1: URL; N=2: URL, tag; N=3: title; N=4: URL, title, tag; N=5: title, tag; N0
+(10, 20, 30, 40, 50) omits DB index -j, --json [file] JSON formatted output for
+-p and search. prints to stdout if argument missing. otherwise writes to given
+file --colors COLORS set output colors in five-letter string --nc disable color
+output -n, --count N show N results per page (default 10) --np do not show the
 subprompt, run and exit -o, --open [...] browse bookmarks by indices and ranges
 open a random bookmark, if no arguments --oa browse all search results
 immediately --replace old new replace old tag with new tag everywhere delete
-old tag, if new tag not specified --shorten index|URL fetch shortened url from
-tny.im service --expand index|URL expand a tny.im shortened url --cached
-index|URL browse a cached page from Wayback Machine --suggest show similar tags
-when adding bookmarks --tacit reduce verbosity, skip some confirmations --
-nostdin do not wait for input (must be first arg) --threads N max network
-connections in full refresh default N=4, min N=1, max N=10 -V check latest
-upstream version available -g, --debug show debug information and verbose logs
-SYMBOLS: > url + comment # tags PROMPT KEYS: 1-N browse search result indices
-and/or ranges O [id|range [...]] open search results/indices in GUI browser
-toggle try GUI browser if no arguments a open all results in browser s keyword
-[...] search for records with ANY keyword S keyword [...] search for records
-with ALL keywords d match substrings ('pen' matches 'opened') r expression run
-a regex search t [tag, ...] search by tags; show taglist, if no args g taglist
-id|range [...] [>>|>|<<] [record id|range ...] append, set, remove (all or
-specific) tags search by taglist id(s) if records are omitted n show next page
-of search results o id|range [...] browse bookmarks by indices and/or ranges p
-id|range [...] print bookmarks by indices and/or ranges w [editor|id] edit and
-add or update a bookmark c id copy URL at search result index to clipboard ?
-show this help q, ^D, double Enter exit buku ``` #### Colors `buku` supports
-custom colors. Visit the wiki page on how to [customize colors](https://
-github.com/jarun/buku/wiki/Customize-colors) for more details. ### Quickstart
-1. Export `VISUAL` or `EDITOR` to point to your favourite editor. Note that
-`VISUAL` takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
+old tag, if new tag not specified --url-redirect when fetching an URL, use the
+resulting URL from following *permanent* redirects (when combined with --
+export, the old URL is included as additional metadata) --tag-redirect [tag]
+when fetching an URL that causes permanent redirect, add a tag in specified
+pattern (using 'http:{}' if not specified) --tag-error [tag] when fetching an
+URL that causes an HTTP error, add a tag in specified pattern (using 'http:{}'
+if not specified) --del-error [...] when fetching an URL causes any (given)
+HTTP error, delete/do not add it --export-on [...] export records affected by
+the above options, including removed info (requires --update and --export;
+specific HTTP response filter can be provided) --shorten index|URL fetch
+shortened url from tny.im service --expand index|URL expand a tny.im shortened
+url --cached index|URL browse a cached page from Wayback Machine --offline add
+a bookmark without connecting to web --suggest show similar tags when adding
+bookmarks --tacit reduce verbosity, skip some confirmations --nostdin do not
+wait for input (must be first arg) --threads N max network connections in full
+refresh default N=4, min N=1, max N=10 -V check latest upstream version
+available -g, --debug show debug information and verbose logs SYMBOLS: > url +
+comment # tags PROMPT KEYS: 1-N browse search result indices and/or ranges O
+[id|range [...]] open search results/indices in GUI browser toggle try GUI
+browser if no arguments a open all results in browser s keyword [...] search
+for records with ANY keyword S keyword [...] search for records with ALL
+keywords d match substrings ('pen' matches 'opened') r expression run a regex
+search t [tag, ...] search by tags; show taglist, if no args g taglist id|range
+[...] [>>|>|<<] [record id|range ...] append, set, remove (all or specific)
+tags search by taglist id(s) if records are omitted n show next page of search
+results o id|range [...] browse bookmarks by indices and/or ranges p id|range
+[...] print bookmarks by indices and/or ranges w [editor|id] edit and add or
+update a bookmark c id copy URL at search result index to clipboard ? show this
+help q, ^D, double Enter exit buku ``` #### Colors `buku` supports custom
+colors. Visit the wiki page on how to [customize colors](https://github.com/
+jarun/buku/wiki/Customize-colors) for more details. ### Quickstart 1. Export
+`VISUAL` or `EDITOR` to point to your favourite editor. Note that `VISUAL`
+takes precedence over `EDITOR`. 2. Create a sweeter shortcut with some
 convenience. alias b='buku --suggest' 3. Auto-import bookmarks from your
 browser(s). Please quit the relevant browsers beforehand to ensure the
 databases are not locked. b --ai 4. Manually add a bookmark (for hands-on). b -
 w 5. List your bookmarks with DB index. b -p 6. For GUI and browser integration
 (or to sync bookmarks with your favourite bookmark management service) refer to
 the wiki page on [System integration](https://github.com/jarun/buku/wiki/
 System-integration). 7. Quick (bash/zsh) commands to fuzzy search with fzf and
@@ -167,120 +208,146 @@
 well: ```sh #!/usr/bin/env sh url=$(buku -p -f4 | fzf -m --reverse --preview
 "buku -p {1}" --preview-window=wrap | cut -f2) if [ -n "$url" ]; then echo
 "$url" | xargs firefox fi ``` ### Examples 1. **Edit and add** a bookmark from
 editor: $ buku -w $ buku -w 'gedit -w' $ buku -w 'macvim -f' -a https://ddg.gg
 search engine, privacy The first command picks editor from the environment
 variable `EDITOR`. The second command opens gedit in blocking mode. The third
 command opens macvim with option -f and the URL and tags populated in template.
-2. **Add** a bookmark with **tags** `search engine` and `privacy`, **comment**
-`Search engine with perks`, **fetch page title** from the web: $ buku -a https:
-//ddg.gg search engine, privacy -c Search engine with perks 336. DuckDuckGo >
-https://ddg.gg + Alternative search engine with perks # privacy,search engine
-where, >: URL, +: comment, #: tags 3. **Add** a bookmark with tags `search
-engine` & `privacy` and **immutable custom title** `DDG`: $ buku -a https://
-ddg.gg search engine, privacy --title 'DDG' --immutable 1 336. DDG (L) > https:
-//ddg.gg # privacy,search engine Note that URL must precede tags. 4. **Add** a
-bookmark **without a title** (works for update too): $ buku -a https://ddg.gg
-search engine, privacy --title 5. **Edit and update** a bookmark from editor: $
-buku -w 15012014 This will open the existing bookmark's details in the editor
-for modifications. Environment variable `EDITOR` must be set. 6. **Update**
-existing bookmark at index 15012014 with new URL, tags and comments, fetch
-title from the web: $ buku -u 15012014 --url http://ddg.gg/ --tag web search,
-utilities -c Private search engine 7. **Fetch and update only title** for
-bookmark at 15012014: $ buku -u 15012014 8. **Update only comment** for
-bookmark at 15012014: $ buku -u 15012014 -c this is a new comment Applies to --
-url, --title and --tag too. 9. **Export** bookmarks tagged `tag 1` or `tag 2`
-to HTML, XBEL, Markdown, Orgfile or a new database: $ buku -e bookmarks.html --
-stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag 1, tag 2 $ buku -
-e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --stag tag 1, tag 2
-$ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are exported if search
-is not opted. 10. **Import** bookmarks from HTML, XBEL, Markdown or Orgfile: $
-buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -i bookmarks.md $ buku -
-i bookmarks.org $ buku -i bookmarks.db 11. **Delete only comment** for bookmark
-at 15012014: $ buku -u 15012014 -c Applies to --title and --tag too. URL cannot
-be deleted without deleting the bookmark. 12. **Update** or refresh **full DB**
-with page titles from the web: $ buku -u $ buku -u --tacit (show only failures
-and exceptions) This operation can update the title or description fields of
-non-immutable bookmarks by parsing the fetched page. Fields are updated only if
-the fetched fields are non-empty. Tags remain untouched. 13. **Delete**
-bookmark at index 15012014: $ buku -d 15012014 Index 15012020 moved to 15012014
-The last index is moved to the deleted index to keep the DB compact. Add `--
-tacit` to delete without confirmation. 14. **Delete all** bookmarks: $ buku -
-d 15. **Delete** a **range or list** of bookmarks: $ buku -d 100-200 $ buku -
-d 100 15 200 16. **Search** bookmarks for **ANY** of the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku kernel debugging $ buku -s kernel
-debugging 17. **Search** bookmarks with **ALL** the keywords `kernel` and
-`debugging` in URL, title or tags: $ buku -S kernel debugging 18. **Search**
-bookmarks **tagged** `general kernel concepts`: $ buku --stag general kernel
-concepts 19. **Search** for bookmarks matching **ANY** of the tags `kernel`,
-`debugging`, `general kernel concepts`: $ buku --stag kernel, debugging,
-general kernel concepts 20. **Search** for bookmarks matching **ALL** of the
-tags `kernel`, `debugging`, `general kernel concepts`: $ buku --stag kernel +
-debugging + general kernel concepts 21. **Search** for bookmarks matching any
-of the keywords `hello` or `world`, excluding the keywords `real` and `life`,
-matching both the tags `kernel` and `debugging`, but **excluding** the tags
-`general kernel concepts` and `books`: $ buku hello world --exclude real life -
--stag 'kernel + debugging - general kernel concepts, books' 22. List **all
-unique tags** alphabetically: $ buku --stag 23. Run a **search and update** the
-results: $ buku -s kernel debugging -u --tag + linux kernel 24. Run a **search
-and delete** the results: $ buku -s kernel debugging -d 25. **Encrypt or
-decrypt** DB with **custom number of iterations** (15) to generate key: $ buku
--l 15 $ buku -k 15 The same number of iterations must be specified for one lock
-& unlock instance. Default is 8, if omitted. 26. **Show details** of bookmarks
-at index 15012014 and ranges 20-30, 40-50: $ buku -p 20-30 15012014 40-50 27.
-Show details of the **last 10 bookmarks**: $ buku -p -10 28. **Show all**
-bookmarks with real index from database: $ buku -p $ buku -p | more 29.
-**Replace tag** 'old tag' with 'new tag': $ buku --replace 'old tag' 'new tag'
-30. **Delete tag** 'old tag' from DB: $ buku --replace 'old tag' 31. **Append
-(or delete) tags** 'tag 1', 'tag 2' to (or from) existing tags of bookmark at
-index 15012014: $ buku -u 15012014 --tag + tag 1, tag 2 $ buku -u 15012014 --
-tag - tag 1, tag 2 32. **Open URL** at index 15012014 in browser: $ buku -
-o 15012014 33. List bookmarks with **no title or tags** for bookkeeping: $ buku
--S blank 34. List bookmarks with **immutable title**: $ buku -S immutable 35.
-**Shorten URL** www.google.com and the URL at index 20: $ buku --shorten
-www.google.com $ buku --shorten 20 36. **Append, remove tags at prompt**
-(taglist index to the left, bookmark index to the right): // append tags at
-taglist indices 4 and 6-9 to existing tags in bookmarks at indices 5 and 2-
-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags at taglist indices 4 and 6-
-9 as tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 > 5 3-2 /
-/ remove all tags from bookmarks at indices 5 and 2-3 buku (? for help) g > 5
-3-2 // remove tags at taglist indices 4 and 6-9 from tags in bookmarks at
-indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 37. List bookmarks with
-**colored output**: $ buku --colors oKlxm -p 38. More **help**: $ buku -h $ man
-buku ### Automation Interactive workflows can be automated using expect. Issue
-[#368](https://github.com/jarun/buku/issues/368) has a working example on
-automating auto-import. ### Troubleshooting #### Editor integration You may
-encounter issues with GUI editors which maintain only one instance by default
-and return immediately from other instances. Use the appropriate editor option
-to block the caller when a new document is opened. See issue [#210](https://
-github.com/jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash
-Jana](https://github.com/jarun) - [Rachmadani Haryono](https://github.com/
-rachmadaniHaryono) - [Johnathan Jenkins](https://github.com/shaggytwodope) -
-[SZ Lin](https://github.com/szlin) Copyright Â© 2015-2022 [Arun Prakash Jana]
-(mailto:engineerarun@gmail.com)
+2. **Add** a simple bookmark: $ buku --nostdin -a https://github.com/ 2648.
+GitHub: Letâs build from here Â· GitHub > https://github.com/ + GitHub is
+where over 94 million developers shape the future of software, together.
+Contribute to the open source community, manage your Git repositories, review
+code like a pro, track bugs and features, power your CI/CD and DevOps
+workflows, and secure code before you commit it. $ buku --nostdin -a https://
+github.com/ [ERROR] URL [https://github.com/] already exists at index 2648 `>`:
+URL, `+`: comment, `#`: tags Title, description and tags will be fetched from
+site. Buku only stores unique URLs and will raise error if the URL already
+present in the database: 3. **Add** a bookmark with **tags** `search engine`
+and `privacy`, **comment** `Search engine with perks`, **fetch page title**
+from the web: $ buku -a https://ddg.gg search engine, privacy -c Search engine
+with perks 336. DuckDuckGo > https://ddg.gg + Alternative search engine with
+perks # privacy,search engine where, `>`: URL, `+`: comment, `#`: tags 4.
+**Add** a bookmark with tags `search engine` & `privacy` and **immutable custom
+title** `DDG`: $ buku -a https://ddg.gg search engine, privacy --title 'DDG' --
+immutable 1 336. DDG (L) > https://ddg.gg # privacy,search engine Note that URL
+must precede tags. 5. **Add** a bookmark **without a title** (works for update
+too): $ buku -a https://ddg.gg search engine, privacy --title 6. **Edit and
+update** a bookmark from editor: $ buku -w 15012014 This will open the existing
+bookmark's details in the editor for modifications. Environment variable
+`EDITOR` must be set. 7. **Update** existing bookmark at index 15012014 with
+new URL, tags and comments, fetch title from the web: $ buku -u 15012014 --url
+http://ddg.gg/ --tag web search, utilities -c Private search engine 8. **Fetch
+and update only title** for bookmark at 15012014: $ buku -u 15012014 9.
+**Update only comment** for bookmark at 15012014: $ buku -u 15012014 -c this is
+a new comment Applies to --url, --title and --tag too. 10. **Export** bookmarks
+tagged `tag 1` or `tag 2` to HTML, XBEL, Markdown, Orgfile or a new database: $
+buku -e bookmarks.html --stag tag 1, tag 2 $ buku -e bookmarks.xbel --stag tag
+1, tag 2 $ buku -e bookmarks.md --stag tag 1, tag 2 $ buku -e bookmarks.org --
+stag tag 1, tag 2 $ buku -e bookmarks.db --stag tag 1, tag 2 All bookmarks are
+exported if search is not opted. 11. **Import** bookmarks from HTML, XBEL,
+Markdown or Orgfile: $ buku -i bookmarks.html $ buku -i bookmarks.xbel $ buku -
+i bookmarks.md $ buku -i bookmarks.org $ buku -i bookmarks.db 12. **Delete only
+comment** for bookmark at 15012014: $ buku -u 15012014 -c Applies to --title
+and --tag too. URL cannot be deleted without deleting the bookmark. 13.
+**Update** or refresh **full DB** with page titles from the web: $ buku -u $
+buku -u --tacit (show only failures and exceptions) This operation can update
+the title or description fields of non-immutable bookmarks by parsing the
+fetched page. Fields are updated only if the fetched fields are non-empty. Tags
+remain untouched. 14. **Delete** bookmark at index 15012014: $ buku -d 15012014
+Index 15012020 moved to 15012014 The last index is moved to the deleted index
+to keep the DB compact. Add `--tacit` to delete without confirmation. 15.
+**Delete all** bookmarks: $ buku -d 16. **Delete** a **range or list** of
+bookmarks: $ buku -d 100-200 $ buku -d 100 15 200 17. **Search** bookmarks for
+**ANY** of the keywords `kernel` and `debugging` in URL, title or tags: $ buku
+kernel debugging $ buku -s kernel debugging 18. **Search** bookmarks with
+**ALL** the keywords `kernel` and `debugging` in URL, title or tags: $ buku -
+S kernel debugging 19. **Search** bookmarks **tagged** `general kernel
+concepts`: $ buku --stag general kernel concepts 20. **Search** for bookmarks
+matching **ANY** of the tags `kernel`, `debugging`, `general kernel concepts`:
+$ buku --stag kernel, debugging, general kernel concepts 21. **Search** for
+bookmarks matching **ALL** of the tags `kernel`, `debugging`, `general kernel
+concepts`: $ buku --stag kernel + debugging + general kernel concepts 22.
+**Search** for bookmarks matching any of the keywords `hello` or `world`,
+excluding the keywords `real` and `life`, matching both the tags `kernel` and
+`debugging`, but **excluding** the tags `general kernel concepts` and `books`:
+$ buku hello world --exclude real life --stag 'kernel + debugging - general
+kernel concepts, books' 23. List **all unique tags** alphabetically: $ buku --
+stag 24. Run a **search and update** the results: $ buku -s kernel debugging -
+u --tag + linux kernel 25. Run a **search and delete** the results: $ buku -
+s kernel debugging -d 26. **Encrypt or decrypt** DB with **custom number of
+iterations** (15) to generate key: $ buku -l 15 $ buku -k 15 The same number of
+iterations must be specified for one lock & unlock instance. Default is 8, if
+omitted. 27. **Show details** of bookmarks at index 15012014 and ranges 20-30,
+40-50: $ buku -p 20-30 15012014 40-50 28. Show details of the **last 10
+bookmarks**: $ buku -p -10 29. **Show all** bookmarks with real index from
+database: $ buku -p $ buku -p | more 30. **Replace tag** 'old tag' with 'new
+tag': $ buku --replace 'old tag' 'new tag' 31. **Delete tag** 'old tag' from
+DB: $ buku --replace 'old tag' 32. **Append (or delete) tags** 'tag 1', 'tag 2'
+to (or from) existing tags of bookmark at index 15012014: $ buku -u 15012014 --
+tag + tag 1, tag 2 $ buku -u 15012014 --tag - tag 1, tag 2 33. **Open URL** at
+index 15012014 in browser: $ buku -o 15012014 34. List bookmarks with **no
+title or tags** for bookkeeping: $ buku -S blank 35. List bookmarks with
+**immutable title**: $ buku -S immutable 36. **Shorten URL** www.google.com and
+the URL at index 20: $ buku --shorten www.google.com $ buku --shorten 20 37.
+**Append, remove tags at prompt** (taglist index to the left, bookmark index to
+the right): // append tags at taglist indices 4 and 6-9 to existing tags in
+bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 >> 5 3-2 // set tags
+at taglist indices 4 and 6-9 as tags in bookmarks at indices 5 and 2-3 buku (?
+for help) g 4 9-6 > 5 3-2 // remove all tags from bookmarks at indices 5 and 2-
+3 buku (? for help) g > 5 3-2 // remove tags at taglist indices 4 and 6-9 from
+tags in bookmarks at indices 5 and 2-3 buku (? for help) g 4 9-6 << 5 3-2 38.
+List bookmarks with **colored output**: $ buku --colors oKlxm -p 39. Add a
+bookmark after following all permanent redirects, but only if the server
+doesn't respond with an error (and there's no network failure) $ buku --add
+http://wikipedia.net --url-redirect --del-error 2. Wikipedia > https://
+www.wikipedia.org/ + Wikipedia is a free online encyclopedia, created and
+edited by volunteers around the world and hosted by the Wikimedia Foundation.
+40. Add a bookmark with tag `http redirect` if the server responds with a
+permanent redirect, or tag shaped like `http 404` on an error response: $ buku
+--add http://wikipedia.net/notfound --tag-redirect 'http redirect' --tag-error
+'http {}' [ERROR] [404] Not Found 3. Not Found > http://wikipedia.net/notfound
+# http 404,http redirect 41. Update all bookmarks matching the search by
+updating the URL if the server responds with a permanent redirect, deleting the
+bookmark if the server responds with HTTP error 400, 401, 402, 403, 404 or 500,
+or adding a tag shaped like `http:{}` in case of any other HTTP error; then
+export those affected by such changes into an HTML file, marking deleted
+records as well as old URLs for those replaced by redirect. $ buku -S ://
+wikipedia.net -u --url-redirect --tag-error --del-error 400-404,500 --export-on
+--export backup.html 42. More **help**: $ buku -h $ man buku ### Automation
+Interactive workflows can be automated using expect. Issue [#368](https://
+github.com/jarun/buku/issues/368) has a working example on automating auto-
+import. ### Troubleshooting #### Editor integration You may encounter issues
+with GUI editors which maintain only one instance by default and return
+immediately from other instances. Use the appropriate editor option to block
+the caller when a new document is opened. See issue [#210](https://github.com/
+jarun/buku/issues/210) for gedit. ### Collaborators - [Arun Prakash Jana]
+(https://github.com/jarun) - [Alexey Gulenko](https://github.com/LeXofLeviafan)
+- [Rachmadani Haryono](https://github.com/rachmadaniHaryono) - [Johnathan
+Jenkins](https://github.com/shaggytwodope) - [SZ Lin](https://github.com/szlin)
+Copyright Â© 2015-2024 [Arun Prakash Jana](mailto:engineerarun@gmail.com)
 _[_g_i_t_t_e_r_ _c_h_a_t_]
 ### Contributions Missing a feature? There's a rolling [ToDo List](https://
 github.com/jarun/buku/issues/484) with identified tasks. Contributions are
 welcome! Please follow the [PR guidelines](https://github.com/jarun/buku/wiki/
-PR-guidelines). ### Related projects - [bukubrow](https://github.com/SamHH/
-bukubrow), WebExtension for browser integration - [oil](https://github.com/
-AndreiUlmeyda/oil), search-as-you-type cli front-end - [buku_run](https://
-github.com/carnager/buku_run), rofi front-end - [pinku](https://github.com/
-mosegontar/pinku), a Pinboard-to-buku import utility - [buku-dmenu](https://
-gitlab.com/benoliver999/buku-dmenu), a simple bash dmenu wrapper - [poku]
-(https://github.com/shanedabes/poku), sync between Pocket and buku - [Ebuku]
-(https://github.com/flexibeast/ebuku), Emacs interface to buku - [diigoku]
-(https://github.com/dppdppd/diigoku), buku importer for Diigo _[_S_t_a_b_l_e_ _D_o_c_s_]###
-Videos - [Buku: Take Your Bookmarks Everywhere You Go](https://www.youtube.com/
-embed/9HzEHrUBQXE) - [Buku is a great open-source bookmark manager](https://
-www.youtube.com/embed/7VxgKMWm-J8) ### In the Press - [2daygeek](http://
-www.2daygeek.com/buku-command-line-bookmark-manager-linux/) - [Hacker Milk]
-(https://hackermilk.blogspot.com/2020/01/how-to-manage-your-browsers-
-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-line-
-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/buku-
-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
+PR-guidelines). See also our documentation here _[_S_t_a_b_l_e_ _D_o_c_s_]### Related
+projects - [bukubrow](https://github.com/SamHH/bukubrow), WebExtension for
+browser integration - [oil](https://github.com/AndreiUlmeyda/oil), search-as-
+you-type cli front-end - [buku_run](https://github.com/carnager/buku_run), rofi
+front-end - [pinku](https://github.com/mosegontar/pinku), a Pinboard-to-buku
+import utility - [buku-dmenu](https://gitlab.com/benoliver999/buku-dmenu), a
+simple bash dmenu wrapper - [poku](https://github.com/shanedabes/poku), sync
+between Pocket and buku - [Ebuku](https://github.com/flexibeast/ebuku), Emacs
+interface to buku - [diigoku](https://github.com/dppdppd/diigoku), buku
+importer for Diigo ### Videos - [Buku: Take Your Bookmarks Everywhere You Go]
+(https://www.youtube.com/embed/9HzEHrUBQXE) - [Buku is a great open-source
+bookmark manager](https://www.youtube.com/embed/7VxgKMWm-J8) ### In the Press -
+[2daygeek](http://www.2daygeek.com/buku-command-line-bookmark-manager-linux/) -
+[Hacker Milk](https://hackermilk.blogspot.com/2020/01/how-to-manage-your-
+browsers-bookmarks.html) - [It's F.O.S.S.](https://itsfoss.com/buku-command-
+line-bookmark-manager-linux/) - [LinOxide](https://linoxide.com/linux-how-to/
+buku-browser-bookmarks-linux/) - [LinuxUser Magazine 01/2017 Issue](http://
 www.linux-community.de/LU/2017/01/Das-Beste-aus-zwei-Welten) - [Make Tech
 Easier](https://www.maketecheasier.com/manage-browser-bookmarks-ubuntu-command-
 line/) - [One Thing Well](http://onethingwell.org/post/144952807044/buku) -
 [Open Source For You](https://opensourceforu.com/2018/05/buku-a-bookmark-
 manager-in-the-command-line/) - [ulno.net](https://ulno.net/blog/2017-07-19/of-
 bookmarks-tags-and-browsers/)
```

### Comparing `buku-4.7.1/buku.egg-info/SOURCES.txt` & `buku-4.9/buku.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,38 +13,48 @@
 buku.egg-info/SOURCES.txt
 buku.egg-info/dependency_links.txt
 buku.egg-info/entry_points.txt
 buku.egg-info/requires.txt
 buku.egg-info/top_level.txt
 bukuserver/__init__.py
 bukuserver/__main__.py
+bukuserver/api.py
 bukuserver/filters.py
 bukuserver/forms.py
 bukuserver/response.py
 bukuserver/server.py
 bukuserver/views.py
+bukuserver/middleware/__init__.py
+bukuserver/middleware/flask_reverse_proxy_fix.py
+bukuserver/static/bukuserver/favicon.svg
+bukuserver/static/bukuserver/css/bookmark.css
 bukuserver/static/bukuserver/js/Chart.js
 bukuserver/static/bukuserver/js/bookmark.js
-bukuserver/templates/bukuserver/base.html
+bukuserver/static/bukuserver/js/last_page.js
+bukuserver/static/bukuserver/js/page_size.js
 bukuserver/templates/bukuserver/bookmark_create.html
 bukuserver/templates/bukuserver/bookmark_create_modal.html
+bukuserver/templates/bukuserver/bookmark_details.html
+bukuserver/templates/bukuserver/bookmark_details_modal.html
 bukuserver/templates/bukuserver/bookmark_edit.html
 bukuserver/templates/bukuserver/bookmark_edit_modal.html
-bukuserver/templates/bukuserver/bookmarks.html
+bukuserver/templates/bukuserver/bookmarklet.url
+bukuserver/templates/bukuserver/bookmarks_list.html
 bukuserver/templates/bukuserver/home.html
-bukuserver/templates/bukuserver/index.html
+bukuserver/templates/bukuserver/lib.html
 bukuserver/templates/bukuserver/statistic.html
-bukuserver/templates/bukuserver/tags.html
+bukuserver/templates/bukuserver/tags_list.html
 tests/__init__.py
 tests/test_BukuCrypt.py
 tests/test_ExtendedArgumentParser.py
 tests/test_buku.py
 tests/test_bukuDb.py
 tests/test_import_firefox_json.py
 tests/test_server.py
 tests/test_setup.py
 tests/test_views.py
+tests/util.py
 tests/test_bukuDb/25491522_res.yaml
 tests/test_bukuDb/25491522_res_nopt.yaml
 tests/test_bukuDb/Bookmarks
 tests/test_bukuDb/firefox_res.yaml
 tests/test_bukuDb/firefox_res_nopt.yaml
```

### Comparing `buku-4.7.1/buku.py` & `buku-4.9/buku.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #!/usr/bin/env python3
 #
 # Bookmark management utility
 #
-# Copyright © 2015-2022 Arun Prakash Jana <engineerarun@gmail.com>
+# Copyright © 2015-2024 Arun Prakash Jana <engineerarun@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with buku.  If not, see <http://www.gnu.org/licenses/>.
+from __future__ import annotations  # for |
 
 import argparse
 import calendar
-import cgi
 import codecs
 import collections
 import contextlib
+import email.message
 import json
 import locale
 import logging
 import os
 import platform
 import re
 import shutil
@@ -40,42 +41,44 @@
 import threading
 import time
 import unicodedata
 import webbrowser
 from enum import Enum
 from itertools import chain
 from subprocess import DEVNULL, PIPE, Popen
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, NamedTuple
+from collections.abc import Sequence, Set, Callable
+from warnings import warn
 
 import urllib3
 from bs4 import BeautifulSoup
+from bs4.dammit import EncodingDetector
 from urllib3.exceptions import LocationParseError
 from urllib3.util import Retry, make_headers, parse_url
 
-# note catch ModuleNotFoundError instead Exception
-# when python3.5 not supported
-try:
-    import readline
-except Exception:
-    import pyreadline as readline  # type: ignore
 try:
     from mypy_extensions import TypedDict
 except ImportError:
     TypedDict = None  # type: ignore
 
-__version__ = '4.7.1'
+__version__ = '4.9'
 __author__ = 'Arun Prakash Jana <engineerarun@gmail.com>'
 __license__ = 'GPLv3'
 
 # Global variables
 INTERRUPTED = False  # Received SIGINT
 DELIM = ','  # Delimiter used to store tags in DB
 SKIP_MIMES = {'.pdf', '.txt'}
 PROMPTMSG = 'buku (? for help): '  # Prompt message string
 
+strip_delim = lambda s, delim=DELIM, sub=' ': str(s).replace(delim, sub)
+taglist = lambda ss: sorted(s.lower() for s in set(ss) if s)
+taglist_str = lambda s: delim_wrap(DELIM.join(taglist(s.split(DELIM))))
+like_escape = lambda s, c='`': s.replace(c, c+c).replace('_', c+'_').replace('%', c+'%')
+
 # Default format specifiers to print records
 ID_STR = '%d. %s [%s]\n'
 ID_DB_STR = '%d. %s'
 MUTE_STR = '%s (L)\n'
 URL_STR = '   > %s\n'
 DESC_STR = '   + %s\n'
 DESC_WRAP = '%s%s'
@@ -91,19 +94,45 @@
     'A': '30;1', 'B': '31;1', 'C': '32;1', 'D': '33;1',
     'E': '34;1', 'F': '35;1', 'G': '36;1', 'H': '37;1',
     'I': '90;1', 'J': '91;1', 'K': '92;1', 'L': '93;1',
     'M': '94;1', 'N': '95;1', 'O': '96;1', 'P': '97;1',
     'x': '0', 'X': '1', 'y': '7', 'Y': '7;1', 'z': '2',
 }.items()}
 
-USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64; rv:101.0) Gecko/20100101 Firefox/101.0'
+# DB flagset values
+[FLAG_NONE, FLAG_IMMUTABLE] = [0x00, 0x01]
+
+FIELD_FILTER = {
+    1: ('id', 'url'),
+    2: ('id', 'url', 'tags'),
+    3: ('id', 'title'),
+    4: ('id', 'url', 'title', 'tags'),
+    5: ('id', 'title', 'tags'),
+    10: ('url',),
+    20: ('url', 'tags'),
+    30: ('title',),
+    40: ('url', 'title', 'tags'),
+    50: ('title', 'tags'),
+}
+ALL_FIELDS = ('id', 'url', 'title', 'desc', 'tags')
+JSON_FIELDS = {'id': 'index', 'url': 'uri', 'desc': 'description'}
+
+USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64; rv:124.0) Gecko/20100101 Firefox/124.0'
 MYHEADERS = None  # Default dictionary of headers
 MYPROXY = None  # Default proxy
 TEXT_BROWSERS = ['elinks', 'links', 'links2', 'lynx', 'w3m', 'www-browser']
 IGNORE_FF_BOOKMARK_FOLDERS = frozenset(["placesRoot", "bookmarksMenuFolder"])
+PERMANENT_REDIRECTS = {301, 308}
+
+# IntSet: TypeAlias = Set[int] | range      # TODO: use after dropping 3.8 & 3.9
+# Ints: TypeAlias = Sequence[int] | IntSet
+# IntOrInts: TypeAlias = int | Ints
+# T = TypeVar('T')
+# Values: TypeAlias = Sequence[T] | Set[T]
+# del T
 
 # Set up logging
 LOGGER = logging.getLogger()
 LOGDBG = LOGGER.debug
 LOGERR = LOGGER.error
 
 # Define the default path to ca-certificates
@@ -358,17 +387,57 @@
         except Exception as e:
             with contextlib.suppress(FileNotFoundError):
                 os.remove(dbfile)
             LOGERR(e)
             sys.exit(1)
 
 
-BookmarkVar = Tuple[int, str, Optional[str], str, str, int]
-# example:
-# (1, 'http://example.com', 'example title', ',tags1,', 'randomdesc', 0))
+class FetchResult(NamedTuple):
+    url: str                            # resulting URL after following PERMANENT redirects
+    title: str = ''
+    desc: str = ''
+    keywords: str = ''
+    mime: bool = False
+    bad: bool = False
+    fetch_status: Optional[int] = None  # None means no fetch occurred (e.g. due to a network error)
+
+    def tag_redirect(self, pattern: str = None) -> str:
+        return ('' if self.fetch_status not in PERMANENT_REDIRECTS else (pattern or 'http:{}').format(self.fetch_status))
+
+    def tag_error(self, pattern: str = None) -> str:
+        return ('' if (self.fetch_status or 0) < 400 else (pattern or 'http:{}').format(self.fetch_status))
+
+    def tags(self, *, keywords: bool = True, redirect: bool | str = False, error: bool | str = False) -> str:
+        _redirect = redirect and self.tag_redirect(None if redirect is True else redirect)
+        _error = error and self.tag_error(None if error is True else error)
+        return DELIM.join(taglist((keywords and self.keywords or '').split(DELIM) + [_redirect, _error]))
+
+
+class BookmarkVar(NamedTuple):
+    """Bookmark data named tuple"""
+    id: int
+    url: str
+    title: Optional[str] = None
+    tags_raw: str = ''
+    desc: str = ''
+    flags: int = FLAG_NONE
+
+    @property
+    def immutable(self) -> bool:
+        return bool(self.flags & FLAG_IMMUTABLE)
+
+    @property
+    def tags(self) -> str:
+        return self.tags_raw[1:-1]
+
+    @property
+    def taglist(self) -> List[str]:
+        return [x for x in self.tags_raw.split(',') if x]
+
+bookmark_vars = lambda xs: (BookmarkVar(*x) for x in xs)
 
 
 class BukuDb:
     """Abstracts all database operations.
 
     Attributes
     ----------
@@ -381,37 +450,39 @@
     field_filter : int
         Indicates format for displaying bookmarks. Default is 0.
     chatty : bool
         Sets the verbosity of the APIs. Default is False.
     """
 
     def __init__(
-            self, json: Optional[str] = None, field_filter: Optional[int] = 0, chatty: Optional[bool] = False,
-            dbfile: Optional[str] = None, colorize: Optional[bool] = True) -> None:
+            self, json: Optional[str] = None, field_filter: int = 0, chatty: bool = False,
+            dbfile: Optional[str] = None, colorize: bool = True) -> None:
         """Database initialization API.
 
         Parameters
         ----------
         json : string
             Empty string if results should be printed in JSON format to stdout.
             Nonempty string if results should be printed in JSON format to file. The string has to be a valid path.
             None if the results should be printed as human-readable plaintext.
-        field_filter : int, optional
+        field_filter : int
             Indicates format for displaying bookmarks. Default is 0.
-        chatty : bool, optional
+        chatty : bool
             Sets the verbosity of the APIs. Default is False.
-        colorize : bool, optional
+        colorize : bool
             Indicates whether color should be used in output. Default is True.
         """
 
         self.json = json
         self.field_filter = field_filter
         self.chatty = chatty
         self.colorize = colorize
         self.conn, self.cur = BukuDb.initdb(dbfile, self.chatty)
+        self._to_export = None  # type: Optional[Dict[str, str | BookmarkVar]]
+        self._to_delete = None  # type: Optional[int | Sequence[int] | Set[int] | range]
 
     @staticmethod
     def get_default_dbdir():
         """Determine the directory path where dbfile will be stored.
 
         If the platform is Windows, use %APPDATA%
         else if $XDG_DATA_HOME is defined, use it
@@ -435,15 +506,15 @@
                     return os.path.abspath('.')
             else:
                 data_home = os.path.join(os.environ.get('HOME'), '.local', 'share')
 
         return os.path.join(data_home, 'buku')
 
     @staticmethod
-    def initdb(dbfile: Optional[str] = None, chatty: Optional[bool] = False) -> Tuple[sqlite3.Connection, sqlite3.Cursor]:
+    def initdb(dbfile: Optional[str] = None, chatty: bool = False) -> Tuple[sqlite3.Connection, sqlite3.Cursor]:
         """Initialize the database connection.
 
         Create DB file and/or bookmarks table if they don't exist.
         Alert on encryption options on first execution.
 
         Parameters
         ----------
@@ -508,194 +579,251 @@
             conn.commit()
         except Exception as e:
             LOGERR('initdb(): %s', e)
             sys.exit(1)
 
         return (conn, cur)
 
+    def _fetch(self, query: str, *args) -> List[BookmarkVar]:
+        self.cur.execute(query, args)
+        return [BookmarkVar(*x) for x in self.cur.fetchall()]
+
+    def _fetch_first(self, query: str, *args) -> Optional[BookmarkVar]:
+        rows = self._fetch(query + ' LIMIT 1', *args)
+        return rows[0] if rows else None
+
     def get_rec_all(self):
         """Get all the bookmarks in the database.
 
         Returns
         -------
         list
             A list of tuples representing bookmark records.
         """
 
-        self.cur.execute('SELECT * FROM bookmarks')
-        return self.cur.fetchall()
+        return self._fetch('SELECT * FROM bookmarks')
 
     def get_rec_by_id(self, index: int) -> Optional[BookmarkVar]:
         """Get a bookmark from database by its ID.
 
         Parameters
         ----------
         index : int
             DB index of bookmark record.
 
         Returns
         -------
-        tuple or None
+        BookmarkVar or None
             Bookmark data, or None if index is not found.
         """
 
-        self.cur.execute('SELECT * FROM bookmarks WHERE id = ? LIMIT 1', (index,))
-        resultset = self.cur.fetchall()
-        return resultset[0] if resultset else None
+        return self._fetch_first('SELECT * FROM bookmarks WHERE id = ?', index)
+
+    def get_rec_all_by_ids(self, indices: Sequence[int] | Set[int] | range):  # Ints
+        """Get all the bookmarks in the database.
+
+        Parameters
+        ----------
+        indices : int[] | int{} | range
+            DB indices of bookmark records.
+
+        Returns
+        -------
+        list
+            A list of tuples representing bookmark records.
+        """
+
+        placeholder = ', '.join(['?'] * len(indices))
+        return indices and self._fetch(f'SELECT * FROM bookmarks WHERE id IN ({placeholder})', list(indices))
 
     def get_rec_id(self, url):
         """Check if URL already exists in DB.
 
         Parameters
         ----------
         url : str
             A URL to search for in the DB.
 
         Returns
         -------
         int
-            DB index, or -1 if URL not found in DB.
+            DB index, or None if URL not found in DB.
         """
 
-        self.cur.execute('SELECT id FROM bookmarks WHERE URL = ? LIMIT 1', (url,))
-        resultset = self.cur.fetchall()
-        return resultset[0][0] if resultset else -1
+        row = self._fetch_first('SELECT * FROM bookmarks WHERE url = ?', url)
+        return row and row.id
+
+    def get_rec_ids(self, urls: Sequence[str] | Set[str]):  # Values[str]
+        """Check if URL already exists in DB.
+
+        Parameters
+        ----------
+        urls : str[] | str{}
+            URLs to search for in the DB.
+
+        Returns
+        -------
+        list
+            A list of DB indices.
+        """
+
+        if not urls:
+            return []
+        placeholder = ', '.join(['?'] * len(urls))
+        self.cur.execute(f'SELECT id FROM bookmarks WHERE url IN ({placeholder})', list(urls))
+        return [x[0] for x in self.cur.fetchall()]
 
     def get_max_id(self) -> int:
         """Fetch the ID of the last record.
 
         Returns
         -------
         int
-            ID of the record if any record exists, else -1.
+            ID of the record if any record exists, else None.
         """
 
-        self.cur.execute('SELECT MAX(id) from bookmarks')
-        resultset = self.cur.fetchall()
-        return -1 if resultset[0][0] is None else resultset[0][0]
+        self.cur.execute('SELECT MAX(id) FROM bookmarks')
+        return self.cur.fetchall()[0][0]
 
     def add_rec(
             self,
             url: str,
             title_in: Optional[str] = None,
             tags_in: Optional[str] = None,
             desc: Optional[str] = None,
-            immutable: Optional[int] = 0,
-            delay_commit: Optional[bool] = False,
-            fetch: Optional[bool] = True) -> int:
+            immutable: bool = False,
+            delay_commit: bool = False,
+            fetch: bool = True,
+            url_redirect: bool = False,
+            tag_redirect: bool | str = False,
+            tag_error: bool | str = False,
+            del_error: Optional[Set[int] | range] = None) -> int:  # Optional[IntSet]
         """Add a new bookmark.
 
         Parameters
         ----------
         url : str
             URL to bookmark.
-        title_in :str, optional
+        title_in : str, optional
             Title to add manually. Default is None.
         tags_in : str, optional
             Comma-separated tags to add manually.
             Must start and end with comma. Default is None.
         desc : str, optional
             Description of the bookmark. Default is None.
-        immutable : int, optional
-            Indicates whether to disable title fetch from web.
-            Default is 0.
-        delay_commit : bool, optional
+        immutable : bool
+            Indicates whether to disable title fetch from web. Default is False.
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
-        fetch : bool, optional
-            Fetch page from web and parse for data
+        fetch : bool
+            Fetch page from web and parse for data. Required fetch-status params to take effect.
+        url_redirect : bool
+            Bookmark the URL produced after following all PERMANENT redirects.
+        tag_redirect : bool | str
+            Adds a tag by the given pattern if the url resolved to a PERMANENT
+            redirect. (True means the default pattern 'http:{}'.)
+        tag_error : bool | str
+            Adds a tag by the given pattern if the url resolved to a HTTP error.
+            (True means the default pattern 'http:{}'.)
+        del_error : int{} | range, optional
+            Do not add the bookmark if HTTP response status is in the given set or range.
+            Also prevents the bookmark from being added on a network error.
 
         Returns
         -------
         int
-            DB index of new bookmark on success, -1 on failure.
+            DB index of new bookmark on success, None on failure.
         """
 
         # Return error for empty URL
-        if not url or url == '':
+        if not url:
             LOGERR('Invalid URL')
-            return -1
+            return None
 
         # Ensure that the URL does not exist in DB already
         id = self.get_rec_id(url)
-        if id != -1:
+        if id:
             LOGERR('URL [%s] already exists at index %d', url, id)
-            return -1
+            return None
 
         if fetch:
             # Fetch data
-            ptitle, pdesc, ptags, mime, bad = network_handler(url)
-            if bad:
+            result = fetch_data(url)
+            if result.bad:
                 print('Malformed URL\n')
-            elif mime:
+            elif result.mime:
                 LOGDBG('HTTP HEAD requested')
-            elif ptitle == '' and title_in is None:
+            elif not result.title and title_in is None:
                 print('No title\n')
             else:
-                LOGDBG('Title: [%s]', ptitle)
+                LOGDBG('Title: [%s]', result.title)
         else:
-            ptitle = pdesc = ptags = ''
-            LOGDBG('ptags: [%s]', ptags)
+            result = FetchResult(url, fetch_status=200)
+            LOGDBG('ptags: [%s]', result.tags(redirect=tag_redirect, error=tag_error))
 
-        if title_in is not None:
-            ptitle = title_in
+        url = (result.url if url_redirect else url)
+        title = (title_in if title_in is not None else result.title)
 
         # Fix up tags, if broken
-        tags_in = delim_wrap(tags_in)
+        tags_in = taglist_str((tags_in or '') + DELIM + result.tags(redirect=tag_redirect, error=tag_error))
 
         # Process description
-        if desc is None:
-            desc = '' if pdesc is None else pdesc
+        desc = (desc if desc is not None else result.desc) or ''
 
         try:
-            flagset = 0
-            if immutable == 1:
-                flagset |= immutable
+            assert not del_error or result.fetch_status is not None, 'Network error'
+            assert not del_error or result.fetch_status not in del_error, f'HTTP error {result.fetch_status}'
+            flagset = FLAG_NONE
+            if immutable:
+                flagset |= FLAG_IMMUTABLE
 
             qry = 'INSERT INTO bookmarks(URL, metadata, tags, desc, flags) VALUES (?, ?, ?, ?, ?)'
-            self.cur.execute(qry, (url, ptitle, tags_in, desc, flagset))
+            self.cur.execute(qry, (url, title, tags_in, desc, flagset))
             if not delay_commit:
                 self.conn.commit()
             if self.chatty:
                 self.print_rec(self.cur.lastrowid)
             return self.cur.lastrowid
         except Exception as e:
             LOGERR('add_rec(): %s', e)
-            return -1
+            return None
 
     def append_tag_at_index(self, index, tags_in, delay_commit=False):
         """Append tags to bookmark tagset at index.
 
         Parameters
         ----------
-        index : int
-            DB index of the record. 0 indicates all records.
+        index : int | int[] | int{} | range, optional
+            DB index of the record. 0 or empty indicates all records.
         tags_in : str
             Comma-separated tags to add manually.
-        delay_commit : bool, optional
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
 
         Returns
         -------
         bool
             True on success, False on failure.
         """
 
         if tags_in is None or tags_in == DELIM:
             return True
+        indices = (None if not index else [index] if isinstance(index, int) else index)
 
-        if index == 0:
+        if not indices:
             resp = read_in('Append the tags to ALL bookmarks? (y/n): ')
             if resp != 'y':
                 return False
 
             self.cur.execute('SELECT id, tags FROM bookmarks ORDER BY id ASC')
         else:
-            self.cur.execute('SELECT id, tags FROM bookmarks WHERE id = ? LIMIT 1', (index,))
+            placeholder = ', '.join(['?'] * len(indices))
+            self.cur.execute(f'SELECT id, tags FROM bookmarks WHERE id IN ({placeholder}) ORDER BY id ASC', tuple(indices))
 
         resultset = self.cur.fetchall()
         if resultset:
             query = 'UPDATE bookmarks SET tags = ? WHERE id = ?'
             for row in resultset:
                 tags = row[1] + tags_in[1:]
                 tags = parse_tags([tags])
@@ -711,61 +839,64 @@
         return True
 
     def delete_tag_at_index(self, index, tags_in, delay_commit=False, chatty=True):
         """Delete tags from bookmark tagset at index.
 
         Parameters
         ----------
-        index : int
-            DB index of bookmark record. 0 indicates all records.
+        index : int | int[] | int{} | range, optional
+            DB index of bookmark record. 0 or empty indicates all records.
         tags_in : str
             Comma-separated tags to delete manually.
-        delay_commit : bool, optional
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
-        chatty: bool, optional
+        chatty: bool
             Skip confirmation when set to False.
 
         Returns
         -------
         bool
             True on success, False on failure.
         """
 
         if tags_in is None or tags_in == DELIM:
             return True
 
         tags_to_delete = tags_in.strip(DELIM).split(DELIM)
+        indices = (None if not index else [index] if isinstance(index, int) else index)
 
-        if index == 0:
-            if chatty:
+        if len(indices or []) != 1:
+            if not indices and chatty:
                 resp = read_in('Delete the tag(s) from ALL bookmarks? (y/n): ')
                 if resp != 'y':
                     return False
 
+            query = "UPDATE bookmarks SET tags = replace(tags, ?, ?) WHERE tags LIKE ? ESCAPE '`'"
+            if indices:
+                query += ' AND id IN ({})'.format(', '.join(['?'] * len(indices)))
+
             count = 0
-            match = "'%' || ? || '%'"
             for tag in tags_to_delete:
                 tag = delim_wrap(tag)
-                q = ("UPDATE bookmarks SET tags = replace(tags, '%s', '%s') "
-                     "WHERE tags LIKE %s" % (tag, DELIM, match))
-                self.cur.execute(q, (tag,))
+                args = (tag, DELIM, '%'+like_escape(tag, '`')+'%') + tuple(indices or [])
+                self.cur.execute(query, args)
                 count += self.cur.rowcount
 
-            if count and not delay_commit:
+            if count > 0 and not delay_commit:
                 self.conn.commit()
                 if self.chatty:
                     print('%d record(s) updated' % count)
 
             return True
 
         # Process a single index
         # Use SELECT and UPDATE to handle multiple tags at once
         query = 'SELECT id, tags FROM bookmarks WHERE id = ? LIMIT 1'
-        self.cur.execute(query, (index,))
+        self.cur.execute(query, list(indices))
         resultset = self.cur.fetchall()
         if resultset:
             query = 'UPDATE bookmarks SET tags = ? WHERE id = ?'
             for row in resultset:
                 tags = row[1]
 
                 for tag in tags_to_delete:
@@ -780,209 +911,299 @@
         else:
             return False
 
         return True
 
     def update_rec(
             self,
-            index: int,
+            index: Optional[int | Sequence[int] | Set[int] | range],  # Optional[IntOrInts]
             url: Optional[str] = None,
             title_in: Optional[str] = None,
             tags_in: Optional[str] = None,
             desc: Optional[str] = None,
-            immutable: Optional[int] = -1,
-            threads: int = 4) -> bool:
-        """Update an existing record at index.
+            immutable: Optional[bool] = None,
+            threads: int = 4,
+            url_redirect: bool = False,
+            tag_redirect: bool | str = False,
+            tag_error: bool | str = False,
+            del_error: Optional[Set[int] | range] = None,             # Optional[IntSet]
+            export_on: Optional[Set[int] | range] = None) -> bool:    # Optional[IntSet]
+        """Update an existing record at (each) index.
 
-        Update all records if index is 0 and url is not specified.
+        Update all records if index is 0 or empty, and url is not specified.
         URL is an exception because URLs are unique in DB.
 
         Parameters
         ----------
-        index : int
-            DB index of record. 0 indicates all records.
+        index : int | int[] | int{} | range, optional
+            DB index(es) of record(s). 0 or empty value indicates all records.
         url : str, optional
             Bookmark address.
         title_in : str, optional
             Title to add manually.
         tags_in : str, optional
             Comma-separated tags to add manually. Must start and end with comma.
             Prefix with '+,' to append to current tags.
             Prefix with '-,' to delete from current tags.
         desc : str, optional
             Description of bookmark.
-        immutable : int, optional
-            Disable title fetch from web if 1. Default is -1.
-        threads : int, optional
+        immutable : bool, optional
+            Disable title fetch from web if True. Default is None (no change).
+        threads : int
             Number of threads to use to refresh full DB. Default is 4.
+        url_redirect : bool
+            Update the URL to one produced after following all PERMANENT redirects.
+            (This could fail if the new URL is bookmarked already.)
+        tag_redirect : bool | str
+            Adds a tag by the given pattern if the url resolved to a PERMANENT
+            redirect. (True means the default pattern 'http:{}'.)
+        tag_error : bool | str
+            Adds a tag by the given pattern if the url resolved to a HTTP error.
+            (True means the default pattern 'http:{}'.)
+        del_error : int{} | range, optional
+            Delete the bookmark if HTTP response status is in the given set or range.
+            Does NOT cause deletion of the bookmark on a network error.
+        export_on : int{} | range, optional
+            Limit the export to URLs returning one of given HTTP codes; store old URLs.
 
         Returns
         -------
         bool
-            True on success, False on Failure.
+            True on success, False on failure. (Deletion by del_error counts as success.)
         """
 
         arguments = []  # type: List[Any]
         query = 'UPDATE bookmarks SET'
-        to_update = False
         tag_modified = False
-        ret = False
+        ret = True
+        indices = (None if not index else [index] if isinstance(index, int) else index)
+        index = indices and list(indices or [])[0]
+        single = len(indices or []) == 1
+        export_on, self._to_export = (export_on or set()), ({} if export_on else None)
+        tags_in = (tags_in or None if not tags_in or re.match('[+-],', tags_in) else delim_wrap(tags_in))
 
-        # Update URL if passed as argument
-        if url is not None and url != '':
-            if index == 0:
-                LOGERR('All URLs cannot be same')
-                return False
-            query += ' URL = ?,'
-            arguments += (url,)
-            to_update = True
-
-        # Update tags if passed as argument
-        if tags_in is not None:
-            if tags_in in ('+,', '-,'):
-                LOGERR('Please specify a tag')
-                return False
+        if url and not single:
+            LOGERR('All URLs cannot be same')
+            return False
 
-            if tags_in.startswith('+,'):
-                chatty = self.chatty
-                self.chatty = False
-                ret = self.append_tag_at_index(index, tags_in[1:])
-                self.chatty = chatty
-                tag_modified = True
-            elif tags_in.startswith('-,'):
-                chatty = self.chatty
-                self.chatty = False
-                ret = self.delete_tag_at_index(index, tags_in[1:])
-                self.chatty = chatty
-                tag_modified = True
-            else:
-                tags_in = delim_wrap(tags_in)
+        if tags_in in ('+,', '-,'):
+            LOGERR('Please specify a tag')
+            return False
 
-                query += ' tags = ?,'
-                arguments += (tags_in,)
-                to_update = True
+        if indices and min(indices) > (self.get_max_id() or 0):  # none of the indices exist in DB?
+            return False
 
         # Update description if passed as an argument
         if desc is not None:
             query += ' desc = ?,'
             arguments += (desc,)
-            to_update = True
 
         # Update immutable flag if passed as argument
-        if immutable != -1:
-            flagset = 1
-            if immutable == 1:
+        if immutable is not None:
+            if immutable:
                 query += ' flags = flags | ?,'
-            elif immutable == 0:
+                arguments += (FLAG_IMMUTABLE,)
+            else:
                 query += ' flags = flags & ?,'
-                flagset = ~flagset
-
-            arguments += (flagset,)
-            to_update = True
+                arguments += (~FLAG_IMMUTABLE,)
 
         # Update title
         #
         # 1. If --title has no arguments, delete existing title
         # 2. If --title has arguments, update existing title
         # 3. If --title option is omitted at cmdline:
         #    If URL is passed, update the title from web using the URL
         # 4. If no other argument (url, tag, comment, immutable) passed,
         #    update title from web using DB URL (if title is mutable)
-        title_to_insert = None
-        pdesc = None
-        ptags = None
-        if title_in is not None:
-            title_to_insert = title_in
-        elif url is not None and url != '':
-            title_to_insert, pdesc, ptags, mime, bad = network_handler(url)
-            if bad:
+        fetch_title = {url, title_in, tags_in, desc, immutable} == {None}
+        network_test = url_redirect or tag_redirect or tag_error or del_error or export_on or fetch_title
+        if url and title_in is None:
+            network_test = False
+            _url = url or self.get_rec_by_id(index).url
+            result = fetch_data(_url)
+            if result.bad:
                 print('Malformed URL')
-            elif mime:
+            elif result.mime:
                 LOGDBG('HTTP HEAD requested')
-            elif title_to_insert == '':
+            elif not result.title:
                 print('No title')
             else:
-                LOGDBG('Title: [%s]', title_to_insert)
+                LOGDBG('Title: [%s]', result.title)
 
-            if not desc:
-                if not pdesc:
-                    pdesc = ''
+            if result.desc and not desc:
                 query += ' desc = ?,'
-                arguments += (pdesc,)
-                to_update = True
-        elif not to_update and not tag_modified:
-            ret = self.refreshdb(index, threads)
-            if ret and index and self.chatty:
-                self.print_rec(index)
-            return ret
+                arguments += (result.desc,)
 
-        if title_to_insert is not None:
+            if url_redirect and result.url != _url:
+                url = result.url
+
+            if result.fetch_status in export_on:  # storing the old URL
+                self._to_export[url or _url] = _url
+        else:
+            result = FetchResult(url, title_in)
+
+        if result.title is not None:
             query += ' metadata = ?,'
-            arguments += (title_to_insert,)
-            to_update = True
+            arguments += (result.title,)
 
-        if not to_update:  # Nothing to update
-            # Show bookmark if tags were appended to deleted
-            if tag_modified and self.chatty:
-                self.print_rec(index)
-            return ret
+        # Update URL if passed as argument
+        if url:
+            query += ' URL = ?,'
+            arguments += (url,)
 
-        if index == 0:  # Update all records
+        if result.fetch_status in (del_error or []):
+            if result.fetch_status in export_on:  # storing the old record
+                self._to_export[url] = self.get_rec_by_id(index)
+            LOGERR('HTTP error %s', result.fetch_status)
+            return self.delete_rec(index)
+
+        if not indices and (arguments or tags_in):
             resp = read_in('Update ALL bookmarks? (y/n): ')
             if resp != 'y':
                 return False
 
-            query = query[:-1]
-        else:
-            query = query[:-1] + ' WHERE id = ?'
-            arguments += (index,)
+        if network_test:  # doing this before updates to backup records to-be-deleted in their original state
+            custom_tags = (tags_in if (tags_in or '').startswith(DELIM) else None)
+            ret = ret and self.refreshdb(indices, threads, url_redirect=url_redirect, tag_redirect=tag_redirect,
+                                         tag_error=tag_error, del_error=del_error, export_on=export_on,
+                                         update_title=fetch_title, custom_url=url, custom_tags=custom_tags, delay_delete=True)
+
+        # Update tags if passed as argument
+        _tags = result.tags(keywords=False, redirect=tag_redirect, error=tag_error)
+        if tags_in or _tags:
+            if not tags_in or tags_in.startswith('+,'):
+                tags = taglist_str((tags_in or '')[1:] + _tags)
+                chatty = self.chatty
+                self.chatty = False
+                ret = self.append_tag_at_index(indices, tags)
+                self.chatty = chatty
+                tag_modified = True
+            elif tags_in.startswith('-,'):
+                chatty = self.chatty
+                self.chatty = False
+                ret = self.delete_tag_at_index(indices, tags_in[1:])
+                if _tags:
+                    self.append_tag_at_index(indices, _tags)
+                self.chatty = chatty
+                tag_modified = True
+            elif not network_test:  # rely on custom_tags to avoid overwriting fetch-status tags
+                query += ' tags = ?,'
+                arguments += (taglist_str(tags_in + _tags),)
+
+        if not arguments:  # no arguments => nothing to update
+            if (tag_modified or network_test) and self.chatty:
+                self.print_rec(indices)
+            self.commit_delete()
+            return ret
+
+        query = query[:-1]
+        if indices:  # Only specified indices
+            query += ' WHERE id IN ({})'.format(', '.join(['?'] * len(indices)))
+            arguments += tuple(indices)
 
         LOGDBG('update_rec query: "%s", args: %s', query, arguments)
 
         try:
             self.cur.execute(query, arguments)
             self.conn.commit()
-            if self.cur.rowcount and self.chatty:
+            if self.cur.rowcount > 0 and self.chatty:
                 self.print_rec(index)
-
-            if self.cur.rowcount == 0:
-                LOGERR('No matching index %d', index)
+            elif self.cur.rowcount == 0:
+                if single:
+                    LOGERR('No matching index %d', index)
+                else:
+                    LOGERR('No matches found')
                 return False
         except sqlite3.IntegrityError:
             LOGERR('URL already exists')
             return False
         except sqlite3.OperationalError as e:
             LOGERR(e)
             return False
+        finally:
+            self.commit_delete()
 
         return True
 
-    def refreshdb(self, index: int, threads: int) -> bool:
-        """Refresh ALL records in the database.
+    def refreshdb(
+            self,
+            index: Optional[int | Sequence[int] | Set[int] | range],  # Optional[IntOrInts]
+            threads: int,
+            url_redirect: bool = False,
+            tag_redirect: bool | str = False,
+            tag_error: bool | str = False,
+            del_error: Optional[Set[int] | range] = None,             # Optional[IntSet]
+            export_on: Optional[Set[int] | range] = None,             # Optional[IntSet]
+            update_title: bool = True,
+            custom_url: Optional[str] = None,
+            custom_tags: Optional[str] = None,
+            delay_delete: bool = False) -> bool:
+        """Refresh ALL (or specified) records in the database.
 
         Fetch title for each bookmark from the web and update the records.
-        Doesn't update the record if fetched title is empty.
+        Doesn't update the title if fetched title is empty.
 
         Notes
         -----
             This API doesn't change DB index, URL or tags of a bookmark.
+            (Unless one or more fetch-status parameters are supplied.)
             This API is verbose.
 
         Parameters
         ----------
-        index : int
-            DB index of record to update. 0 indicates all records.
+        index : int | int[] | int{} | range, optional
+            DB index(es) of record(s) to update. 0 or empty value indicates all records.
         threads: int
             Number of threads to use to refresh full DB. Default is 4.
+        url_redirect : bool
+            Update the URL to one produced after following all PERMANENT redirects.
+            (This could fail if the new URL is bookmarked already.)
+        tag_redirect : bool | str
+            Adds a tag by the given pattern if the url resolved to a PERMANENT
+            redirect. (True means the default pattern 'http:{}'.)
+        tag_error : bool | str
+            Adds a tag by the given pattern if the url resolved to a HTTP error.
+            (True means the default pattern 'http:{}'.)
+        del_error : int{} | range, optional
+            Delete the bookmark if HTTP response status is in the given set or range.
+        export_on : int{} | range, optional
+            Limit the export to URLs returning one of given HTTP codes; store old URLs.
+        update_title : bool
+            Update titles/descriptions. (Can be turned off for network testing.)
+        custom_url : str, optional
+            Override URL to fetch. (Use for network testing of a single record before updating it.)
+        custom_tags : str, optional
+            Overwrite all tags. (Use to combine network testing with tags overwriting.)
+        delay_delete : bool
+            Delay scheduled deletions by del_error. (Use for network testing during update.)
+
+        Returns
+        -------
+        bool
+            True on success, False on failure. (Deletion by del_error counts as success.)
         """
 
-        if index == 0:
-            self.cur.execute('SELECT id, url, flags FROM bookmarks ORDER BY id ASC')
+        indices = (None if not index else [index] if isinstance(index, int) else index)
+        index = indices and list(indices)[0]
+        export_on, self._to_export = (export_on or set()), ({} if export_on else None)
+        self._to_delete = []
+
+        if not update_title and not (url_redirect or tag_redirect or tag_error or del_error or export_on):
+            LOGERR('Noop update request')
+            return False
+        if custom_url and len(indices or []) != 1:
+            LOGERR('custom_url is only supported for a singular index')
+            return False
+
+        if not indices:
+            self.cur.execute('SELECT id, url, tags, flags FROM bookmarks ORDER BY id ASC')
         else:
-            self.cur.execute('SELECT id, url, flags FROM bookmarks WHERE id = ? LIMIT 1', (index,))
+            placeholder = ', '.join(['?'] * len(indices))
+            self.cur.execute(f'SELECT id, url, tags, flags FROM bookmarks WHERE id IN ({placeholder}) ORDER BY id ASC',
+                             tuple(indices))
 
         resultset = self.cur.fetchall()
         recs = len(resultset)
         if not recs:
             LOGERR('No matching index or title immutable or empty DB')
             return False
 
@@ -998,15 +1219,15 @@
             blank_url_str = 'Index %d: No title\n'
             success_str = 'Title: [%s]\nIndex %d: updated\n'
 
         done = {'value': 0}  # count threads completed
         processed = {'value': 0}  # count number of records processed
 
         # An additional call to generate default headers
-        # gen_headers() is called within network_handler()
+        # gen_headers() is called within fetch_data()
         # However, this initial call to setup headers
         # ensures there is no race condition among the
         # initial threads to setup headers
         if not MYHEADERS:
             gen_headers()
 
         cond = threading.Condition()
@@ -1026,106 +1247,145 @@
 
             while True:
                 query = 'UPDATE bookmarks SET'
                 arguments = []
 
                 cond.acquire()
                 if resultset:
-                    row = resultset.pop()
+                    id, url, tags, flags = resultset.pop()
                 else:
                     cond.release()
                     break
                 cond.release()
 
-                title, desc, tags, mime, bad = network_handler(row[1], row[2] & 1)
+                result = fetch_data(custom_url or url, http_head=(flags & FLAG_IMMUTABLE) > 0)
                 count += 1
 
                 cond.acquire()
 
-                if bad:
-                    print(bad_url_str % row[0])
+                if result.bad:
+                    print(bad_url_str % id)
+                    if custom_tags:
+                        self.cur.execute('UPDATE bookmarks SET tags = ? WHERE id = ?', (custom_tags, id))
                     cond.release()
                     continue
 
-                if mime:
-                    if self.chatty:
-                        print(mime_str % row[0])
+                if result.fetch_status in (del_error or []):
+                    if result.fetch_status in export_on:
+                        self._to_export[url] = self.get_rec_by_id(id)
+                    LOGERR('HTTP error %s', result.fetch_status)
+                    self._to_delete += [id]
+                    if result.mime and self.chatty:
+                        print(mime_str % id)
+                    if custom_tags:
+                        self.cur.execute('UPDATE bookmarks SET tags = ? WHERE id = ?', (custom_tags, id))
                     cond.release()
                     continue
 
-                to_update = False
+                if result.mime:
+                    if self.chatty:
+                        print(mime_str % id)
+                    if custom_tags:
+                        self.cur.execute('UPDATE bookmarks SET tags = ? WHERE id = ?', (custom_tags, id))
+                    cond.release()
+                    continue
 
-                if not title or title == '':
-                    LOGERR(blank_url_str, row[0])
-                else:
+                if not result.title:
+                    LOGERR(blank_url_str, id)
+                elif update_title:
                     query += ' metadata = ?,'
-                    arguments += (title,)
-                    to_update = True
+                    arguments += (result.title,)
 
-                if desc:
+                if update_title and result.desc:
                     query += ' desc = ?,'
-                    arguments += (desc,)
-                    to_update = True
+                    arguments += (result.desc,)
+
+                _url = url
+                if url_redirect and result.url != url:
+                    query += ' url = ?,'
+                    arguments += (result.url,)
+                    _url = result.url
+
+                if result.fetch_status in export_on:
+                    self._to_export[_url] = url
+
+                _tags = result.tags(keywords=False, redirect=tag_redirect, error=tag_error)
+                if _tags:
+                    query += ' tags = ?,'
+                    arguments += (taglist_str((custom_tags or tags) + DELIM + _tags),)
+                elif custom_tags:
+                    query += ' tags = ?,'
+                    arguments += (taglist_str(custom_tags),)
 
-                if not to_update:
+                if not arguments:  # nothing to update
                     cond.release()
                     continue
 
                 query = query[:-1] + ' WHERE id = ?'
-                arguments += (row[0],)
+                arguments += (id,)
                 LOGDBG('refreshdb query: "%s", args: %s', query, arguments)
 
                 self.cur.execute(query, arguments)
 
                 # Save after fetching 32 titles per thread
-                if count & 0b11111 == 0:
+                if count % 32 == 0:
                     self.conn.commit()
 
                 if self.chatty:
-                    print(success_str % (title, row[0]))
+                    print(success_str % (result.title, id))
                 cond.release()
 
                 if INTERRUPTED:
                     break
 
             LOGDBG('Thread %d: processed %d', threading.get_ident(), count)
             with cond:
                 done['value'] += 1
                 processed['value'] += count
                 cond.notify()
 
-        if recs < threads:
-            threads = recs
+        threads = min(threads, recs)
 
         for i in range(threads):
             thread = threading.Thread(target=refresh, args=(i, cond))
             thread.start()
 
         while done['value'] < threads:
             cond.wait()
             LOGDBG('%d threads completed', done['value'])
 
         # Guard: records found == total records processed
         if recs != processed['value']:
             LOGERR('Records: %d, processed: %d !!!', recs, processed['value'])
 
         cond.release()
-        self.conn.commit()
+        if delay_delete:
+            self.conn.commit()
+        else:
+            self.commit_delete()
         return True
 
-    def edit_update_rec(self, index, immutable=-1):
+    def commit_delete(self, apply: bool = True):
+        """Commit delayed delete commands."""
+        if apply and self._to_delete is not None:
+            for id in sorted(set(self._to_delete), reverse=True):
+                self.delete_rec(id, delay_commit=True, chatty=False)
+            self.conn.commit()
+        self._to_delete = None
+
+    def edit_update_rec(self, index, immutable=None):
         """Edit in editor and update a record.
 
         Parameters
         ----------
         index : int
             DB index of the record.
             Last record, if index is -1.
-        immutable : int, optional
-            Diable title fetch from web if 1. Default is -1.
+        immutable : bool, optional
+            Disable title fetch from web if True. Default is None (no change).
 
         Returns
         -------
         bool
             True if updated, else False.
         """
 
@@ -1133,33 +1393,32 @@
         if editor == 'none':
             LOGERR('EDITOR must be set to use index with -w')
             return False
 
         if index == -1:
             # Edit the last records
             index = self.get_max_id()
-            if index == -1:
+            if not index:
                 LOGERR('Empty database')
                 return False
 
         rec = self.get_rec_by_id(index)
         if not rec:
             LOGERR('No matching index %d', index)
             return False
 
         # If reading from DB, show empty title and desc as empty lines. We have to convert because
         # even in case of add with a blank title or desc, '' is used as initializer to show '-'.
-        result = edit_rec(editor, rec[1], rec[2] if rec[2] != '' else None,
-                          rec[3], rec[4] if rec[4] != '' else None)
+        result = edit_rec(editor, rec.url, rec.title or None, rec.tags_raw, rec.desc or None)
         if result is not None:
             url, title, tags, desc = result
             return self.update_rec(index, url, title, tags, desc, immutable)
 
-        if immutable != -1:
-            return self.update_rec(index, immutable)
+        if immutable is not None:
+            return self.update_rec(index, immutable=immutable)
 
         return False
 
     def list_using_id(self, ids=[]):
         """List entries in the DB using the specified id list.
 
         Parameters
@@ -1188,48 +1447,47 @@
                     q0 += ','.join(list(map(str, part_ids)))
                 else:
                     q0 += idx + ','
             q0 = q0.rstrip(',')
             q0 += ')'
 
         try:
-            self.cur.execute(q0, [])
+            return self._fetch(q0)
         except sqlite3.OperationalError as e:
             LOGERR(e)
-            return None
-        return self.cur.fetchall()
+            return []
 
     def searchdb(
             self,
             keywords: List[str],
-            all_keywords: Optional[bool] = False,
-            deep: Optional[bool] = False,
-            regex: Optional[bool] = False
-    ) -> Optional[Iterable[Any]]:
+            all_keywords: bool = False,
+            deep: bool = False,
+            regex: bool = False
+    ) -> List[BookmarkVar]:
         """Search DB for entries where tags, URL, or title fields match keywords.
 
         Parameters
         ----------
         keywords : list of str
             Keywords to search.
-        all_keywords : bool, optional
+        all_keywords : bool
             True to return records matching ALL keywords.
             False (default value) to return records matching ANY keyword.
-        deep : bool, optional
+        deep : bool
             True to search for matching substrings. Default is False.
-        regex : bool, optional
+        regex : bool
             Match a regular expression if True. Default is False.
 
         Returns
         -------
-        list or None
-            List of search results, or None if no matches.
+        list
+            List of search results.
         """
         if not keywords:
-            return None
+            return []
 
         # Deep query string
         q1 = ("(tags LIKE ('%' || ? || '%') OR "
               "URL LIKE ('%' || ? || '%') OR "
               "metadata LIKE ('%' || ? || '%') OR "
               "desc LIKE ('%' || ? || '%')) ")
         # Non-deep query string
@@ -1246,15 +1504,15 @@
                 if not token:
                     continue
 
                 q0 += case_statement(q2) + ' + '
                 qargs += (token, token, token, token,)
 
             if not qargs:
-                return None
+                return []
 
             q0 = q0[:-3] + ' AS score FROM bookmarks WHERE score > 0 ORDER BY score DESC)'
         elif all_keywords:
             if len(keywords) == 1 and keywords[0] == 'blank':
                 q0 = "SELECT * FROM bookmarks WHERE metadata = '' OR tags = ? "
                 qargs += (DELIM,)
             elif len(keywords) == 1 and keywords[0] == 'immutable':
@@ -1275,15 +1533,15 @@
                             _post = '\\b'
                         token = _pre + re.escape(token.rstrip('/')) + _post
                         q0 += q2 + 'AND '
 
                     qargs += (token, token, token, token,)
 
                 if not qargs:
-                    return None
+                    return []
 
                 q0 = q0[:-4]
             q0 += 'ORDER BY id ASC'
         elif not all_keywords:
             q0 = 'SELECT id, url, metadata, tags, desc, flags FROM (SELECT *, '
             for token in keywords:
                 if not token:
@@ -1299,57 +1557,55 @@
                         _post = '\\b'
                     token = _pre + re.escape(token.rstrip('/')) + _post
                     q0 += case_statement(q2) + ' + '
 
                 qargs += (token, token, token, token,)
 
             if not qargs:
-                return None
+                return []
 
             q0 = q0[:-3] + ' AS score FROM bookmarks WHERE score > 0 ORDER BY score DESC)'
         else:
             LOGERR('Invalid search option')
-            return None
+            return []
 
         LOGDBG('query: "%s", args: %s', q0, qargs)
 
         try:
-            self.cur.execute(q0, qargs)
+            return self._fetch(q0, *qargs)
         except sqlite3.OperationalError as e:
             LOGERR(e)
-            return None
+            return []
 
-        return self.cur.fetchall()
-
-    def search_by_tag(self, tags: Optional[str]) -> Optional[List[BookmarkVar]]:
+    def search_by_tag(self, tags: Optional[str]) -> List[BookmarkVar]:
         """Search bookmarks for entries with given tags.
 
         Parameters
         ----------
         tags : str
             String of tags to search for.
             Retrieves entries matching ANY tag if tags are
             delimited with ','.
             Retrieves entries matching ALL tags if tags are
             delimited with '+'.
 
         Returns
         -------
-        list or None
-            List of search results, or None if no matches.
+        list
+            List of search results.
         """
 
         LOGDBG(tags)
         if tags is None or tags == DELIM or tags == '':
-            return None
+            return []
 
         tags_, search_operator, excluded_tags = prep_tag_search(tags)
         if search_operator is None:
             LOGERR("Cannot use both '+' and ',' in same search")
-            return None
+            return []
 
         LOGDBG('tags: %s', tags_)
         LOGDBG('search_operator: %s', search_operator)
         LOGDBG('excluded_tags: %s', excluded_tags)
 
         if search_operator == 'AND':
             query = ("SELECT id, url, metadata, tags, desc, flags FROM bookmarks "
@@ -1375,135 +1631,134 @@
             if excluded_tags:
                 tags_.append(excluded_tags)
                 query += ' AND tags NOT REGEXP ? '
 
             query += ' ORDER BY score DESC)'
 
         LOGDBG('query: "%s", args: %s', query, tags_)
-        self.cur.execute(query, tuple(tags_, ))
-        return self.cur.fetchall()
+        return self._fetch(query, *tags_)
 
     def search_keywords_and_filter_by_tags(
             self,
             keywords: List[str],
             all_keywords: bool,
             deep: bool,
             regex: bool,
-            stag: str) -> Optional[List[BookmarkVar]]:
+            stag: str) -> List[BookmarkVar]:
         """Search bookmarks for entries with keywords and specified
         criteria while filtering out entries with matching tags.
 
         Parameters
         ----------
         keywords : list of str
             Keywords to search.
-        all_keywords : bool, optional
+        all_keywords : bool
             True to return records matching ALL keywords.
             False to return records matching ANY keyword.
-        deep : bool, optional
+        deep : bool
             True to search for matching substrings.
-        regex : bool, optional
+        regex : bool
             Match a regular expression if True.
         stag : str
             String of tags to search for.
             Retrieves entries matching ANY tag if tags are
             delimited with ','.
             Retrieves entries matching ALL tags if tags are
             delimited with '+'.
 
         Returns
         -------
-        list or None
-            List of search results, or None if no matches.
+        list
+            List of search results.
         """
 
         keyword_results = self.searchdb(keywords, all_keywords, deep, regex)
-        keyword_results = keyword_results if keyword_results is not None else []
         stag_results = self.search_by_tag(''.join(stag))
-        stag_results = stag_results if stag_results is not None else []
         return list(set(keyword_results) & set(stag_results))
 
     def exclude_results_from_search(self, search_results, without, deep):
         """Excludes records that match keyword search using without parameters
 
         Parameters
         ----------
         search_results : list
             List of search results
         without : list of str
             Keywords to search.
-        deep : bool, optional
+        deep : bool
             True to search for matching substrings.
 
         Returns
         -------
-        list or None
-            List of search results, or None if no matches.
+        list
+            List of search results.
         """
 
         return list(set(search_results) - set(self.searchdb(without, False, deep)))
 
     def compactdb(self, index: int, delay_commit: bool = False):
         """When an entry at index is deleted, move the
         last entry in DB to index, if index is lesser.
 
         Parameters
         ----------
         index : int
             DB index of deleted entry.
-        delay_commit : bool, optional
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
         """
 
         # Return if the last index left in DB was just deleted
         max_id = self.get_max_id()
-        if max_id == -1:
+        if not max_id:
             return
 
         query1 = 'SELECT id, URL, metadata, tags, desc, flags FROM bookmarks WHERE id = ? LIMIT 1'
         query2 = 'DELETE FROM bookmarks WHERE id = ?'
         query3 = 'INSERT INTO bookmarks(id, URL, metadata, tags, desc, flags) VALUES (?, ?, ?, ?, ?, ?)'
 
         # NOOP if the just deleted index was the last one
         if max_id > index:
-            self.cur.execute(query1, (max_id,))
-            results = self.cur.fetchall()
+            results = self._fetch(query1, max_id)
             for row in results:
-                self.cur.execute(query2, (row[0],))
-                self.cur.execute(query3, (index, row[1], row[2], row[3], row[4], row[5]))
+                self.cur.execute(query2, (row.id,))
+                self.cur.execute(query3, (index, row.url, row.title, row.tags_raw, row.desc, row.flags))
                 if not delay_commit:
                     self.conn.commit()
                 if self.chatty:
-                    print('Index %d moved to %d' % (row[0], index))
+                    print('Index %d moved to %d' % (row.id, index))
 
     def delete_rec(
             self,
             index: int = None,
             low: int = 0,
             high: int = 0,
             is_range: bool = False,
-            delay_commit: bool = False
+            delay_commit: bool = False,
+            chatty: Optional[bool] = None,
     ) -> bool:
         """Delete a single record or remove the table if index is 0.
 
         Parameters
         ----------
         index : int, optional
             DB index of deleted entry.
-        low : int, optional
+        low : int
             Actual lower index of range.
-        high : int, optional
+        high : int
             Actual higher index of range.
-        is_range : bool, optional
+        is_range : bool
             A range is passed using low and high arguments.
             An index is ignored if is_range is True.
-        delay_commit : bool, optional
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
+        chatty : Optional[bool]
+            Override for self.chatty
 
         Raises
         ------
         TypeError
             If any of index, low, or high variable is not integer.
 
         Returns
@@ -1538,29 +1793,30 @@
         >>> sdb.add_rec('https://example.com')
         1
         >>> sdb.delete_rec()
         Traceback (most recent call last):
         ...
         TypeError: index, low, or high variable is not integer
 
-        Negative number on `high` and `low` paramaters when is_range is True
+        Negative number on `high` and `low` parameters when is_range is True
         will log error and return False
 
         >>> edb = buku.BukuDb(dbfile=NamedTemporaryFile().name)
         >>> edb.delete_rec(low=-1, high=-1, is_range=True)
         False
 
         Remove the table
 
         >>> sdb = buku.BukuDb(dbfile=NamedTemporaryFile().name)
         >>> sdb.delete_rec(0)  # doctest: +SKIP
         Remove ALL bookmarks? (y/n): y
         All bookmarks deleted
         True
         """
+        chatty = (chatty if chatty is not None else self.chatty)
         params = [low, high]
         if not is_range:
             params.append(index)
         if any(map(lambda x: not isinstance(x, int), params)):
             raise TypeError('index, low, or high variable is not integer')
 
         if is_range:  # Delete a range of indices
@@ -1572,15 +1828,15 @@
                 low, high = high, low
 
             # If range starts from 0, delete all records
             if low == 0:
                 return self.cleardb()
 
             try:
-                if self.chatty:
+                if chatty:
                     self.cur.execute('SELECT COUNT(*) from bookmarks where id '
                                      'BETWEEN ? AND ?', (low, high))
                     count = self.cur.fetchone()
                     if count[0] < 1:
                         print('Index %d-%d: 0 deleted' % (low, high))
                         return False
 
@@ -1606,15 +1862,15 @@
             except IndexError:
                 LOGERR('No matching index')
                 return False
         elif index == 0:  # Remove the table
             return self.cleardb()
         else:  # Remove a single entry
             try:
-                if self.chatty:
+                if chatty:
                     self.cur.execute('SELECT COUNT(*) FROM bookmarks WHERE '
                                      'id = ? LIMIT 1', (index,))
                     count = self.cur.fetchone()
                     if count[0] < 1:
                         LOGERR('No matching index %d', index)
                         return False
 
@@ -1681,15 +1937,15 @@
         return True
 
     def delete_rec_all(self, delay_commit=False):
         """Removes all records in the Bookmarks table.
 
         Parameters
         ----------
-        delay_commit : bool, optional
+        delay_commit : bool
             True if record should not be committed to the DB,
             leaving commit responsibility to caller. Default is False.
 
         Returns
         -------
         bool
             True on success, False on failure.
@@ -1722,30 +1978,32 @@
             self.cur.execute('VACUUM')
             self.conn.commit()
             print('All bookmarks deleted')
             return True
 
         return False
 
-    def print_rec(self, index: int = 0, low: int = 0, high: int = 0, is_range: bool = False) -> bool:
+    def print_rec(self, index: Optional[int | Sequence[int] | Set[int] | range] = 0,  # Optional[IntOrInts]
+                  low: int = 0, high: int = 0, is_range: bool = False) -> bool:
         """Print bookmark details at index or all bookmarks if index is 0.
 
         A negative index behaves like tail, if title is blank show "Untitled".
 
         Empty database check will run when `index` < 0 and `is_range` is False.
 
         Parameters
         -----------
-        index : int, optional
-            DB index of record to print. 0 prints all records.
-        low : int, optional
+        index : int | int[] | int{} | range, optional
+            DB index(es) of record(s) to print. 0 or empty prints all records.
+            Negative value prints out last `index` rows.
+        low : int
             Actual lower index of range.
-        high : int, optional
+        high : int
             Actual higher index of range.
-        is_range : bool, optional
+        is_range : bool
             A range is passed using low and high arguments.
             An index is ignored if is_range is True.
 
         Returns
         -------
         bool
             True on success, False on failure.
@@ -1769,32 +2027,34 @@
         >>> sdb.add_rec('https://example.com')
         1
         >>> assert sdb.print_rec()
         1. Example Domain
            > https://example.com
         <BLANKLINE>
 
-        Negative number on `high` and `low` paramaters when is_range is True
+        Negative number on `high` and `low` parameters when is_range is True
         will log error and return False
 
         >>> sdb.print_rec(low=-1, high=-1, is_range=True)
         False
         >>> edb.print_rec(low=-1, high=-1, is_range=True)
         False
         """
-        if not is_range and index < 0:
+        if isinstance(index, range) and index.step == 1:
+            return self.print_rec(None, is_range=True, low=index.start, high=index.stop)
+
+        if not is_range and isinstance(index, int) and index < 0:
             # Show the last n records
             _id = self.get_max_id()
-            if _id == -1:
+            if not _id:
                 LOGERR('Empty database')
                 return False
 
             low = (1 if _id <= -index else _id + index + 1)
-            high = _id
-            is_range = True
+            return self.print_rec(None, is_range=True, low=low, high=_id)
 
         if is_range:
             if low < 0 or high < 0:
                 LOGERR('Negative range boundary')
                 return False
 
             if low > high:
@@ -1807,36 +2067,37 @@
                     resultset = self.cur.execute(query)
                 else:
                     query = 'SELECT * from bookmarks where id BETWEEN ? AND ?'
                     resultset = self.cur.execute(query, (low, high))
             except IndexError:
                 LOGERR('Index out of range')
                 return False
-        elif index != 0:  # Show record at index
+        elif index:  # Show record at index
             try:
-                query = 'SELECT * FROM bookmarks WHERE id = ? LIMIT 1'
-                self.cur.execute(query, (index,))
-                results = self.cur.fetchall()
-                if not results:
-                    LOGERR('No matching index %d', index)
-                    return False
+                if isinstance(index, int):
+                    results = self._fetch('SELECT * FROM bookmarks WHERE id = ? LIMIT 1', index)
+                else:
+                    placeholder = ', '.join(['?'] * len(index))
+                    results = self._fetch(f'SELECT * FROM bookmarks WHERE id IN ({placeholder}) ORDER BY id', *index)
             except IndexError:
-                LOGERR('No matching index %d', index)
+                results = None
+            if not results:
+                LOGERR('No matching index %s', index)
                 return False
 
             if self.json is None:
                 print_rec_with_filter(results, self.field_filter)
             elif self.json:
                 write_string_to_file(format_json(results, True, self.field_filter), self.json)
             else:
                 print_json_safe(results, True, self.field_filter)
 
             return True
         else:  # Show all entries
-            self.cur.execute('SELECT * FROM bookmarks')
+            self.cur.execute('SELECT * FROM bookmarks ORDER BY id')
             resultset = self.cur.fetchall()
 
         if not resultset:
             LOGERR('0 records')
             return True
 
         if self.json is None:
@@ -1934,45 +2195,46 @@
                 tags.append(delim_wrap(unique_tags[int(index) - 1]))
             except Exception as e:
                 LOGERR(e)
                 continue
 
         return parse_tags(tags)
 
-    def replace_tag(self, orig: str, new: Optional[List[str]] = None) -> bool:
+    def replace_tag(self, orig: str, new: List[str] = []):
         """Replace original tag by new tags in all records.
 
         Remove original tag if new tag is empty.
 
         Parameters
         ----------
         orig : str
             Original tag.
         new : list
             Replacement tags.
 
-        Returns
+        Raises
         -------
-        bool
-            True on success, False on failure.
+        ValueError: Invalid input(s) provided.
+        RuntimeError: Tag deletion failed.
+
         """
 
-        newtags = DELIM
+        if DELIM in orig:
+            raise ValueError("Original tag cannot contain delimiter ({}).".format(DELIM))
 
         orig = delim_wrap(orig)
-        if new is not None:
-            newtags = parse_tags(new)
+        newtags = parse_tags([DELIM.join(new)])
 
         if orig == newtags:
-            print('Tags are same.')
-            return False
+            raise ValueError("Original and replacement tags are the same.")
 
         # Remove original tag from DB if new tagset reduces to delimiter
         if newtags == DELIM:
-            return self.delete_tag_at_index(0, orig)
+            if not self.delete_tag_at_index(0, orig):
+                raise RuntimeError("Tag deletion failed.")
 
         # Update bookmarks with original tag
         query = 'SELECT id, tags FROM bookmarks WHERE tags LIKE ?'
         self.cur.execute(query, ('%' + orig + '%',))
         results = self.cur.fetchall()
         if results:
             query = 'UPDATE bookmarks SET tags = ? WHERE id = ?'
@@ -1980,16 +2242,14 @@
                 tags = row[1].replace(orig, newtags)
                 tags = parse_tags([tags])
                 self.cur.execute(query, (tags, row[0],))
                 print('Index %d updated' % row[0])
 
             self.conn.commit()
 
-        return True
-
     def get_tagstr_from_taglist(self, id_list, taglist):
         """Get a string of delimiter-separated (and enclosed) string
         of tags from a dictionary of tags by matching ids.
 
         The inputs are the outputs from BukuDb.get_tag_all().
 
         Parameters
@@ -2181,33 +2441,35 @@
         except IndexError:
             LOGERR('No matching index %d', index)
 
         return False
 
     def exportdb(self, filepath: str, resultset: Optional[List[BookmarkVar]] = None) -> bool:
         """Export DB bookmarks to file.
-        Exports full DB, if resultset is None
+        Exports full DB, if resultset is None.
+        Additionally, if run after a (batch) update with export_on, only export those records.
 
         If destination file name ends with '.db', bookmarks are
         exported to a buku database file.
         If destination file name ends with '.md', bookmarks are
         exported to a Markdown file.
         If destination file name ends with '.org' bookmarks are
-        exported to a org file.
+        exported to an org file.
         If destination file name ends with '.xbel' bookmarks are
         exported to a XBEL file.
         Otherwise, bookmarks are exported to a Firefox bookmarks.html
         formatted file.
 
         Parameters
         ----------
         filepath : str
             Path to export destination file.
         resultset : list of tuples
-            List of results to export.
+            List of results to export. Use `None` to get current DB.
+            Ignored if run after a (batch) update with export_on.
 
 
         Returns
         -------
         bool
             True on success, False on failure.
         """
@@ -2216,49 +2478,63 @@
 
         if not resultset:
             resultset = self.get_rec_all()
             if not resultset:
                 print('No records found')
                 return False
 
+        old = self._to_export or {}
+        if self._to_export is not None:
+            _resultset = dict(old)
+            _resultset.update({x.url: x for x in resultset if x.url in old})
+            resultset = list(_resultset.values())
+            self._to_export = None
+            if not resultset:
+                print('No records to export')
+                return False
+
         if os.path.exists(filepath):
             resp = read_in(filepath + ' exists. Overwrite? (y/n): ')
             if resp != 'y':
                 return False
 
             if filepath.endswith('.db'):
                 os.remove(filepath)
 
         if filepath.endswith('.db'):
             outdb = BukuDb(dbfile=filepath)
             qry = 'INSERT INTO bookmarks(URL, metadata, tags, desc, flags) VALUES (?, ?, ?, ?, ?)'
             for row in resultset:
-                outdb.cur.execute(qry, (row[1], row[2], row[3], row[4], row[5]))
+                _old = old.get(row.url)
+                _add = (f' (OLD URL = {_old})' if isinstance(_old, str) and _old != row.url else
+                        ' (DELETED)' if _old is row else '')
+                title = ((row.title or '') + _add if _add else row.title)
+                outdb.cur.execute(qry, (row.url, title, row.tags_raw, row.desc, row.flags))
                 count += 1
             outdb.conn.commit()
             outdb.close()
             print('%s exported' % count)
             return True
 
         with open(filepath, mode='w', encoding='utf-8') as outfp:
             res = {}  # type: Dict
             if filepath.endswith('.md'):
-                res = convert_bookmark_set(resultset, 'markdown')
+                res = convert_bookmark_set(resultset, 'markdown', old)
                 count += res['count']
                 outfp.write(res['data'])
             elif filepath.endswith('.org'):
-                res = convert_bookmark_set(resultset, 'org')
+                res = convert_bookmark_set(resultset, 'org', old)
                 count += res['count']
                 outfp.write(res['data'])
             elif filepath.endswith('.xbel'):
-                res = convert_bookmark_set(resultset, 'xbel')
+                res = convert_bookmark_set(resultset, 'xbel', old)
                 count += res['count']
                 outfp.write(res['data'])
             else:
-                res = convert_bookmark_set(resultset, 'html')
+                res = convert_bookmark_set(resultset, 'html', old)
                 count += res['count']
                 outfp.write(res['data'])
             print('%s exported' % count)
             return True
         return False
 
     def traverse_bm_folder(self, sublist, unique_tag, folder_name, add_parent_folder_as_tag):
@@ -2279,21 +2555,20 @@
         -------
         tuple
             Bookmark record data.
         """
 
         for item in sublist:
             if item['type'] == 'folder':
-                next_folder_name = folder_name + ',' + item['name']
-                for i in self.traverse_bm_folder(
+                next_folder_name = folder_name + DELIM + strip_delim(item['name'])
+                yield from self.traverse_bm_folder(
                         item['children'],
                         unique_tag,
                         next_folder_name,
-                        add_parent_folder_as_tag):
-                    yield i
+                        add_parent_folder_as_tag)
             elif item['type'] == 'url':
                 try:
                     if is_nongeneric_url(item['url']):
                         continue
                 except KeyError:
                     continue
 
@@ -2379,22 +2654,19 @@
                         title, parent_id = parent
                         bookmark_tags.append(title)
 
             if unique_tag:
                 # add timestamp tag
                 bookmark_tags.append(unique_tag)
 
-            formatted_tags = [DELIM + tag for tag in bookmark_tags]
+            formatted_tags = [DELIM + strip_delim(tag) for tag in bookmark_tags]
             tags = parse_tags(formatted_tags)
 
             # get the title
-            if row[2]:
-                title = row[2]
-            else:
-                title = ''
+            title = row[2] or ''
 
             self.add_rec(url, title, tags, None, 0, True, False)
         try:
             cur.close()
             conn.close()
         except Exception as e:
             LOGERR(e)
@@ -2423,147 +2695,169 @@
             for item in self.traverse_bm_folder(
                     roots[entry]['children'],
                     unique_tag,
                     roots[entry]['name'],
                     add_parent_folder_as_tag):
                 self.add_rec(*item)
 
-    def auto_import_from_browser(self):
+    def auto_import_from_browser(self, firefox_profile=None):
         """Import bookmarks from a browser default database file.
 
-        Supports Firefox, Google Chrome and Microsoft Edge.
+        Supports Firefox, Google Chrome, Vivaldi, and Microsoft Edge.
 
         Returns
         -------
         bool
             True on success, False on failure.
         """
 
-        ff_bm_db_path = None
+        ff_bm_db_paths = {}
+        firefox_profile = firefox_profile and [firefox_profile]
 
         if sys.platform.startswith(('linux', 'freebsd', 'openbsd')):
             gc_bm_db_path = '~/.config/google-chrome/Default/Bookmarks'
             cb_bm_db_path = '~/.config/chromium/Default/Bookmarks'
+            vi_bm_db_path = '~/.config/vivaldi/Default/Bookmarks'
 
             default_ff_folder = os.path.expanduser('~/.mozilla/firefox')
-            profile = get_firefox_profile_name(default_ff_folder)
-            if profile:
-                ff_bm_db_path = '~/.mozilla/firefox/{}/places.sqlite'.format(profile)
+            profiles = firefox_profile or get_firefox_profile_names(default_ff_folder)
+            if profiles:
+                ff_bm_db_paths = {s: '~/.mozilla/firefox/{}/places.sqlite'.format(s)
+                                  for s in profiles}
 
             me_bm_db_path = '~/.config/microsoft-edge/Default/Bookmarks'
         elif sys.platform == 'darwin':
             gc_bm_db_path = '~/Library/Application Support/Google/Chrome/Default/Bookmarks'
             cb_bm_db_path = '~/Library/Application Support/Chromium/Default/Bookmarks'
+            vi_bm_db_path = '~/Library/Application Support/Vivaldi/Default/Bookmarks'
 
             default_ff_folder = os.path.expanduser('~/Library/Application Support/Firefox')
-            profile = get_firefox_profile_name(default_ff_folder)
-            if profile:
-                ff_bm_db_path = ('~/Library/Application Support/Firefox/'
-                                 '{}/places.sqlite'.format(profile))
+            profiles = firefox_profile or get_firefox_profile_names(default_ff_folder)
+            if profiles:
+                ff_bm_db_paths = {s: '~/Library/Application Support/Firefox/{}/places.sqlite'.format(s)
+                                  for s in profiles}
 
             me_bm_db_path = '~/Library/Application Support/Microsoft Edge/Default/Bookmarks'
         elif sys.platform == 'win32':
-            username = os.getlogin()
-
-            gc_bm_db_path = ('C:/Users/{}/AppData/Local/Google/Chrome/User Data/'
-                             'Default/Bookmarks'.format(username))
-            cb_bm_db_path = ('C:/Users/{}/AppData/Local/Chromium/User Data/'
-                             'Default/Bookmarks'.format(username))
-
-            default_ff_folder = 'C:/Users/{}/AppData/Roaming/Mozilla/Firefox/'.format(username)
-            profile = get_firefox_profile_name(default_ff_folder)
-            if profile:
-                ff_bm_db_path = os.path.join(default_ff_folder, '{}/places.sqlite'.format(profile))
+            gc_bm_db_path = os.path.expandvars('%LOCALAPPDATA%/Google/Chrome/User Data/Default/Bookmarks')
+            cb_bm_db_path = os.path.expandvars('%LOCALAPPDATA%/Chromium/User Data/Default/Bookmarks')
+            vi_bm_db_path = os.path.expandvars('%LOCALAPPDATA%/Vivaldi/User Data/Default/Bookmarks')
+
+            default_ff_folder = os.path.expandvars('%APPDATA%/Mozilla/Firefox/')
+            profiles = firefox_profile or get_firefox_profile_names(default_ff_folder)
+            if profiles:
+                ff_bm_db_paths = {s: os.path.join(default_ff_folder, '{}/places.sqlite'.format(s))
+                                  for s in profiles}
 
-            me_bm_db_path = ('C:/Users/{}/AppData/Local/Microsoft/Edge/User Data/'
-                             'Default/Bookmarks'.format(username))
+            me_bm_db_path = os.path.expandvars('%LOCALAPPDATA%/Microsoft/Edge/User Data/Default/Bookmarks')
         else:
             LOGERR('buku does not support {} yet'.format(sys.platform))
             self.close_quit(1)
 
         if self.chatty:
             resp = input('Generate auto-tag (YYYYMonDD)? (y/n): ')
             if resp == 'y':
                 newtag = gen_auto_tag()
             else:
                 newtag = None
             resp = input('Add parent folder names as tags? (y/n): ')
         else:
             newtag = None
             resp = 'y'
-        add_parent_folder_as_tag = (resp == 'y')
+        add_parent_folder_as_tag = resp == 'y'
 
         resp = 'y'
 
         try:
-            if self.chatty:
-                resp = input('Import bookmarks from google chrome? (y/n): ')
-            if resp == 'y':
-                bookmarks_database = os.path.expanduser(gc_bm_db_path)
-                if not os.path.exists(bookmarks_database):
-                    raise FileNotFoundError
-                self.load_chrome_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+            if os.path.isfile(os.path.expanduser(gc_bm_db_path)):
+                if self.chatty:
+                    resp = input('Import bookmarks from google chrome? (y/n): ')
+                if resp == 'y':
+                    bookmarks_database = os.path.expanduser(gc_bm_db_path)
+                    if not os.path.exists(bookmarks_database):
+                        raise FileNotFoundError
+                    self.load_chrome_database(bookmarks_database, newtag, add_parent_folder_as_tag)
         except Exception as e:
             LOGERR(e)
             print('Could not import bookmarks from google-chrome')
 
         try:
-            if self.chatty:
-                resp = input('Import bookmarks from chromium? (y/n): ')
-            if resp == 'y':
-                bookmarks_database = os.path.expanduser(cb_bm_db_path)
-                if not os.path.exists(bookmarks_database):
-                    raise FileNotFoundError
-                self.load_chrome_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+            if os.path.isfile(os.path.expanduser(cb_bm_db_path)):
+                if self.chatty:
+                    resp = input('Import bookmarks from chromium? (y/n): ')
+                if resp == 'y':
+                    bookmarks_database = os.path.expanduser(cb_bm_db_path)
+                    if not os.path.exists(bookmarks_database):
+                        raise FileNotFoundError
+                    self.load_chrome_database(bookmarks_database, newtag, add_parent_folder_as_tag)
         except Exception as e:
             LOGERR(e)
             print('Could not import bookmarks from chromium')
 
         try:
-            if self.chatty:
-                resp = input('Import bookmarks from Firefox? (y/n): ')
-            if resp == 'y':
-                bookmarks_database = os.path.expanduser(ff_bm_db_path)
-                if not os.path.exists(bookmarks_database):
-                    raise FileNotFoundError
-                self.load_firefox_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+            if os.path.isfile(os.path.expanduser(vi_bm_db_path)):
+                if self.chatty:
+                    resp = input('Import bookmarks from Vivaldi? (y/n): ')
+                if resp == 'y':
+                    bookmarks_database = os.path.expanduser(vi_bm_db_path)
+                    if not os.path.exists(bookmarks_database):
+                        raise FileNotFoundError
+                    self.load_chrome_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+        except Exception as e:
+            LOGERR(e)
+            print('Could not import bookmarks from Vivaldi')
+
+        try:
+            ff_bm_db_paths = {k: s for k, s in ff_bm_db_paths.items() if os.path.isfile(os.path.expanduser(s))}
+            for idx, (name, ff_bm_db_path) in enumerate(ff_bm_db_paths.items(), start=1):
+                if self.chatty:
+                    profile = ('' if len(ff_bm_db_paths) < 2 else
+                               f' profile {name} [{idx}/{len(ff_bm_db_paths)}]')
+                    resp = input(f'Import bookmarks from Firefox{profile}? (y/n): ')
+                if resp == 'y':
+                    bookmarks_database = os.path.expanduser(ff_bm_db_path)
+                    if not os.path.exists(bookmarks_database):
+                        raise FileNotFoundError
+                    self.load_firefox_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+                    break
         except Exception as e:
             LOGERR(e)
             print('Could not import bookmarks from Firefox.')
 
         try:
-            if self.chatty:
-                resp = input('Import bookmarks from microsoft edge? (y/n): ')
-            if resp == 'y':
-                bookmarks_database = os.path.expanduser(me_bm_db_path)
-                if not os.path.exists(bookmarks_database):
-                    raise FileNotFoundError
-                self.load_edge_database(bookmarks_database, newtag, add_parent_folder_as_tag)
+            if os.path.isfile(os.path.expanduser(me_bm_db_path)):
+                if self.chatty:
+                    resp = input('Import bookmarks from microsoft edge? (y/n): ')
+                if resp == 'y':
+                    bookmarks_database = os.path.expanduser(me_bm_db_path)
+                    if not os.path.exists(bookmarks_database):
+                        raise FileNotFoundError
+                    self.load_edge_database(bookmarks_database, newtag, add_parent_folder_as_tag)
         except Exception as e:
             LOGERR(e)
             print('Could not import bookmarks from microsoft-edge')
 
         self.conn.commit()
 
         if newtag:
             print('\nAuto-generated tag: %s' % newtag)
 
     def importdb(self, filepath, tacit=False):
-        """Import bookmarks from a HTML or a Markdown file.
+        """Import bookmarks from an HTML or a Markdown file.
 
         Supports Firefox, Google Chrome, and IE exported HTML bookmarks.
         Supports XBEL standard bookmarks.
         Supports Markdown files with extension '.md, .org'.
         Supports importing bookmarks from another buku database file.
 
         Parameters
         ----------
         filepath : str
             Path to file to import.
-        tacit : bool, optional
+        tacit : bool
             If True, no questions asked and folder names are automatically
             imported as tags from bookmarks HTML.
             If True, automatic timestamp tag is NOT added.
             Default is False.
 
         Returns
         -------
@@ -2587,15 +2881,15 @@
         elif filepath.endswith('org'):
             items = import_org(filepath=filepath, newtag=newtag)
         elif filepath.endswith('json'):
             if not tacit:
                 resp = input('Add parent folder names as tags? (y/n): ')
             else:
                 resp = 'y'
-            add_bookmark_folder_as_tag = (resp == 'y')
+            add_bookmark_folder_as_tag = resp == 'y'
             try:
                 with open(filepath, 'r', encoding='utf-8') as datafile:
                     data = json.load(datafile)
 
                 items = import_firefox_json(data, add_bookmark_folder_as_tag, newtag)
             except ValueError as e:
                 LOGERR("ff_json: JSON Decode Error: {}".format(e))
@@ -2658,15 +2952,15 @@
                     use_nested_folder_structure = True
 
             items = import_html(soup, add_parent_folder_as_tag, newtag, use_nested_folder_structure)
             infp.close()
 
         for item in items:
             add_rec_res = self.add_rec(*item)
-            if add_rec_res == -1 and append_tags_resp == 'y':
+            if not add_rec_res and append_tags_resp == 'y':
                 rec_id = self.get_rec_id(item[0])
                 self.append_tag_at_index(rec_id, item[2])
 
         self.conn.commit()
 
         if newtag:
             print('\nAuto-generated tag: %s' % newtag)
@@ -2695,41 +2989,41 @@
             indb_cur.execute('SELECT * FROM bookmarks')
         except Exception as e:
             LOGERR(e)
             return False
 
         resultset = indb_cur.fetchall()
         if resultset:
-            for row in resultset:
-                self.add_rec(row[1], row[2], row[3], row[4], row[5], True, False)
+            for row in bookmark_vars(resultset):
+                self.add_rec(row.url, row.title, row.tags_raw, row.desc, row.flags, True, False)
 
             self.conn.commit()
 
         try:
             indb_cur.close()
             indb_conn.close()
         except Exception:
             pass
 
         return True
 
     def tnyfy_url(
             self,
-            index: Optional[int] = 0,
+            index: Optional[int] = None,
             url: Optional[str] = None,
-            shorten: Optional[bool] = True) -> Optional[str]:
+            shorten: bool = True) -> Optional[str]:
         """Shorten a URL using Google URL shortener.
 
         Parameters
         ----------
         index : int, optional (if URL is provided)
-            DB index of the bookmark with the URL to shorten. Default is 0.
+            DB index of the bookmark with the URL to shorten. Default is None.
         url : str, optional (if index is provided)
             URL to shorten.
-        shorten : bool, optional
+        shorten : bool
             True to shorten, False to expand. Default is False.
 
         Returns
         -------
         str
             Shortened url on success, None on failure.
         """
@@ -2746,15 +3040,15 @@
             if not results:
                 return None
 
             url = results[0][0]
 
         from urllib.parse import quote_plus as qp
 
-        url = url if url is not None else ''
+        url = url or ''
         urlbase = 'https://tny.im/yourls-api.php?action='
         if shorten:
             _u = urlbase + 'shorturl&format=simple&url=' + qp(url)
         else:
             _u = urlbase + 'expand&format=simple&shorturl=' + qp(url)
 
         if MYPROXY is None:
@@ -2880,15 +3174,15 @@
                 pass
 
     def close_quit(self, exitval=0):
         """Close a DB connection and exit.
 
         Parameters
         ----------
-        exitval : int, optional
+        exitval : int
             Program exit value.
         """
 
         if self.conn is not None:
             try:
                 self.cur.close()
                 self.conn.close()
@@ -2903,39 +3197,39 @@
 
     @staticmethod
     def program_info(file=sys.stdout):
         """Print program info.
 
         Parameters
         ----------
-        file : file, optional
+        file : file
             File to write program info to. Default is sys.stdout.
         """
         if sys.platform == 'win32' and file == sys.stdout:
             file = sys.stderr
 
         file.write('''
 SYMBOLS:
       >                    url
       +                    comment
       #                    tags
 
 Version %s
-Copyright © 2015-2022 %s
+Copyright © 2015-2024 %s
 License: %s
 Webpage: https://github.com/jarun/buku
 ''' % (__version__, __author__, __license__))
 
     @staticmethod
     def prompt_help(file=sys.stdout):
         """Print prompt help.
 
         Parameters
         ----------
-        file : file, optional
+        file : file
             File to write program info to. Default is sys.stdout.
         """
         file.write('''
 PROMPT KEYS:
     1-N                    browse search result indices and/or ranges
     O [id|range [...]]     open search results/indices in GUI browser
                            toggle try GUI browser if no arguments
@@ -2987,15 +3281,15 @@
 
     # Help
     def print_help(self, file=sys.stdout):
         """Print help prompt.
 
         Parameters
         ----------
-        file : file, optional
+        file : file
             File to write program info to. Default is sys.stdout.
         """
         super().print_help(file)
         self.program_info(file)
 
 
 # ----------------
@@ -3008,80 +3302,80 @@
 
 def convert_tags_to_org_mode_tags(tags: str) -> str:
     """convert buku tags to org-mode compatible tags."""
     if tags != DELIM:
         buku_tags = tags.split(DELIM)[1:-1]
         buku_tags = [re.sub(r'[^a-zA-Z0-9_@]', ' ', tag) for tag in buku_tags]
         buku_tags = [re.sub(r'\s+', ' ', tag) for tag in buku_tags]
-        buku_tags = list(
-            sorted(set(map(lambda x: x.replace(' ', '_'), buku_tags)), reverse=False))
+        buku_tags = taglist(x.replace(' ', '_') for x in buku_tags)
         if buku_tags:
             return ' :{}:\n'.format(':'.join(buku_tags))
     return '\n'
 
 
 def convert_bookmark_set(
         bookmark_set: List[BookmarkVar],
-        export_type: str) -> ConverterResult:  # type: ignore
+        export_type: str,
+        old: Optional[Dict[str, str | BookmarkVar]] = None) -> ConverterResult:  # type: ignore
     """Convert list of bookmark set into multiple data format.
 
     Parameters
     ----------
         bookmark_set: bookmark set
-        export type: one of supported type: markdown, html, org, XBEL
+        export_type: one of supported type: markdown, html, org, XBEL
+        old: cached values of deleted records/replaced URLs to save
 
     Returns
     -------
         converted data and count of converted bookmark set
     """
     import html
     assert export_type in ['markdown', 'html', 'org', 'xbel']
     #  compatibility
-    resultset = bookmark_set
+    resultset = bookmark_vars(bookmark_set)
+    old = old or {}
+
+    def title(row, fallback=''):
+        _old = old.get(row.url)
+        _add = (f' (OLD URL = {_old})' if isinstance(_old, str) and _old != row.url else
+                ' (DELETED)' if _old == row else '')
+        return (row.title or fallback) + _add
 
     count = 0
     out = ''
     if export_type == 'markdown':
         for row in resultset:
-            if not row[2] or row[2] is None:
-                out += '- [Untitled](' + row[1] + ')'
-            else:
-                out += '- [' + row[2] + '](' + row[1] + ')'
+            out += '- [' + title(row, 'Untitled') + '](' + row.url + ')'
 
-            if row[3] != DELIM:
-                out += ' <!-- TAGS: {} -->\n'.format(row[3][1:-1])
+            if row.tags:
+                out += ' <!-- TAGS: {} -->\n'.format(row.tags)
             else:
                 out += '\n'
 
             count += 1
     elif export_type == 'org':
         for row in resultset:
-            if not row[2]:
-                out += '* [[{}][Untitled]]'.format(row[1])
-            else:
-                out += '* [[{}][{}]]'.format(row[1], row[2])
-            out += convert_tags_to_org_mode_tags(row[3])
+            out += '* [[{}][{}]]'.format(row.url, title(row, 'Untitled'))
+            out += convert_tags_to_org_mode_tags(row.tags_raw)
             count += 1
     elif export_type == 'xbel':
         timestamp = str(int(time.time()))
         out = (
             '<?xml version="1.0" encoding="UTF-8"?>\n'
-            '<!DOCTYPE xbel PUBLIC\
-"+//IDN python.org//DTD XML Bookmark Exchange Language 1.0//EN//XML"\
+            '<!DOCTYPE xbel PUBLIC \
+"+//IDN python.org//DTD XML Bookmark Exchange Language 1.0//EN//XML" \
 "http://pyxml.sourceforge.net/topics/dtds/xbel.dtd">\n'
-            '<xbel version="1.0">\n'
-            '    <title ADD_DATE="{0}" LAST_MODIFIED="{0}" '
-            'PERSONAL_TOOLBAR_FOLDER="true">buku bookmarks</title>\n'.format(timestamp))
+            '<xbel version="1.0">\n')
 
         for row in resultset:
-            out += '<bookmark href="%s"' % (html.escape(row[1])).encode('ascii', 'xmlcharrefreplace').decode('utf-8')
-            if row[3] != DELIM:
-                out += ' TAGS="' + html.escape(row[3][1:-1]).encode('ascii', 'xmlcharrefreplace').decode('utf-8') + '"'
+            out += '<bookmark href="%s"' % (html.escape(row.url)).encode('ascii', 'xmlcharrefreplace').decode('utf-8')
+            if row.tags:
+                out += ' TAGS="' + html.escape(row.tags).encode('ascii', 'xmlcharrefreplace').decode('utf-8') + '"'
             out += '>\n<title>{}</title>\n</bookmark>\n'\
-                .format(html.escape(row[2]).encode('ascii', 'xmlcharrefreplace').decode('utf-8') if row[2] else '')
+                .format(html.escape(title(row)).encode('ascii', 'xmlcharrefreplace').decode('utf-8'))
             count += 1
 
         out += '</xbel>'
     elif export_type == 'html':
         timestamp = str(int(time.time()))
         out = (
             '<!DOCTYPE NETSCAPE-Bookmark-file-1>\n\n'
@@ -3090,73 +3384,73 @@
             '<H1>Bookmarks</H1>\n\n'
             '<DL><p>\n'
             '    <DT><H3 ADD_DATE="{0}" LAST_MODIFIED="{0}" '
             'PERSONAL_TOOLBAR_FOLDER="true">buku bookmarks</H3>\n'
             '    <DL><p>\n'.format(timestamp))
 
         for row in resultset:
-            out += '        <DT><A HREF="%s" ADD_DATE="%s" LAST_MODIFIED="%s"' % (row[1], timestamp, timestamp)
-            if row[3] != DELIM:
-                out += ' TAGS="' + row[3][1:-1] + '"'
-            out += '>{}</A>\n'.format(row[2] if row[2] else '')
-            if row[4] != '':
-                out += '        <DD>' + row[4] + '\n'
+            out += '        <DT><A HREF="%s" ADD_DATE="%s" LAST_MODIFIED="%s"' % (row.url, timestamp, timestamp)
+            if row.tags:
+                out += ' TAGS="' + row.tags + '"'
+            out += '>{}</A>\n'.format(title(row))
+            if row.desc:
+                out += '        <DD>' + row.desc + '\n'
             count += 1
 
         out += '    </DL><p>\n</DL><p>'
 
     return {'data': out, 'count': count}
 
 
-def get_firefox_profile_name(path):
-    """List folder and detect default Firefox profile name.
+def get_firefox_profile_names(path):
+    """List folder and detect default Firefox profile names for all installs.
 
     Returns
     -------
-    profile : str
-        Firefox profile name.
+    profiles : [str]
+        All default Firefox profile names.
     """
     from configparser import ConfigParser, NoOptionError
 
+    profiles = []
     profile_path = os.path.join(path, 'profiles.ini')
     if os.path.exists(profile_path):
         config = ConfigParser()
         config.read(profile_path)
 
         install_names = [section for section in config.sections() if section.startswith('Install')]
         for name in install_names:
             try:
-                profile_path = config.get(name, 'default')
-                return profile_path
+                profiles += [config.get(name, 'default')]
             except NoOptionError:
                 pass
+        if profiles:
+            return profiles
 
         profiles_names = [section for section in config.sections() if section.startswith('Profile')]
-        if not profiles_names:
-            return None
         for name in profiles_names:
             try:
                 # If profile is default
                 if config.getboolean(name, 'default'):
-                    profile_path = config.get(name, 'path')
-                    return profile_path
+                    profiles += [config.get(name, 'path')]
+                    continue
             except NoOptionError:
                 pass
             try:
                 # alternative way to detect default profile
                 if config.get(name, 'name').lower() == "default":
-                    profile_path = config.get(name, 'path')
-                    return profile_path
+                    profiles += [config.get(name, 'path')]
             except NoOptionError:
                 pass
 
-        # There is no default profile
-        return None
-    LOGDBG('get_firefox_profile_name(): {} does not exist'.format(path))
-    return None
+        return profiles
+
+    # There are no default profiles
+    LOGDBG('get_firefox_profile_names(): {} does not exist'.format(path))
+    return profiles
 
 
 def walk(root):
     """Recursively iterate over JSON.
 
     Parameters
     ----------
@@ -3470,16 +3764,16 @@
 
         if comment_tag:
             desc = comment_tag.find(text=True, recursive=False)
 
         if add_parent_folder_as_tag:
             # add parent folder as tag
             if use_nested_folder_structure:
-                # New method that would generalize for else case too
-                # Stucture of folders
+                # New method that would generalize for else case to
+                # structure of folders
                 # folder
                 #   title (folder name)
                 #   folder
                 #       title
                 #           bookmark (could be h3, and continue recursively)
                 parents = tag.find_parents('folder')
                 for parent in parents:
@@ -3547,53 +3841,53 @@
         except KeyError:
             continue
 
         desc = None
         comment_tag = tag.findNextSibling('dd')
 
         if comment_tag:
-            desc = comment_tag.find(text=True, recursive=False)
+            desc = comment_tag.find(string=True, recursive=False)
 
         if add_parent_folder_as_tag:
             # add parent folder as tag
             if use_nested_folder_structure:
-                # New method that would generalize for else case too
-                # Stucture of folders
+                # New method that would generalize for else case to
+                # structure of folders
                 # dt
                 #   h3 (folder name)
                 #   dl
                 #       dt
                 #           a (could be h3, and continue recursively)
                 parents = tag.find_parents('dl')
                 for parent in parents:
                     header = parent.find_previous_sibling('h3')
                     if header:
                         if tag.has_attr('tags'):
-                            tag['tags'] += (DELIM + header.text)
+                            tag['tags'] += (DELIM + strip_delim(header.text))
                         else:
-                            tag['tags'] = header.text
+                            tag['tags'] = strip_delim(header.text)
             else:
                 # could be its folder or not
                 possible_folder = tag.find_previous('h3')
                 # get list of tags within that folder
                 tag_list = tag.parent.parent.find_parent('dl')
 
                 if ((possible_folder) and possible_folder.parent in list(tag_list.parents)):
                     # then it's the folder of this bookmark
                     if tag.has_attr('tags'):
-                        tag['tags'] += (DELIM + possible_folder.text)
+                        tag['tags'] += (DELIM + strip_delim(possible_folder.text))
                     else:
-                        tag['tags'] = possible_folder.text
+                        tag['tags'] = strip_delim(possible_folder.text)
 
         # add unique tag if opted
         if newtag:
             if tag.has_attr('tags'):
-                tag['tags'] += (DELIM + newtag)
+                tag['tags'] += (DELIM + strip_delim(newtag))
             else:
-                tag['tags'] = newtag
+                tag['tags'] = strip_delim(newtag)
 
         yield (
             tag['href'], tag.string,
             parse_tags([tag['tags']]) if tag.has_attr('tags') else None,
             desc if not desc else desc.strip(), 0, True, False
         )
 
@@ -3655,14 +3949,15 @@
 
     ignored_prefix = [
         'about:',
         'apt:',
         'chrome://',
         'file://',
         'place:',
+        'vivaldi://',
     ]
 
     for prefix in ignored_prefix:
         if url.startswith(prefix):
             return True
 
     return False
@@ -3728,17 +4023,17 @@
 
     Returns
     -------
     tuple
         (title, description, keywords).
     """
 
-    title = None
-    desc = None
-    keys = None
+    title = ''
+    desc = ''
+    keys = ''
 
     soup = BeautifulSoup(page, 'html5lib')
 
     try:
         title = soup.find('title').text.strip().replace('\n', ' ')
         if title:
             title = re.sub(r'\s{2,}', ' ', title)
@@ -3771,23 +4066,23 @@
                 if keys not in (title, desc):
                     LOGDBG('keywords to description: %s', keys)
                     if desc:
                         desc = desc + '\n## ' + keys
                     else:
                         desc = '* ' + keys
 
-                keys = None
+                keys = ''
     except Exception as e:
         LOGDBG(e)
 
     LOGDBG('title: %s', title)
     LOGDBG('desc : %s', desc)
     LOGDBG('keys : %s', keys)
 
-    return (title, desc, keys)
+    return (title, desc, keys and keys.strip(DELIM))
 
 
 def get_data_from_page(resp):
     """Detect HTTP response encoding and invoke parser with decoded data.
 
     Parameters
     ----------
@@ -3797,33 +4092,21 @@
     Returns
     -------
     tuple
         (title, description, keywords).
     """
 
     try:
-        soup = BeautifulSoup(resp.data, 'html.parser')
-    except Exception as e:
-        LOGERR('get_data_from_page(): %s', e)
+        charset = EncodingDetector.find_declared_encoding(resp.data, is_html=True)
 
-    try:
-        charset = None
-
-        if soup.meta and soup.meta.get('charset') is not None:
-            charset = soup.meta.get('charset')
-        elif 'content-type' in resp.headers:
-            _, params = cgi.parse_header(resp.headers['content-type'])
-            if params.get('charset') is not None:
-                charset = params.get('charset')
-
-        if not charset and soup:
-            meta_tag = soup.find('meta', attrs={'http-equiv': 'Content-Type'})
-            if meta_tag:
-                _, params = cgi.parse_header(meta_tag.attrs['content'])
-                charset = params.get('charset', charset)
+        if not charset and 'content-type' in resp.headers:
+            m = email.message.Message()
+            m['content-type'] = resp.headers['content-type']
+            if m.get_param('charset') is not None:
+                charset = m.get_param('charset')
 
         if charset:
             LOGDBG('charset: %s', charset)
             title, desc, keywords = parse_decoded_page(resp.data.decode(charset, errors='replace'))
         else:
             title, desc, keywords = parse_decoded_page(resp.data.decode(errors='replace'))
 
@@ -3882,96 +4165,120 @@
         timeout=15,
         cert_reqs='CERT_REQUIRED',
         ca_certs=ca_certs)
 
 
 def network_handler(
         url: str,
-        http_head: Optional[bool] = False
-) -> Tuple[Optional[str], Optional[str], Optional[str], int, int]:
+        http_head: bool = False
+) -> Tuple[str, str, str, int, int]:
+    """Handle server connection and redirections.
+
+    Deprecated; use fetch_data() instead.
+
+    Returns
+    -------
+    tuple
+        (title, description, tags, recognized mime, bad url)
+    """
+    warn('\'buku.network_handler()\' is deprecated; use \'buku.fetch_data()\' instead.', DeprecationWarning)
+    result = fetch_data(url, http_head)
+    return (result.title, result.desc, result.keywords, int(result.mime), int(result.bad))
+
+
+def fetch_data(
+        url: str,
+        http_head: bool = False
+) -> FetchResult:
     """Handle server connection and redirections.
 
     Parameters
     ----------
     url : str
         URL to fetch.
     http_head : bool
         If True, send only HTTP HEAD request. Default is False.
 
     Returns
     -------
-    tuple
-        (title, description, tags, recognized mime, bad url).
+    FetchResult
+        (url, title, desc, keywords, mime, bad, fetch_status)
     """
 
-    page_title = None
-    page_desc = None
-    page_keys = None
+    page_status = None
+    page_url = url
+    page_title = ''
+    page_desc = ''
+    page_keys = ''
     exception = False
 
     if is_nongeneric_url(url) or is_bad_url(url):
-        return (None, None, None, 0, 1)
+        return FetchResult(url, bad=True)
 
     if is_ignored_mime(url) or http_head:
         method = 'HEAD'
     else:
         method = 'GET'
 
     if not MYHEADERS:
         gen_headers()
 
     try:
         manager = get_PoolManager()
 
         while True:
             resp = manager.request(method, url, retries=Retry(redirect=10))
+            page_status = resp.status
 
             if resp.status == 200:
                 if method == 'GET':
+                    for retry in resp.retries.history:
+                        if retry.status not in PERMANENT_REDIRECTS:
+                            break
+                        page_status, page_url = retry.status, retry.redirect_location
                     page_title, page_desc, page_keys = get_data_from_page(resp)
             elif resp.status == 403 and url.endswith('/'):
                 # HTTP response Forbidden
                 # Handle URLs in the form of https://www.domain.com/
                 # which fail when trying to fetch resource '/'
                 # retry without trailing '/'
 
                 LOGDBG('Received status 403: retrying...')
                 # Remove trailing /
                 url = url[:-1]
                 resp.close()
                 continue
             else:
+                page_title, page_desc, page_keys = get_data_from_page(resp)
                 LOGERR('[%s] %s', resp.status, resp.reason)
 
             if resp:
                 resp.close()
 
             break
     except Exception as e:
-        LOGERR('network_handler(): %s', e)
+        LOGERR('fetch_data(): %s', e)
         exception = True
-    finally:
-        if manager:
-            manager.clear()
-        if exception:
-            return (None, None, None, 0, 0)
-        if method == 'HEAD':
-            return ('', '', '', 1, 0)
-        if page_title is None:
-            return ('', page_desc, page_keys, 0, 0)
 
-        return (page_title, page_desc, page_keys, 0, 0)
+    if manager:
+        manager.clear()
+    if exception:
+        return FetchResult(url)
+    if method == 'HEAD':
+        return FetchResult(url, mime=True, fetch_status=page_status)
+
+    return FetchResult(page_url, title=page_title, desc=page_desc, keywords=page_keys, fetch_status=page_status)
 
 
 def parse_tags(keywords=[]):
     """Format and get tag string from tokens.
 
     Parameters
     ----------
-    keywords : list, optional
+    keywords : list
         List of tags to parse. Default is empty list.
 
     Returns
     -------
     str
         Comma-delimited string of tags.
     DELIM : str
@@ -3979,15 +4286,15 @@
     None
         If keywords is None.
     """
 
     if keywords is None:
         return None
 
-    if not keywords or len(keywords) < 1 or not keywords[0]:
+    if not keywords or not keywords[0]:
         return DELIM
 
     tags = DELIM
 
     # Cleanse and get the tags
     tagstr = ' '.join(keywords)
     marker = tagstr.find(DELIM)
@@ -4008,22 +4315,16 @@
 
     LOGDBG('keywords: %s', keywords)
     LOGDBG('parsed tags: [%s]', tags)
 
     if tags == DELIM:
         return tags
 
-    # original tags in lower case
-    orig_tags = tags.lower().strip(DELIM).split(DELIM)
-
-    # Create list of unique tags and sort
-    unique_tags = sorted(set(orig_tags))
-
-    # Wrap with delimiter
-    return delim_wrap(DELIM.join(unique_tags))
+    # sorted unique tags in lowercase, wrapped with delimiter
+    return taglist_str(tags)
 
 
 def prep_tag_search(tags: str) -> Tuple[List[str], Optional[str], Optional[str]]:
     """Prepare list of tags to search and determine search operator.
 
     Parameters
     ----------
@@ -4099,15 +4400,15 @@
 
     Parameters
     ----------
     obj : BukuDb instance
         A valid instance of BukuDb class.
     nav : str
         Navigation command argument passed at prompt by user.
-    suggest : bool, optional
+    suggest : bool
         If True, suggest similar tags on new bookmark addition.
     """
 
     if nav == 'w':
         editor = get_system_editor()
         if not is_editor_valid(editor):
             return
@@ -4151,23 +4452,23 @@
 
     Parameters
     ----------
     obj : BukuDb instance
         A valid instance of BukuDb class.
     results : list
         Search result set from a DB query.
-    noninteractive : bool, optional
+    noninteractive : bool
         If True, does not seek user input. Shows all results. Default is False.
-    deep : bool, optional
+    deep : bool
         Use deep search. Default is False.
-    listtags : bool, optional
+    listtags : bool
         If True, list all tags.
-    suggest : bool, optional
+    suggest : bool
         If True, suggest similar tags on edit and add bookmark.
-    num : int, optional
+    num : int
         Number of results to show per page. Default is 10.
     """
 
     if not isinstance(obj, BukuDb):
         LOGERR('Not a BukuDb instance')
         return
 
@@ -4186,16 +4487,15 @@
     if noninteractive:
         try:
             for row in results:
                 count += 1
                 print_single_rec(row, count, columns)
         except Exception:
             pass
-        finally:
-            return
+        return
 
     while True:
         if new_results or nav == 'n':
             count = 0
 
             if results:
                 total_results = len(results)
@@ -4466,128 +4766,105 @@
     by using the --format option.
 
     Parameters
     ----------
     records : list or sqlite3.Cursor object
         List of bookmark records to print
     field_filter : int
-        Integer indicating which fields to print.
+        Integer indicating which fields to print. Default is 0 ("all fields").
     """
 
     try:
-        if field_filter == 0:
-            for row in records:
-                try:
-                    columns, _ = os.get_terminal_size()
-                except OSError:
-                    columns = 0
-                print_single_rec(row, columns=columns)
-        elif field_filter == 1:
-            for row in records:
-                print('%s\t%s' % (row[0], row[1]))
-        elif field_filter == 2:
-            for row in records:
-                print('%s\t%s\t%s' % (row[0], row[1], row[3][1:-1]))
-        elif field_filter == 3:
+        records = bookmark_vars(records)
+        fields = FIELD_FILTER.get(field_filter)
+        if fields:
+            pattern = '\t'.join('%s' for k in fields)
             for row in records:
-                print('%s\t%s' % (row[0], row[2]))
-        elif field_filter == 4:
-            for row in records:
-                print('%s\t%s\t%s\t%s' % (row[0], row[1], row[2], row[3][1:-1]))
-        elif field_filter == 5:
-            for row in records:
-                print('%s\t%s\t%s' % (row[0], row[2], row[3][1:-1]))
-        elif field_filter == 10:
-            for row in records:
-                print(row[1])
-        elif field_filter == 20:
-            for row in records:
-                print('%s\t%s' % (row[1], row[3][1:-1]))
-        elif field_filter == 30:
-            for row in records:
-                print(row[2])
-        elif field_filter == 40:
-            for row in records:
-                print('%s\t%s\t%s' % (row[1], row[2], row[3][1:-1]))
-        elif field_filter == 50:
+                print(pattern % tuple(getattr(row, k) for k in fields))
+        else:
+            try:
+                columns, _ = os.get_terminal_size()
+            except OSError:
+                columns = 0
             for row in records:
-                print('%s\t%s' % (row[2], row[3][1:-1]))
+                print_single_rec(row, columns=columns)
     except BrokenPipeError:
         sys.stdout = os.fdopen(1)
         sys.exit(1)
 
 
-def print_single_rec(row: BookmarkVar, idx: Optional[int]=0, columns: Optional[int]=0):  # NOQA
+def print_single_rec(row: BookmarkVar, idx: int=0, columns: int=0):  # NOQA
     """Print a single DB record.
 
     Handles both search results and individual record.
 
     Parameters
     ----------
     row : tuple
         Tuple representing bookmark record data.
-    idx : int, optional
+    idx : int
         Search result index. If 0, print with DB index.
         Default is 0.
-    columns : int, optional
+    columns : int
         Number of columns to wrap comments to.
         Default is 0.
     """
 
     str_list = []
+    row = BookmarkVar(*row)  # ensuring named tuple
 
     # Start with index and title
     if idx != 0:
-        id_title_res = ID_STR % (idx, row[2] if row[2] else 'Untitled', row[0])
+        id_title_res = ID_STR % (idx, row.title or 'Untitled', row.id)
     else:
-        id_title_res = ID_DB_STR % (row[0], row[2] if row[2] else 'Untitled')
+        id_title_res = ID_DB_STR % (row.id, row.title or 'Untitled')
         # Indicate if record is immutable
-        if row[5] & 1:
-            id_title_res = MUTE_STR % (id_title_res)
+        if row.immutable:
+            id_title_res = MUTE_STR % (id_title_res,)
         else:
             id_title_res += '\n'
 
     try:
         print(id_title_res, end='')
-        print(URL_STR % (row[1]), end='')
+        print(URL_STR % (row.url,), end='')
         if columns == 0:
-            if row[4]:
-                print(DESC_STR % (row[4]), end='')
-            if row[3] != DELIM:
-                print(TAG_STR % (row[3][1:-1]), end='')
+            if row.desc:
+                print(DESC_STR % (row.desc,), end='')
+            if row.tags:
+                print(TAG_STR % (row.tags,), end='')
             print()
             return
 
         INDENT = 5
         ln_num = 1
         fillwidth = columns - INDENT
 
-        for line in textwrap.wrap(row[4].replace('\n', ''), width=fillwidth):
+        for line in textwrap.wrap(row.desc.replace('\n', ''), width=fillwidth):
             if ln_num == 1:
                 print(DESC_STR % line, end='')
                 ln_num += 1
             else:
                 print(DESC_WRAP % (' ' * INDENT, line))
 
         ln_num = 1
-        for line in textwrap.wrap(row[3][1:-1].replace('\n', ''), width=fillwidth):
+        for line in textwrap.wrap(row.tags.replace('\n', ''), width=fillwidth):
             if ln_num == 1:
                 print(TAG_STR % line, end='')
                 ln_num += 1
             else:
                 print(TAG_WRAP % (' ' * INDENT, line))
         print()
     except UnicodeEncodeError:
         str_list = []
         str_list.append(id_title_res)
-        str_list.append(URL_STR % (row[1]))
-        if row[4]:
-            str_list.append(DESC_STR % (row[4]))
-        if row[3] != DELIM:
-            str_list.append(TAG_STR % (row[3][1:-1]))
+        str_list.append(URL_STR % (row.url,))
+        if row.desc:
+            str_list.append(DESC_STR % (row.desc,))
+        if row.tags:
+            str_list.append(TAG_STR % (row.tags,))
         sys.stdout.buffer.write((''.join(str_list) + '\n').encode('utf-8'))
     except BrokenPipeError:
         sys.stdout = os.fdopen(1)
         sys.exit(1)
 
 
 def write_string_to_file(content: str, filepath: str):
@@ -4612,81 +4889,45 @@
 def format_json(resultset, single_record=False, field_filter=0):
     """Return results in JSON format.
 
     Parameters
     ----------
     resultset : list
         Search results from DB query.
-    single_record : bool, optional
+    single_record : bool
         If True, indicates only one record. Default is False.
-    field_filter : int, optional
-        Indicates format for displaying bookmarks. Default is 0.
+    field_filter : int
+        Indicates format for displaying bookmarks. Default is 0 ("all fields").
 
     Returns
     -------
     json
         Record(s) in JSON format.
     """
 
+    resultset = bookmark_vars(resultset)
+    fields = [(k, JSON_FIELDS.get(k, k)) for k in FIELD_FILTER.get(field_filter, ALL_FIELDS)]
+    marks = [{field: getattr(row, k) for k, field in fields} for row in resultset]
     if single_record:
-        marks = {}
-        for row in resultset:
-            if field_filter == 1:
-                marks['uri'] = row[1]
-            elif field_filter == 2:
-                marks['uri'] = row[1]
-                marks['tags'] = row[3][1:-1]
-            elif field_filter == 3:
-                marks['title'] = row[2]
-            elif field_filter == 4:
-                marks['uri'] = row[1]
-                marks['tags'] = row[3][1:-1]
-                marks['title'] = row[2]
-            else:
-                marks['index'] = row[0]
-                marks['uri'] = row[1]
-                marks['title'] = row[2]
-                marks['description'] = row[4]
-                marks['tags'] = row[3][1:-1]
-    else:
-        marks = []
-        for row in resultset:
-            if field_filter == 1:
-                record = {'uri': row[1]}
-            elif field_filter == 2:
-                record = {'uri': row[1], 'tags': row[3][1:-1]}
-            elif field_filter == 3:
-                record = {'title': row[2]}
-            elif field_filter == 4:
-                record = {'uri': row[1], 'title': row[2], 'tags': row[3][1:-1]}
-            else:
-                record = {
-                    'index': row[0],
-                    'uri': row[1],
-                    'title': row[2],
-                    'description': row[4],
-                    'tags': row[3][1:-1]
-                }
-
-            marks.append(record)
+        marks = marks[-1] if marks else {}
 
     return json.dumps(marks, sort_keys=True, indent=4)
 
 
 def print_json_safe(resultset, single_record=False, field_filter=0):
     """Prints json results and handles IOError
 
     Parameters
     ----------
     resultset : list
         Search results from DB query.
-    single_record : bool, optional
+    single_record : bool
         If True, indicates only one record. Default is False.
-    field_filter : int, optional
-        Indicates format for displaying bookmarks. Default is 0.
+    field_filter : int
+        Indicates format for displaying bookmarks. Default is 0 ("all fields").
 
     Returns
     -------
     None
     """
 
     try:
@@ -4755,14 +4996,16 @@
         for name in [b for b in webbrowser._tryorder if b not in TEXT_BROWSERS]:
             browser = webbrowser.get(name)
             LOGDBG(browser)
 
             # Found a GUI browser, suppress browser output
             browse.suppress_browser_output = True
             break
+    if sys.platform == 'win32':  # GUI apps have no terminal IO on Windows
+        browse.suppress_browser_output = False
 
     if browse.suppress_browser_output:
         _stderr = os.dup(2)
         os.close(2)
         _stdout = os.dup(1)
         if "microsoft" not in platform.uname()[3].lower():
             os.close(1)
@@ -5305,18 +5548,64 @@
     def textwrap_fill(text, width=70, **kwargs):
         return '\n'.join(textwrap_wrap(text, width=width, **kwargs))
     textwrap.wrap = textwrap_wrap
     textwrap.fill = textwrap_fill
     textwrap.wrap.patched = True
     textwrap.fill.patched = True
 
+
+def parse_range(tokens: Optional[str | Sequence[str] | Set[str]],  # Optional[str | Values[str]]
+                valid: Optional[Callable[[int], bool]] = None) -> Optional[Set[int]]:
+    """Convert a token or sequence/set of token into a set of indices.
+
+    Raises a ValueError on invalid token. Returns None if passed None as tokens.
+
+    Parameters
+    ----------
+    tokens : str | str[] | str{}, optional
+        String(s) containing an index (#), or a range (#-#), or a comma-separated list thereof.
+    valid : (int) -> bool, optional
+        Additional check for invalid indices (default is None).
+
+    Returns
+    -------
+    Optional[Set[int]]
+        None if tokens is None, otherwise parsed indices as unordered set.
+    """
+    if tokens is None:
+        return None
+    result = set()
+    for token in ([tokens] if isinstance(tokens, str) else tokens):
+        for idx in token.split(','):
+            if is_int(idx):
+                result |= {int(idx)}
+            elif '-' in idx:
+                l, r = map(int, idx.split('-'))
+                if l > r:
+                    l, r = r, l
+                result |= set(range(l, r + 1))
+            elif idx:
+                raise ValueError(f'Invalid token: {idx}')
+    if valid and any(not valid(idx) for idx in result):
+        raise ValueError('Not a valid range')
+    return result
+
+
 # main starts here
 def main():
     """Main."""
     global ID_STR, ID_DB_STR, MUTE_STR, URL_STR, DESC_STR, DESC_WRAP, TAG_STR, TAG_WRAP, PROMPTMSG
+    # readline should not be loaded when buku is used as a library
+    import readline
+    if sys.platform == 'win32':
+        try:
+            import colorama
+            colorama.just_fix_windows_console()  # noop on non-Windows systems
+        except ImportError:
+            pass
 
     title_in = None
     tags_in = None
     desc_in = None
     pipeargs = []
     colorstr_env = os.getenv('BUKU_COLORS')
 
@@ -5395,15 +5684,17 @@
     --immutable N        disable web-fetch during auto-refresh
                          N=0: mutable (default), N=1: immutable''')
     addarg = edit_grp.add_argument
     addarg('--url', nargs=1, help=hide)
     addarg('--tag', nargs='*', help=hide)
     addarg('--title', nargs='*', help=hide)
     addarg('-c', '--comment', nargs='*', help=hide)
-    addarg('--immutable', type=int, default=-1, choices={0, 1}, help=hide)
+    addarg('--immutable', type=int, choices={0, 1}, help=hide)
+    _bool = lambda x: x if x is None else bool(x)
+    _immutable = lambda args: _bool(args.immutable)
 
     # --------------------
     # SEARCH OPTIONS GROUP
     # --------------------
 
     search_grp = argparser.add_argument_group(
         title='SEARCH OPTIONS',
@@ -5444,25 +5735,28 @@
 
     # ----------------
     # POWER TOYS GROUP
     # ----------------
 
     power_grp = argparser.add_argument_group(
         title='POWER TOYS',
-        description='''    --ai                 auto-import (Firefox/Chrome/Chromium/Edge)
+        description='''    --ai                 auto-import bookmarks from web browsers
+                         Firefox, Chrome, Chromium, Vivaldi, Edge
+                         (Firefox profile can be specified using
+                         environment variable FIREFOX_PROFILE)
     -e, --export file    export bookmarks to Firefox format HTML
                          export XBEL, if file ends with '.xbel'
                          export Markdown, if file ends with '.md'
                          format: [title](url) <!-- TAGS -->
                          export Orgfile, if file ends with '.org'
                          format: *[[url][title]] :tags:
                          export buku DB, if file ends with '.db'
                          combines with search results, if opted
-    -i, --import file    import bookmarks based on file extension
-                         supports 'html', 'xbel', 'json', 'md', 'org', 'db'
+    -i, --import file    import bookmarks from file
+                         supports .html .xbel .json .md .org .db
     -p, --print [...]    show record details by indices, ranges
                          print all bookmarks, if no arguments
                          -n shows the last n results (like tail)
     -f, --format N       limit fields in -p or JSON search output
                          N=1: URL; N=2: URL, tag; N=3: title;
                          N=4: URL, title, tag; N=5: title, tag;
                          N0 (10, 20, 30, 40, 50) omits DB index
@@ -5474,17 +5768,34 @@
     -n, --count N        show N results per page (default 10)
     --np                 do not show the subprompt, run and exit
     -o, --open [...]     browse bookmarks by indices and ranges
                          open a random bookmark, if no arguments
     --oa                 browse all search results immediately
     --replace old new    replace old tag with new tag everywhere
                          delete old tag, if new tag not specified
+    --url-redirect       when fetching an URL, use the resulting
+                         URL from following *permanent* redirects
+                         (when combined with --export, the old URL
+                         is included as additional metadata)
+    --tag-redirect [tag] when fetching an URL that causes permanent
+                         redirect, add a tag in specified pattern
+                         (using 'http:{}' if not specified)
+    --tag-error [tag]    when fetching an URL that causes an HTTP
+                         error, add a tag in specified pattern
+                         (using 'http:{}' if not specified)
+    --del-error [...]    when fetching an URL causes any (given)
+                         HTTP error, delete/do not add it
+    --export-on [...]    export records affected by the above
+                         options, including removed info
+                         (requires --update and --export; specific
+                         HTTP response filter can be provided)
     --shorten index|URL  fetch shortened url from tny.im service
     --expand index|URL   expand a tny.im shortened url
     --cached index|URL   browse a cached page from Wayback Machine
+    --offline            add a bookmark without connecting to web
     --suggest            show similar tags when adding bookmarks
     --tacit              reduce verbosity, skip some confirmations
     --nostdin            do not wait for input (must be first arg)
     --threads N          max network connections in full refresh
                          default N=4, min N=1, max N=10
     -V                   check latest upstream version available
     -g, --debug          show debug information and verbose logs''')
@@ -5498,17 +5809,23 @@
     addarg('--colors', dest='colorstr', type=argparser.is_colorstr, metavar='COLORS', help=hide)
     addarg('--nc', action='store_true', help=hide)
     addarg('-n', '--count', nargs='?', const=10, type=int, default=0, help=hide)
     addarg('--np', action='store_true', help=hide)
     addarg('-o', '--open', nargs='*', help=hide)
     addarg('--oa', action='store_true', help=hide)
     addarg('--replace', nargs='+', help=hide)
+    addarg('--url-redirect', action='store_true', help=hide)
+    addarg('--tag-redirect', nargs='?', const=True, default=False, help=hide)
+    addarg('--tag-error', nargs='?', const=True, default=False, help=hide)
+    addarg('--del-error', nargs='*', help=hide)
+    addarg('--export-on', nargs='*', help=hide)
     addarg('--shorten', nargs=1, help=hide)
     addarg('--expand', nargs=1, help=hide)
     addarg('--cached', nargs=1, help=hide)
+    addarg('--offline', action='store_true', help=hide)
     addarg('--suggest', action='store_true', help=hide)
     addarg('--tacit', action='store_true', help=hide)
     addarg('--nostdin', action='store_true', help=hide)
     addarg('--threads', type=int, default=4, choices=range(1, 11), help=hide)
     addarg('-V', dest='upstream', action='store_true', help=hide)
     addarg('-g', '--debug', action='store_true', help=hide)
     # Undocumented APIs
@@ -5529,14 +5846,18 @@
     # we'd better check for known working console emulators first. Currently,
     # only ConEmu is supported. If the user does not use ConEmu, colors are
     # disabled unless --colors or %BUKU_COLORS% is specified.
     if sys.platform == 'win32' and os.environ.get('ConemuDir') is None:
         if args.colorstr is None and colorstr_env is not None:
             args.nc = True
 
+    # Handle NO_COLOR as well:
+    if os.environ.get('NO_COLOR') is not None:
+        args.nc = True
+
     # Handle color output preference
     if args.nc:
         logging.basicConfig(format='[%(levelname)s] %(message)s')
     else:
         # Set colors
         if colorstr_env is not None:
             # Someone set BUKU_COLORS.
@@ -5591,32 +5912,55 @@
     if args.lock is not None:
         BukuCrypt.encrypt_file(args.lock)
     elif args.unlock is not None:
         BukuCrypt.decrypt_file(args.unlock)
 
     # Set up title
     if args.title is not None:
-        if args.title:
-            title_in = ' '.join(args.title)
-        else:
-            title_in = ''
+        title_in = ' '.join(args.title)
 
     # Set up tags
     if args.tag is not None:
-        if args.tag:
-            tags_in = args.tag
-        else:
-            tags_in = [DELIM, ]
+        tags_in = args.tag or [DELIM]
 
     # Set up comment
     if args.comment is not None:
-        if args.comment:
-            desc_in = ' '.join(args.comment)
-        else:
-            desc_in = ''
+        desc_in = ' '.join(args.comment)
+
+    # validating HTTP-code handling args
+    tag_redirect = args.tag_redirect
+    if isinstance(args.tag_redirect, str):
+        try:
+            args.tag_redirect.format(301)
+            tag_redirect = args.tag_redirect.strip() or True
+        except (IndexError, KeyError):
+            LOGERR('Invalid format of --tag-redirect (should use "{}" as placeholder)')
+            sys.exit(1)
+    tag_error = args.tag_error
+    if isinstance(args.tag_error, str):
+        try:
+            args.tag_error.format(301)
+            tag_error = args.tag_error.strip() or True
+        except (IndexError, KeyError):
+            LOGERR('Invalid format of --tag-error (should use "{}" as placeholder)')
+            sys.exit(1)
+    try:
+        del_error = (None if args.del_error is None else
+                     parse_range(args.del_error, lambda x: 400 <= x < 600) or range(400, 600))
+    except ValueError:
+        LOGERR('Invalid HTTP code(s) given for --del-error (should be within 4xx/5xx ranges)')
+        sys.exit(1)
+    try:
+        _default = (set() if not args.url_redirect and not tag_redirect else PERMANENT_REDIRECTS)
+        _default |= set([] if not tag_error else range(400, 600)) | set(del_error or [])
+        export_on = (None if args.export_on is None else
+                     parse_range(args.export_on, lambda x: 100 <= x < 600) or _default)
+    except ValueError:
+        LOGERR('Invalid HTTP code(s) given for --export-on')
+        sys.exit(1)
 
     # Initialize the database and get handles, set verbose by default
     bdb = BukuDb(
         args.json,
         args.format,
         not args.tacit,
         dbfile=args.db[0] if args.db is not None else None,
@@ -5625,15 +5969,15 @@
 
     # Editor mode
     if args.write is not None:
         if not is_editor_valid(args.write):
             bdb.close_quit(1)
 
         if is_int(args.write):
-            if not bdb.edit_update_rec(int(args.write), args.immutable):
+            if not bdb.edit_update_rec(int(args.write), _immutable(args)):
                 bdb.close_quit(1)
         elif args.add is None:
             # Edit and add a new bookmark
             # Parse tags into a comma-separated string
             if tags_in:
                 if tags_in[0] == '+':
                     tags = '+' + parse_tags(tags_in[1:])
@@ -5645,15 +5989,15 @@
                 tags = DELIM
 
             result = edit_rec(args.write, '', title_in, tags, desc_in)
             if result is not None:
                 url, title_in, tags, desc_in = result
                 if args.suggest:
                     tags = bdb.suggest_similar_tag(tags)
-                bdb.add_rec(url, title_in, tags, desc_in, args.immutable)
+                bdb.add_rec(url, title_in, tags, desc_in, _immutable(args), False, not args.offline)
 
     # Add record
     if args.add is not None:
         if args.url is not None and args.update is None:
             LOGERR('Bookmark a single URL at a time')
             bdb.close_quit(1)
 
@@ -5683,15 +6027,16 @@
                 url, title_in, tags, desc_in = result
             else:
                 edit_aborted = True
 
         if edit_aborted is False:
             if args.suggest:
                 tags = bdb.suggest_similar_tag(tags)
-            bdb.add_rec(url, title_in, tags, desc_in, args.immutable)
+            bdb.add_rec(url, title_in, tags, desc_in, _immutable(args), delay_commit=False, fetch=not args.offline,
+                        url_redirect=args.url_redirect, tag_redirect=tag_redirect, tag_error=tag_error, del_error=del_error)
 
     # Search record
     search_results = None
     search_opted = True
     tags_search = bool(args.stag is not None and len(args.stag))
     exclude_results = bool(args.exclude is not None and len(args.exclude))
 
@@ -5837,15 +6182,15 @@
         elif args.json:
             write_string_to_file(format_json(search_results, field_filter=args.format), args.json)
         else:
             # Printing in JSON format is non-interactive
             print_json_safe(search_results, field_filter=args.format)
 
         # Export the results, if opted
-        if args.export is not None:
+        if args.export and not (args.update is not None and export_on):
             bdb.exportdb(args.export[0], search_results)
 
         # In case of search and delete/update,
         # prompt should be non-interactive
         # delete gets priority over update
         if args.delete is not None and not args.delete:
             bdb.delete_resultset(search_results)
@@ -5870,85 +6215,35 @@
         else:
             tags = None
 
         # No arguments to --update, update all
         if not args.update:
             # Update all records only if search was not opted
             if not search_opted:
-                bdb.update_rec(0, url_in, title_in, tags, desc_in, args.immutable, args.threads)
-            elif update_search_results and search_results is not None:
+                _indices = []
+            elif search_results and update_search_results:
                 if not args.tacit:
                     print('Updated results:\n')
 
-                pos = len(search_results) - 1
-                while pos >= 0:
-                    idx = search_results[pos][0]
-                    bdb.update_rec(
-                        idx,
-                        url_in,
-                        title_in,
-                        tags,
-                        desc_in,
-                        args.immutable,
-                        args.threads
-                    )
-
-                    # Commit at every 200th removal
-                    if pos % 200 == 0:
-                        bdb.conn.commit()
-
-                    pos -= 1
-        else:
-            for idx in args.update:
-                if is_int(idx):
-                    bdb.update_rec(
-                        int(idx),
-                        url_in,
-                        title_in,
-                        tags,
-                        desc_in,
-                        args.immutable,
-                        args.threads
-                    )
-                elif '-' in idx:
-                    try:
-                        vals = [int(x) for x in idx.split('-')]
-                        if vals[0] > vals[1]:
-                            vals[0], vals[1] = vals[1], vals[0]
-
-                        # Update only once if range starts from 0 (all)
-                        if vals[0] == 0:
-                            bdb.update_rec(
-                                0,
-                                url_in,
-                                title_in,
-                                tags,
-                                desc_in,
-                                args.immutable,
-                                args.threads
-                            )
-                        else:
-                            for _id in range(vals[0], vals[1] + 1):
-                                bdb.update_rec(
-                                    _id,
-                                    url_in,
-                                    title_in,
-                                    tags,
-                                    desc_in,
-                                    args.immutable,
-                                    args.threads
-                                )
-                                if INTERRUPTED:
-                                    break
-                    except ValueError:
-                        LOGERR('Invalid index or range to update')
-                        bdb.close_quit(1)
-
-                if INTERRUPTED:
-                    break
+                _indices = [x.id for x in search_results]
+            else:
+                _indices = None
+        else:
+            try:
+                _indices = parse_range(args.update, lambda x: x >= 0)
+            except ValueError:
+                LOGERR('Invalid index or range to update')
+                bdb.close_quit(1)
+            _indices = ([] if 0 in _indices else _indices)
+        if _indices is not None:
+            bdb.update_rec(_indices, url_in, title_in, tags, desc_in, _immutable(args), threads=args.threads,
+                           url_redirect=args.url_redirect, tag_redirect=tag_redirect,
+                           tag_error=tag_error, del_error=del_error, export_on=export_on)
+            if args.export and bdb._to_export is not None:
+                bdb.exportdb(args.export[0], None)
 
     # Delete record
     if args.delete is not None:
         if not args.delete:
             # Attempt delete-all only if search was not opted
             if not search_opted:
                 bdb.cleardb()
@@ -6002,27 +6297,31 @@
                     bdb.close_quit(1)
 
     # Replace a tag in DB
     if args.replace is not None:
         if len(args.replace) == 1:
             bdb.delete_tag_at_index(0, args.replace[0])
         else:
-            bdb.replace_tag(args.replace[0], args.replace[1:])
+            try:
+                bdb.replace_tag(args.replace[0], [' '.join(args.replace[1:])])
+            except Exception as e:
+                LOGERR(str(e))
+                bdb.close_quit(1)
 
     # Export bookmarks
-    if args.export is not None and not search_opted:
+    if args.export and not search_opted and not export_on:
         bdb.exportdb(args.export[0])
 
     # Import bookmarks
     if args.importfile is not None:
         bdb.importdb(args.importfile[0], args.tacit)
 
     # Import bookmarks from browser
     if args.ai:
-        bdb.auto_import_from_browser()
+        bdb.auto_import_from_browser(firefox_profile=os.environ.get('FIREFOX_PROFILE'))
 
     # Open URL in browser
     if args.open is not None:
         if not args.open:
             bdb.browse_by_index(0)
         else:
             try:
```

### Comparing `buku-4.7.1/bukuserver/filters.py` & `buku-4.9/bukuserver/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,37 +110,27 @@
                 raise ValueError
         if isinstance(value, str):
             return value.strip()
         return value
 
 
 class BookmarkBukuFilter(BaseFilter):
+    keys = {
+        'all_keywords': 'match all',
+        'deep': 'deep',
+        'regex': 'regex'
+    }
 
     def __init__(self, *args, **kwargs):
-        self.keys = {
-            'all_keywords': 'match all',
-            'deep': 'deep',
-            'regex': 'regex'
-        }
-        for key, value in kwargs.items():
-            if key in self.keys and value:
-                setattr(self, key, value)
-            else:
-                setattr(self, key, False)
-        list(map(lambda x: kwargs.pop(x), self.keys))
+        self.params = {key: kwargs.pop(key, False) for key in self.keys}
         super().__init__('buku', *args, **kwargs)
 
     def operation(self):
-        parts = []
-        for key, value in self.keys.items():
-            if getattr(self, key):
-                parts.append(value)
-        if not parts:
-            return 'search'
-        return 'search ' + ', '.join(parts)
+        parts = ', '.join(v for k, v in self.keys.items() if self.params[k])
+        return 'search' + (parts and ' ' + parts)
 
     def apply(self, query, value):
         return query
 
 
 class BookmarkBaseFilter(BaseFilter):
```

### Comparing `buku-4.7.1/bukuserver/static/bukuserver/js/Chart.js` & `buku-4.9/bukuserver/static/bukuserver/js/Chart.js`

 * *Files identical despite different names*

### Comparing `buku-4.7.1/bukuserver/templates/bukuserver/statistic.html` & `buku-4.9/bukuserver/templates/bukuserver/statistic.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 {% extends "bukuserver/home.html" %}
+{% import 'bukuserver/lib.html' as buku with context %}
+
+{% block head %}
+  {{ super() }}
+  {{ buku.close_if_popup() }}
+{% endblock %}
 
 {% block body %}
 <div class="container">
   <form class="form-inline" action="{{url_for('statistic.index')}}" method="POST">
     Data created
     <span rel="tooltip" title="{{datetime}}">{{datetime_text}}</span>
     <button type="submit" class="btn btn-default btn-sm">refresh</button>
@@ -25,15 +31,15 @@
         <th>Rank</th>
         <th>Netloc</th>
         <th>Number</th>
       </tr>
       {% for item, number, _ in most_common_netlocs %}
       <tr>
         <td>{{loop.index}}</td>
-        <td> <a href="{{url_for('bookmark.index_view', flt1_url_netloc_match=item)}}">{{item}}</a> </td>
+        <td> <a href="{{buku.filter('url_netloc_match', item)}}">{{item}}</a> </td>
         <td class="text-right">{{number}}</td>
       </tr>
       {% endfor %}
     </table>
   </div>
   {% else %}
   <span> No bookmark found.</span>
@@ -56,15 +62,15 @@
             </tr>
             {% for item, number in netloc_counter.most_common() %}
               {% if number > 1 %}
               <tr>
                 <td>{{loop.index}}</td>
                 <td>
                   {% if item %}
-                  <a href="{{url_for('bookmark.index_view', flt1_url_netloc_match=item)}}">{{item}}</a>
+                  <a href="{{buku.filter('url_netloc_match', item)}}">{{item}}</a>
                   {% else %}
                   <span class="btn btn-default" disabled="disabled">(No Netloc)</span>
                   {% endif %}
                 </td>
                 <td class="text-right">{{number}}</td>
               </tr>
               {% endif %}
@@ -95,15 +101,15 @@
         <th>Tag</th>
         <th>Number</th>
       </tr>
       {% for item, number, _ in most_common_tags %}
       <tr>
         <td>{{loop.index}}</td>
         <td>
-          <a href="{{url_for('bookmark.index_view', flt3_tags_contain=item)}}">{{item}}</a>
+          <a href="{{buku.filter('tags_contain', item)}}">{{item}}</a>
         </td>
         <td class="text-right">{{number}}</td>
       </tr>
       {% endfor %}
     </table>
   </div>
   {% else %}
@@ -112,27 +118,27 @@
 
   {% if show_tag_rank_table %}
   <div class="modal fade" id="tagRankModal" tabindex="-1" role="dialog">
     <div class="modal-dialog" role="document">
       <div class="modal-content">
         <div class="modal-header">
           <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
-          <h4 class="modal-title" id="myModalLabel">Netloc ranking</h4>
+          <h4 class="modal-title" id="myModalLabel">Tag ranking</h4>
         </div>
         <div class="modal-body">
           <table class="table table-condensed">
             <tr>
               <th>Rank</th>
               <th>Tag</th>
               <th>Number</th>
             </tr>
             {% for item, number in tag_counter.most_common() %}
               <tr>
                 <td>{{loop.index}}</td>
-                <td> <a href="{{url_for('bookmark.index_view', flt3_tags_contain=item)}}">{{item}}</a> </td>
+                <td> <a href="{{buku.filter('tags_contain', item)}}">{{item}}</a> </td>
                 <td class="text-right">{{number}}</td>
               </tr>
             {% endfor %}
           </table>
         </div>
       </div>
     </div>
@@ -159,15 +165,15 @@
         <th>Number</th>
       </tr>
       {% for item, number, _ in most_common_titles %}
       <tr>
         <td>{{loop.index}}</td>
         <td>
           {% if item %}
-          <a href="{{url_for('bookmark.index_view', flt0_title_equals=item)}}">{{item}}</a>
+          <a href="{{buku.filter('title_equals', item)}}">{{item}}</a>
           {% else %}
           (No Title)
           {% endif %}
         </td>
         <td class="text-right">{{number}}</td>
       </tr>
       {% endfor %}
@@ -194,15 +200,15 @@
             </tr>
             {% for item, number in title_counter.most_common() %}
               {% if number > 1 %}
               <tr>
                 <td>{{loop.index}}</td>
                 <td style="word-break:break-all;">
                   {% if item %}
-                  <a href="{{url_for('bookmark.index_view', flt0_title_equals=item)}}">{{item}}</a>
+                  <a href="{{buku.filter('title_equals', item)}}">{{item}}</a>
                   {% else %}
                   <span class="btn btn-default" disabled="disabled">(No Title)</span>
                   {% endif %}
                 </td>
                 <td class="text-right">{{number}}</td>
               </tr>
               {% endif %}
@@ -213,45 +219,46 @@
     </div>
   </div>
   {% endif %}
 {% endblock %}
 
 {% block tail %}
   {{ super() }}
-  <script src="{{url_for('static', filename='bukuserver/js/Chart.js')}}"></script>
+  {{ buku.script('Chart.js') }}
   <script>
-  var ctx = document.getElementById("mostCommonChart").getContext('2d');
-  var netlocChart = new Chart(ctx, {
+  var netlocCtx = document.getElementById("mostCommonChart").getContext('2d');
+  var netlocChart = new Chart(netlocCtx, {
     type: 'pie',
     data: {
       datasets: [{
         data: [
           {% for val in most_common_netlocs %} {{val.1}}, {% endfor %}
         ],
         backgroundColor: [
-          {% for val in most_common_netlocs %} "{{val.2}}", {% endfor %}
+          {% for val in most_common_netlocs %} {{val.2|tojson}}, {% endfor %}
         ],
       }],
       // These labels appear in the legend and in the tooltips when hovering different arcs
       labels: [
-        {% for val in most_common_netlocs %} "{{val.0}}", {% endfor %}
+        {% for val in most_common_netlocs %} {{val.0|tojson}}, {% endfor %}
       ]
     },
     options: {
-      'onClick' : function (evt, item) {
+      onClick (evt, item) {
+        if (!item[0]) return;
         var value = this.data.labels[item[0]._index];
         var form = $('<form></form>');
 
         form.attr("method", "get");
         form.attr("action", "{{url_for('bookmark.index_view')}}");
 
         var field = $('<input></input>');
 
         field.attr("type", "hidden");
-        field.attr("name", "flt1_url_netloc_match");
+        field.attr("name", "flt0_url_netloc_match");
         field.attr("value", value);
         form.append(field);
 
         // The form needs to be a part of the document in
         // order for us to be able to submit it.
         $(document.body).append(form);
         form.submit();
@@ -264,50 +271,52 @@
     type: 'pie',
     data: {
       datasets: [{
         data: [
           {% for val in most_common_tags %} {{val.1}}, {% endfor %}
         ],
         backgroundColor: [
-          {% for val in most_common_tags %} "{{val.2}}", {% endfor %}
+          {% for val in most_common_tags %} {{val.2|tojson}}, {% endfor %}
         ],
       }],
       // These labels appear in the legend and in the tooltips when hovering different arcs
       labels: [
-        {% for val in most_common_tags %} "{{val.0}}", {% endfor %}
+        {% for val in most_common_tags %} {{val.0|tojson}}, {% endfor %}
       ]
     },
     options: {
-      'onClick' : function (evt, item) {
+      onClick (evt, item) {
+        if (!item[0]) return;
         var tagStr = this.data.labels[item[0]._index];
-        var url = "{{url_for('bookmark.index_view')}}?flt3_tags_contain=" + tagStr;
+        var url = "{{url_for('bookmark.index_view')}}?flt0_tags_contain=" + encodeURIComponent(tagStr);
         window.location.href = url;
       }
     }
   });
 
-  var ctx = document.getElementById("mostCommonTitleChart").getContext('2d');
-  var netlocChart = new Chart(ctx, {
+  var titleCtx = document.getElementById("mostCommonTitleChart").getContext('2d');
+  var titleChart = new Chart(titleCtx, {
     type: 'pie',
     data: {
       datasets: [{
         data: [
           {% for val in most_common_titles %} {{val.1}}, {% endfor %}
         ],
         backgroundColor: [
-          {% for val in most_common_titles %} "{{val.2}}", {% endfor %}
+          {% for val in most_common_titles %} {{val.2|tojson}}, {% endfor %}
         ],
       }],
       // These labels appear in the legend and in the tooltips when hovering different arcs
       labels: [
-        {% for val in most_common_titles %} "{{val.0|trim}}", {% endfor %}
+        {% for val in most_common_titles %} {{val.0|trim|tojson}}, {% endfor %}
       ]
     },
     options: {
-      'onClick' : function (evt, item) {
+      onClick (evt, item) {
+        if (!item[0]) return;
         var value = this.data.labels[item[0]._index];
         var form = $('<form></form>');
 
         form.attr("method", "get");
         form.attr("action", "{{url_for('bookmark.index_view')}}");
 
         var field = $('<input></input>');
@@ -321,12 +330,12 @@
         // order for us to be able to submit it.
         $(document.body).append(form);
         form.submit();
       }
     }
   });
 
-  netlocChart.canvas.parentNode.style.height = '128px';
+  titleChart.canvas.parentNode.style.height = '128px';
   </script>
 
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-{% extends "bukuserver/home.html" %} {% block body %}
+{% extends "bukuserver/home.html" %} {% import 'bukuserver/lib.html' as buku
+with context %} {% block head %} {{ super() }} {{ buku.close_if_popup() }} {%
+endblock %} {% block body %}
 Data created {{datetime_text}} refresh
 ******** NNeettlloocc ********
 {% if most_common_netlocs %}
 {% if show_netloc_table %} View all {% endif %}
 RRaannkk           NNeettlloocc   NNuummbbeerr
 {{loop.index}} _{_{_i_t_e_m_}_} {{number}}
 {% else %} No bookmark found. {% endif %} {% if show_netloc_table %}
@@ -15,15 +17,15 @@
 ******** TTaagg ********
 {% if most_common_tags %}
 {% if show_tag_rank_table %} View all {% endif %}
 RRaannkk           TTaagg      NNuummbbeerr
 {{loop.index}} _{_{_i_t_e_m_}_} {{number}}
 {% else %} No tag found. {% endif %} {% if show_tag_rank_table %}
 ×
-****** NNeettlloocc rraannkkiinngg ******
+****** TTaagg rraannkkiinngg ******
 RRaannkk           TTaagg      NNuummbbeerr
 {{loop.index}} _{_{_i_t_e_m_}_} {{number}}
 {% endif %}
 ******** TTiittllee ********
 {% if most_common_titles %}
 {% if show_title_rank_table %} View all {% endif %}
 RRaannkk           TTiittllee                                                 NNuummbbeerr
@@ -31,9 +33,10 @@
                %}
 {% else %} No Title found. {% endif %} {% if show_title_rank_table %}
 ×
 ****** TTiittllee rraannkkiinngg ******
 RRaannkk           TTiittllee                                                 NNuummbbeerr
 {{loop.index}} {% if item %} _{_{_i_t_e_m_}_} {% else %} (No Title) {% endif {{number}}
                %}
-{% endif %} {% endblock %} {% block tail %} {{ super() }}
+{% endif %} {% endblock %} {% block tail %} {{ super() }} {{ buku.script
+('Chart.js') }}
 {% endblock %}
```

### Comparing `buku-4.7.1/bukuserver/views.py` & `buku-4.9/bukuserver/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """views module."""
 import functools
 import itertools
 import logging
+import types
 from argparse import Namespace
 from collections import Counter
-from types import SimpleNamespace
 from typing import Any, List, Optional, Tuple
 from urllib.parse import urlparse
 
 import arrow
 import wtforms
-from flask import current_app, flash, redirect, request, url_for
+from flask import current_app, flash, redirect, request, session, url_for
 from flask_admin.babel import gettext
 from flask_admin.base import AdminIndexView, BaseView, expose
 from flask_admin.model import BaseModelView
 from flask_wtf import FlaskForm
-from markupsafe import Markup
+from markupsafe import Markup, escape
 
 import buku
 
 try:
     from . import filters as bs_filters
     from . import forms
     from .filters import BookmarkField, FilterType
@@ -36,52 +36,66 @@
 
 
 class CustomAdminIndexView(AdminIndexView):
     @expose("/")
     def index(self):
         return self.render("bukuserver/home.html", form=forms.HomeForm())
 
-    @expose(
-        "/",
-        methods=[
-            "POST",
-        ],
-    )
+    @expose('/', methods=['POST'])
     def search(self):
         "redirect to bookmark search"
         form = forms.HomeForm()
-        bbm_filter = bs_filters.BookmarkBukuFilter(
-            all_keywords=False, deep=form.deep.data, regex=form.regex.data
-        )
-        op_text = bbm_filter.operation()
-        values_combi = sorted(itertools.product([True, False], repeat=3))
-        choosen_idx = None
-        for idx, (all_keywords, deep, regex) in enumerate(values_combi):
-            if deep == form.deep.data and regex == form.regex.data and not all_keywords:
-                choosen_idx = idx
-        url_op_text = op_text.replace(", ", "_").replace("  ", " ").replace(" ", "_")
-        kwargs = {}
-        if choosen_idx:
-            key = "".join(["flt", str(choosen_idx), "_buku_", url_op_text])
-            kwargs = {key: form.keyword.data}
-        url = url_for("bookmark.index_view", **kwargs)
+        buku_filter = bs_filters.BookmarkBukuFilter(deep=form.deep.data, regex=form.regex.data)
+        url = url_for('bookmark.index_view', **{filter_key(buku_filter): form.keyword.data})
         return redirect(url)
 
 
-class CustomBukuDbModel:  # pylint: disable=too-few-public-methods
-    def __init__(self, bukudb_inst, name):
-        self.bukudb = bukudb_inst
-        self.name = name
-
-    @property
-    def __name__(self):
-        return self.name
+def last_page(self):
+    """Generic '/last_page' endpoint handler; based on
+    https://github.com/flask-admin/flask-admin/blob/v1.6.0/flask_admin/model/base.py#L1956-L1969 """
+    # Grab parameters from URL
+    view_args = self._get_list_extra_args()
+
+    # Map column index to column name
+    sort_column = self._get_column_by_idx(view_args.sort)
+    if sort_column is not None:
+        sort_column = sort_column[0]
+
+    # Get page size
+    page_size = view_args.page_size or self.page_size
+
+    # Get count and data
+    count, data = self.get_list(-1, sort_column, view_args.sort_desc,
+                                view_args.search, view_args.filters, page_size=page_size)
+
+    args = request.args.copy()
+    args.setlist('page', [max(0, (count - 1) // page_size)])
+    return redirect(url_for('.index_view', **args))
+
+
+def readonly_check(self):
+    if current_app.config.get("BUKUSERVER_READONLY", False):
+        self.can_create = False
+        self.can_edit = False
+        self.can_delete = False
 
 
 class BookmarkModelView(BaseModelView):
+    @staticmethod
+    def _filter_arg(flt):
+        """Exposes filter slugify logic; works because BookmarkModelView.named_filter_urls = True"""
+        return BaseModelView.get_filter_arg(BookmarkModelView, None, flt)
+
+    def _saved(self, id, url, ok=True):
+        if id and ok:
+            session['saved'] = id
+        else:
+            raise ValueError('Duplicate URL' if self.model.bukudb.get_rec_id(url) not in [id, None] else
+                             'Rejected by the database')
+
     def _apply_filters(self, models, filters):
         for idx, _, value in filters:
             if self._filters:
                 flt = self._filters[idx]
                 clean_value = flt.clean(value)
                 models = list(flt.apply(models, clean_value))
         return models
@@ -94,121 +108,122 @@
         parsed_url = urlparse(model.url)
         netloc = parsed_url.netloc
         tag_text = []
         br_tag = "<br/>"
         get_index_view_url = functools.partial(url_for, "bookmark.index_view")
         for tag in filter(None, model.tags.split(",")):
             tag_text.append(
-                f'<a class="btn btn-default" href="{get_index_view_url(flt2_tags_contain=tag.strip())}">{tag}</a>'
+                f'<a class="btn btn-default" href="{escape(get_index_view_url(flt0_tags_contain=tag.strip()))}">{escape(tag)}</a>'
             )
         tag_text_markup = "".join(tag_text)
-        if not netloc and not parsed_url.scheme:
-            escaped_url = Markup.escape(model.url)
-            return Markup(
-                f"""{model.title}{br_tag}{escaped_url}{br_tag}{tag_text_markup}{model.description}"""
-            )
+        description = model.description and br_tag.join(map(escape, model.description.split('\n')))
+        if not netloc:
+            return Markup(br_tag.join([escape(model.title), escape(model.url), tag_text_markup, description]))
         res = []
         if not current_app.config.get("BUKUSERVER_DISABLE_FAVICON", False) and netloc:
             res.append(
-                f'<img src="http://www.google.com/s2/favicons?domain={netloc}"/>'
+                f'<img src="http://www.google.com/s2/favicons?domain={netloc}"/> '
             )
-        title = model.title if model.title else "&lt;EMPTY TITLE&gt;"
-        open_in_new_tab = current_app.config.get("BUKUSERVER_OPEN_IN_NEW_TAB", False)
+        title = model.title or escape('<EMPTY TITLE>')
+        target = ' target="_blank"' if current_app.config.get("BUKUSERVER_OPEN_IN_NEW_TAB", False) else ""
         url_for_index_view_netloc = None
         if netloc:
-            url_for_index_view_netloc = get_index_view_url(flt2_url_netloc_match=netloc)
-        if parsed_url.scheme and not open_in_new_tab:
-            target = 'target="_blank"' if open_in_new_tab else ""
-            res.append(f'<a href="{model.url}"{target}>{title}</a>')
+            url_for_index_view_netloc = get_index_view_url(flt0_url_netloc_match=netloc)
+        if parsed_url.scheme:
+            res.append(f'<a href="{escape(model.url)}"{target}>{escape(title)}</a>')
         else:
-            res.append(title)
+            res.append(escape(title))
         if self.url_render_mode == "netloc" and url_for_index_view_netloc:
-            res.append(f'(<a href="{url_for_index_view_netloc}">{netloc}</a>)')
+            res.append(f' (<a href="{url_for_index_view_netloc}">{netloc}</a>)')
         res.append(br_tag)
         if not parsed_url.scheme:
-            res.extend((model.url, br_tag))
+            res.extend((escape(model.url), br_tag))
         elif self.url_render_mode is None or self.url_render_mode == "full":
-            res.extend((f'<a href="{model.url}">{model.url}</a>', br_tag))
+            res.extend((f'<a href="{escape(model.url)}"{target}>{escape(model.url)}</a>', br_tag))
         if self.url_render_mode != "netloc" and url_for_index_view_netloc:
             res.append(
                 f'<a class="btn btn-default" href="{url_for_index_view_netloc}">netloc:{netloc}</a>'
             )
         if tag_text_markup:
-            res.append("".join(tag_text))
-        description = model.description
+            res.append(tag_text_markup)
         if description:
-            res.extend((br_tag, description.replace("\n", br_tag)))
+            res.extend((br_tag, description))
         return Markup("".join(res))
 
     can_set_page_size = True
     can_view_details = True
     column_filters = ["buku", "id", "url", "title", "tags"]
     column_formatters = {
         "Entry": _list_entry,
     }
     column_list = ["Entry"]
+    list_template = 'bukuserver/bookmarks_list.html'
     create_modal = True
     create_modal_template = "bukuserver/bookmark_create_modal.html"
     create_template = "bukuserver/bookmark_create.html"
     details_modal = True
+    details_modal_template = 'bukuserver/bookmark_details_modal.html'
+    details_template = 'bukuserver/bookmark_details.html'
     edit_modal = True
     edit_modal_template = "bukuserver/bookmark_edit_modal.html"
     edit_template = "bukuserver/bookmark_edit.html"
     named_filter_urls = True
+    extra_css = ['/static/bukuserver/css/bookmark.css']
+    extra_js = ['/static/bukuserver/js/' + it for it in ('page_size.js', 'last_page.js')]
+    last_page = expose('/last-page')(last_page)
 
     def __init__(self, *args, **kwargs):
+        readonly_check(self)
         self.bukudb: buku.BukuDb = args[0]
-        custom_model = CustomBukuDbModel(args[0], "bookmark")
-        args = [
-            custom_model,
-        ] + list(args[1:])
-        self.page_size = kwargs.pop("page_size", DEFAULT_PER_PAGE)
-        self.url_render_mode = kwargs.pop("url_render_mode", DEFAULT_URL_RENDER_MODE)
+        custom_model = types.SimpleNamespace(bukudb=self.bukudb, __name__="bookmark")
+        args = [custom_model] + list(args[1:])
         super().__init__(*args, **kwargs)
 
+    @property
+    def page_size(self):
+        return current_app.config.get('BUKUSERVER_PER_PAGE', DEFAULT_PER_PAGE)
+
+    @property
+    def url_render_mode(self):
+        return current_app.config.get('BUKUSERVER_URL_RENDER_MODE', DEFAULT_URL_RENDER_MODE)
+
     def create_form(self, obj=None):
         form = super().create_form(obj)
-        args = request.args
-        args_url = args.get("url")
-        if args_url and not args_url.startswith("/bookmark/"):
-            form.url.data = args_url
-        if "title" in args.keys():
-            form.title.data = args.get("title")
-        if "description" in args.keys():
-            form.description.data = args.get("description")
+        if not form.data.get('csrf_token'):  # don't override POST data with URL arguments
+            form.url.data = request.args.get('link', form.url.data)
+            form.title.data = request.args.get('title', form.title.data)
+            form.description.data = request.args.get('description', form.description.data)
         return form
 
     def create_model(self, form):
         try:
-            model = SimpleNamespace(
-                id=None, url=None, title=None, tags=None, description=None
-            )
+            model = types.SimpleNamespace(id=None, url=None, title=None, tags=None, description=None, fetch=True)
             form.populate_obj(model)
             vars(model).pop("id")
             self._on_model_change(form, model, True)
-            if not model.url.strip():
+            if not model.url:
                 raise ValueError(f"url invalid: {model.url}")
-            kwargs = {"url": model.url}
+            kwargs = {'url': model.url, 'fetch': model.fetch}
             if model.tags.strip():
                 kwargs["tags_in"] = buku.parse_tags([model.tags])
             for key, item in (("title_in", model.title), ("desc", model.description)):
                 if item.strip():
                     kwargs[key] = item
-            self.model.bukudb.add_rec(**kwargs)
+            vars(model)['id'] = self.model.bukudb.add_rec(**kwargs)
+            self._saved(model.id, model.url)
         except Exception as ex:
             if not self.handle_view_exception(ex):
                 msg = "Failed to create record."
                 flash(
                     gettext("%(msg)s %(error)s", msg=msg, error=str(ex)),
                     "error",
                 )
                 LOG.exception(msg)
             return False
-        else:
-            self.after_model_change(form, model, True)
+        self.after_model_change(form, model, True)
         return model
 
     def delete_model(self, model):
         try:
             self.on_model_delete(model)
             res = self.bukudb.delete_rec(model.id)
         except Exception as ex:
@@ -216,97 +231,70 @@
                 msg = "Failed to delete record."
                 flash(
                     gettext("%(msg)s %(error)s", msg=msg, error=str(ex)),
                     "error",
                 )
                 LOG.exception(msg)
             return False
-        else:
-            self.after_model_delete(model)
+        self.after_model_delete(model)
         return res
 
     def get_list(self, page, sort_field, sort_desc, _, filters, page_size=None):
         bukudb = self.bukudb
-        contain_buku_search = any(x[1] == "buku" for x in filters)
-        if contain_buku_search:
-            mode_id = [x[0] for x in filters]
-            if len(list(set(mode_id))) > 1:
+        buku_filters = [x for x in filters if x[1] == 'buku']
+        if buku_filters:
+            keywords = [x[2] for x in buku_filters]
+            mode_id = {x[0] for x in buku_filters}
+            if len(mode_id) > 1:
                 flash(gettext("Invalid search mode combination"), "error")
                 return 0, []
-            keywords = [x[2] for x in filters]
-            flt = None
-            for idx, flt_name, value in filters:
-                if flt_name == "buku" and self._filters:
-                    flt = self._filters[idx]
-            kwargs = (
-                dict(all_keywords=flt.all_keywords, deep=flt.deep, regex=flt.regex)
-                if flt
-                else {}
-            )
+            try:
+                kwargs = self._filters[mode_id.pop()].params
+            except IndexError:
+                kwargs = {}
             bookmarks = bukudb.searchdb(keywords, **kwargs)
         else:
             bookmarks = bukudb.get_rec_all()
-        bookmarks = self._apply_filters(bookmarks, filters)
-        if sort_field:
-            key_idx = [x.value for x in BookmarkField if x.name.lower() == sort_field][
-                0
-            ]
-            bookmarks = sorted(bookmarks, key=lambda x: x[key_idx], reverse=sort_desc)
+        bookmarks = self._apply_filters(bookmarks or [], filters)
         count = len(bookmarks)
-        if page_size and bookmarks:
-            try:
-                bookmarks = list(chunks(bookmarks, page_size))[page]
-            except IndexError:
-                bookmarks = []
+        bookmarks = page_of(bookmarks, page_size, page)
         data = []
         for bookmark in bookmarks:
-            bm_sns = SimpleNamespace(
-                id=None, url=None, title=None, tags=None, description=None
-            )
+            bm_sns = types.SimpleNamespace(id=None, url=None, title=None, tags=None, description=None)
             for field in list(BookmarkField):
-                if field == BookmarkField.TAGS:
-                    value = bookmark[field.value]
-                    if value.startswith(","):
-                        value = value[1:]
-                    if value.endswith(","):
-                        value = value[:-1]
-                    setattr(bm_sns, field.name.lower(), value)
-                else:
-                    setattr(bm_sns, field.name.lower(), bookmark[field.value])
+                setattr(bm_sns, field.name.lower(), format_value(field, bookmark))
             data.append(bm_sns)
         return count, data
 
     def get_one(self, id):
         bookmark = self.model.bukudb.get_rec_by_id(id)
-        bm_sns = SimpleNamespace(
-            id=None, url=None, title=None, tags=None, description=None
-        )
+        if bookmark is None:
+            return None
+        bm_sns = types.SimpleNamespace(id=None, url=None, title=None, tags=None, description=None)
         for field in list(BookmarkField):
-            if field == BookmarkField.TAGS and bookmark[field.value].startswith(","):
-                value = bookmark[field.value]
-                if value.startswith(","):
-                    value = value[1:]
-                if value.endswith(","):
-                    value = value[:-1]
-                setattr(bm_sns, field.name.lower(), value)
-            else:
-                setattr(bm_sns, field.name.lower(), bookmark[field.value])
+            setattr(bm_sns, field.name.lower(), format_value(field, bookmark, spacing=' '))
+        session['netloc'] = urlparse(bookmark.url).netloc
         return bm_sns
 
     def get_pk_value(self, model):
         return model.id
 
     def scaffold_list_columns(self):
         return [x.name.lower() for x in BookmarkField]
 
     def scaffold_list_form(self, widget=None, validators=None):
         pass
 
     def scaffold_sortable_columns(self):
-        return {x: x for x in self.scaffold_list_columns()}
+        """Returns a dictionary of sortable columns.
+
+        from flask-admin docs:
+        `If your backend does not support sorting, return None or an empty dictionary.`
+        """
+        return {}
 
     def scaffold_filters(self, name):
         res = []
         if name == "buku":
             values_combi = sorted(itertools.product([True, False], repeat=3))
             for all_keywords, deep, regex in values_combi:
                 res.append(
@@ -364,42 +352,35 @@
                     bs_filters.BookmarkBaseFilter(
                         name, filter_type=FilterType.NOT_IN_LIST
                     ),
                 ]
             )
         elif name == BookmarkField.TAGS.name.lower():
 
+            def get_list_from_buku_tags(item):
+                return [x.strip() for x in item.split(",")]
+
             def tags_contain_func(query, value, index):
                 for item in query:
-                    for tag in item[index].split(","):
-                        if tag and tag == value:
-                            yield item
+                    if value in get_list_from_buku_tags(item[index]):
+                        yield item
 
             def tags_not_contain_func(query, value, index):
                 for item in query:
-                    for tag in item[index].split(","):
-                        if tag and tag != value:
-                            yield item
+                    if value not in get_list_from_buku_tags(item[index]):
+                        yield item
 
             res.extend(
                 [
                     bs_filters.BookmarkBaseFilter(name, "contain", tags_contain_func),
-                    bs_filters.BookmarkBaseFilter(
-                        name, "not contain", tags_not_contain_func
-                    ),
+                    bs_filters.BookmarkBaseFilter(name, "not contain", tags_not_contain_func),
                     bs_filters.BookmarkTagNumberEqualFilter(name, "number equal"),
-                    bs_filters.BookmarkTagNumberNotEqualFilter(
-                        name, "number not equal"
-                    ),
-                    bs_filters.BookmarkTagNumberGreaterFilter(
-                        name, "number greater than"
-                    ),
-                    bs_filters.BookmarkTagNumberSmallerFilter(
-                        name, "number smaller than"
-                    ),
+                    bs_filters.BookmarkTagNumberNotEqualFilter(name, "number not equal"),
+                    bs_filters.BookmarkTagNumberGreaterFilter(name, "number greater than"),
+                    bs_filters.BookmarkTagNumberSmallerFilter(name, "number smaller than"),
                 ]
             )
         elif name in self.scaffold_list_columns():
             pass
         else:
             return super().scaffold_filters(name)
         return res
@@ -416,25 +397,25 @@
             res = self.bukudb.update_rec(
                 model.id,
                 url=model.url,
                 title_in=model.title,
                 tags_in=buku.parse_tags([model.tags]),
                 desc=model.description,
             )
+            self._saved(model.id, model.url, res)
         except Exception as ex:
             if not self.handle_view_exception(ex):
                 msg = "Failed to update record."
                 flash(
                     gettext("%(msg)s %(error)s", msg=msg, error=str(ex)),
                     "error",
                 )
                 LOG.exception(msg)
             return False
-        else:
-            self.after_model_change(form, model, False)
+        self.after_model_change(form, model, False)
         return res
 
 
 class TagModelView(BaseModelView):
     def _create_ajax_loader(self, name, options):
         pass
 
@@ -444,43 +425,45 @@
                 flt = self._filters[idx]
                 clean_value = flt.clean(value)
                 models = list(flt.apply(models, clean_value))
         return models
 
     def _name_formatter(self, _, model, name):
         data = getattr(model, name)
-        if not data:
-            return Markup(
-                '<a href="{}">{}</a>'.format(
-                    url_for("bookmark.index_view", flt2_tags_number_equal=0),
-                    "&lt;EMPTY TAG&gt;",
-                )
-            )
-        return Markup(
-            '<a href="{}">{}</a>'.format(
-                url_for("bookmark.index_view", flt1_tags_contain=data), data
-            )
-        )
+        query, title = (({'flt0_tags_contain': data}, data) if data else
+                        ({'flt0_tags_number_equal': 0}, '<EMPTY TAG>'))
+        return Markup(f'<a href="{escape(url_for("bookmark.index_view", **query))}">{escape(title)}</a>')
 
     can_create = False
     can_set_page_size = True
     column_filters = ["name", "usage_count"]
     column_formatters = {
         "name": _name_formatter,
     }
+    list_template = 'bukuserver/tags_list.html'
+    extra_js = ['/static/bukuserver/js/' + it for it in ('page_size.js', 'last_page.js')]
+    last_page = expose('/last-page')(last_page)
 
     def __init__(self, *args, **kwargs):
+        readonly_check(self)
         self.bukudb = args[0]
-        custom_model = CustomBukuDbModel(args[0], "tag")
-        args = [
-            custom_model,
-        ] + list(args[1:])
-        self.page_size = kwargs.pop("page_size", DEFAULT_PER_PAGE)
+        self.all_tags = self.bukudb.get_tag_all()
+        custom_model = types.SimpleNamespace(bukudb=self.bukudb, __name__="tag")
+        args = [custom_model] + list(args[1:])
         super().__init__(*args, **kwargs)
 
+    @property
+    def page_size(self):
+        return current_app.config.get('BUKUSERVER_PER_PAGE', DEFAULT_PER_PAGE)
+
+    @expose('/refresh', methods=['POST'])
+    def refresh(self):
+        self.all_tags = self.bukudb.get_tag_all()
+        return redirect(request.referrer or url_for('.index_view'))
+
     def scaffold_list_columns(self):
         return ["name", "usage_count"]
 
     def scaffold_sortable_columns(self):
         return {x: x for x in self.scaffold_list_columns()}
 
     def scaffold_form(self):
@@ -496,45 +479,41 @@
         self,
         page: int,
         sort_field: str,
         sort_desc: bool,
         search: Optional[Any],
         filters: List[Tuple[int, str, str]],
         page_size: int = None,
-    ) -> Tuple[int, List[SimpleNamespace]]:
+    ) -> Tuple[int, List[types.SimpleNamespace]]:
         logging.debug("search: %s", search)
-        bukudb = self.bukudb
-        tags = bukudb.get_tag_all()[1]
-        tags = sorted(tags.items())
-        tags = self._apply_filters(tags, filters)
+        tags = self._apply_filters(sorted(self.all_tags[1].items()), filters)
         sort_field_dict = {"usage_count": 1, "name": 0}
         if sort_field in sort_field_dict:
             tags = list(
                 sorted(
                     tags,
                     key=lambda x: x[sort_field_dict[sort_field]],
                     reverse=sort_desc,
                 )
             )
         count = len(tags)
-        if page_size and tags:
-            tags = list(chunks(tags, page_size))[page]
+        tags = page_of(tags, page_size, page)
         data = []
         for name, usage_count in tags:
-            tag_sns = SimpleNamespace(name=None, usage_count=None)
+            tag_sns = types.SimpleNamespace(name=None, usage_count=None)
             tag_sns.name, tag_sns.usage_count = name, usage_count
             data.append(tag_sns)
         return count, data
 
     def get_pk_value(self, model):
         return model.name
 
     def get_one(self, id):
-        tags = self.bukudb.get_tag_all()[1]
-        tag_sns = SimpleNamespace(name=id, usage_count=tags[id])
+        tags = self.all_tags[1]
+        tag_sns = types.SimpleNamespace(name=id, usage_count=tags[id])
         return tag_sns
 
     def scaffold_filters(self, name):
         res = []
 
         def top_most_common_func(query, value, index):
             counter = Counter(x[index] for x in query)
@@ -569,46 +548,45 @@
         return res
 
     def delete_model(self, model):
         res = None
         try:
             self.on_model_delete(model)
             res = self.bukudb.delete_tag_at_index(0, model.name, chatty=False)
+            self.all_tags = self.bukudb.get_tag_all()
         except Exception as ex:
             if not self.handle_view_exception(ex):
                 msg = "Failed to delete record."
                 flash(
                     gettext("%(msg)s %(error)s", msg=msg, error=str(ex)),
                     "error",
                 )
                 LOG.exception(msg)
             return False
-        else:
-            self.after_model_delete(model)
+        self.after_model_delete(model)
         return res
 
     def update_model(self, form, model):
-        res = None
         try:
             original_name = model.name
             form.populate_obj(model)
             self._on_model_change(form, model, False)
-            res = self.bukudb.replace_tag(original_name, [model.name])
+            self.bukudb.replace_tag(original_name, [model.name])
+            self.all_tags = self.bukudb.get_tag_all()
         except Exception as ex:
             if not self.handle_view_exception(ex):
                 msg = "Failed to update record."
                 flash(
                     gettext("%(msg)s %(error)s", msg=msg, error=str(ex)),
                     "error",
                 )
                 LOG.exception(msg)
             return False
-        else:
-            self.after_model_change(form, model, False)
-        return res
+        self.after_model_change(form, model, False)
+        return True
 
     def create_model(self, form):
         pass
 
 
 class StatisticView(BaseView):  # pylint: disable=too-few-public-methods
     def __init__(self, *args, **kwargs):
@@ -720,8 +698,21 @@
                 arrow.now(), granularity="second"
             ),
         )
 
 
 def chunks(arr, n):
     n = max(1, n)
-    return (arr[i : i + n] for i in range(0, len(arr), n))
+    return [arr[i : i + n] for i in range(0, len(arr), n)]
+
+def page_of(items, size, idx):
+    try:
+        return chunks(items, size)[idx] if size and items else items
+    except IndexError:
+        return []
+
+def filter_key(flt, idx=''):
+    return 'flt' + str(idx) + '_' + BookmarkModelView._filter_arg(flt)
+
+def format_value(field, bookmark, spacing=''):
+    s = bookmark[field.value]
+    return s if field != BookmarkField.TAGS else s.strip(',').replace(',', ','+spacing)
```

### Comparing `buku-4.7.1/setup.py` & `buku-4.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,96 +21,93 @@
     'Click>=7.0',
     'flake8>=3.4.1',
     'hypothesis>=6.0.0',
     'mypy-extensions==0.4.1',
     'py>=1.5.0',
     'pylint>=1.7.2',
     'pytest-cov',
-    'pytest-vcr>=1.0.2',
+    'pytest-recording>=0.12.1',
     'pytest>=6.2.1',
     'PyYAML>=4.2b1',
     'setuptools>=41.0.1',
     'vcrpy>=1.13.0',
+    'lxml',
+    'flask_babel',
 ]
 
 
 server_require = [
-    "appdirs>=1.4.3",
-    "arrow>=0.12.1",
-    "beautifulsoup4>=4.5.3",
-    "cffi>=1.9.1",
-    "click>=6.7",
-    "Flask-Admin>=1.5.1",
-    "Flask-API>=0.6.9",
+    "arrow>=1.2.2",
+    "Flask-Admin>=1.6.1",
+    "Flask-API>=3.0.post1",
     "Flask-Bootstrap>=3.3.7.1",
-    "flask-paginate>=0.5.1",
-    "flask-reverse-proxy-fix @ https://github.com/rachmadaniHaryono/flask-reverse-proxy-fix/archive/refs/tags/v0.2.2rc1.zip",
-    "Flask-WTF>=0.14.2",
-    "Flask>=1.0.2,<2.0",
-    "idna>=2.5",
-    "itsdangerous>=0.24",
-    "Jinja2>=2.10.1",
-    "markupsafe==2.0.1",
-    "packaging>=16.8",
-    "pyasn1>=0.2.3",
-    "pycparser>=2.17",
-    "requests>=2.21.0",
-    "six>=1.10.0",
-    "urllib3>=1.25.2",
-    "Werkzeug>=0.11.15",
+    "flask-paginate>=2022.1.8",
+    "Flask-WTF>=1.0.1",
+    "Flask>=2.2.2,<2.3",
+    "werkzeug<2.4",
+]
+install_requires = [
+    'beautifulsoup4>=4.4.1',
+    'certifi',
+    'cryptography>=1.2.3',
+    'html5lib>=1.0.1',
+    'urllib3>=1.23,<2',
+    'pyreadline3; sys_platform == \'win32\'',
+    'colorama>=0.4.6; sys_platform == \'win32\'',
 ]
 
 setup(
     name='buku',
     version=version,
     description='Bookmark manager like a text-based mini-web.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Arun Prakash Jana',
     author_email='engineerarun@gmail.com',
     url='https://github.com/jarun/buku',
     license='GPLv3',
-    python_requires='>=3.6',  # requires pip>=9.0.0
+    python_requires='>=3.8',  # requires pip>=9.0.0
     platforms=['any'],
     py_modules=['buku'],
-    install_requires=[
-        'beautifulsoup4>=4.4.1',
-        'cryptography>=1.2.3',
-        'urllib3>=1.23',
-        'html5lib>=1.0.1',
-    ],
+    install_requires=install_requires,
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
     entry_points={
         'console_scripts': ['buku=buku:main', 'bukuserver=bukuserver.server:cli']
     },
     extras_require={
-        "ca-certificates": ["certifi"],
         "tests": tests_require + server_require,
         "server": server_require,
         "docs": [
             "myst-parser>=0.17.0",
             "sphinx-rtd-theme>=1.0.0",
             "sphinx-autobuild>=2021.3.14",
         ],
         "packaging": ["twine>=1.11.0"],
     },
     test_suite='tests',
     tests_require=tests_require,
     keywords='cli bookmarks tag utility',
+    project_urls={
+        "Documentation": "https://buku.readthedocs.io/en/latest",
+        "Funding": "https://github.com/sponsors/jarun",
+        "Source": "https://github.com/jarun/buku",
+        "Tracker": "https://github.com/jarun/buku/issues",
+    },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Indexing/Search',
         'Topic :: Utilities'
     ]
 )
```

### Comparing `buku-4.7.1/tests/test_BukuCrypt.py` & `buku-4.9/tests/test_BukuCrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     with open(test_file, 'w', encoding="utf8", errors="surrogateescape") as f:
         f.write('test')
     from buku import BukuCrypt
     res = BukuCrypt.get_filehash(test_file)
     assert res == exp_res
 
 
+@pytest.mark.slow
 @pytest.mark.parametrize(
     'filesize',
     list(range(0, 17)) + [511, 512, 513, 1023, 1024, 1025, 524288, 524289, 1000000, 1048576, 2097152, 4194304]
 )
 def test_encrypt_decrypt(tmpdir, filesize):
     """test method."""
     dbfile = os.path.join(tmpdir.strpath, 'test_encrypt_decrypt_dbfile')
```

### Comparing `buku-4.7.1/tests/test_ExtendedArgumentParser.py` & `buku-4.9/tests/test_ExtendedArgumentParser.py`

 * *Files identical despite different names*

### Comparing `buku-4.7.1/tests/test_buku.py` & `buku-4.9/tests/test_buku.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """test module."""
 import json
 import logging
 import os
 import signal
-import sys
 import unittest
 from itertools import product
 from unittest import mock
 from urllib.parse import urlparse
 
 import pytest
 
-from buku import DELIM, is_int, prep_tag_search
-
-only_python_3_5 = pytest.mark.skipif(sys.version_info < (3, 5), reason="requires Python 3.5 or later")
+from buku import DELIM, FIELD_FILTER, ALL_FIELDS, FetchResult, is_int, prep_tag_search, print_rec_with_filter, parse_range
 
 
 def check_import_html_results_contains(result, expected_result):
     count = 0
     for r in result:
         for idx, exp_r in enumerate(expected_result):
             if r == exp_r:
@@ -129,94 +126,33 @@
 
 def test_parse_tags_no_args():
     import buku
 
     assert buku.parse_tags() == DELIM
 
 
-@pytest.mark.parametrize(
-    "records, field_filter, exp_res",
-    [
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            1,
-            ["1\thttp://url1.com", "2\thttp://url2.com"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            2,
-            ["1\thttp://url1.com\ttag1", "2\thttp://url2.com\ttag1,tag2"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            3,
-            ["1\ttitle1", "2\ttitle2"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            4,
-            [
-                "1\thttp://url1.com\ttitle1\ttag1",
-                "2\thttp://url2.com\ttitle2\ttag1,tag2",
-            ],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            10,
-            ["http://url1.com", "http://url2.com"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            20,
-            ["http://url1.com\ttag1", "http://url2.com\ttag1,tag2"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            30,
-            ["title1", "title2"],
-        ],
-        [
-            [
-                (1, "http://url1.com", "title1", ",tag1,"),
-                (2, "http://url2.com", "title2", ",tag1,tag2,"),
-            ],
-            40,
-            ["http://url1.com\ttitle1\ttag1", "http://url2.com\ttitle2\ttag1,tag2"],
-        ],
-    ],
-)
-def test_print_rec_with_filter(records, field_filter, exp_res):
-    """test func."""
-    with mock.patch("buku.print", create=True) as m_print:
-        import buku
-
-        buku.print_rec_with_filter(records, field_filter)
-        for res in exp_res:
-            m_print.assert_any_call(res)
+@pytest.mark.parametrize("field_filter, exp_res", [
+    (0, ["1. title1\n   > http://url1.com\n   + desc1\n   # tag1\n",
+         "2. title2\n   > http://url2.com\n   + desc2\n   # tag1,tag2\n"]),
+    (1, ["1\thttp://url1.com", "2\thttp://url2.com"]),
+    (2, ["1\thttp://url1.com\ttag1", "2\thttp://url2.com\ttag1,tag2"]),
+    (3, ["1\ttitle1", "2\ttitle2"]),
+    (4, ["1\thttp://url1.com\ttitle1\ttag1", "2\thttp://url2.com\ttitle2\ttag1,tag2"]),
+    (5, ["1\ttitle1\ttag1", "2\ttitle2\ttag1,tag2"]),
+    (10, ["http://url1.com", "http://url2.com"]),
+    (20, ["http://url1.com\ttag1", "http://url2.com\ttag1,tag2"]),
+    (30, ["title1", "title2"]),
+    (40, ["http://url1.com\ttitle1\ttag1", "http://url2.com\ttitle2\ttag1,tag2"]),
+    (50, ["title1\ttag1", "title2\ttag1,tag2"]),
+])
+def test_print_rec_with_filter(capfd, field_filter, exp_res):
+    records = [(1, "http://url1.com", "title1", ",tag1,", "desc1"),
+               (2, "http://url2.com", "title2", ",tag1,tag2,", "desc2")]
+    print_rec_with_filter(records, field_filter)
+    assert capfd.readouterr().out == ''.join(f'{s}\n' for s in exp_res)
 
 
 @pytest.mark.parametrize(
     "taglist, exp_res",
     [
         ["tag1, tag2+3", ([",tag1,", ",tag2+3,"], "OR", None)],
         ["tag1 + tag2-3 + tag4", ([",tag1,", ",tag2-3,", ",tag4,"], "AND", None)],
@@ -259,32 +195,30 @@
         else:
             editor = nav[2:]
         m_edit_rec.assert_called_once_with(editor, "", None, buku.DELIM, None)
         if edit_rec_retval is not None:
             obj.add_rec(*edit_rec_retval)
 
 
-@pytest.mark.parametrize("field_filter, single_record", product(list(range(4)), [True, False]))
+@pytest.mark.parametrize('single_record', [True, False])
+@pytest.mark.parametrize('field_filter', [0, 1, 2, 3, 4, 5, 10, 20, 30, 40, 50])
 def test_format_json(field_filter, single_record):
-    """test func."""
-    resultset = [["row{}".format(x) for x in range(5)]]
-    if field_filter == 1:
-        marks = {"uri": "row1"}
-    elif field_filter == 2:
-        marks = {"uri": "row1", "tags": "row3"[1:-1]}
-    elif field_filter == 3:
-        marks = {"title": "row2"}
-    else:
-        marks = {
-            "index": "row0",
-            "uri": "row1",
-            "title": "row2",
-            "description": "row4",
-            "tags": "row3"[1:-1],
-        }
+    resultset = [[f'<row{x}>' for x in range(5)]]
+    fields = FIELD_FILTER.get(field_filter, ALL_FIELDS)
+    marks = {}
+    if 'id' in fields:
+        marks['index'] = '<row0>'
+    if 'url' in fields:
+        marks['uri'] = '<row1>'
+    if 'title' in fields:
+        marks['title'] = '<row2>'
+    if 'tags' in fields:
+        marks['tags'] = 'row3'
+    if 'desc' in fields:
+        marks['description'] = '<row4>'
     if not single_record:
         marks = [marks]
 
     with mock.patch("buku.json") as m_json:
         import buku
 
         res = buku.format_json(resultset, single_record, field_filter)
@@ -328,15 +262,14 @@
         buku.browse(url)
         if platform == "win32":
             m_webbrowser.open.assert_called_once_with(opened_url, new=2)
         else:
             get_func_retval.open.assert_called_once_with(opened_url, new=2)
 
 
-@only_python_3_5
 @pytest.mark.parametrize("status_code, latest_release", product([200, 404], [True, False]))
 def test_check_upstream_release(status_code, latest_release):
     """test func."""
     resp = mock.Mock()
     resp.status = status_code
     m_manager = mock.Mock()
     m_manager.request.return_value = resp
@@ -375,15 +308,14 @@
     """test func."""
     import buku
 
     res = buku.delim_wrap(token)
     assert res == exp_res
 
 
-@only_python_3_5
 def test_read_in():
     """test func."""
     message = mock.Mock()
     with mock.patch("buku.disable_sigint_handler"), mock.patch("buku.enable_sigint_handler"), mock.patch(
         "buku.input", return_value=message
     ):
         import buku
@@ -491,15 +423,14 @@
     """test func."""
     import buku
 
     res = buku.parse_temp_file_content(content)
     assert res == exp_res
 
 
-@only_python_3_5
 @pytest.mark.skip(reason="can't patch subprocess")
 def test_edit_rec():
     """test func."""
     editor = "nanoe"
     args = ("url", "title_in", "tags_in", "desc")
     with mock.patch("buku.to_temp_file_content"), mock.patch("buku.os"), mock.patch("buku.open"), mock.patch(
         "buku.parse_temp_file_content"
@@ -548,69 +479,59 @@
         # assert exited with 1
         assert error.args[0] == 1
         # assert proper error message
         assert out == ""
         assert err == "\nInterrupted.\n"
 
 
+@pytest.mark.vcr("tests/vcr_cassettes/test_fetch_data_with_url.yaml")
 @pytest.mark.parametrize(
     "url, exp_res",
     [
-        ["http://example.com.", (None, None, None, 0, 1)],
-        ["http://example.com", ("Example Domain", None, None, 0, 0)],
-        ["http://example.com/page1.txt", (("", "", "", 1, 0))],
-        ["about:new_page", ((None, None, None, 0, 1))],
-        ["chrome://version/", ((None, None, None, 0, 1))],
-        ["chrome://version/", ((None, None, None, 0, 1))],
+        ["http://example.com.", {'bad': True}],
+        ["http://example.com", {'title': 'Example Domain', 'fetch_status': 200}],
+        ["http://example.com/page1.txt", {'mime': True, 'fetch_status': 404}],
+        ["about:new_page", {'bad': True}],
+        ["chrome://version/", {'bad': True}],
+        ["chrome://version/", {'bad': True}],
         # [
         #     'http://4pda.ru/forum/index.php?showtopic=182463&st=1640#entry6044923',
-        #     (
-        #         'Samsung GT-I5800 Galaxy 580 - Обсуждение - 4PDA',
-        #         'Samsung GT-I5800 Galaxy 580 - Обсуждение - 4PDA',
-        #         None,
-        #         0, 0
-        #     )
+        #     {'title': 'Samsung GT-I5800 Galaxy 580 - Обсуждение - 4PDA',
+        #      'desc':  'Samsung GT-I5800 Galaxy 580 - Обсуждение - 4PDA',
+        #      'fetch_status': 200},
         # ],
         [
             "https://www.google.ru/search?"
             "newwindow=1&safe=off&q=xkbcomp+alt+gr&"
             "oq=xkbcomp+alt+gr&"
             "gs_l=serp.3..33i21.28976559.28977886.0."
             "28978017.6.6.0.0.0.0.167.668.0j5.5.0....0...1c.1.64."
             "serp..1.2.311.06cSKPTLo18",
-            ("xkbcomp alt gr", None, None, 0, 0),
+            {'title': 'xkbcomp alt gr', 'fetch_status': 200},
         ],
         [
             "http://www.vim.org/scripts/script.php?script_id=4641",
-            (
-                'mlessnau_case - "in-case" selection, deletion and substitution for underscore, camel, mixed case : vim online',
-                None,
-                None,
-                0,
-                0,
-            ),
+            {'title': 'mlessnau_case - "in-case" selection, deletion and substitution for underscore, camel, mixed case : vim online',
+             'fetch_status': 200},
         ],
     ],
+    ids=lambda s: (s.split('?')[0] + '~' if isinstance(s, str) and '?' in s else None),
 )
-def test_network_handler_with_url(url, exp_res):
+def test_fetch_data_with_url(url, exp_res):
     """test func."""
     import urllib3
 
     import buku
 
     buku.urllib3 = urllib3
     buku.myproxy = None
-    res = buku.network_handler(url)
+    res = buku.fetch_data(url)
     if urlparse(url).netloc == "www.google.ru":
-        temp_res = [
-            res[0].split(" - ")[0],
-        ]
-        temp_res.extend(res[1:])
-        res = tuple(temp_res)
-    assert res == exp_res
+        res = res._replace(title=res.title.split(' - ')[0])
+    assert res == FetchResult(url, **exp_res)
 
 
 @pytest.mark.parametrize(
     "url, exp_res",
     [
         ("http://example.com", False),
         ("apt:package1,package2,package3", True),
@@ -766,18 +687,18 @@
 
 
 def test_import_html_and_add_parent():
     from bs4 import BeautifulSoup
 
     from buku import import_html
 
-    html_text = """<DT><H3>1s</H3>
+    html_text = """<DT><H3>1s (blah,blah)</H3>
 <DL><p>
 <DT><A HREF="http://example.com/"></A>"""
-    exp_res = ("http://example.com/", None, ",1s,", None, 0, True, False)
+    exp_res = ("http://example.com/", None, ",1s (blah blah),", None, 0, True, False)
     html_soup = BeautifulSoup(html_text, "html.parser")
     res = list(import_html(html_soup, True, None))
     assert res[0] == exp_res
 
 
 @pytest.mark.parametrize(
     "add_all_parent, exp_res",
@@ -794,15 +715,15 @@
                     0,
                     True,
                     False,
                 ),
                 (
                     "http://example13.com",
                     None,
-                    ",folder11,folder12,folder13,tag3,tag4,",
+                    ",folder11,folder12,folder13 (blah blah),tag3,tag4,",
                     None,
                     0,
                     True,
                     False,
                 ),
                 (
                     "http://example121.com",
@@ -817,15 +738,15 @@
         ),
         (
             False,
             [
                 ("http://example11.com", None, ",folder11,", None, 0, True, False),
                 ("http://example121.com", None, ",folder121,", None, 0, True, False),
                 ("http://example12.com", None, None, None, 0, True, False),
-                ("http://example13.com", None, ",folder13,tag3,tag4,", None, 0, True, False),
+                ("http://example13.com", None, ",folder13 (blah blah),tag3,tag4,", None, 0, True, False),
             ],
         ),
     ],
 )
 def test_import_html_and_add_all_parent(add_all_parent, exp_res):
     from bs4 import BeautifulSoup
 
@@ -845,15 +766,15 @@
 <DT><H3>Folder11</H3><DL><p>
     <DT><A HREF="http://example11.com"></A></DT>
     <DT><H3>Folder12</H3><DL><p>
         <DT><H3>Folder121</H3><DL><p>
             <DT><A HREF="http://example121.com"></A></DT>
         </DL><p></DT>
         <DT><A HREF="http://example12.com"></A></DT>
-        <DT><H3>Folder13</H3><DL><p>
+        <DT><H3>Folder13 (blah,blah)</H3><DL><p>
             <DT><A HREF="http://example13.com" TAGS="tag3,tag4"></A></DT>
         </DL><p></DT>
     </DL><p></DT>
 </DL><p></DT></DL>
 """
     html_soup = BeautifulSoup(html_text, "html.parser")
     res = list(import_html(html_soup, True, None, add_all_parent))  # pylint: disable=E1121
@@ -938,14 +859,36 @@
             "* [[htttp://example.com][Untitled]]\n* [[htttp://example.org][Untitled]]\n* [[http://google.com][Google]]\n",
         ],
         [
             "markdown",
             "- [Untitled](htttp://example.com)\n- [Untitled](htttp://example.org)\n- [Google](http://google.com)\n",
         ],
         ["random", None],
+        [
+            "xbel",
+            "\n".join(
+                [
+                    '<?xml version="1.0" encoding="UTF-8"?>',
+                    '<!DOCTYPE xbel PUBLIC "+//IDN python.org//'
+                    'DTD XML Bookmark Exchange Language 1.0//EN//XML" '
+                    '"http://pyxml.sourceforge.net/topics/dtds/xbel.dtd">',
+                    '<xbel version="1.0">',
+                    '<bookmark href="htttp://example.com">',
+                    "<title></title>",
+                    "</bookmark>",
+                    '<bookmark href="htttp://example.org">',
+                    "<title></title>",
+                    "</bookmark>",
+                    '<bookmark href="http://google.com">',
+                    "<title>Google</title>",
+                    "</bookmark>",
+                    "</xbel>",
+                ]
+            ),
+        ],
     ],
 )
 def test_convert_bookmark_set(export_type, exp_res, monkeypatch):
     import buku
     from buku import convert_bookmark_set
 
     bms = [
@@ -980,7 +923,45 @@
     ],
 )
 def test_convert_tags_to_org_mode_tags(tags, data):
     from buku import convert_tags_to_org_mode_tags
 
     res = convert_tags_to_org_mode_tags(tags)
     assert res == data
+
+
+@pytest.mark.parametrize('charset', ['ISO-8859-1', 'UTF-8'])
+@pytest.mark.parametrize('mode', ['charset', 'content', 'header'])
+def test_get_data_from_page(charset, mode):
+    from urllib3.response import HTTPResponse
+    from buku import get_data_from_page
+    title = 'Répertoire des articles relatifs à l\'Asiminier - Asimina triloba (L.) Dunal (site Les Fruitiers Rares)'
+    headers = (None if mode != 'header' else {'Content-Type': f'text/html; charset={charset}'})
+    meta = {
+        'charset': f'\n<meta charset="{charset}"/>',
+        'content': f'\n<meta http-equiv="content-type" content="text/html; charset={charset}"/>',
+    }.get(mode, '')
+    body = f'<html>\n\n<head>{meta}\n<title>{title}</title>\n</head>\n<body></body>\n\n</html>\n'
+    resp = HTTPResponse(body.encode(charset), headers)
+    parsed_title, desc, keywords = get_data_from_page(resp)
+    assert parsed_title == title
+
+
+@pytest.mark.parametrize('tokens, valid, expected', [
+    (None, None, None),
+    ('404', None, {404}),
+    ('403,404', None, {403, 404}),
+    ({'400', '500'}, None, {400, 500}),
+    (('400-404', '500'), None, {400, 401, 402, 403, 404, 500}),
+    (['400-404', '500'], lambda x: x in range(400, 600), {400, 401, 402, 403, 404, 500}),
+    (['400-404', '300'], lambda x: x in range(400, 600), ValueError('Not a valid range')),
+])
+def test_parse_range(tokens, valid, expected):
+    if not isinstance(expected, Exception):
+        assert parse_range(tokens, valid) == expected
+    else:
+        try:
+            parse_range(tokens, valid)
+            assert False, 'error expected'
+        except Exception as e:
+            assert type(e) is type(expected)
+            assert str(e) == str(expected)
```

### Comparing `buku-4.7.1/tests/test_bukuDb/25491522_res.yaml` & `buku-4.9/tests/test_bukuDb/firefox_res.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-? !!python/tuple ['http://voyagerlive.org/', Voyager, ',bookmarks bar,', null, 0,
-  true, false]
+? !!python/tuple ['http://voyagerlive.org/', Voyager, ',bookmarks toolbar,', null,
+  0, true, false]
 : {}
 ? !!python/tuple ['http://wiki.ubuntu.com/', Ubuntu Wiki (community-edited website),
-  ',bookmarks bar,imported from firefox,ubuntu and free software links,', null, 0,
-  true, false]
+  ',bookmarks menu,ubuntu  and free software links,', null, 0, true, false]
 : {}
 ? !!python/tuple ['http://www.debian.org/', Debian (Ubuntu is based on Debian), ',bookmarks
-    bar,imported from firefox,ubuntu and free software links,', null, 0, true, false]
+    menu,ubuntu  and free software links,', null, 0, true, false]
 : {}
-? !!python/tuple ['http://www.ubuntu.com/', Ubuntu, ',bookmarks bar,imported from
-    firefox,ubuntu and free software links,', null, 0, true, false]
+? !!python/tuple ['http://www.ubuntu.com/', Ubuntu, ',bookmarks menu,ubuntu  and free
+    software links,', null, 0, true, false]
+: {}
+? !!python/tuple ['https://addons.mozilla.org/fr/firefox/addon/adblock-plus/', '',
+  ',language,tags,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://addons.mozilla.org/fr/firefox/addon/adblock-plus/', Adblock
-    Plus, ',bookmarks bar,f+,', null, 0, true, false]
+    Plus, ',bookmarks toolbar,f+,language,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://addons.mozilla.org/fr/firefox/addon/searchpreview/', SearchPreview,
-  ',bookmarks bar,f+,', null, 0, true, false]
+  ',bookmarks toolbar,f+,', null, 0, true, false]
+: {}
+? !!python/tuple ['https://addons.mozilla.org/fr/firefox/language-tools/', '', ',hello,language,tags,',
+  null, 0, true, false]
 : {}
 ? !!python/tuple ['https://addons.mozilla.org/fr/firefox/language-tools/', Language
-    Tools, ',bookmarks bar,f+,', null, 0, true, false]
+    Tools, ',bookmarks toolbar,f+,hello,language,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://answers.launchpad.net/ubuntu/+addquestion', Make a Support
-    Request to the Ubuntu Community, ',bookmarks bar,imported from firefox,ubuntu
-    and free software links,', null, 0, true, false]
+    Request to the Ubuntu Community, ',bookmarks menu,ubuntu  and free software links,',
+  null, 0, true, false]
 : {}
 ? !!python/tuple ['https://one.ubuntu.com/', Ubuntu One - The personal cloud that
-    brings your digital life together, ',bookmarks bar,imported from firefox,ubuntu
-    and free software links,', null, 0, true, false]
+    brings your digital life together, ',bookmarks menu,ubuntu  and free software links,',
+  null, 0, true, false]
 : {}
-? !!python/tuple ['https://www.google.com/', Google, ',other bookmarks,', null, 0,
-  true, false]
+? !!python/tuple ['https://www.google.co.in/', '', ',bookmarks menu,', null, 0, true, false]
 : {}
-? !!python/tuple ['https://www.mozilla.org/en-US/about/', About Us, ',bookmarks bar,imported
-    from firefox,mozilla firefox,', null, 0, true, false]
+? !!python/tuple ['https://www.mozilla.org/en-US/about/', About Us, ',bookmarks menu,mozilla
+    firefox,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://www.mozilla.org/en-US/contribute/', Get Involved, ',bookmarks
-    bar,imported from firefox,mozilla firefox,', null, 0, true, false]
+    menu,mozilla firefox,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://www.mozilla.org/en-US/firefox/customize/', Customize Firefox,
-  ',bookmarks bar,imported from firefox,mozilla firefox,', null, 0, true, false]
+  ',bookmarks menu,mozilla firefox,', null, 0, true, false]
 : {}
 ? !!python/tuple ['https://www.mozilla.org/en-US/firefox/help/', Help and Tutorials,
-  ',bookmarks bar,imported from firefox,mozilla firefox,', null, 0, true, false]
+  ',bookmarks menu,mozilla firefox,', null, 0, true, false]
 : {}
```

### Comparing `buku-4.7.1/tests/test_bukuDb/25491522_res_nopt.yaml` & `buku-4.9/tests/test_bukuDb/25491522_res_nopt.yaml`

 * *Files identical despite different names*

### Comparing `buku-4.7.1/tests/test_bukuDb/Bookmarks` & `buku-4.9/tests/test_bukuDb/Bookmarks`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999517746913581%*

 * *Differences: {"'roots'": "{'bookmark_bar': {'children': {3: {'name': 'Imported From Firefox (2011-09-02, "*

 * *            "06:03:50)'}}}}"}*

```diff
@@ -335,15 +335,15 @@
                             "name": "Mozilla Firefox",
                             "type": "folder"
                         }
                     ],
                     "date_added": "13149362306507580",
                     "date_modified": "13149362306507581",
                     "id": "41",
-                    "name": "Imported From Firefox",
+                    "name": "Imported From Firefox (2011-09-02, 06:03:50)",
                     "type": "folder"
                 }
             ],
             "date_added": "13149362288728239",
             "date_modified": "0",
             "id": "1",
             "name": "Bookmarks bar",
```

### Comparing `buku-4.7.1/tests/test_bukuDb/firefox_res_nopt.yaml` & `buku-4.9/tests/test_bukuDb/firefox_res_nopt.yaml`

 * *Files identical despite different names*

### Comparing `buku-4.7.1/tests/test_bukuDb.py` & `buku-4.9/tests/test_bukuDb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 #!/usr/bin/env python3
 #
 # Unit test cases for buku
 #
-import logging
 import math
 import os
 import re
-import shutil
 import sqlite3
 import sys
 import unittest
-import urllib
-import zipfile
-
-# fmt: off
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from unittest import mock
-from genericpath import exists
-# fmt: on
 
 import pytest
-import vcr
 import yaml
+from genericpath import exists
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
-from buku import BukuDb, parse_tags, prompt
+from buku import PERMANENT_REDIRECTS, BukuDb, FetchResult, BookmarkVar, bookmark_vars, parse_tags, prompt
+from tests.util import mock_http, mock_fetch, _add_rec, _tagset
 
-logging.basicConfig()  # you need to initialize logging, otherwise you will not see anything from vcrpy
-vcr_log = logging.getLogger("vcr")
-vcr_log.setLevel(logging.INFO)
 
 def get_temp_dir_path():
     with TemporaryDirectory(prefix="bukutest_") as dir_obj:
         return dir_obj
 
 TEST_TEMP_DIR_PATH = get_temp_dir_path()
 TEST_TEMP_DBDIR_PATH = os.path.join(TEST_TEMP_DIR_PATH, "buku")
@@ -69,21 +59,41 @@
 
 @pytest.fixture(scope="module")
 def vcr_cassette_dir(request):
     # Put all cassettes in vhs/{module}/{test}.yaml
     return os.path.join("tests", "vcr_cassettes", request.module.__name__)
 
 
+def rmdb(*bdbs):
+    for bdb in bdbs:
+        try:
+            bdb.cur.close()
+            bdb.conn.close()
+        except Exception:
+            pass
+    if exists(TEST_TEMP_DBFILE_PATH):
+        os.remove(TEST_TEMP_DBFILE_PATH)
+
+
 @pytest.fixture()
-def setup():
+def bukuDb():
     os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
 
     # start every test from a clean state
-    if exists(TEST_TEMP_DBFILE_PATH):
-        os.remove(TEST_TEMP_DBFILE_PATH)
+    rmdb()
+
+    bdbs = []
+
+    def _bukuDb(*args, **kwargs):
+        nonlocal bdbs
+        bdbs += [BukuDb(*args, **kwargs)]
+        return bdbs[-1]
+
+    yield _bukuDb
+    rmdb(*bdbs)
 
 
 class PrettySafeLoader(
     yaml.SafeLoader
 ):  # pylint: disable=too-many-ancestors,too-few-public-methods
     def construct_python_tuple(self, node):
         return tuple(self.construct_sequence(node))
@@ -95,71 +105,71 @@
 
 
 class TestBukuDb(unittest.TestCase):
     def setUp(self):
         os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
 
         # start every test from a clean state
-        if exists(TEST_TEMP_DBFILE_PATH):
-            os.remove(TEST_TEMP_DBFILE_PATH)
+        rmdb()
 
         self.bookmarks = TEST_BOOKMARKS
         self.bdb = BukuDb()
 
     def tearDown(self):
         os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
+        rmdb(self.bdb)
 
     @pytest.mark.non_tox
     def test_get_default_dbdir(self):
         dbdir_expected = TEST_TEMP_DBDIR_PATH
-        dbdir_local_expected = os.path.join(
-            os.path.expanduser("~"), ".local", "share", "buku"
-        )
+        home = os.path.expanduser("~")
+        dbdir_local_expected = (os.path.join(home, ".local", "share", "buku") if sys.platform != 'win32' else
+                                os.path.join(home, "AppData", "Roaming", "buku"))
         dbdir_relative_expected = os.path.abspath(".")
 
         # desktop linux
         self.assertEqual(dbdir_expected, BukuDb.get_default_dbdir())
 
         # desktop generic
         os.environ.pop("XDG_DATA_HOME")
         self.assertEqual(dbdir_local_expected, BukuDb.get_default_dbdir())
 
         # no desktop
 
         # -- home is defined differently on various platforms.
         # -- keep a copy and set it back once done
         originals = {}
-        for env_var in ["HOME", "HOMEPATH", "HOMEDIR"]:
-            try:
+        for env_var in ["HOME", "HOMEPATH", "HOMEDIR", "APPDATA"]:
+            if env_var in os.environ:
                 originals[env_var] = os.environ.pop(env_var)
-            except KeyError:
-                pass
-        self.assertEqual(dbdir_relative_expected, BukuDb.get_default_dbdir())
-        for key, value in list(originals.items()):
-            os.environ[key] = value
+        try:
+            self.assertEqual(dbdir_relative_expected, BukuDb.get_default_dbdir())
+        finally:
+            os.environ.update(originals)
 
     # # not sure how to test this in nondestructive manner
     # def test_move_legacy_dbfile(self):
     #     self.fail()
 
     def test_initdb(self):
-        if exists(TEST_TEMP_DBFILE_PATH):
-            os.remove(TEST_TEMP_DBFILE_PATH)
+        rmdb(self.bdb)
         self.assertIs(False, exists(TEST_TEMP_DBFILE_PATH))
-        conn, curr = BukuDb.initdb()
-        self.assertIsInstance(conn, sqlite3.Connection)
-        self.assertIsInstance(curr, sqlite3.Cursor)
-        self.assertIs(True, exists(TEST_TEMP_DBFILE_PATH))
-        curr.close()
-        conn.close()
+        try:
+            conn, curr = BukuDb.initdb()
+            self.assertIsInstance(conn, sqlite3.Connection)
+            self.assertIsInstance(curr, sqlite3.Cursor)
+            self.assertIs(True, exists(TEST_TEMP_DBFILE_PATH))
+        finally:
+            curr.close()
+            conn.close()
 
     def test_get_rec_by_id(self):
         for bookmark in self.bookmarks:
             # adding bookmark from self.bookmarks
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         # the expected bookmark
         expected = (
             1,
             "http://slashdot.org",
             "SLASHDOT",
             ",news,old,",
@@ -171,40 +181,40 @@
         self.assertEqual(expected, bookmark_from_db)
         # asserting None returned if index out of range
         self.assertIsNone(self.bdb.get_rec_by_id(len(self.bookmarks[0]) + 1))
 
     def test_get_rec_id(self):
         for idx, bookmark in enumerate(self.bookmarks):
             # adding bookmark from self.bookmarks to database
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
             # asserting index is in order
             idx_from_db = self.bdb.get_rec_id(bookmark[0])
             self.assertEqual(idx + 1, idx_from_db)
 
-        # asserting -1 is returned for nonexistent url
+        # asserting None is returned for nonexistent url
         idx_from_db = self.bdb.get_rec_id("http://nonexistent.url")
-        self.assertEqual(-1, idx_from_db)
+        self.assertIsNone(idx_from_db)
 
     def test_add_rec(self):
         for bookmark in self.bookmarks:
             # adding bookmark from self.bookmarks to database
-            self.bdb.add_rec(*bookmark)
+            self.bdb.add_rec(*bookmark, fetch=False)
             # retrieving bookmark from database
             index = self.bdb.get_rec_id(bookmark[0])
             from_db = self.bdb.get_rec_by_id(index)
             self.assertIsNotNone(from_db)
             # comparing data
             for pair in zip(from_db[1:], bookmark):
                 self.assertEqual(*pair)
 
         # TODO: tags should be passed to the api as a sequence...
 
     def test_suggest_tags(self):
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         tagstr = ",test,old,"
         with mock.patch("builtins.input", return_value="1 2 3"):
             expected_results = ",es,est,news,old,test,"
             suggested_results = self.bdb.suggest_similar_tag(tagstr)
             self.assertEqual(expected_results, suggested_results)
 
@@ -215,28 +225,28 @@
         self.assertEqual(expected_results, suggested_results)
 
     def test_update_rec(self):
         old_values = self.bookmarks[0]
         new_values = self.bookmarks[1]
 
         # adding bookmark and getting index
-        self.bdb.add_rec(*old_values)
+        _add_rec(self.bdb, *old_values)
         index = self.bdb.get_rec_id(old_values[0])
         # updating with new values
         self.bdb.update_rec(index, *new_values)
         # retrieving bookmark from database
         from_db = self.bdb.get_rec_by_id(index)
         self.assertIsNotNone(from_db)
         # checking if values are updated
         for pair in zip(from_db[1:], new_values):
             self.assertEqual(*pair)
 
     def test_append_tag_at_index(self):
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         # tags to add
         old_tags = self.bdb.get_rec_by_id(1)[3]
         new_tags = ",foo,bar,baz"
         self.bdb.append_tag_at_index(1, new_tags)
         # updated list of tags
         from_db = self.bdb.get_rec_by_id(1)[3]
@@ -244,15 +254,15 @@
         # checking if new tags were added to the bookmark
         self.assertTrue(split_and_test_membership(new_tags, from_db))
         # checking if old tags still exist
         self.assertTrue(split_and_test_membership(old_tags, from_db))
 
     def test_append_tag_at_all_indices(self):
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         # tags to add
         new_tags = ",foo,bar,baz"
         # record of original tags for each bookmark
         old_tagsets = {
             i: self.bdb.get_rec_by_id(i)[3]
             for i in inclusive_range(1, len(self.bookmarks))
@@ -270,15 +280,15 @@
                 self.assertTrue(split_and_test_membership(new_tags, tagset))
                 # checking if old tags still exist for bookmark
                 self.assertTrue(split_and_test_membership(old_tagsets[index], tagset))
 
     def test_delete_tag_at_index(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         get_tags_at_idx = lambda i: self.bdb.get_rec_by_id(i)[3]
         # list of two-tuples, each containing bookmark index and corresponding tags
         tags_by_index = [
             (i, get_tags_at_idx(i)) for i in inclusive_range(1, len(self.bookmarks))
         ]
 
@@ -289,15 +299,15 @@
             # get updated tags from db
             from_db = get_tags_at_idx(i)
             self.assertNotIn(to_delete, from_db)
 
     def test_search_keywords_and_filter_by_tags(self):
         # adding bookmark
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         with mock.patch("buku.prompt"):
             expected = [
                 (
                     3,
                     "http://example.com/",
                     "test",
@@ -341,15 +351,15 @@
             )
             self.assertIn(expected[0], results)
             self.assertIn(expected[1], results)
 
     def test_searchdb(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         get_first_tag = lambda x: "".join(x[2].split(",")[:2])
         for i, bookmark in enumerate(self.bookmarks):
             tag_search = get_first_tag(bookmark)
             # search by the domain name for url
             url_search = re.match(r"https?://(.*)?\..*", bookmark[0]).group(1)
             title_search = bookmark[1]
@@ -363,30 +373,29 @@
                     # search by keyword
                     results = self.bdb.searchdb([keyword])
                     self.assertEqual(results, expected)
 
     def test_search_by_tag(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         with mock.patch("buku.prompt"):
             get_first_tag = lambda x: "".join(x[2].split(",")[:2])
             for i, bookmark in enumerate(self.bookmarks):
                 # search for bookmark with a tag that is known to exist
                 results = self.bdb.search_by_tag(get_first_tag(bookmark))
                 # Expect a five-tuple containing all bookmark data
                 # db index, URL, title, tags, description
                 expected = [(i + 1,) + tuple(bookmark)]
                 expected[0] += tuple([0])
                 self.assertEqual(results, expected)
 
-    @vcr.use_cassette(
-        "tests/vcr_cassettes/test_search_by_multiple_tags_search_any.yaml"
-    )
+    @pytest.mark.slow
+    @pytest.mark.vcr("tests/vcr_cassettes/test_search_by_multiple_tags_search_any.yaml")
     def test_search_by_multiple_tags_search_any(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
             self.bdb.add_rec(*bookmark)
 
         new_bookmark = [
             "https://newbookmark.com",
@@ -428,17 +437,16 @@
                     ",es,est,tes,test,",
                     "a case for replace_tag test",
                     0,
                 ),
             ]
             self.assertEqual(results, expected)
 
-    @vcr.use_cassette(
-        "tests/vcr_cassettes/test_search_by_multiple_tags_search_all.yaml"
-    )
+    @pytest.mark.slow
+    @pytest.mark.vcr("tests/vcr_cassettes/test_search_by_multiple_tags_search_all.yaml")
     def test_search_by_multiple_tags_search_all(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
             self.bdb.add_rec(*bookmark)
 
         new_bookmark = [
             "https://newbookmark.com",
@@ -478,16 +486,16 @@
         bookmark2 = [
             "https://bookmark2.com",
             "Bookmark Two",
             parse_tags(["tag,two, tag-two"]),
             "test case for bookmark with hyphenated tag",
         ]
 
-        self.bdb.add_rec(*bookmark1)
-        self.bdb.add_rec(*bookmark2)
+        _add_rec(self.bdb, *bookmark1)
+        _add_rec(self.bdb, *bookmark2)
 
         with mock.patch("buku.prompt"):
             # check that space separation for ' + ' operator is enforced
             results = self.bdb.search_by_tag("tag+two")
             # Expect a list of five-element tuples containing all bookmark data
             # db index, URL, title, tags, description
             expected = [
@@ -523,24 +531,24 @@
                 ),
             ]
             self.assertEqual(results, expected)
 
     def test_search_by_tags_exclusion(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         new_bookmark = [
             "https://newbookmark.com",
             "New Bookmark",
             parse_tags(["test,old,new"]),
             "additional bookmark to test multiple tag search",
         ]
 
-        self.bdb.add_rec(*new_bookmark)
+        _add_rec(self.bdb, *new_bookmark)
 
         with mock.patch("buku.prompt"):
             # search for bookmarks matching ANY of the supplied tags
             # while excluding bookmarks from results that match a given tag
             results = self.bdb.search_by_tag("test, old - est")
             # Expect a list of five-element tuples containing all bookmark data
             # db index, URL, title, tags, description
@@ -560,17 +568,15 @@
                     parse_tags([",news,old,"]),
                     "News for old nerds, stuff that doesn't matter",
                     0,
                 ),
             ]
             self.assertEqual(results, expected)
 
-    @vcr.use_cassette(
-        "tests/vcr_cassettes/test_search_by_tags_enforces_space_seprations_exclusion.yaml"
-    )
+    @pytest.mark.vcr("tests/vcr_cassettes/test_search_by_tags_enforces_space_seprations_exclusion.yaml")
     def test_search_by_tags_enforces_space_seprations_exclusion(self):
 
         bookmark1 = [
             "https://bookmark1.com",
             "Bookmark One",
             parse_tags(["tag, two,tag+two"]),
             "test case for bookmark with '+' in tag",
@@ -621,18 +627,18 @@
                     parse_tags([",tag,tag three,"]),
                     "second test case for bookmark with hyphenated tag",
                     0,
                 ),
             ]
             self.assertEqual(results, expected)
 
-    def test_search_and_open_in_broswer_by_range(self):
+    def test_search_and_open_in_browser_by_range(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
 
         # simulate user input, select range of indices 1-3
         index_range = "1-%s" % len(self.bookmarks)
         with mock.patch("builtins.input", side_effect=[index_range]):
             with mock.patch("buku.browse") as mock_browse:
                 try:
                     # search the db with keywords from each bookmark
@@ -649,15 +655,16 @@
                 # collect arguments passed to browse
                 arg_list = [args[0] for args, _ in mock_browse.call_args_list]
                 # expect a list of one-tuples that are bookmark URLs
                 expected = [x[0] for x in self.bookmarks]
                 # checking if browse called with expected arguments
                 self.assertEqual(arg_list, expected)
 
-    @vcr.use_cassette("tests/vcr_cassettes/test_search_and_open_all_in_browser.yaml")
+    @pytest.mark.slow
+    @pytest.mark.vcr("tests/vcr_cassettes/test_search_and_open_all_in_browser.yaml")
     def test_search_and_open_all_in_browser(self):
         # adding bookmarks
         for bookmark in self.bookmarks:
             self.bdb.add_rec(*bookmark)
 
         # simulate user input, select 'a' to open all bookmarks in results
         with mock.patch("builtins.input", side_effect=["a"]):
@@ -679,15 +686,15 @@
                 # expect a list of one-tuples that are bookmark URLs
                 expected = [x[0] for x in self.bookmarks][:2]
                 # checking if browse called with expected arguments
                 self.assertEqual(arg_list, expected)
 
     def test_delete_rec(self):
         # adding bookmark and getting index
-        self.bdb.add_rec(*self.bookmarks[0])
+        _add_rec(self.bdb, *self.bookmarks[0])
         index = self.bdb.get_rec_id(self.bookmarks[0][0])
         # deleting bookmark
         self.bdb.delete_rec(index)
         # asserting it doesn't exist
         from_db = self.bdb.get_rec_by_id(index)
         self.assertIsNone(from_db)
 
@@ -699,26 +706,26 @@
     def test_delete_rec_no(self):
         # checking that non-"y" response causes delete_rec to return None
         with mock.patch("builtins.input", return_value="n"):
             self.assertFalse(self.bdb.delete_rec(0))
 
     def test_cleardb(self):
         # adding bookmarks
-        self.bdb.add_rec(*self.bookmarks[0])
+        _add_rec(self.bdb, *self.bookmarks[0])
         # deleting all bookmarks
         with mock.patch("builtins.input", return_value="y"):
             self.bdb.cleardb()
         # assert table has been dropped
         assert self.bdb.get_rec_by_id(0) is None
 
     def test_replace_tag(self):
         indices = []
         for bookmark in self.bookmarks:
             # adding bookmark, getting index
-            self.bdb.add_rec(*bookmark)
+            _add_rec(self.bdb, *bookmark)
             index = self.bdb.get_rec_id(bookmark[0])
             indices += [index]
 
         # replacing tags
         with mock.patch("builtins.input", return_value="y"):
             self.bdb.replace_tag("news", ["__01"])
         with mock.patch("builtins.input", return_value="y"):
@@ -751,21 +758,24 @@
                 self.assertEqual(from_db[3], parse_tags(["__01"]))
             elif title == "ZAŻÓŁĆ":
                 self.assertEqual(from_db[3], parse_tags(["__02,__03,jaźń"]))
             elif title == "test":
                 self.assertEqual(from_db[3], parse_tags(["test,tes,est,__04"]))
 
     def test_tnyfy_url(self):
+        tny, full = 'http://tny.im/yt', 'https://www.google.com'
         # shorten a well-known url
-        shorturl = self.bdb.tnyfy_url(url="https://www.google.com", shorten=True)
-        self.assertEqual(shorturl, "http://tny.im/yt")
+        with mock_http(tny, status=200):
+            shorturl = self.bdb.tnyfy_url(url=full, shorten=True)
+        self.assertEqual(shorturl, tny)
 
         # expand a well-known short url
-        url = self.bdb.tnyfy_url(url="http://tny.im/yt", shorten=False)
-        self.assertEqual(url, "https://www.google.com")
+        with mock_http(full, status=200):
+            url = self.bdb.tnyfy_url(url=tny, shorten=False)
+        self.assertEqual(url, full)
 
     # def test_browse_by_index(self):
     # self.fail()
 
     def test_close_quit(self):
         # quitting with no args
         try:
@@ -778,27 +788,286 @@
         except SystemExit as err:
             self.assertEqual(err.args[0], 1)
 
     # def test_import_bookmark(self):
     # self.fail()
 
 
+@pytest.mark.parametrize('status', [None, 200, 302, 307, 404, 500])
+@pytest.mark.parametrize('fetch, url_redirect, tag_redirect, tag_error, del_error', [
+    (False, False, False, False, None),                # offline
+    (True, True, False, False, None),                  # url-redirect
+    (True, False, True, True, None),                   # tag-redirect, tag-error
+    (True, True, 'http-{}', 'error:{}', None),         # url-redirect, fetch-tags (custom patterns)
+    (True, True, 'redirect', 'error', None),           # ... (patterns without codes)
+    (True, True, 'redirect', False, range(400, 600)),  # del-error (any errors)
+    (True, True, 'redirect', 'error', {404}),          # ... (some errors)
+])
+def test_add_rec_fetch(bukuDb, caplog, fetch, url_redirect, tag_redirect, tag_error, del_error, status):
+    '''Testing add_rec() behaviour with fetch-status params'''
+    title_in, title, desc = 'Custom Title', 'Fetched Title', 'Fetched description.'
+    tags_in, url_in, url_new = ',custom,tags,', 'https://example.com', 'https://example.com/redirect'
+    url = (url_new if status in PERMANENT_REDIRECTS else url_in)
+    bdb = bukuDb()
+    with mock_fetch(url=url, title=title, desc=desc, fetch_status=status) as fetch_data:
+        index = bdb.add_rec(url=url_in, title_in=title_in, tags_in=tags_in, fetch=fetch,
+                            url_redirect=url_redirect, tag_redirect=tag_redirect,
+                            tag_error=tag_error, del_error=del_error)
+
+    # del-error?
+    if del_error and (not status or status in del_error):
+        assert index is None
+        assert bdb.get_max_id() is None
+        err = ('Network error' if not status else 'HTTP error {}'.format(status))
+        assert caplog.record_tuples == [('root', 40, 'add_rec(): '+err)]
+        return
+    rec = bdb.get_rec_by_id(index)
+
+    # offline?
+    if not fetch:
+        fetch_data.assert_not_called()
+        assert (rec.url, rec.title, rec.desc) == (url_in, title_in, '')
+        assert _tagset(rec.tags_raw) == _tagset(tags_in)
+        return
+
+    # url-redirect?
+    if url_redirect and status in PERMANENT_REDIRECTS:
+        assert rec.url == url_new
+    else:
+        assert rec.url == url_in
+
+    # custom title, fetched description
+    assert (rec.title, rec.desc) == (title_in, desc), 'custom title overrides fetched title'
+
+    # fetch-tags?
+    _tags = _tagset(tags_in)
+    if tag_redirect and status in PERMANENT_REDIRECTS:
+        _tags |= {('http:{}' if tag_redirect is True else tag_redirect).format(status).lower()}
+    if tag_error and (status or 0) >= 400:
+        _tags |= {('http:{}' if tag_error is True else tag_error).format(status).lower()}
+    assert _tagset(rec.tags) == _tags
+
+
+@pytest.mark.parametrize('index', [1, {2, 3}, None])
+@pytest.mark.parametrize('export_on', [None, PERMANENT_REDIRECTS, range(400, 600), PERMANENT_REDIRECTS | {404}])
+@pytest.mark.parametrize('url_in, title_in, tags_in, url_redirect, tag_redirect, tag_error, del_error', [
+    (None, None, None, False, False, False, None),                                          # fetched title/desc, no network test
+    (None, 'Custom Title', ',custom,tags,', False, False, False, None),                     # title, tags, no network test
+    ('http://custom.url', None, None, False, False, False, None),                           # url, fetched title/desc, no network test
+    ('http://custom.url', 'Custom Title', ',custom,tags,', False, False, False, None),      # url, title, tags, no network test
+    (None, 'Custom Title', '+,custom,tags,', True, False, False, None),                     # title, +tags, url-redirect
+    ('http://custom.url', 'Custom Title', '+,custom,tags,', False, True, True, None),       # url, title, +tags, fetch-tags
+    (None, 'Custom Title', None, True, 'http-{}', 'error:{}', None),                        # title, url-redirect, fetch-tags (custom)
+    (None, None, '-,initial%,', True, 'redirect', 'error', None),                           # -tags, url-redirect, fetch-tags (no codes)
+    ('http://custom.url', 'Custom Title', None, True, 'redirect', False, range(400, 600)),  # url, title, url-redirect, del-error
+    (None, None, ',custom,tags,', True, 'redirect', 'error', {404}),                        # tags, url-redirect, fetch-tags, del-error
+])
+def test_update_rec_fetch(bukuDb, caplog, url_in, title_in, tags_in, url_redirect, tag_redirect, tag_error, del_error, export_on, index):
+    '''Testing update_rec() behaviour with fetch-status params'''
+    # redirected URL, nonexistent page, nonexistend domain
+    urls = {
+        'http://wikipedia.net': {'fetch_status': 301, 'url': 'https://www.wikipedia.org', 'title': 'Wikipedia',
+                                 'desc': 'Wikipedia is a free online encyclopedia, created and edited blah blah'},
+        'https://python.org/notfound': {'fetch_status': 404, 'title': 'Welcome to Python.org',
+                                        'desc': 'The official home of the Python Programming Language'},
+        'http://nonexistent.url': {'fetch_status': None},  # unable to resolve host address
+    }
+    # for the URL override
+    custom_url = {'fetch_status': 200, 'title': 'Fetched Title', 'desc': 'Fetched description.'}
+
+    def custom_fetch(url, http_head=False):
+        data = dict(urls.get(url, custom_url))
+        _url = data.pop('url', url)
+        return FetchResult(url_in or _url, **data)
+
+    # computed test parameters
+    title_initial, tags_initial, desc = 'Initial Title', ',initial%,tags,', 'Initial description.'
+    fetch_title = title_in is tags_in is None  # when no custom params are passed (except for URL), titles are fetched
+    network_test = url_redirect or tag_redirect or tag_error or del_error or export_on or fetch_title
+    indices = ({index} if isinstance(index, int) else index or range(1, len(urls)+1))
+    tags = _tagset(tags_in if (tags_in or '').startswith(',') else tags_initial)
+    if not (tags_in or ',').startswith(','):
+        tags = (tags | _tagset(tags_in[1:]) if tags_in.startswith('+') else tags - _tagset(tags_in[1:]))
+
+    # setup
+    bdb = bukuDb()
+    for url_initial in urls:
+        _add_rec(bdb, url_initial, title_in=title_initial, tags_in=tags_initial, desc=desc)
+    assert bdb.get_max_id() == len(urls), 'expecting correct setup'
+    with mock_fetch(custom_fetch) as fetch_data:
+        with mock.patch('buku.read_in', return_value='y'):
+            ok = bdb.update_rec(index=index, url=url_in, title_in=title_in, tags_in=tags_in,
+                                url_redirect=url_redirect, tag_redirect=tag_redirect,
+                                tag_error=tag_error, del_error=del_error, export_on=export_on)
+    recs = bdb.get_rec_all()
+
+    # custom URL on multiple records?
+    if url_in and len(indices) != 1:
+        assert not ok, 'expected to fail'
+        assert caplog.record_tuples == [('root', 40, 'All URLs cannot be same')]
+        fetch_data.assert_not_called()
+        assert recs == [BookmarkVar(id, url, title_initial, tags_initial, desc)
+                        for id, url in enumerate(urls, start=1)]
+        return
+    assert ok, 'expected to succeed'
+
+    # offline?
+    if not network_test and not (url_in and title_in is None):
+        _tags = ',' + ','.join(sorted(tags)) + ','
+        fetch_data.assert_not_called()
+        for rec, url in zip(recs, urls):
+            if rec.id in indices:
+                assert rec == BookmarkVar(rec.id, url_in or url, title_in or title_initial, _tags, desc)
+            else:
+                assert rec == BookmarkVar(rec.id, url, title_initial, tags_initial, desc)
+        return
+
+    # export-on (given HTTP codes)?
+    if not export_on:
+        assert bdb._to_export is None, f'expected no to_export backup: {bdb._to_export}'
+    else:
+        assert isinstance(bdb._to_export, dict), f'to_export backup is not a dict: {bdb._to_export}'
+    to_export = dict(bdb._to_export or {})
+    _urls, _recs = set(urls), {x.url: x for x in recs}
+
+    # one fetch per index
+    assert fetch_data.call_count == len(indices), f'expected {len(indices)} fetches, done {fetch_data.call_count}'
+    for call in fetch_data.call_args_list:
+        # determining fetched, original and redirected URLs, along with fetched data
+        url = call.args[0]
+        url_old = url if not url_in else list(urls)[index-1]  # url_in applies to a single record
+        _urls -= {url_old}
+        data = urls.get(url, custom_url)
+        url_new = (url if not url_redirect else data.get('url', url))
+        rec = _recs.pop(url_new, None)
+        status = data.get('fetch_status')
+
+        # del-error? export-on?
+        old = to_export.pop(url_new, None)
+        if not export_on or status not in export_on:
+            assert old is None, f'{url_old}: backup not expected'
+        if del_error and status in del_error:
+            assert rec is None, f'{url_old}: HTTP error {status}, should delete'
+            if export_on and status in export_on:
+                assert isinstance(old, BookmarkVar), f'{url_old}: should backup old record'
+                assert (old.url, old.title, old.tags_raw, old.desc) == (url_old, title_initial, tags_initial, desc)
+            continue
+        if export_on and status in export_on:
+            assert old == url_old, f'{url_old}: should backup old url on redirect'
+
+        # url-redirect?
+        if url_redirect and status in PERMANENT_REDIRECTS:
+            assert url_new != url_old, f'{url_old}: redirect expected'
+            assert rec.url == url_new, f'{url_old}: should replace with {url_new}'
+        else:
+            assert url_new == rec.url, f'{url_old}: redirect not expected'
+            assert url_new == (url_in or url_old), f'{url_old}: URL should not be changed'
+
+        # title
+        if title_in or (fetch_title and 'title' in data):
+            assert rec.title == (title_in or data['title']), f'{url_old}: should update title'
+        else:
+            assert rec.title == title_initial, f'{url_old}: should not update title'
+
+        # description
+        if fetch_title and 'desc' in data:
+            assert rec.desc == data['desc'], f'{url_old}: should update description'
+        else:
+            assert rec.desc == desc, f'{url_old}: should not update description'
+
+        # tags (+fetch-tags)
+        _tags = set()
+        if tag_redirect and status in PERMANENT_REDIRECTS:
+            _tags |= {('http:{}' if tag_redirect is True else tag_redirect).format(status).lower()}
+        elif tag_error and status in range(400, 600):
+            _tags |= {('http:{}' if tag_error is True else tag_error).format(status).lower()}
+        _tags_str = ',' + ','.join(sorted(_tags)) + ','
+        assert _tagset(rec.tags) == tags | _tags, f'{url_old}: [{tags_initial} | {tags_in or ","} | {_tags_str}] -> {rec.tags}'
+
+    # other records should not have been affected (other than possibly indices)
+    assert not to_export, f'unexpected to_export backup: {to_export}'
+    assert set(_recs) == _urls
+    for rec in _recs.values():
+        assert rec == BookmarkVar(rec.id, rec.url, title_initial, tags_initial, desc)
+
+
+@pytest.mark.parametrize('ext, expected', [
+    ('db', [(1, 'http://custom.url', 'Fetched Title (DELETED)', ',', 'Fetched description.'),
+            (2, 'https://www.wikipedia.org', 'Wikipedia (OLD URL = http://wikipedia.net)', ',http:301,', 'Wikipedia is a free...'),
+            (3, 'https://python.org/notfound', 'Welcome to Python.org', ',http:404,', 'The official home...')]),
+    ('md', ['- [Fetched Title (DELETED)](http://custom.url)',
+            '- [Wikipedia (OLD URL = http://wikipedia.net)](https://www.wikipedia.org) <!-- TAGS: http:301 -->',
+            '- [Welcome to Python.org](https://python.org/notfound) <!-- TAGS: http:404 -->']),
+    ('org', ['* [[http://custom.url][Fetched Title (DELETED)]]',
+             '* [[https://www.wikipedia.org][Wikipedia (OLD URL = http://wikipedia.net)]] :http_301:',
+             '* [[https://python.org/notfound][Welcome to Python.org]] :http_404:']),
+    ('xbel', ['<?xml version="1.0" encoding="UTF-8"?>',
+              '<!DOCTYPE xbel PUBLIC "+//IDN python.org//DTD XML Bookmark Exchange Language 1.0//EN//XML" '
+                                    '"http://pyxml.sourceforge.net/topics/dtds/xbel.dtd">',
+              '<xbel version="1.0">',
+                  '<bookmark href="http://custom.url">', '<title>Fetched Title (DELETED)</title>', '</bookmark>',
+                  '<bookmark href="https://www.wikipedia.org" TAGS="http:301">',
+                      '<title>Wikipedia (OLD URL = http://wikipedia.net)</title>',
+                  '</bookmark>',
+                  '<bookmark href="https://python.org/notfound" TAGS="http:404">',
+                      '<title>Welcome to Python.org</title>',
+                  '</bookmark>',
+              '</xbel>',]),
+    ('html', ['<!DOCTYPE NETSCAPE-Bookmark-file-1>', '',
+              '<META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=UTF-8">',
+              '<TITLE>Bookmarks</TITLE>', '<H1>Bookmarks</H1>', '',
+              '<DL><p>',
+              '    <DT><H3 ADD_DATE="{0}" LAST_MODIFIED="{0}" PERSONAL_TOOLBAR_FOLDER="true">buku bookmarks</H3>',
+              '    <DL><p>',
+              '        <DT><A HREF="http://custom.url" ADD_DATE="{0}" LAST_MODIFIED="{0}">Fetched Title (DELETED)</A>',
+              '        <DD>Fetched description.',
+              '        <DT><A HREF="https://www.wikipedia.org" ADD_DATE="{0}" LAST_MODIFIED="{0}" '
+                             'TAGS="http:301">Wikipedia (OLD URL = http://wikipedia.net)</A>',
+              '        <DD>Wikipedia is a free...',
+              '        <DT><A HREF="https://python.org/notfound" ADD_DATE="{0}" LAST_MODIFIED="{0}" '
+                             'TAGS="http:404">Welcome to Python.org</A>',
+              '        <DD>The official home...',
+              '    </DL><p>',
+              '</DL><p>']),
+])
+def test_export_on(bukuDb, ext, expected):
+    '''Testing exportdb() behaviour after update_rec() with export_on'''
+    outfile = TEST_TEMP_DIR_PATH + '/export-on.' + ext
+    bdb = bukuDb()
+    _add_rec(bdb, 'https://www.wikipedia.org', 'Wikipedia', ',http:301,', 'Wikipedia is a free...')
+    _add_rec(bdb, 'https://python.org/notfound', 'Welcome to Python.org', ',http:404,', 'The official home...')
+    _add_rec(bdb, 'https://nonexistent.url', 'Custom Title')                    # not exported
+    to_export = {'http://custom.url': BookmarkVar(1, 'http://custom.url', 'Fetched Title', ',', 'Fetched description.'),  # deleted
+                 'https://www.wikipedia.org': 'http://wikipedia.net',           # redirect
+                 'https://python.org/notfound': 'https://python.org/notfound'}  # unchanged
+    bdb._to_export = dict(to_export)
+    bdb.exportdb(outfile, None)
+    if ext == 'db':
+        assert BukuDb(dbfile=outfile).get_rec_all() == list(bookmark_vars(expected))
+    else:
+        with open(outfile, encoding='utf-8') as fout:
+            output = fout.read()
+        match = re.search('ADD_DATE="([0-9]+)"', output)
+        timestamp = match and match.group(1)
+        assert output.splitlines() == [s.format(timestamp) for s in expected]
+
+
 @pytest.fixture(scope="function")
 def refreshdb_fixture():
     # Setup
     os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
 
     # start every test from a clean state
-    if exists(TEST_TEMP_DBFILE_PATH):
-        os.remove(TEST_TEMP_DBFILE_PATH)
+    rmdb()
 
     bdb = BukuDb()
 
     yield bdb
 
+    rmdb(bdb)
     # Teardown
     os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
 
 
 @pytest.mark.parametrize(
     "title_in, exp_res",
     [
@@ -809,16 +1078,17 @@
     ],
 )
 def test_refreshdb(refreshdb_fixture, title_in, exp_res):
     bdb = refreshdb_fixture
     args = ["http://example.com"]
     if title_in:
         args.append(title_in)
-    bdb.add_rec(*args)
-    bdb.refreshdb(1, 1)
+    _add_rec(bdb, *args)
+    with mock_fetch(title=exp_res):
+        bdb.refreshdb(1, 1)
     from_db = bdb.get_rec_by_id(1)
     assert from_db[2] == exp_res, "from_db: {}".format(from_db)
 
 
 @pytest.fixture
 def test_print_caplog(caplog):
     caplog.handler.records.clear()
@@ -860,45 +1130,45 @@
         [{"low": 0, "high": 0, "is_range": True}, None, (True, [])],
         [{"low": 0, "high": 1, "is_range": True}, None, (True, [])],
         [{"low": 0, "high": 2, "is_range": True}, None, (True, [])],
         [{"low": 2, "high": 2, "is_range": True}, None, (True, [])],
         [{"low": 2, "high": 3, "is_range": True}, None, (True, [])],
     ],
 )
-def test_print_rec(setup, kwargs, rec, exp_res, tmp_path, caplog):
-    bdb = BukuDb(dbfile=tmp_path / "tmp.db")
+def test_print_rec(bukuDb, kwargs, rec, exp_res, tmp_path, caplog):
+    bdb = bukuDb(dbfile=tmp_path / "tmp.db")
     if rec:
-        bdb.add_rec(*rec)
+        _add_rec(bdb, *rec)
     # run the function
     assert (bdb.print_rec(**kwargs), caplog.record_tuples) == exp_res
 
 
-def test_list_tags(capsys, setup):
-    bdb = BukuDb()
+def test_list_tags(capsys, bukuDb):
+    bdb = bukuDb()
 
     # adding bookmarks
-    bdb.add_rec("http://one.com", "", parse_tags(["cat,ant,bee,1"]), "")
-    bdb.add_rec("http://two.com", "", parse_tags(["Cat,Ant,bee,1"]), "")
-    bdb.add_rec("http://three.com", "", parse_tags(["Cat,Ant,3,Bee,2"]), "")
+    _add_rec(bdb, "http://one.com", "", parse_tags(["cat,ant,bee,1"]), "")
+    _add_rec(bdb, "http://two.com", "", parse_tags(["Cat,Ant,bee,1"]), "")
+    _add_rec(bdb, "http://three.com", "", parse_tags(["Cat,Ant,3,Bee,2"]), "")
 
     # listing tags, asserting output
     out, err = capsys.readouterr()
     prompt(bdb, None, True, listtags=True)
     out, err = capsys.readouterr()
     exp_out = "     1. 1 (2)\n     2. 2 (1)\n     3. 3 (1)\n     4. ant (3)\n     5. bee (3)\n     6. cat (3)\n\n"
     assert out == exp_out
     assert err == ""
 
 
-def test_compactdb(setup):
-    bdb = BukuDb()
+def test_compactdb(bukuDb):
+    bdb = bukuDb()
 
     # adding bookmarks
     for bookmark in TEST_BOOKMARKS:
-        bdb.add_rec(*bookmark)
+        _add_rec(bdb, *bookmark)
 
     # manually deleting 2nd index from db, calling compactdb
     bdb.cur.execute("DELETE FROM bookmarks WHERE id = ?", (2,))
     bdb.compactdb(2)
 
     # asserting bookmarks have correct indices
     assert bdb.get_rec_by_id(1) == (
@@ -949,24 +1219,24 @@
                 False,
                 [tuple([x] + y + [0]) for x, y in zip(range(1, 4), TEST_BOOKMARKS)],
             ),
         ],
     ],
 )
 def test_delete_rec_range_and_delay_commit(
-    setup, tmp_path, low, high, delay_commit, input_retval, exp_res
+    bukuDb, tmp_path, low, high, delay_commit, input_retval, exp_res
 ):
     """test delete rec, range and delay commit."""
-    bdb = BukuDb(dbfile=tmp_path / "tmp.db")
+    bdb = bukuDb(dbfile=tmp_path / "tmp.db")
     kwargs = {"is_range": True, "low": low, "high": high, "delay_commit": delay_commit}
     kwargs["index"] = 0
 
     # Fill bookmark
     for bookmark in TEST_BOOKMARKS:
-        bdb.add_rec(*bookmark)
+        _add_rec(bdb, *bookmark)
 
     with mock.patch("builtins.input", return_value=input_retval):
         res = bdb.delete_rec(**kwargs)
 
     assert (res, bdb.get_rec_all()) == exp_res
 
     # teardown
@@ -981,35 +1251,35 @@
         [1, False, True],
         [1, False, False],
         [1, True, True],
         [1, True, False],
         [100, False, True],
     ],
 )
-def test_delete_rec_index_and_delay_commit(index, delay_commit, input_retval):
+def test_delete_rec_index_and_delay_commit(bukuDb, index, delay_commit, input_retval):
     """test delete rec, index and delay commit."""
-    bdb = BukuDb()
-    bdb_dc = BukuDb()  # instance for delay_commit check.
+    bdb = bukuDb()
+    bdb_dc = bukuDb()  # instance for delay_commit check.
 
     # Fill bookmark
     for bookmark in TEST_BOOKMARKS:
-        bdb.add_rec(*bookmark)
+        _add_rec(bdb, *bookmark)
     db_len = len(TEST_BOOKMARKS)
 
     n_index = index
 
     with mock.patch("builtins.input", return_value=input_retval):
         res = bdb.delete_rec(index=index, delay_commit=delay_commit)
 
     if n_index < 0:
         assert not res
     elif n_index > db_len:
         assert not res
         assert len(bdb.get_rec_all()) == db_len
-    elif index == 0 and input_retval != "y":
+    elif index == 0 and not input_retval:
         assert not res
         assert len(bdb.get_rec_all()) == db_len
     else:
         assert res
         assert len(bdb.get_rec_all()) == db_len - 1
         if delay_commit:
             assert len(bdb_dc.get_rec_all()) == db_len
@@ -1027,17 +1297,17 @@
         (0, True, 1, 1),
         # range on zero index
         (0, True, 0, 0),
         # zero index only
         (0, False, 0, 0),
     ],
 )
-def test_delete_rec_on_empty_database(setup, index, is_range, low, high):
+def test_delete_rec_on_empty_database(bukuDb, index, is_range, low, high):
     """test delete rec, on empty database."""
-    bdb = BukuDb()
+    bdb = bukuDb()
     with mock.patch("builtins.input", return_value="y"):
         res = bdb.delete_rec(index, is_range, low, high)
 
     if (is_range and any([low == 0, high == 0])) or (not is_range and index == 0):
         assert res
         # teardown
         os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
@@ -1049,31 +1319,31 @@
     # teardown
     os.environ["XDG_DATA_HOME"] = TEST_TEMP_DIR_PATH
 
 
 @pytest.mark.parametrize(
     "kwargs, exp_res, raise_error",
     [
-        [dict(index="a", low="a", high=1, is_range=True), None, True],
-        [dict(index="a", low="a", high=1, is_range=False), None, True],
-        [dict(index="a", low=1, high="a", is_range=True), None, True],
-        [dict(index="a", is_range=False), None, True],
-        [dict(index="a", is_range=True), None, True],
+        [{"index": 'a', "low": 'a', "high": 1, "is_range": True}, None, True],
+        [{"index": 'a', "low": 'a', "high": 1, "is_range": False}, None, True],
+        [{"index": 'a', "low": 1, "high": 'a', "is_range": True}, None, True],
+        [{"index": 'a', "is_range": False}, None, True],
+        [{"index": 'a', "is_range": True}, None, True],
     ],
 )
 def test_delete_rec_on_non_integer(
-    setup, tmp_path, monkeypatch, kwargs, exp_res, raise_error
+    bukuDb, tmp_path, monkeypatch, kwargs, exp_res, raise_error
 ):
     """test delete rec on non integer arg."""
     import buku
 
-    bdb = BukuDb(dbfile=tmp_path / "tmp.db")
+    bdb = bukuDb(dbfile=tmp_path / "tmp.db")
 
     for bookmark in TEST_BOOKMARKS:
-        bdb.add_rec(*bookmark)
+        _add_rec(bdb, *bookmark)
 
     def mockreturn():
         return "y"
 
     exp_res = None
     res = None
     monkeypatch.setattr(buku, "read_in", mockreturn)
@@ -1082,126 +1352,119 @@
             res = bdb.delete_rec(**kwargs)
     else:
         res = bdb.delete_rec(**kwargs)
     assert res == exp_res
 
 
 @pytest.mark.parametrize("url", ["", False, None, 0])
-def test_add_rec_add_invalid_url(caplog, url):
+def test_add_rec_add_invalid_url(bukuDb, caplog, url):
     """test method."""
-    bdb = BukuDb()
-    res = bdb.add_rec(url=url)
-    assert res == -1
+    bdb = bukuDb()
+    res = _add_rec(bdb, url=url)
+    assert res is None
     caplog.records[0].levelname == "ERROR"
     caplog.records[0].getMessage() == "Invalid URL"
 
 
 @pytest.mark.parametrize(
     "kwargs, exp_arg",
     [
-        [{"url": "example.com"}, ("example.com", "Example Domain", ",", "", 0)],
+        [{"url": "example.com"}, ("example.com", "Example Domain", ",", "", False)],
         [
             {"url": "http://example.com"},
-            ("http://example.com", "Example Domain", ",", "", 0),
+            ("http://example.com", "Example Domain", ",", "", False),
         ],
         [
-            {"url": "http://example.com", "immutable": 1},
-            ("http://example.com", "Example Domain", ",", "", 1),
+            {"url": "http://example.com", "immutable": True},
+            ("http://example.com", "Example Domain", ",", "", True),
         ],
         [
             {"url": "http://example.com", "desc": "randomdesc"},
-            ("http://example.com", "Example Domain", ",", "randomdesc", 0),
+            ("http://example.com", "Example Domain", ",", "randomdesc", False),
         ],
         [
             {"url": "http://example.com", "title_in": "randomtitle"},
-            ("http://example.com", "randomtitle", ",", "", 0),
+            ("http://example.com", "randomtitle", ",", "", False),
         ],
         [
             {"url": "http://example.com", "tags_in": "tag1"},
-            ("http://example.com", "Example Domain", ",tag1,", "", 0),
+            ("http://example.com", "Example Domain", ",tag1,", "", False),
         ],
         [
             {"url": "http://example.com", "tags_in": ",tag1"},
-            ("http://example.com", "Example Domain", ",tag1,", "", 0),
+            ("http://example.com", "Example Domain", ",tag1,", "", False),
         ],
         [
             {"url": "http://example.com", "tags_in": ",tag1,"},
-            ("http://example.com", "Example Domain", ",tag1,", "", 0),
+            ("http://example.com", "Example Domain", ",tag1,", "", False),
         ],
     ],
 )
-def test_add_rec_exec_arg(kwargs, exp_arg):
+def test_add_rec_exec_arg(bukuDb, kwargs, exp_arg):
     """test func."""
-    bdb = BukuDb()
-    bdb.cur = mock.Mock()
-    bdb.get_rec_id = mock.Mock(return_value=-1)
-    bdb.add_rec(**kwargs)
-    assert bdb.cur.execute.call_args[0][1] == exp_arg
+    bdb = bukuDb()
+    _cur = bdb.cur
+    try:
+        bdb.cur = mock.Mock()
+        bdb.get_rec_id = mock.Mock(return_value=None)
+        with mock_fetch(title=exp_arg[1]):
+            bdb.add_rec(**kwargs)
+        assert bdb.cur.execute.call_args[0][1] == exp_arg
+    finally:
+        bdb.cur = _cur
 
 
-def test_update_rec_index_0(caplog):
+def test_update_rec_index_0(bukuDb, caplog):
     """test method."""
-    bdb = BukuDb()
+    bdb = bukuDb()
     res = bdb.update_rec(index=0, url="http://example.com")
     assert not res
     assert caplog.records[0].getMessage() == "All URLs cannot be same"
     assert caplog.records[0].levelname == "ERROR"
 
 
 @pytest.mark.parametrize(
     "kwargs, exp_res",
     [
-        [dict(index=1), False],
-        [dict(index=1, url="url"), False],
-        [dict(index=1, url=""), False],
+        [{"index": 1}, False],
+        [{"index": 1, "url": 'url'}, False],
+        [{"index": 1, "url": ''}, False],
     ],
 )
-def test_update_rec(tmp_path, kwargs, exp_res):
-    bdb = BukuDb(tmp_path / "tmp.db")
+def test_update_rec(bukuDb, tmp_path, kwargs, exp_res):
+    bdb = bukuDb(tmp_path / "tmp.db")
     res = bdb.update_rec(**kwargs)
     assert res == exp_res
 
 
 @pytest.mark.parametrize("invalid_tag", ["+,", "-,"])
-def test_update_rec_invalid_tag(caplog, invalid_tag):
+def test_update_rec_invalid_tag(bukuDb, caplog, invalid_tag):
     """test method."""
     url = "http://example.com"
-    bdb = BukuDb()
+    bdb = bukuDb()
     res = bdb.update_rec(index=1, url=url, tags_in=invalid_tag)
     assert not res
-    try:
-        assert caplog.records[0].getMessage() == "Please specify a tag"
-        assert caplog.records[0].levelname == "ERROR"
-    except IndexError as e:
-        if (sys.version_info.major, sys.version_info.minor) == (3, 4):
-            print("caplog records: {}".format(caplog.records))
-            for idx, record in enumerate(caplog.records):
-                print(
-                    "idx:{};{};message:{};levelname:{}".format(
-                        idx, record, record.getMessage(), record.levelname
-                    )
-                )
-        else:
-            raise e
+    assert caplog.records[0].getMessage() == "Please specify a tag"
+    assert caplog.records[0].levelname == "ERROR"
 
 
 @pytest.mark.parametrize(
     "read_in_retval, exp_res, record_tuples",
     [
-        ["y", False, [("root", 40, "No matching index 0")]],
+        ["y", False, [("root", 40, "No matches found")]],
         ["n", False, []],
         ["", False, []],
     ],
 )
 def test_update_rec_update_all_bookmark(
-    caplog, tmp_path, setup, read_in_retval, exp_res, record_tuples
+    caplog, tmp_path, bukuDb, read_in_retval, exp_res, record_tuples
 ):
     """test method."""
     with mock.patch("buku.read_in", return_value=read_in_retval):
-        bdb = BukuDb(tmp_path / "tmp.db")
+        bdb = bukuDb(tmp_path / "tmp.db")
         res = bdb.update_rec(index=0, tags_in="tags1")
         assert (res, caplog.record_tuples) == (exp_res, record_tuples)
 
 
 @pytest.mark.parametrize(
     "get_system_editor_retval, index, exp_res",
     [
@@ -1215,15 +1478,15 @@
         import buku
 
         bdb = buku.BukuDb()
         res = bdb.edit_update_rec(index=index)
         assert res == exp_res
 
 
-@vcr.use_cassette("tests/vcr_cassettes/test_browse_by_index.yaml")
+@pytest.mark.vcr("tests/vcr_cassettes/test_browse_by_index.yaml")
 @given(
     low=st.integers(min_value=-2, max_value=3),
     high=st.integers(min_value=-2, max_value=3),
     index=st.integers(min_value=-2, max_value=3),
     is_range=st.booleans(),
     empty_database=st.booleans(),
 )
@@ -1299,27 +1562,23 @@
         with open(res_yaml_file, "w", encoding="utf8", errors="surrogateescape") as f:
             yaml.dump(call_args_list_dict, f)
         print("call args list dict dumped to:{}".format(res_yaml_file))
 
 
 @pytest.fixture()
 def firefox_db(tmpdir):
-    zip_url = "https://github.com/jarun/buku/files/1319933/bookmarks.zip"
     dir_path = os.path.dirname(os.path.realpath(__file__))
     res_yaml_file = os.path.join(dir_path, "test_bukuDb", "firefox_res.yaml")
     res_nopt_yaml_file = os.path.join(dir_path, "test_bukuDb", "firefox_res_nopt.yaml")
     ff_db_path = os.path.join(dir_path, "test_bukuDb", "places.sqlite")
     if not os.path.isfile(ff_db_path):
-        tmp_zip = tmpdir.join("bookmarks.zip")
-        with urllib.request.urlopen(zip_url) as response, open(
-            tmp_zip.strpath, "wb"
-        ) as out_file:
-            shutil.copyfileobj(response, out_file)
-        with zipfile.ZipFile(tmp_zip.strpath) as zip_obj:
-            zip_obj.extractall(path=os.path.join(dir_path, "test_bukuDb"))
+        db = sqlite3.connect(ff_db_path)
+        with open(os.path.join(dir_path, 'test_bukuDb', 'places.sql'), encoding='utf-8') as sql:
+            db.cursor().executescript(sql.read())
+        db.commit()
     return ff_db_path, res_yaml_file, res_nopt_yaml_file
 
 
 @pytest.mark.parametrize("add_pt", [True, False])
 def test_load_firefox_database(firefox_db, add_pt):
     # compatibility
     ff_db_path = firefox_db[0]
@@ -1393,49 +1652,51 @@
         db = BukuDb(dbfile=f.name)
         with NamedTemporaryFile(delete=False) as f2:
             res = db.exportdb(f2.name)
             assert not res
 
 
 def test_exportdb_single_rec(tmpdir):
-    with NamedTemporaryFile(delete=False) as f:
-        db = BukuDb(dbfile=f.name)
-        db.add_rec("http://example.com")
-        exp_file = tmpdir.join("export")
-        db.exportdb(exp_file.strpath)
-        with open(exp_file.strpath, encoding="utf8", errors="surrogateescape") as f:
-            assert f.read()
+    f1 = NamedTemporaryFile(delete=False)
+    f1.close()
+    db = BukuDb(dbfile=f1.name)
+    _add_rec(db, "http://example.com")
+    exp_file = tmpdir.join("export")
+    db.exportdb(exp_file.strpath)
+    with open(exp_file.strpath, encoding="utf8", errors="surrogateescape") as f2:
+        assert f2.read()
 
 
 def test_exportdb_to_db():
-    with NamedTemporaryFile(delete=False) as f1, NamedTemporaryFile(
-        delete=False, suffix=".db"
-    ) as f2:
-        db = BukuDb(dbfile=f1.name)
-        db.add_rec("http://example.com")
-        db.add_rec("http://google.com")
-        with mock.patch("builtins.input", return_value="y"):
-            db.exportdb(f2.name)
-        db2 = BukuDb(dbfile=f2.name)
-        assert db.get_rec_all() == db2.get_rec_all()
+    f1 = NamedTemporaryFile(delete=False)
+    f1.close()
+    f2 = NamedTemporaryFile(delete=False, suffix=".db")
+    f2.close()
+    db = BukuDb(dbfile=f1.name)
+    _add_rec(db, "http://example.com")
+    _add_rec(db, "http://google.com")
+    with mock.patch("builtins.input", return_value="y"):
+        db.exportdb(f2.name)
+    db2 = BukuDb(dbfile=f2.name)
+    assert db.get_rec_all() == db2.get_rec_all()
 
 
 @pytest.mark.parametrize(
     "urls, exp_res",
     [
-        [[], -1],
+        [[], None],
         [["http://example.com"], 1],
         [["htttp://example.com", "http://google.com"], 2],
     ],
 )
 def test_get_max_id(urls, exp_res):
     with NamedTemporaryFile(delete=False) as f:
         db = BukuDb(dbfile=f.name)
         if urls:
-            list(map(lambda x: db.add_rec(x), urls))
+            list(map(lambda x: _add_rec(db, x), urls))
         assert db.get_max_id() == exp_res
 
 
 # Helper functions for testcases
 
 
 def split_and_test_membership(a, b):
```

### Comparing `buku-4.7.1/tests/test_import_firefox_json.py` & `buku-4.9/tests/test_import_firefox_json.py`

 * *Files identical despite different names*

