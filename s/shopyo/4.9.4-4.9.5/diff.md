# Comparing `tmp/shopyo-4.9.4.tar.gz` & `tmp/shopyo-4.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopyo-4.9.4.tar", last modified: Thu Apr  4 05:50:50 2024, max compression
+gzip compressed data, was "shopyo-4.9.5.tar", last modified: Sun Apr  7 05:17:42 2024, max compression
```

## Comparing `shopyo-4.9.4.tar` & `shopyo-4.9.5.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-04 05:50:46.000000 shopyo-4.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 05:50:46.000000 shopyo-4.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-04 05:50:50.883421 shopyo-4.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-04 05:50:46.000000 shopyo-4.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.839420 shopyo-4.9.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 05:50:50.883421 shopyo-4.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 05:50:46.000000 shopyo-4.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.839420 shopyo-4.9.4/shopyo/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/.test.prod.env
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.843420 shopyo-4.9.4/shopyo/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.843420 shopyo-4.9.4/shopyo/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cli_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cmd_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/icons.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/app.txt
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/autoapp.py.example
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/config_demo.json
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/info.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/add.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/static/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/register.html
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/shop_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/base/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/base/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/default_styles.html
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/flashed_messages.html
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/resources.html
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/main_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/module_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/nav_base.html
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/view.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/box_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/global.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/info.json
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/test_i18n_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/test_i18n_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/page/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/page/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/all_pages.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/info.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/global.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/info.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/box_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/global.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/info.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/static/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/static/file.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/test_test1_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/test_test1_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/resource/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/resource/templates/resource/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/resource/templates/resource/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/templates/resource/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/global.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/info.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/static/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/static/file.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/templates/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/templates/tests/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/templates/tests/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/templates/tests/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/tests/test_tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/tests/test_tests_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/global.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/info.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/www/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/templates/www/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/templates/www/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/templates/www/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/templates/www/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/shopyo_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/
--rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    78636 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   144878 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/box.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/css/b4vtabs.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/css/simple_sidebar.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/default/
--rw-r--r--   0 runner    (1001) docker     (127)   213806 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/default/default_product.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  3753798 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/default/default_subcategory.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.871420 shopyo-4.9.4/shopyo/static/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.875420 shopyo-4.9.4/shopyo/static/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/all.css
--rw-r--r--   0 runner    (1001) docker     (127)    54457 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/brands.css
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/brands.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    66628 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (127)    53030 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/regular.css
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/regular.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/solid.css
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/solid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.css
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    41032 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.css
--rw-r--r--   0 runner    (1001) docker     (127)    26441 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   659641 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144371 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   815282 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/jquery_3.2.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/js/python.js
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/shopyo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/shopyo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/back/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/themes/back/boogle/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/boogle/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/boogle/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/themes/back/mistrello/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/mistrello/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/mistrello/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/front/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/static/themes/front/blogus/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/index.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/info.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/render_demo.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/resources.html
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_dunder_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/wsgi.py.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-07 05:17:38.000000 shopyo-4.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-07 05:17:38.000000 shopyo-4.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-07 05:17:42.165744 shopyo-4.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-07 05:17:38.000000 shopyo-4.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.121744 shopyo-4.9.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/tests.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-07 05:17:38.000000 shopyo-4.9.5/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 05:17:42.165744 shopyo-4.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-07 05:17:38.000000 shopyo-4.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.125744 shopyo-4.9.5/shopyo/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/.test.prod.env
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.125744 shopyo-4.9.5/shopyo/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-07 05:17:41.000000 shopyo-4.9.5/shopyo/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.129744 shopyo-4.9.5/shopyo/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/cli_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21487 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/cmd_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/icons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.129744 shopyo-4.9.5/shopyo/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/api/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/autoapp.py.example
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/config_demo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.129744 shopyo-4.9.5/shopyo/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.129744 shopyo-4.9.5/shopyo/modules/box__default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.129744 shopyo-4.9.5/shopyo/modules/box__default/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/add.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/appadmin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/appadmin/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/shop_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.133744 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/test_auth_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/test_auth_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/tests/test_auth_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/auth/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/base/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/default_styles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/flashed_messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/main_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/module_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/nav_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/base/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/box_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/dashboard/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/dashboard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/dashboard/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/dashboard/templates/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/dashboard/templates/dashboard/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/dashboard/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/dashboard/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/i18n/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/i18n/templates/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/i18n/templates/i18n/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/templates/i18n/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/i18n/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/tests/test_i18n_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/tests/test_i18n_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/i18n/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.137744 shopyo-4.9.5/shopyo/modules/box__default/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.113744 shopyo-4.9.5/shopyo/modules/box__default/page/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/all_pages.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/dashboard_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/view_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/page/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/box__default/settings/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/settings/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/box__default/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/theme/templates/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__default/theme/templates/theme/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/templates/theme/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/templates/theme/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__default/theme/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.141744 shopyo-4.9.5/shopyo/modules/box__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/box_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/box__tests/test1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/box__tests/test1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/static/file.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/box__tests/test1/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/box__tests/test1/templates/test1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/box__tests/test1/templates/test1/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/templates/test1/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/templates/test1/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/box__tests/test1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/tests/test_test1_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/tests/test_test1_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/box__tests/test1/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/resource/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/resource/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/resource/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/resource/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/resource/templates/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/resource/templates/resource/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/resource/templates/resource/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/resource/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/static/file.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/tests/templates/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/tests/templates/tests/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/templates/tests/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/templates/tests/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/tests/test_tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/tests/test_tests_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/tests/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/www/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/modules/www/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/www/templates/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.145744 shopyo-4.9.5/shopyo/modules/www/templates/www/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/templates/www/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/templates/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/modules/www/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/shopyo_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.149744 shopyo-4.9.5/shopyo/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    78636 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   144878 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/box.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.149744 shopyo-4.9.5/shopyo/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/css/b4vtabs.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/css/simple_sidebar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.149744 shopyo-4.9.5/shopyo/static/default/
+-rw-r--r--   0 runner    (1001) docker     (127)   213806 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/default/default_product.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  3753798 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/default/default_subcategory.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.153744 shopyo-4.9.5/shopyo/static/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.157744 shopyo-4.9.5/shopyo/static/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54457 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/brands.css
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    66628 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    53030 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/regular.css
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/regular.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/solid.css
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/solid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/svg-with-js.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/svg-with-js.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41032 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/v4-shims.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26441 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/css/v4-shims.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.161744 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   659641 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144371 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   815282 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/jquery_3.2.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.161744 shopyo-4.9.5/shopyo/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/js/python.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/shopyo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/shopyo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/static/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.117744 shopyo-4.9.5/shopyo/static/themes/back/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.161744 shopyo-4.9.5/shopyo/static/themes/back/boogle/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/back/boogle/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/back/boogle/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/shopyo/static/themes/back/mistrello/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/back/mistrello/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/back/mistrello/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.121744 shopyo-4.9.5/shopyo/static/themes/front/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/shopyo/static/themes/front/blogus/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/render_demo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/shopyo/static/themes/front/blogus/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/sections/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/sections/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/static/themes/front/blogus/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/shopyo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/tests/test_dunder_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-07 05:17:38.000000 shopyo-4.9.5/shopyo/wsgi.py.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:42.165744 shopyo-4.9.5/shopyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 05:17:42.000000 shopyo-4.9.5/shopyo.egg-info/top_level.txt
```

### Comparing `shopyo-4.9.4/LICENSE` & `shopyo-4.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/PKG-INFO` & `shopyo-4.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopyo
-Version: 4.9.4
+Version: 4.9.5
 Summary: Highly modular web framework built for big apps on top of Flask with Django advantages
 Home-page: https://github.com/shopyo/shopyo
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/shopyo/shopyo/
 Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/issues/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shopyo Version: 4.9.4 Summary: Highly modular web
