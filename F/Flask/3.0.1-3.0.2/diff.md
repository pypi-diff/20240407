# Comparing `tmp/flask-3.0.1.tar.gz` & `tmp/flask-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-3.0.1.tar", last modified: Thu Jan 18 19:57:33 2024, max compression
+gzip compressed data, was "flask-3.0.2.tar", last modified: Sat Feb  3 20:54:41 2024, max compression
```

## Comparing `flask-3.0.1.tar` & `flask-3.0.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0    68499 2024-01-18 19:57:33.000000 flask-3.0.1/CHANGES.rst
--rw-r--r--   0        0        0     8000 2024-01-18 19:57:33.000000 flask-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1475 2024-01-18 19:57:33.000000 flask-3.0.1/LICENSE.rst
--rw-r--r--   0        0        0     2063 2024-01-18 19:57:33.000000 flask-3.0.1/README.rst
--rw-r--r--   0        0        0      634 2024-01-18 19:57:33.000000 flask-3.0.1/docs/Makefile
--rw-r--r--   0        0        0   207889 2024-01-18 19:57:33.000000 flask-3.0.1/docs/_static/debugger.png
--rw-r--r--   0        0        0    24796 2024-01-18 19:57:33.000000 flask-3.0.1/docs/_static/flask-horizontal.png
--rw-r--r--   0        0        0    16021 2024-01-18 19:57:33.000000 flask-3.0.1/docs/_static/flask-vertical.png
--rw-r--r--   0        0        0    99654 2024-01-18 19:57:33.000000 flask-3.0.1/docs/_static/pycharm-run-config.png
--rw-r--r--   0        0        0     4027 2024-01-18 19:57:33.000000 flask-3.0.1/docs/_static/shortcut-icon.png
--rw-r--r--   0        0        0    21704 2024-01-18 19:57:33.000000 flask-3.0.1/docs/api.rst
--rw-r--r--   0        0        0     5127 2024-01-18 19:57:33.000000 flask-3.0.1/docs/appcontext.rst
--rw-r--r--   0        0        0     5112 2024-01-18 19:57:33.000000 flask-3.0.1/docs/async-await.rst
--rw-r--r--   0        0        0    12559 2024-01-18 19:57:33.000000 flask-3.0.1/docs/blueprints.rst
--rw-r--r--   0        0        0       45 2024-01-18 19:57:33.000000 flask-3.0.1/docs/changes.rst
--rw-r--r--   0        0        0    16701 2024-01-18 19:57:33.000000 flask-3.0.1/docs/cli.rst
--rw-r--r--   0        0        0     3238 2024-01-18 19:57:33.000000 flask-3.0.1/docs/conf.py
--rw-r--r--   0        0        0    24377 2024-01-18 19:57:33.000000 flask-3.0.1/docs/config.rst
--rw-r--r--   0        0        0       33 2024-01-18 19:57:33.000000 flask-3.0.1/docs/contributing.rst
--rw-r--r--   0        0        0     3462 2024-01-18 19:57:33.000000 flask-3.0.1/docs/debugging.rst
--rw-r--r--   0        0        0     2364 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/apache-httpd.rst
--rw-r--r--   0        0        0      673 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/asgi.rst
--rw-r--r--   0        0        0     2405 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/eventlet.rst
--rw-r--r--   0        0        0     2417 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/gevent.rst
--rw-r--r--   0        0        0     4042 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/gunicorn.rst
--rw-r--r--   0        0        0     3186 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/index.rst
--rw-r--r--   0        0        0     2813 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/mod_wsgi.rst
--rw-r--r--   0        0        0     2316 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/nginx.rst
--rw-r--r--   0        0        0     1365 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/proxy_fix.rst
--rw-r--r--   0        0        0     4768 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/uwsgi.rst
--rw-r--r--   0        0        0     2336 2024-01-18 19:57:33.000000 flask-3.0.1/docs/deploying/waitress.rst
--rw-r--r--   0        0        0    11074 2024-01-18 19:57:33.000000 flask-3.0.1/docs/design.rst
--rw-r--r--   0        0        0    18373 2024-01-18 19:57:33.000000 flask-3.0.1/docs/errorhandling.rst
--rw-r--r--   0        0        0    12781 2024-01-18 19:57:33.000000 flask-3.0.1/docs/extensiondev.rst
--rw-r--r--   0        0        0     1372 2024-01-18 19:57:33.000000 flask-3.0.1/docs/extensions.rst
--rw-r--r--   0        0        0     1887 2024-01-18 19:57:33.000000 flask-3.0.1/docs/index.rst
--rw-r--r--   0        0        0     3771 2024-01-18 19:57:33.000000 flask-3.0.1/docs/installation.rst
--rw-r--r--   0        0        0       71 2024-01-18 19:57:33.000000 flask-3.0.1/docs/license.rst
--rw-r--r--   0        0        0     8947 2024-01-18 19:57:33.000000 flask-3.0.1/docs/lifecycle.rst
--rw-r--r--   0        0        0     5910 2024-01-18 19:57:33.000000 flask-3.0.1/docs/logging.rst
--rw-r--r--   0        0        0      760 2024-01-18 19:57:33.000000 flask-3.0.1/docs/make.bat
--rw-r--r--   0        0        0     6507 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/appdispatch.rst
--rw-r--r--   0        0        0     4096 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/appfactories.rst
--rw-r--r--   0        0        0      653 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/caching.rst
--rw-r--r--   0        0        0     8670 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/celery.rst
--rw-r--r--   0        0        0     1848 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/deferredcallbacks.rst
--rw-r--r--   0        0        0     2071 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/favicon.rst
--rw-r--r--   0        0        0     7297 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/fileuploads.rst
--rw-r--r--   0        0        0     4536 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/flashing.rst
--rw-r--r--   0        0        0      961 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/index.rst
--rw-r--r--   0        0        0     8964 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/javascript.rst
--rw-r--r--   0        0        0       96 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/jquery.rst
--rw-r--r--   0        0        0     3847 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/lazyloading.rst
--rw-r--r--   0        0        0     1456 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/methodoverrides.rst
--rw-r--r--   0        0        0     2858 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/mongoengine.rst
--rw-r--r--   0        0        0     4105 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/packages.rst
--rw-r--r--   0        0        0     1861 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/requestchecksum.rst
--rw-r--r--   0        0        0      731 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/singlepageapplications.rst
--rw-r--r--   0        0        0     7294 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/sqlalchemy.rst
--rw-r--r--   0        0        0     4956 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/sqlite3.rst
--rw-r--r--   0        0        0     2635 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/streaming.rst
--rw-r--r--   0        0        0      676 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/subclassing.rst
--rw-r--r--   0        0        0     2197 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/templateinheritance.rst
--rw-r--r--   0        0        0     4306 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/urlprocessors.rst
--rw-r--r--   0        0        0     6318 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/viewdecorators.rst
--rw-r--r--   0        0        0     4709 2024-01-18 19:57:33.000000 flask-3.0.1/docs/patterns/wtforms.rst
--rw-r--r--   0        0        0    32281 2024-01-18 19:57:33.000000 flask-3.0.1/docs/quickstart.rst
--rw-r--r--   0        0        0     9334 2024-01-18 19:57:33.000000 flask-3.0.1/docs/reqcontext.rst
--rw-r--r--   0        0        0    10737 2024-01-18 19:57:33.000000 flask-3.0.1/docs/security.rst
--rw-r--r--   0        0        0     3715 2024-01-18 19:57:33.000000 flask-3.0.1/docs/server.rst
--rw-r--r--   0        0        0     3646 2024-01-18 19:57:33.000000 flask-3.0.1/docs/shell.rst
--rw-r--r--   0        0        0     6187 2024-01-18 19:57:33.000000 flask-3.0.1/docs/signals.rst
--rw-r--r--   0        0        0     7787 2024-01-18 19:57:33.000000 flask-3.0.1/docs/templating.rst
--rw-r--r--   0        0        0    10425 2024-01-18 19:57:33.000000 flask-3.0.1/docs/testing.rst
--rw-r--r--   0        0        0    11387 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/blog.rst
--rw-r--r--   0        0        0     6719 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/database.rst
--rw-r--r--   0        0        0     3699 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/deploy.rst
--rw-r--r--   0        0        0     5921 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/factory.rst
--rw-r--r--   0        0        0    13259 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/flaskr_edit.png
--rw-r--r--   0        0        0    11675 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/flaskr_index.png
--rw-r--r--   0        0        0     7455 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/flaskr_login.png
--rw-r--r--   0        0        0     2061 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/index.rst
--rw-r--r--   0        0        0     2838 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/install.rst
--rw-r--r--   0        0        0     2942 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/layout.rst
--rw-r--r--   0        0        0     1631 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/next.rst
--rw-r--r--   0        0        0     3170 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/static.rst
--rw-r--r--   0        0        0     6961 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/templates.rst
--rw-r--r--   0        0        0    18265 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/tests.rst
--rw-r--r--   0        0        0    10920 2024-01-18 19:57:33.000000 flask-3.0.1/docs/tutorial/views.rst
--rw-r--r--   0        0        0    10270 2024-01-18 19:57:33.000000 flask-3.0.1/docs/views.rst
--rw-r--r--   0        0        0      950 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/README.md
--rw-r--r--   0        0        0      102 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/make_celery.py
--rw-r--r--   0        0        0      378 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/pyproject.toml
--rw-r--r--   0        0        0     1073 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/requirements.txt
--rw-r--r--   0        0        0     1019 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/src/task_app/__init__.py
--rw-r--r--   0        0        0      484 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/src/task_app/tasks.py
--rw-r--r--   0        0        0     2909 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/src/task_app/templates/index.html
--rw-r--r--   0        0        0      954 2024-01-18 19:57:33.000000 flask-3.0.1/examples/celery/src/task_app/views.py
--rw-r--r--   0        0        0      119 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/.gitignore
--rw-r--r--   0        0        0     1475 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/LICENSE.rst
--rw-r--r--   0        0        0     1082 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/README.rst
--rw-r--r--   0        0        0       97 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/__init__.py
--rw-r--r--   0        0        0     1178 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/templates/base.html
--rw-r--r--   0        0        0      852 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/templates/fetch.html
--rw-r--r--   0        0        0      666 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/templates/jquery.html
--rw-r--r--   0        0        0      933 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/templates/xhr.html
--rw-r--r--   0        0        0      429 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/js_example/views.py
--rw-r--r--   0        0        0      689 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/pyproject.toml
--rw-r--r--   0        0        0      216 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/tests/conftest.py
--rw-r--r--   0        0        0      725 2024-01-18 19:57:33.000000 flask-3.0.1/examples/javascript/tests/test_js_example.py
--rw-r--r--   0        0        0      119 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/.gitignore
--rw-r--r--   0        0        0     1475 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/LICENSE.rst
--rw-r--r--   0        0        0     1273 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/README.rst
--rw-r--r--   0        0        0     1437 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/__init__.py
--rw-r--r--   0        0        0     3296 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/auth.py
--rw-r--r--   0        0        0     3305 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/blog.py
--rw-r--r--   0        0        0     1199 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/db.py
--rw-r--r--   0        0        0      498 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/schema.sql
--rw-r--r--   0        0        0     1696 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/static/style.css
--rw-r--r--   0        0        0      424 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/auth/login.html
--rw-r--r--   0        0        0      428 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/auth/register.html
--rw-r--r--   0        0        0      752 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/base.html
--rw-r--r--   0        0        0      447 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/blog/create.html
--rw-r--r--   0        0        0      790 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/blog/index.html
--rw-r--r--   0        0        0      690 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/flaskr/templates/blog/update.html
--rw-r--r--   0        0        0      729 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/pyproject.toml
--rw-r--r--   0        0        0     1454 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/conftest.py
--rw-r--r--   0        0        0      394 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/data.sql
--rw-r--r--   0        0        0     2070 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/test_auth.py
--rw-r--r--   0        0        0     2503 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/test_blog.py
--rw-r--r--   0        0        0      616 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/test_db.py
--rw-r--r--   0        0        0      298 2024-01-18 19:57:33.000000 flask-3.0.1/examples/tutorial/tests/test_factory.py
--rw-r--r--   0        0        0     2592 2024-01-18 19:57:33.000000 flask-3.0.1/pyproject.toml
--rw-r--r--   0        0        0        6 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/build.in
--rw-r--r--   0        0        0      227 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/build.txt
--rw-r--r--   0        0        0       61 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/dev.in
--rw-r--r--   0        0        0     2793 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/dev.txt
--rw-r--r--   0        0        0       81 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/docs.in
--rw-r--r--   0        0        0     1323 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/docs.txt
--rw-r--r--   0        0        0       64 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/tests.in
--rw-r--r--   0        0        0      335 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/tests.txt
--rw-r--r--   0        0        0       76 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/typing.in
--rw-r--r--   0        0        0      526 2024-01-18 19:57:33.000000 flask-3.0.1/requirements/typing.txt
--rw-r--r--   0        0        0     2625 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/__init__.py
--rw-r--r--   0        0        0       30 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/__main__.py
--rw-r--r--   0        0        0    59706 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/app.py
--rw-r--r--   0        0        0     3160 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/blueprints.py
--rw-r--r--   0        0        0    35715 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/cli.py
--rw-r--r--   0        0        0    13328 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/config.py
--rw-r--r--   0        0        0    15120 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/ctx.py
--rw-r--r--   0        0        0     6080 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/debughelpers.py
--rw-r--r--   0        0        0     1713 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/globals.py
--rw-r--r--   0        0        0    23084 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/helpers.py
--rw-r--r--   0        0        0     5602 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/json/__init__.py
--rw-r--r--   0        0        0     7646 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/json/provider.py
--rw-r--r--   0        0        0     9280 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/json/tag.py
--rw-r--r--   0        0        0     2377 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/logging.py
--rw-r--r--   0        0        0        0 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/py.typed
--rw-r--r--   0        0        0      228 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/sansio/README.md
--rw-r--r--   0        0        0    38209 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/sansio/app.py
--rw-r--r--   0        0        0    24637 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/sansio/blueprints.py
--rw-r--r--   0        0        0    30855 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/sansio/scaffold.py
--rw-r--r--   0        0        0    14518 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/sessions.py
--rw-r--r--   0        0        0      750 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/signals.py
--rw-r--r--   0        0        0     7537 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/templating.py
--rw-r--r--   0        0        0    10163 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/testing.py
--rw-r--r--   0        0        0     3190 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/typing.py
--rw-r--r--   0        0        0     6939 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/views.py
--rw-r--r--   0        0        0     5831 2024-01-18 19:57:33.000000 flask-3.0.1/src/flask/wrappers.py
--rw-r--r--   0        0        0     4320 2024-01-18 19:57:33.000000 flask-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0       54 2024-01-18 19:57:33.000000 flask-3.0.1/tests/static/config.json
--rw-r--r--   0        0        0       35 2024-01-18 19:57:33.000000 flask-3.0.1/tests/static/config.toml
--rw-r--r--   0        0        0       22 2024-01-18 19:57:33.000000 flask-3.0.1/tests/static/index.html
--rw-r--r--   0        0        0       55 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/_macro.html
--rw-r--r--   0        0        0       36 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/context_template.html
--rw-r--r--   0        0        0      147 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/escaping_template.html
--rw-r--r--   0        0        0       14 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/mail.txt
--rw-r--r--   0        0        0       11 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/nested/nested.txt
--rw-r--r--   0        0        0      169 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/non_escaping_template.txt
--rw-r--r--   0        0        0       23 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/simple_template.html
--rw-r--r--   0        0        0       26 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/template_filter.html
--rw-r--r--   0        0        0       51 2024-01-18 19:57:33.000000 flask-3.0.1/tests/templates/template_test.html
--rw-r--r--   0        0        0     4978 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_appctx.py
--rw-r--r--   0        0        0       33 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/.env
--rw-r--r--   0        0        0       28 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/.flaskenv
--rw-r--r--   0        0        0      256 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/__init__.py
--rw-r--r--   0        0        0      366 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/admin/__init__.py
--rw-r--r--   0        0        0       18 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/admin/static/css/test.css
--rw-r--r--   0        0        0       11 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/admin/static/test.txt
--rw-r--r--   0        0        0       21 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/admin/templates/admin/index.html
--rw-r--r--   0        0        0      327 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/frontend/__init__.py
--rw-r--r--   0        0        0       24 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html
--rw-r--r--   0        0        0        0 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/__init__.py
--rw-r--r--   0        0        0       52 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/app.py
--rw-r--r--   0        0        0      169 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/factory.py
--rw-r--r--   0        0        0       73 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/importerrorapp.py
--rw-r--r--   0        0        0       55 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/inner1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/inner1/inner2/__init__.py
--rw-r--r--   0        0        0       47 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/inner1/inner2/flask.py
--rw-r--r--   0        0        0       38 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/message.txt
--rw-r--r--   0        0        0       67 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/cliapp/multiapp.py
--rw-r--r--   0        0        0      104 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/helloworld/hello.py
--rw-r--r--   0        0        0       36 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/helloworld/wsgi.py
--rw-r--r--   0        0        0       73 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/subdomaintestmodule/__init__.py
--rw-r--r--   0        0        0       16 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_apps/subdomaintestmodule/static/hello.txt
--rw-r--r--   0        0        0     3335 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_async.py
--rw-r--r--   0        0        0    51848 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_basic.py
--rw-r--r--   0        0        0    28931 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_blueprints.py
--rw-r--r--   0        0        0    19849 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     7748 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_config.py
--rw-r--r--   0        0        0     1093 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_converters.py
--rw-r--r--   0        0        0    10286 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_helpers.py
--rw-r--r--   0        0        0     3359 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_instance_config.py
--rw-r--r--   0        0        0     8741 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_json.py
--rw-r--r--   0        0        0     1998 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_json_tag.py
--rw-r--r--   0        0        0     2529 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_logging.py
--rw-r--r--   0        0        0      712 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_regression.py
--rw-r--r--   0        0        0     8691 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_reqctx.py
--rw-r--r--   0        0        0      792 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_session_interface.py
--rw-r--r--   0        0        0     4864 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_signals.py
--rw-r--r--   0        0        0      475 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_subclassing.py
--rw-r--r--   0        0        0    12323 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_templating.py
--rw-r--r--   0        0        0    10622 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_testing.py
--rw-r--r--   0        0        0     8436 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_user_error_handler.py
--rw-r--r--   0        0        0     6732 2024-01-18 19:57:33.000000 flask-3.0.1/tests/test_views.py
--rw-r--r--   0        0        0      605 2024-01-18 19:57:33.000000 flask-3.0.1/tests/typing/typing_app_decorators.py
--rw-r--r--   0        0        0      647 2024-01-18 19:57:33.000000 flask-3.0.1/tests/typing/typing_error_handler.py
--rw-r--r--   0        0        0     2532 2024-01-18 19:57:33.000000 flask-3.0.1/tests/typing/typing_route.py
--rw-r--r--   0        0        0      775 2024-01-18 19:57:33.000000 flask-3.0.1/tox.ini
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 flask-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    68708 2024-02-03 20:54:41.000000 flask-3.0.2/CHANGES.rst
+-rw-r--r--   0        0        0     8000 2024-02-03 20:54:41.000000 flask-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1475 2024-02-03 20:54:41.000000 flask-3.0.2/LICENSE.rst
+-rw-r--r--   0        0        0     2063 2024-02-03 20:54:41.000000 flask-3.0.2/README.rst
+-rw-r--r--   0        0        0      634 2024-02-03 20:54:41.000000 flask-3.0.2/docs/Makefile
+-rw-r--r--   0        0        0   207889 2024-02-03 20:54:41.000000 flask-3.0.2/docs/_static/debugger.png
+-rw-r--r--   0        0        0    24796 2024-02-03 20:54:41.000000 flask-3.0.2/docs/_static/flask-horizontal.png
+-rw-r--r--   0        0        0    16021 2024-02-03 20:54:41.000000 flask-3.0.2/docs/_static/flask-vertical.png
+-rw-r--r--   0        0        0    99654 2024-02-03 20:54:41.000000 flask-3.0.2/docs/_static/pycharm-run-config.png
+-rw-r--r--   0        0        0     4027 2024-02-03 20:54:41.000000 flask-3.0.2/docs/_static/shortcut-icon.png
+-rw-r--r--   0        0        0    21704 2024-02-03 20:54:41.000000 flask-3.0.2/docs/api.rst
+-rw-r--r--   0        0        0     5127 2024-02-03 20:54:41.000000 flask-3.0.2/docs/appcontext.rst
+-rw-r--r--   0        0        0     5112 2024-02-03 20:54:41.000000 flask-3.0.2/docs/async-await.rst
+-rw-r--r--   0        0        0    12559 2024-02-03 20:54:41.000000 flask-3.0.2/docs/blueprints.rst
+-rw-r--r--   0        0        0       45 2024-02-03 20:54:41.000000 flask-3.0.2/docs/changes.rst
+-rw-r--r--   0        0        0    16701 2024-02-03 20:54:41.000000 flask-3.0.2/docs/cli.rst
+-rw-r--r--   0        0        0     3238 2024-02-03 20:54:41.000000 flask-3.0.2/docs/conf.py
+-rw-r--r--   0        0        0    24377 2024-02-03 20:54:41.000000 flask-3.0.2/docs/config.rst
+-rw-r--r--   0        0        0       33 2024-02-03 20:54:41.000000 flask-3.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0     3462 2024-02-03 20:54:41.000000 flask-3.0.2/docs/debugging.rst
+-rw-r--r--   0        0        0     2364 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/apache-httpd.rst
+-rw-r--r--   0        0        0      673 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/asgi.rst
+-rw-r--r--   0        0        0     2405 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/eventlet.rst
+-rw-r--r--   0        0        0     2417 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/gevent.rst
+-rw-r--r--   0        0        0     4042 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/gunicorn.rst
+-rw-r--r--   0        0        0     3186 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/index.rst
+-rw-r--r--   0        0        0     2813 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/mod_wsgi.rst
+-rw-r--r--   0        0        0     2316 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/nginx.rst
+-rw-r--r--   0        0        0     1365 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/proxy_fix.rst
+-rw-r--r--   0        0        0     4768 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/uwsgi.rst
+-rw-r--r--   0        0        0     2336 2024-02-03 20:54:41.000000 flask-3.0.2/docs/deploying/waitress.rst
+-rw-r--r--   0        0        0    11074 2024-02-03 20:54:41.000000 flask-3.0.2/docs/design.rst
+-rw-r--r--   0        0        0    18373 2024-02-03 20:54:41.000000 flask-3.0.2/docs/errorhandling.rst
+-rw-r--r--   0        0        0    12781 2024-02-03 20:54:41.000000 flask-3.0.2/docs/extensiondev.rst
+-rw-r--r--   0        0        0     1372 2024-02-03 20:54:41.000000 flask-3.0.2/docs/extensions.rst
+-rw-r--r--   0        0        0     1887 2024-02-03 20:54:41.000000 flask-3.0.2/docs/index.rst
+-rw-r--r--   0        0        0     3771 2024-02-03 20:54:41.000000 flask-3.0.2/docs/installation.rst
+-rw-r--r--   0        0        0       71 2024-02-03 20:54:41.000000 flask-3.0.2/docs/license.rst
+-rw-r--r--   0        0        0     8947 2024-02-03 20:54:41.000000 flask-3.0.2/docs/lifecycle.rst
+-rw-r--r--   0        0        0     5910 2024-02-03 20:54:41.000000 flask-3.0.2/docs/logging.rst
+-rw-r--r--   0        0        0      760 2024-02-03 20:54:41.000000 flask-3.0.2/docs/make.bat
+-rw-r--r--   0        0        0     6507 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/appdispatch.rst
+-rw-r--r--   0        0        0     4096 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/appfactories.rst
+-rw-r--r--   0        0        0      653 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/caching.rst
+-rw-r--r--   0        0        0     8670 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/celery.rst
+-rw-r--r--   0        0        0     1848 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/deferredcallbacks.rst
+-rw-r--r--   0        0        0     2071 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/favicon.rst
+-rw-r--r--   0        0        0     7297 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/fileuploads.rst
+-rw-r--r--   0        0        0     4536 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/flashing.rst
+-rw-r--r--   0        0        0      961 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/index.rst
+-rw-r--r--   0        0        0     8964 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/javascript.rst
+-rw-r--r--   0        0        0       96 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/jquery.rst
+-rw-r--r--   0        0        0     3847 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/lazyloading.rst
+-rw-r--r--   0        0        0     1456 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/methodoverrides.rst
+-rw-r--r--   0        0        0     2858 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/mongoengine.rst
+-rw-r--r--   0        0        0     4105 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/packages.rst
+-rw-r--r--   0        0        0     1861 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/requestchecksum.rst
+-rw-r--r--   0        0        0      731 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/singlepageapplications.rst
+-rw-r--r--   0        0        0     7294 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/sqlalchemy.rst
+-rw-r--r--   0        0        0     4956 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/sqlite3.rst
+-rw-r--r--   0        0        0     2635 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/streaming.rst
+-rw-r--r--   0        0        0      676 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/subclassing.rst
+-rw-r--r--   0        0        0     2197 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/templateinheritance.rst
+-rw-r--r--   0        0        0     4306 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/urlprocessors.rst
+-rw-r--r--   0        0        0     6318 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/viewdecorators.rst
+-rw-r--r--   0        0        0     4709 2024-02-03 20:54:41.000000 flask-3.0.2/docs/patterns/wtforms.rst
+-rw-r--r--   0        0        0    32281 2024-02-03 20:54:41.000000 flask-3.0.2/docs/quickstart.rst
+-rw-r--r--   0        0        0     9334 2024-02-03 20:54:41.000000 flask-3.0.2/docs/reqcontext.rst
+-rw-r--r--   0        0        0    10737 2024-02-03 20:54:41.000000 flask-3.0.2/docs/security.rst
+-rw-r--r--   0        0        0     3715 2024-02-03 20:54:41.000000 flask-3.0.2/docs/server.rst
+-rw-r--r--   0        0        0     3646 2024-02-03 20:54:41.000000 flask-3.0.2/docs/shell.rst
+-rw-r--r--   0        0        0     6187 2024-02-03 20:54:41.000000 flask-3.0.2/docs/signals.rst
+-rw-r--r--   0        0        0     7787 2024-02-03 20:54:41.000000 flask-3.0.2/docs/templating.rst
+-rw-r--r--   0        0        0    10425 2024-02-03 20:54:41.000000 flask-3.0.2/docs/testing.rst
+-rw-r--r--   0        0        0    11387 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/blog.rst
+-rw-r--r--   0        0        0     6719 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/database.rst
+-rw-r--r--   0        0        0     3699 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/deploy.rst
+-rw-r--r--   0        0        0     5921 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/factory.rst
+-rw-r--r--   0        0        0    13259 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/flaskr_edit.png
+-rw-r--r--   0        0        0    11675 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/flaskr_index.png
+-rw-r--r--   0        0        0     7455 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/flaskr_login.png
+-rw-r--r--   0        0        0     2061 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/index.rst
+-rw-r--r--   0        0        0     2838 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/install.rst
+-rw-r--r--   0        0        0     2942 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/layout.rst
+-rw-r--r--   0        0        0     1631 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/next.rst
+-rw-r--r--   0        0        0     3170 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/static.rst
+-rw-r--r--   0        0        0     6961 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/templates.rst
+-rw-r--r--   0        0        0    18265 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/tests.rst
+-rw-r--r--   0        0        0    10920 2024-02-03 20:54:41.000000 flask-3.0.2/docs/tutorial/views.rst
+-rw-r--r--   0        0        0    10270 2024-02-03 20:54:41.000000 flask-3.0.2/docs/views.rst
+-rw-r--r--   0        0        0      950 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/README.md
+-rw-r--r--   0        0        0      102 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/make_celery.py
+-rw-r--r--   0        0        0      378 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/pyproject.toml
+-rw-r--r--   0        0        0     1073 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/requirements.txt
+-rw-r--r--   0        0        0     1019 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/src/task_app/__init__.py
+-rw-r--r--   0        0        0      484 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/src/task_app/tasks.py
+-rw-r--r--   0        0        0     2909 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/src/task_app/templates/index.html
+-rw-r--r--   0        0        0      954 2024-02-03 20:54:41.000000 flask-3.0.2/examples/celery/src/task_app/views.py
+-rw-r--r--   0        0        0      119 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/.gitignore
+-rw-r--r--   0        0        0     1475 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/LICENSE.rst
+-rw-r--r--   0        0        0     1082 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/README.rst
+-rw-r--r--   0        0        0       97 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/__init__.py
+-rw-r--r--   0        0        0     1178 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/templates/base.html
+-rw-r--r--   0        0        0      852 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/templates/fetch.html
+-rw-r--r--   0        0        0      666 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/templates/jquery.html
+-rw-r--r--   0        0        0      933 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/templates/xhr.html
+-rw-r--r--   0        0        0      429 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/js_example/views.py
+-rw-r--r--   0        0        0      689 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/tests/conftest.py
+-rw-r--r--   0        0        0      725 2024-02-03 20:54:41.000000 flask-3.0.2/examples/javascript/tests/test_js_example.py
+-rw-r--r--   0        0        0      119 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/.gitignore
+-rw-r--r--   0        0        0     1475 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/LICENSE.rst
+-rw-r--r--   0        0        0     1273 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/README.rst
+-rw-r--r--   0        0        0     1437 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/__init__.py
+-rw-r--r--   0        0        0     3296 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/auth.py
+-rw-r--r--   0        0        0     3305 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/blog.py
+-rw-r--r--   0        0        0     1199 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/db.py
+-rw-r--r--   0        0        0      498 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/schema.sql
+-rw-r--r--   0        0        0     1696 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/static/style.css
+-rw-r--r--   0        0        0      424 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/auth/login.html
+-rw-r--r--   0        0        0      428 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/auth/register.html
+-rw-r--r--   0        0        0      752 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/base.html
+-rw-r--r--   0        0        0      447 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/blog/create.html
+-rw-r--r--   0        0        0      790 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/blog/index.html
+-rw-r--r--   0        0        0      690 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/flaskr/templates/blog/update.html
+-rw-r--r--   0        0        0      729 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/pyproject.toml
+-rw-r--r--   0        0        0     1454 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/conftest.py
+-rw-r--r--   0        0        0      394 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/data.sql
+-rw-r--r--   0        0        0     2070 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/test_auth.py
+-rw-r--r--   0        0        0     2503 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/test_blog.py
+-rw-r--r--   0        0        0      616 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/test_db.py
+-rw-r--r--   0        0        0      298 2024-02-03 20:54:41.000000 flask-3.0.2/examples/tutorial/tests/test_factory.py
+-rw-r--r--   0        0        0     2592 2024-02-03 20:54:41.000000 flask-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/build.in
+-rw-r--r--   0        0        0      227 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/build.txt
+-rw-r--r--   0        0        0       61 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/dev.in
+-rw-r--r--   0        0        0     2793 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/dev.txt
+-rw-r--r--   0        0        0       81 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/docs.in
+-rw-r--r--   0        0        0     1323 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/docs.txt
+-rw-r--r--   0        0        0       64 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/tests.in
+-rw-r--r--   0        0        0      335 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/tests.txt
+-rw-r--r--   0        0        0       76 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/typing.in
+-rw-r--r--   0        0        0      526 2024-02-03 20:54:41.000000 flask-3.0.2/requirements/typing.txt
+-rw-r--r--   0        0        0     2625 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/__init__.py
+-rw-r--r--   0        0        0       30 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/__main__.py
+-rw-r--r--   0        0        0    59706 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/app.py
+-rw-r--r--   0        0        0     3160 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/blueprints.py
+-rw-r--r--   0        0        0    35833 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/cli.py
+-rw-r--r--   0        0        0    13328 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/config.py
+-rw-r--r--   0        0        0    15120 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/ctx.py
+-rw-r--r--   0        0        0     6080 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/debughelpers.py
+-rw-r--r--   0        0        0     1713 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/globals.py
+-rw-r--r--   0        0        0    23084 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/helpers.py
+-rw-r--r--   0        0        0     5602 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/json/__init__.py
+-rw-r--r--   0        0        0     7646 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/json/provider.py
+-rw-r--r--   0        0        0     9280 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/json/tag.py
+-rw-r--r--   0        0        0     2377 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/logging.py
+-rw-r--r--   0        0        0        0 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/py.typed
+-rw-r--r--   0        0        0      228 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/sansio/README.md
+-rw-r--r--   0        0        0    38209 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/sansio/app.py
+-rw-r--r--   0        0        0    24637 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/sansio/blueprints.py
+-rw-r--r--   0        0        0    30879 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/sansio/scaffold.py
+-rw-r--r--   0        0        0    14518 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/sessions.py
+-rw-r--r--   0        0        0      750 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/signals.py
+-rw-r--r--   0        0        0     7537 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/templating.py
+-rw-r--r--   0        0        0    10163 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/testing.py
+-rw-r--r--   0        0        0     3190 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/typing.py
+-rw-r--r--   0        0        0     6939 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/views.py
+-rw-r--r--   0        0        0     5831 2024-02-03 20:54:41.000000 flask-3.0.2/src/flask/wrappers.py
+-rw-r--r--   0        0        0     4320 2024-02-03 20:54:41.000000 flask-3.0.2/tests/conftest.py
+-rw-r--r--   0        0        0       54 2024-02-03 20:54:41.000000 flask-3.0.2/tests/static/config.json
+-rw-r--r--   0        0        0       35 2024-02-03 20:54:41.000000 flask-3.0.2/tests/static/config.toml
+-rw-r--r--   0        0        0       22 2024-02-03 20:54:41.000000 flask-3.0.2/tests/static/index.html
+-rw-r--r--   0        0        0       55 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/_macro.html
+-rw-r--r--   0        0        0       36 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/context_template.html
+-rw-r--r--   0        0        0      147 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/escaping_template.html
+-rw-r--r--   0        0        0       14 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/mail.txt
+-rw-r--r--   0        0        0       11 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/nested/nested.txt
+-rw-r--r--   0        0        0      169 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/non_escaping_template.txt
+-rw-r--r--   0        0        0       23 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/simple_template.html
+-rw-r--r--   0        0        0       26 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/template_filter.html
+-rw-r--r--   0        0        0       51 2024-02-03 20:54:41.000000 flask-3.0.2/tests/templates/template_test.html
+-rw-r--r--   0        0        0     4978 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_appctx.py
+-rw-r--r--   0        0        0       33 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/.env
+-rw-r--r--   0        0        0       28 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/.flaskenv
+-rw-r--r--   0        0        0      256 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/__init__.py
+-rw-r--r--   0        0        0      366 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/admin/__init__.py
+-rw-r--r--   0        0        0       18 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/admin/static/css/test.css
+-rw-r--r--   0        0        0       11 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/admin/static/test.txt
+-rw-r--r--   0        0        0       21 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/admin/templates/admin/index.html
+-rw-r--r--   0        0        0      327 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/frontend/__init__.py
+-rw-r--r--   0        0        0       24 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html
+-rw-r--r--   0        0        0        0 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/__init__.py
+-rw-r--r--   0        0        0       52 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/app.py
+-rw-r--r--   0        0        0      169 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/factory.py
+-rw-r--r--   0        0        0       73 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/importerrorapp.py
+-rw-r--r--   0        0        0       55 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/inner1/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/inner1/inner2/__init__.py
+-rw-r--r--   0        0        0       47 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/inner1/inner2/flask.py
+-rw-r--r--   0        0        0       38 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/message.txt
+-rw-r--r--   0        0        0       67 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/cliapp/multiapp.py
+-rw-r--r--   0        0        0      104 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/helloworld/hello.py
+-rw-r--r--   0        0        0       36 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/helloworld/wsgi.py
+-rw-r--r--   0        0        0       73 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/subdomaintestmodule/__init__.py
+-rw-r--r--   0        0        0       16 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_apps/subdomaintestmodule/static/hello.txt
+-rw-r--r--   0        0        0     3335 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_async.py
+-rw-r--r--   0        0        0    51848 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0    28931 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_blueprints.py
+-rw-r--r--   0        0        0    20016 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     7748 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     1093 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_converters.py
+-rw-r--r--   0        0        0    10286 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_helpers.py
+-rw-r--r--   0        0        0     3359 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_instance_config.py
+-rw-r--r--   0        0        0     8741 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_json.py
+-rw-r--r--   0        0        0     1998 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_json_tag.py
+-rw-r--r--   0        0        0     2529 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_logging.py
+-rw-r--r--   0        0        0      712 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_regression.py
+-rw-r--r--   0        0        0     8691 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_reqctx.py
+-rw-r--r--   0        0        0      792 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_session_interface.py
+-rw-r--r--   0        0        0     4864 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_signals.py
+-rw-r--r--   0        0        0      475 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_subclassing.py
+-rw-r--r--   0        0        0    12323 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_templating.py
+-rw-r--r--   0        0        0    10622 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_testing.py
+-rw-r--r--   0        0        0     8436 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_user_error_handler.py
+-rw-r--r--   0        0        0     6732 2024-02-03 20:54:41.000000 flask-3.0.2/tests/test_views.py
+-rw-r--r--   0        0        0      605 2024-02-03 20:54:41.000000 flask-3.0.2/tests/typing/typing_app_decorators.py
+-rw-r--r--   0        0        0      647 2024-02-03 20:54:41.000000 flask-3.0.2/tests/typing/typing_error_handler.py
+-rw-r--r--   0        0        0     2532 2024-02-03 20:54:41.000000 flask-3.0.2/tests/typing/typing_route.py
+-rw-r--r--   0        0        0      775 2024-02-03 20:54:41.000000 flask-3.0.2/tox.ini
+-rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 flask-3.0.2/PKG-INFO
```

### Comparing `flask-3.0.1/CHANGES.rst` & `flask-3.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Version 3.0.2
+-------------
+
+Released 2024-02-03
+
+-   Correct type for ``jinja_loader`` property. :issue:`5388`
+-   Fix error with ``--extra-files`` and ``--exclude-patterns`` CLI options.
+    :issue:`5391`
+
+
 Version 3.0.1
 -------------
 
 Released 2024-01-18
 
 -   Correct type for ``path`` argument to ``send_file``. :issue:`5230`
 -   Fix a typo in an error message for the ``flask run --key`` option. :pr:`5344`