+Metadata-Version: 2.1 Name: shopyo Version: 4.9.5 Summary: Highly modular web
 framework built for big apps on top of Flask with Django advantages Home-page:
 https://github.com/shopyo/shopyo Author: Abdur-Rahmaan Janhangeer Author-email:
 arj.python@gmail.com License: MIT Project-URL: Source Code, https://github.com/
 shopyo/shopyo/ Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/
 issues/ Project-URL: Changelog, https://github.com/shopyo/shopyo/blob/dev/
 CHANGES.md/ Project-URL: Twitter, https://twitter.com/shopyoproject/ Keywords:
 Flask,Django,web framework,modular Classifier: Environment :: Web Environment
```

### Comparing `shopyo-4.9.4/README.md` & `shopyo-4.9.5/README.md`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/requirements/dev.txt` & `shopyo-4.9.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/requirements/docs.txt` & `shopyo-4.9.5/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/requirements/tests.txt` & `shopyo-4.9.5/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/setup.cfg` & `shopyo-4.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/setup.py` & `shopyo-4.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/CHANGELOG.md` & `shopyo-4.9.5/shopyo/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/__init__.py` & `shopyo-4.9.5/shopyo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-version_info = (4, 9, 4)
+version_info = (4, 9, 5)
 __version__ = ".".join([str(v) for v in version_info])
 
 
 """
+4.9.5
+
+- initialize supports sqlalchemy 2.0
+
 4.9.4
 
 - loosen sqlalchemy requirment; initialize still expected to fail, but package usable
 
 4.9.3
 
 - Remove marshmallow from deps
```