```

### Comparing `flask-3.0.1/CONTRIBUTING.rst` & `flask-3.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/LICENSE.rst` & `flask-3.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/README.rst` & `flask-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/Makefile` & `flask-3.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/_static/debugger.png` & `flask-3.0.2/docs/_static/debugger.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/_static/flask-horizontal.png` & `flask-3.0.2/docs/_static/flask-horizontal.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/_static/flask-vertical.png` & `flask-3.0.2/docs/_static/flask-vertical.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/_static/pycharm-run-config.png` & `flask-3.0.2/docs/_static/pycharm-run-config.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/_static/shortcut-icon.png` & `flask-3.0.2/docs/_static/shortcut-icon.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/api.rst` & `flask-3.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/appcontext.rst` & `flask-3.0.2/docs/appcontext.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/async-await.rst` & `flask-3.0.2/docs/async-await.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/blueprints.rst` & `flask-3.0.2/docs/blueprints.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/cli.rst` & `flask-3.0.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/conf.py` & `flask-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/config.rst` & `flask-3.0.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/debugging.rst` & `flask-3.0.2/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/apache-httpd.rst` & `flask-3.0.2/docs/deploying/apache-httpd.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/asgi.rst` & `flask-3.0.2/docs/deploying/asgi.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/eventlet.rst` & `flask-3.0.2/docs/deploying/eventlet.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/gevent.rst` & `flask-3.0.2/docs/deploying/gevent.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/gunicorn.rst` & `flask-3.0.2/docs/deploying/gunicorn.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/index.rst` & `flask-3.0.2/docs/deploying/index.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/mod_wsgi.rst` & `flask-3.0.2/docs/deploying/mod_wsgi.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/nginx.rst` & `flask-3.0.2/docs/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/proxy_fix.rst` & `flask-3.0.2/docs/deploying/proxy_fix.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/uwsgi.rst` & `flask-3.0.2/docs/deploying/uwsgi.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/deploying/waitress.rst` & `flask-3.0.2/docs/deploying/waitress.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/design.rst` & `flask-3.0.2/docs/design.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/errorhandling.rst` & `flask-3.0.2/docs/errorhandling.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/extensiondev.rst` & `flask-3.0.2/docs/extensiondev.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/extensions.rst` & `flask-3.0.2/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/index.rst` & `flask-3.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/installation.rst` & `flask-3.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/lifecycle.rst` & `flask-3.0.2/docs/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/logging.rst` & `flask-3.0.2/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/make.bat` & `flask-3.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/appdispatch.rst` & `flask-3.0.2/docs/patterns/appdispatch.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/appfactories.rst` & `flask-3.0.2/docs/patterns/appfactories.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/caching.rst` & `flask-3.0.2/docs/patterns/caching.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/celery.rst` & `flask-3.0.2/docs/patterns/celery.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/deferredcallbacks.rst` & `flask-3.0.2/docs/patterns/deferredcallbacks.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/favicon.rst` & `flask-3.0.2/docs/patterns/favicon.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/fileuploads.rst` & `flask-3.0.2/docs/patterns/fileuploads.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/flashing.rst` & `flask-3.0.2/docs/patterns/flashing.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/index.rst` & `flask-3.0.2/docs/patterns/index.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/javascript.rst` & `flask-3.0.2/docs/patterns/javascript.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/lazyloading.rst` & `flask-3.0.2/docs/patterns/lazyloading.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/methodoverrides.rst` & `flask-3.0.2/docs/patterns/methodoverrides.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/mongoengine.rst` & `flask-3.0.2/docs/patterns/mongoengine.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/packages.rst` & `flask-3.0.2/docs/patterns/packages.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/requestchecksum.rst` & `flask-3.0.2/docs/patterns/requestchecksum.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/singlepageapplications.rst` & `flask-3.0.2/docs/patterns/singlepageapplications.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/sqlalchemy.rst` & `flask-3.0.2/docs/patterns/sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/sqlite3.rst` & `flask-3.0.2/docs/patterns/sqlite3.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/streaming.rst` & `flask-3.0.2/docs/patterns/streaming.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/subclassing.rst` & `flask-3.0.2/docs/patterns/subclassing.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/templateinheritance.rst` & `flask-3.0.2/docs/patterns/templateinheritance.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/urlprocessors.rst` & `flask-3.0.2/docs/patterns/urlprocessors.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/viewdecorators.rst` & `flask-3.0.2/docs/patterns/viewdecorators.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/patterns/wtforms.rst` & `flask-3.0.2/docs/patterns/wtforms.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/quickstart.rst` & `flask-3.0.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/reqcontext.rst` & `flask-3.0.2/docs/reqcontext.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/security.rst` & `flask-3.0.2/docs/security.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/server.rst` & `flask-3.0.2/docs/server.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/shell.rst` & `flask-3.0.2/docs/shell.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/signals.rst` & `flask-3.0.2/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/templating.rst` & `flask-3.0.2/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/testing.rst` & `flask-3.0.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/blog.rst` & `flask-3.0.2/docs/tutorial/blog.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/database.rst` & `flask-3.0.2/docs/tutorial/database.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/deploy.rst` & `flask-3.0.2/docs/tutorial/deploy.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/factory.rst` & `flask-3.0.2/docs/tutorial/factory.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/flaskr_edit.png` & `flask-3.0.2/docs/tutorial/flaskr_edit.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/flaskr_index.png` & `flask-3.0.2/docs/tutorial/flaskr_index.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/flaskr_login.png` & `flask-3.0.2/docs/tutorial/flaskr_login.png`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/index.rst` & `flask-3.0.2/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/install.rst` & `flask-3.0.2/docs/tutorial/install.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/layout.rst` & `flask-3.0.2/docs/tutorial/layout.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/next.rst` & `flask-3.0.2/docs/tutorial/next.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/static.rst` & `flask-3.0.2/docs/tutorial/static.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/templates.rst` & `flask-3.0.2/docs/tutorial/templates.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/tests.rst` & `flask-3.0.2/docs/tutorial/tests.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/tutorial/views.rst` & `flask-3.0.2/docs/tutorial/views.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/docs/views.rst` & `flask-3.0.2/docs/views.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/celery/README.md` & `flask-3.0.2/examples/celery/README.md`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/celery/requirements.txt` & `flask-3.0.2/examples/celery/requirements.txt`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/celery/src/task_app/__init__.py` & `flask-3.0.2/examples/celery/src/task_app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/celery/src/task_app/templates/index.html` & `flask-3.0.2/examples/celery/src/task_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/celery/src/task_app/views.py` & `flask-3.0.2/examples/celery/src/task_app/views.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/LICENSE.rst` & `flask-3.0.2/examples/javascript/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/README.rst` & `flask-3.0.2/examples/javascript/README.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/js_example/templates/base.html` & `flask-3.0.2/examples/javascript/js_example/templates/base.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/js_example/templates/fetch.html` & `flask-3.0.2/examples/javascript/js_example/templates/fetch.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/js_example/templates/jquery.html` & `flask-3.0.2/examples/javascript/js_example/templates/jquery.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/js_example/templates/xhr.html` & `flask-3.0.2/examples/javascript/js_example/templates/xhr.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/pyproject.toml` & `flask-3.0.2/examples/javascript/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/javascript/tests/test_js_example.py` & `flask-3.0.2/examples/javascript/tests/test_js_example.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/LICENSE.rst` & `flask-3.0.2/examples/tutorial/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/README.rst` & `flask-3.0.2/examples/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/__init__.py` & `flask-3.0.2/examples/tutorial/flaskr/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/auth.py` & `flask-3.0.2/examples/tutorial/flaskr/auth.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/blog.py` & `flask-3.0.2/examples/tutorial/flaskr/blog.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/db.py` & `flask-3.0.2/examples/tutorial/flaskr/db.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/static/style.css` & `flask-3.0.2/examples/tutorial/flaskr/static/style.css`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/templates/base.html` & `flask-3.0.2/examples/tutorial/flaskr/templates/base.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/templates/blog/index.html` & `flask-3.0.2/examples/tutorial/flaskr/templates/blog/index.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/flaskr/templates/blog/update.html` & `flask-3.0.2/examples/tutorial/flaskr/templates/blog/update.html`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/pyproject.toml` & `flask-3.0.2/examples/tutorial/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/tests/conftest.py` & `flask-3.0.2/examples/tutorial/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/tests/test_auth.py` & `flask-3.0.2/examples/tutorial/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/tests/test_blog.py` & `flask-3.0.2/examples/tutorial/tests/test_blog.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/examples/tutorial/tests/test_db.py` & `flask-3.0.2/examples/tutorial/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/pyproject.toml` & `flask-3.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Flask"
-version = "3.0.1"
+version = "3.0.2"
 description = "A simple framework for building complex web applications."
 readme = "README.rst"
 license = {file = "LICENSE.rst"}
 maintainers = [{name = "Pallets", email = "contact@palletsprojects.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
```

### Comparing `flask-3.0.1/requirements/dev.txt` & `flask-3.0.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/requirements/docs.txt` & `flask-3.0.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/requirements/typing.txt` & `flask-3.0.2/requirements/typing.txt`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/__init__.py` & `flask-3.0.2/src/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/app.py` & `flask-3.0.2/src/flask/app.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/blueprints.py` & `flask-3.0.2/src/flask/blueprints.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/cli.py` & `flask-3.0.2/src/flask/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -854,15 +854,17 @@
     validated as a :class:`click.Path` type.
     """
 
     def convert(
         self, value: t.Any, param: click.Parameter | None, ctx: click.Context | None
     ) -> t.Any:
         items = self.split_envvar_value(value)
-        return [super().convert(item, param, ctx) for item in items]
+        # can't call no-arg super() inside list comprehension until Python 3.12
+        super_convert = super().convert
+        return [super_convert(item, param, ctx) for item in items]
 
 
 @click.command("run", short_help="Run a development server.")
 @click.option("--host", "-h", default="127.0.0.1", help="The interface to bind to.")
 @click.option("--port", "-p", default=5000, help="The port to bind to.")
 @click.option(
     "--cert",
```

### Comparing `flask-3.0.1/src/flask/config.py` & `flask-3.0.2/src/flask/config.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/ctx.py` & `flask-3.0.2/src/flask/ctx.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/debughelpers.py` & `flask-3.0.2/src/flask/debughelpers.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/globals.py` & `flask-3.0.2/src/flask/globals.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/helpers.py` & `flask-3.0.2/src/flask/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/json/__init__.py` & `flask-3.0.2/src/flask/json/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/json/provider.py` & `flask-3.0.2/src/flask/json/provider.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/json/tag.py` & `flask-3.0.2/src/flask/json/tag.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/logging.py` & `flask-3.0.2/src/flask/logging.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/sansio/app.py` & `flask-3.0.2/src/flask/sansio/app.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/sansio/blueprints.py` & `flask-3.0.2/src/flask/sansio/blueprints.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/sansio/scaffold.py` & `flask-3.0.2/src/flask/sansio/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pathlib
 import sys
 import typing as t
 from collections import defaultdict
 from functools import update_wrapper
 
 import click
+from jinja2 import BaseLoader
 from jinja2 import FileSystemLoader
 from werkzeug.exceptions import default_exceptions
 from werkzeug.exceptions import HTTPException
 from werkzeug.utils import cached_property
 
 from .. import typing as ft
 from ..cli import AppGroup
@@ -268,15 +269,15 @@
     def static_url_path(self, value: str | None) -> None:
         if value is not None:
             value = value.rstrip("/")
 
         self._static_url_path = value
 
     @cached_property
-    def jinja_loader(self) -> FileSystemLoader | None:
+    def jinja_loader(self) -> BaseLoader | None:
         """The Jinja loader for this object's templates. By default this
         is a class :class:`jinja2.loaders.FileSystemLoader` to
         :attr:`template_folder` if it is set.
 
         .. versionadded:: 0.5
         """
         if self.template_folder is not None:
```

### Comparing `flask-3.0.1/src/flask/sessions.py` & `flask-3.0.2/src/flask/sessions.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/signals.py` & `flask-3.0.2/src/flask/signals.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/templating.py` & `flask-3.0.2/src/flask/templating.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/testing.py` & `flask-3.0.2/src/flask/testing.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/typing.py` & `flask-3.0.2/src/flask/typing.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/views.py` & `flask-3.0.2/src/flask/views.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/src/flask/wrappers.py` & `flask-3.0.2/src/flask/wrappers.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/conftest.py` & `flask-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_appctx.py` & `flask-3.0.2/tests/test_appctx.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_async.py` & `flask-3.0.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_basic.py` & `flask-3.0.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_blueprints.py` & `flask-3.0.2/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_cli.py` & `flask-3.0.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -675,7 +675,12 @@
 def test_cli_empty(app):
     """If a Blueprint's CLI group is empty, do not register it."""
     bp = Blueprint("blue", __name__, cli_group="blue")
     app.register_blueprint(bp)
 
     result = app.test_cli_runner().invoke(args=["blue", "--help"])
     assert result.exit_code == 2, f"Unexpected success:\n\n{result.output}"