### Comparing `shopyo-4.9.4/shopyo/__main__.py` & `shopyo-4.9.5/shopyo/__main__.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/assets.py` & `shopyo-4.9.5/shopyo/api/assets.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/cli.py` & `shopyo-4.9.5/shopyo/api/cli.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/cli_content.py` & `shopyo-4.9.5/shopyo/api/cli_content.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/cmd.py` & `shopyo-4.9.5/shopyo/api/cmd.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/cmd_helper.py` & `shopyo-4.9.5/shopyo/api/cmd_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Helper utility functions for commandline api
 """
 import importlib
 import json
 import os
 import re
 import sys
+from importlib.metadata import version
 from subprocess import run
 
 import click
 from flask import current_app
 
 from shopyo.api.cli_content import get_dashboard_html_content
 from shopyo.api.cli_content import get_global_py_content
@@ -52,15 +53,25 @@
     try:
         db = current_app.extensions["sqlalchemy"].db
     except:
         db = current_app.extensions["sqlalchemy"]
 
     if clear_db:
         db.drop_all()
-        db.engine.execute("DROP TABLE IF EXISTS alembic_version;")
+        sqlalchemy_version = version("sqlalchemy").split(".")
+
+        sql = "DROP TABLE IF EXISTS alembic_version;"
+        if int(sqlalchemy_version[0]) <= 1:
+            db.engine.execute(sql)
+        else:
+            from sqlalchemy import text
+
+            with db.engine.begin() as conn:
+                result = conn.execute(text(sql))
+                conn.commit()
 
         tryrmfile(os.path.join(os.getcwd(), "shopyo.db"), verbose=verbose)
         if verbose:
             click.echo("[x] all tables dropped")
     elif clear_db is False:
         if verbose:
             click.echo("[ ] db clearing skipped")
```

### Comparing `shopyo-4.9.4/shopyo/api/database.py` & `shopyo-4.9.5/shopyo/api/database.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/email.py` & `shopyo-4.9.5/shopyo/api/email.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/file.py` & `shopyo-4.9.5/shopyo/api/file.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/forms.py` & `shopyo-4.9.5/shopyo/api/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/html.py` & `shopyo-4.9.5/shopyo/api/html.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/icons.txt` & `shopyo-4.9.5/shopyo/api/icons.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/models.py` & `shopyo-4.9.5/shopyo/api/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/module.py` & `shopyo-4.9.5/shopyo/api/module.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/security.py` & `shopyo-4.9.5/shopyo/api/security.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/conftest.py` & `shopyo-4.9.5/shopyo/api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_cli.py` & `shopyo-4.9.5/shopyo/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_cli_integration.py` & `shopyo-4.9.5/shopyo/api/tests/test_cli_integration.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_email.py` & `shopyo-4.9.5/shopyo/api/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_models.py` & `shopyo-4.9.5/shopyo/api/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_print_info.py` & `shopyo-4.9.5/shopyo/api/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/tests/test_validators.py` & `shopyo-4.9.5/shopyo/api/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/api/validators.py` & `shopyo-4.9.5/shopyo/api/validators.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/app.py` & `shopyo-4.9.5/shopyo/app.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/app.txt` & `shopyo-4.9.5/shopyo/app.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/config.py` & `shopyo-4.9.5/shopyo/config.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/conftest.py` & `shopyo-4.9.5/shopyo/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/init.py` & `shopyo-4.9.5/shopyo/init.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/admin.py` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/add.html` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/add.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/index.html` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_admin.py` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/appadmin/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/appadmin/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/forms.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/models.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html` & `shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html` & `shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/login.html` & `shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/register.html` & `shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/register.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html` & `shopyo-4.9.5/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/conftest.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/factories.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/tests/factories.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_functional.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/tests/test_auth_functional.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_models.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/tests/test_auth_models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/upload.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/upload.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/auth/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/auth/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/resources.html` & `shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/blocks/resources.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/module_base.html` & `shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/module_base.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/nav_base.html` & `shopyo-4.9.5/shopyo/modules/box__default/base/templates/base/nav_base.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/base/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/base/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/index.html` & `shopyo-4.9.5/shopyo/modules/box__default/dashboard/templates/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/test_dashboard.py` & `shopyo-4.9.5/shopyo/modules/box__default/dashboard/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/dashboard/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/dashboard/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/i18n/global.py` & `shopyo-4.9.5/shopyo/modules/box__default/i18n/global.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/i18n/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/i18n/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/forms.py` & `shopyo-4.9.5/shopyo/modules/box__default/page/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/models.py` & `shopyo-4.9.5/shopyo/modules/box__default/page/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/all_pages.html` & `shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/all_pages.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard.html` & `shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/dashboard.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html` & `shopyo-4.9.5/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/page/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/page/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/edit.html` & `shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/edit.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/index.html` & `shopyo-4.9.5/shopyo/modules/box__default/settings/templates/settings/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/settings/upload.py` & `shopyo-4.9.5/shopyo/modules/box__default/settings/upload.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/theme/global.py` & `shopyo-4.9.5/shopyo/modules/box__default/theme/global.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/index.html` & `shopyo-4.9.5/shopyo/modules/box__default/theme/templates/theme/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__default/theme/view.py` & `shopyo-4.9.5/shopyo/modules/box__default/theme/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/box__tests/test1/view.py` & `shopyo-4.9.5/shopyo/modules/box__tests/test1/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/resource/models.py` & `shopyo-4.9.5/shopyo/modules/resource/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/resource/view.py` & `shopyo-4.9.5/shopyo/modules/resource/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/tests/view.py` & `shopyo-4.9.5/shopyo/modules/tests/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/www/templates/www/index.html` & `shopyo-4.9.5/shopyo/modules/www/templates/www/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/modules/www/view.py` & `shopyo-4.9.5/shopyo/modules/www/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/shopyo_admin.py` & `shopyo-4.9.5/shopyo/shopyo_admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/bootstrap-grid.min.css` & `shopyo-4.9.5/shopyo/static/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/bootstrap-reboot.min.css` & `shopyo-4.9.5/shopyo/static/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/bootstrap.bundle.min.js` & `shopyo-4.9.5/shopyo/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/bootstrap.min.css` & `shopyo-4.9.5/shopyo/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/box.svg` & `shopyo-4.9.5/shopyo/static/box.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/css/b4vtabs.min.css` & `shopyo-4.9.5/shopyo/static/css/b4vtabs.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/css/simple_sidebar.css` & `shopyo-4.9.5/shopyo/static/css/simple_sidebar.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/default/default_product.jpg` & `shopyo-4.9.5/shopyo/static/default/default_product.jpg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/default/default_subcategory.jpg` & `shopyo-4.9.5/shopyo/static/default/default_subcategory.jpg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/favicon.ico` & `shopyo-4.9.5/shopyo/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/LICENSE.txt` & `shopyo-4.9.5/shopyo/static/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/all.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/all.min.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/brands.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.min.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/regular.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/solid.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.min.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.min.css` & `shopyo-4.9.5/shopyo/static/fontawesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.eot` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.svg` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.eot` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.svg` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.eot` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.svg` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2` & `shopyo-4.9.5/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/jquery_3.2.1.min.js` & `shopyo-4.9.5/shopyo/static/jquery_3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/js/python.js` & `shopyo-4.9.5/shopyo/static/js/python.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/shopyo.png` & `shopyo-4.9.5/shopyo/static/shopyo.png`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/shopyo.svg` & `shopyo-4.9.5/shopyo/static/shopyo.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/themes/back/boogle/styles.css` & `shopyo-4.9.5/shopyo/static/themes/back/boogle/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/themes/back/mistrello/styles.css` & `shopyo-4.9.5/shopyo/static/themes/back/mistrello/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/static/themes/front/blogus/styles.css` & `shopyo-4.9.5/shopyo/static/themes/front/blogus/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/tests/conftest.py` & `shopyo-4.9.5/shopyo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/tests/test_configs.py` & `shopyo-4.9.5/shopyo/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/tests/test_dunder_main.py` & `shopyo-4.9.5/shopyo/tests/test_dunder_main.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo/wsgi.py.example` & `shopyo-4.9.5/shopyo/wsgi.py.example`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.4/shopyo.egg-info/PKG-INFO` & `shopyo-4.9.5/shopyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopyo
-Version: 4.9.4
+Version: 4.9.5
 Summary: Highly modular web framework built for big apps on top of Flask with Django advantages
 Home-page: https://github.com/shopyo/shopyo
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/shopyo/shopyo/
 Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/issues/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shopyo Version: 4.9.4 Summary: Highly modular web
+Metadata-Version: 2.1 Name: shopyo Version: 4.9.5 Summary: Highly modular web
 framework built for big apps on top of Flask with Django advantages Home-page:
 https://github.com/shopyo/shopyo Author: Abdur-Rahmaan Janhangeer Author-email:
 arj.python@gmail.com License: MIT Project-URL: Source Code, https://github.com/
 shopyo/shopyo/ Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/
 issues/ Project-URL: Changelog, https://github.com/shopyo/shopyo/blob/dev/
 CHANGES.md/ Project-URL: Twitter, https://twitter.com/shopyoproject/ Keywords:
 Flask,Django,web framework,modular Classifier: Environment :: Web Environment
```

### Comparing `shopyo-4.9.4/shopyo.egg-info/SOURCES.txt` & `shopyo-4.9.5/shopyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