+
+
+def test_run_exclude_patterns():
+    ctx = run_command.make_context("run", ["--exclude-patterns", __file__])
+    assert ctx.params["exclude_patterns"] == [__file__]
```

### Comparing `flask-3.0.1/tests/test_config.py` & `flask-3.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_converters.py` & `flask-3.0.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_helpers.py` & `flask-3.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_instance_config.py` & `flask-3.0.2/tests/test_instance_config.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_json.py` & `flask-3.0.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_json_tag.py` & `flask-3.0.2/tests/test_json_tag.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_logging.py` & `flask-3.0.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_regression.py` & `flask-3.0.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_reqctx.py` & `flask-3.0.2/tests/test_reqctx.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_session_interface.py` & `flask-3.0.2/tests/test_session_interface.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_signals.py` & `flask-3.0.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_templating.py` & `flask-3.0.2/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_testing.py` & `flask-3.0.2/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_user_error_handler.py` & `flask-3.0.2/tests/test_user_error_handler.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/test_views.py` & `flask-3.0.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/typing/typing_app_decorators.py` & `flask-3.0.2/tests/typing/typing_app_decorators.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/typing/typing_error_handler.py` & `flask-3.0.2/tests/typing/typing_error_handler.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tests/typing/typing_route.py` & `flask-3.0.2/tests/typing/typing_route.py`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/tox.ini` & `flask-3.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `flask-3.0.1/PKG-INFO` & `flask-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask
-Version: 3.0.1
+Version: 3.0.2
 Summary: A simple framework for building complex web applications.
 Maintainer-email: Pallets <contact@palletsprojects.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
```

