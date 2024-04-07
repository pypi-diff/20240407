# Comparing `tmp/django-mp-invoices-1.1.4.tar.gz` & `tmp/django-mp-invoices-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mp-invoices-1.1.4.tar", last modified: Sat Dec 16 08:33:17 2023, max compression
+gzip compressed data, was "django-mp-invoices-1.1.5.tar", last modified: Sun Apr  7 06:41:58 2024, max compression
```

## Comparing `django-mp-invoices-1.1.4.tar` & `django-mp-invoices-1.1.5.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2022-05-18 15:26:05.000000 django-mp-invoices-1.1.4/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      321 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      369 2021-07-19 12:58:49.000000 django-mp-invoices-1.1.4/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/customers/
--rw-rw-r--   0 dev       (1000) dev       (1000)      241 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/customers/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      978 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/customers/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1207 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/customers/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.937328 django-mp-invoices-1.1.4/customers/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.937328 django-mp-invoices-1.1.4/customers/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/customers/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1357 2022-04-21 15:17:41.000000 django-mp-invoices-1.1.4/customers/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2115 2022-04-21 15:17:37.000000 django-mp-invoices-1.1.4/customers/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/customers/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)      842 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.4/customers/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      415 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.4/customers/migrations/0002_customer_discount.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.4/customers/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1103 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/customers/models.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.937328 django-mp-invoices-1.1.4/customers/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/customers/templates/customers/
--rw-rw-r--   0 dev       (1000) dev       (1000)      421 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.4/customers/templates/customers/actions_cell.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1395 2022-06-13 08:48:00.000000 django-mp-invoices-1.1.4/customers/templates/customers/detail.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      411 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.4/customers/templates/customers/sale_count_cell.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      339 2022-06-20 10:46:11.000000 django-mp-invoices-1.1.4/customers/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2464 2022-06-20 10:46:11.000000 django-mp-invoices-1.1.4/customers/views.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      321 2023-12-16 08:33:17.000000 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     4774 2023-12-16 08:33:17.000000 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-12-16 08:33:17.000000 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      289 2023-12-16 08:33:17.000000 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       46 2023-12-16 08:33:17.000000 django-mp-invoices-1.1.4/django_mp_invoices.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1808 2023-12-16 07:20:09.000000 django-mp-invoices-1.1.4/invoices/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      315 2023-09-21 13:52:11.000000 django-mp-invoices-1.1.4/invoices/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3247 2023-12-16 07:51:59.000000 django-mp-invoices-1.1.4/invoices/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      467 2022-11-20 09:48:42.000000 django-mp-invoices-1.1.4/invoices/conf.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3786 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.4/invoices/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     3880 2022-11-20 10:05:54.000000 django-mp-invoices-1.1.4/invoices/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)    11001 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.4/invoices/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     4508 2022-11-20 10:05:54.000000 django-mp-invoices-1.1.4/invoices/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)    10693 2022-11-20 09:51:41.000000 django-mp-invoices-1.1.4/invoices/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/management/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2019-02-15 15:34:44.000000 django-mp-invoices-1.1.4/invoices/management/__init__.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/management/commands/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2019-02-15 15:34:44.000000 django-mp-invoices-1.1.4/invoices/management/commands/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1577 2022-05-25 16:33:50.000000 django-mp-invoices-1.1.4/invoices/management/commands/sync_arrivals.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      387 2022-04-15 10:45:14.000000 django-mp-invoices-1.1.4/invoices/middleware.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     4585 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1269 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/migrations/0002_invoice_creator.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      561 2021-03-13 06:00:05.000000 django-mp-invoices-1.1.4/invoices/migrations/0003_change_qty_to_float.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1187 2022-05-18 14:13:24.000000 django-mp-invoices-1.1.4/invoices/migrations/0004_auto_20220115_1231.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      619 2022-04-21 15:32:08.000000 django-mp-invoices-1.1.4/invoices/migrations/0005_arrival_supplier.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1035 2022-05-25 13:11:32.000000 django-mp-invoices-1.1.4/invoices/migrations/0006_invoice_currency.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      566 2022-07-24 08:17:09.000000 django-mp-invoices-1.1.4/invoices/migrations/0007_currency_rate.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      759 2022-11-20 07:46:02.000000 django-mp-invoices-1.1.4/invoices/migrations/0008_totals.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      776 2022-12-05 15:12:13.000000 django-mp-invoices-1.1.4/invoices/migrations/0009_auto_20221205_1712.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)    14016 2023-12-16 08:00:09.000000 django-mp-invoices-1.1.4/invoices/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4370 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.4/invoices/service.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/invoices/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/static/invoices/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1517 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/static/invoices/CategoryTree.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      937 2023-12-16 08:28:56.000000 django-mp-invoices-1.1.4/invoices/static/invoices/ContactChoiceField.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      501 2022-07-24 08:31:54.000000 django-mp-invoices-1.1.4/invoices/static/invoices/CurrencyRateInput.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      505 2022-05-25 13:11:32.000000 django-mp-invoices-1.1.4/invoices/static/invoices/CurrencySelect.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     3635 2023-12-16 08:28:56.000000 django-mp-invoices-1.1.4/invoices/static/invoices/InvoiceList.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      464 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/static/invoices/InvoiceTotal.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      703 2022-04-23 13:05:23.000000 django-mp-invoices-1.1.4/invoices/static/invoices/SelectProductList.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      303 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/static/invoices/SelectServiceItemList.js
--rw-rw-r--   0 dev       (1000) dev       (1000)      680 2022-07-24 08:27:54.000000 django-mp-invoices-1.1.4/invoices/static/invoices/invoices.css
--rwxrwxr-x   0 dev       (1000) dev       (1000)     8012 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/static/invoices/jquery.scannerdetection.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/templates/
--rw-rw-r--   0 dev       (1000) dev       (1000)       33 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/accounting.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/templates/invoices/
--rw-rw-r--   0 dev       (1000) dev       (1000)      280 2022-05-22 07:56:13.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/contact-select.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2639 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/history.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1349 2021-03-13 06:57:34.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/index_page_section.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1332 2022-06-13 08:48:00.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/item.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      172 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/list_item_actions.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     9644 2022-12-05 15:19:27.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/manage.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      181 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/name_cell.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     3414 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/print.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      579 2021-04-15 10:18:49.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/product-items.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     3357 2022-05-24 12:10:30.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/product-select-list.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/templates/invoices/report/
--rw-rw-r--   0 dev       (1000) dev       (1000)      135 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/report/arrival-report.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     5299 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/report/base.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1201 2022-12-14 14:54:05.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/report/report-item.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     3469 2022-12-06 09:39:32.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/report/sale-report.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2927 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templates/invoices/service-select-list.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/invoices/templatetags/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.4/invoices/templatetags/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1977 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.4/invoices/templatetags/invoices.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1001 2022-11-03 18:38:52.000000 django-mp-invoices-1.1.4/invoices/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     6952 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.4/invoices/views.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/managers/
--rw-rw-r--   0 dev       (1000) dev       (1000)      236 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/managers/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      124 2022-05-18 14:13:24.000000 django-mp-invoices-1.1.4/managers/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      633 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/managers/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/managers/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/managers/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/managers/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      823 2022-05-22 08:02:05.000000 django-mp-invoices-1.1.4/managers/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     1172 2022-05-22 08:02:05.000000 django-mp-invoices-1.1.4/managers/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/managers/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)      648 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.4/managers/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.4/managers/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      763 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/managers/models.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/products/
--rw-rw-r--   0 dev       (1000) dev       (1000)      454 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/products/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3222 2023-10-30 10:35:16.000000 django-mp-invoices-1.1.4/products/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1936 2023-10-30 10:35:55.000000 django-mp-invoices-1.1.4/products/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/products/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/products/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/products/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     1948 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/products/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/products/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1378 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2444 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)      358 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/managers.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/products/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     3049 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      576 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/migrations/0002_tecdoc.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      418 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/migrations/0003_product_tecdoc_description.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      351 2022-06-18 06:32:22.000000 django-mp-invoices-1.1.4/products/migrations/0004_remove_product_tecdoc_description.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2153 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/products/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      892 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/querysets.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1691 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.4/products/tasks.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/products/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.945329 django-mp-invoices-1.1.4/products/templates/products/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/products/templates/products/admin/
--rw-rw-r--   0 dev       (1000) dev       (1000)      379 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/templates/products/admin/changeform.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      725 2022-06-13 08:57:28.000000 django-mp-invoices-1.1.4/products/templates/products/admin/list_item_actions.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      176 2022-06-13 08:57:28.000000 django-mp-invoices-1.1.4/products/templates/products/admin/product_name.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2149 2022-06-13 09:26:27.000000 django-mp-invoices-1.1.4/products/templates/products/history.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      377 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/templates/products/print_bar_code.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      662 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.4/products/templates/products/print_name.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      681 2022-06-20 10:35:46.000000 django-mp-invoices-1.1.4/products/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2947 2022-06-20 10:37:41.000000 django-mp-invoices-1.1.4/products/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      289 2023-12-16 07:32:04.000000 django-mp-invoices-1.1.4/requirements.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/services/
--rw-rw-r--   0 dev       (1000) dev       (1000)      354 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.4/services/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      671 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1732 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.4/services/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/services/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/services/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/services/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     4031 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/services/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/services/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2845 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     5230 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)      303 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/managers.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      387 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/middleware.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/services/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2775 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1114 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/migrations/0002_worker.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3975 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.4/services/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      561 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/querysets.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1250 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.4/services/service.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.941329 django-mp-invoices-1.1.4/services/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/services/templates/services/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2438 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/add-service-item.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      974 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/item.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     5168 2023-12-16 08:29:51.000000 django-mp-invoices-1.1.4/services/templates/services/manage.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1457 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/print-service-items.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1057 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/print-services-table.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1722 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/print-services.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2728 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/report.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      459 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/templates/services/service-items.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      786 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.4/services/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4118 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.4/services/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)       38 2023-12-16 08:33:17.949329 django-mp-invoices-1.1.4/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      544 2023-12-16 07:12:57.000000 django-mp-invoices-1.1.4/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.918197 django-mp-invoices-1.1.5/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2022-05-18 15:26:05.000000 django-mp-invoices-1.1.5/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      321 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      369 2021-07-19 12:58:49.000000 django-mp-invoices-1.1.5/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/customers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      241 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/customers/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      978 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/customers/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1207 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/customers/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/customers/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/customers/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/customers/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1357 2022-04-21 15:17:41.000000 django-mp-invoices-1.1.5/customers/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2115 2022-04-21 15:17:37.000000 django-mp-invoices-1.1.5/customers/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/customers/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      842 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.5/customers/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      415 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.5/customers/migrations/0002_customer_discount.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.5/customers/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1103 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/customers/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/customers/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/customers/templates/customers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      421 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.5/customers/templates/customers/actions_cell.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1395 2022-06-13 08:48:00.000000 django-mp-invoices-1.1.5/customers/templates/customers/detail.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      411 2022-02-09 10:39:38.000000 django-mp-invoices-1.1.5/customers/templates/customers/sale_count_cell.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      339 2022-06-20 10:46:11.000000 django-mp-invoices-1.1.5/customers/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2464 2022-06-20 10:46:11.000000 django-mp-invoices-1.1.5/customers/views.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      321 2024-04-07 06:41:58.000000 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4774 2024-04-07 06:41:58.000000 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2024-04-07 06:41:58.000000 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      289 2024-04-07 06:41:58.000000 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       46 2024-04-07 06:41:58.000000 django-mp-invoices-1.1.5/django_mp_invoices.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1808 2023-12-16 07:20:09.000000 django-mp-invoices-1.1.5/invoices/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      315 2023-09-21 13:52:11.000000 django-mp-invoices-1.1.5/invoices/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3247 2023-12-16 07:51:59.000000 django-mp-invoices-1.1.5/invoices/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      467 2022-11-20 09:48:42.000000 django-mp-invoices-1.1.5/invoices/conf.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3786 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.5/invoices/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/invoices/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/invoices/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3880 2022-11-20 10:05:54.000000 django-mp-invoices-1.1.5/invoices/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)    11001 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.5/invoices/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/invoices/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4508 2022-11-20 10:05:54.000000 django-mp-invoices-1.1.5/invoices/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)    10693 2022-11-20 09:51:41.000000 django-mp-invoices-1.1.5/invoices/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/management/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2019-02-15 15:34:44.000000 django-mp-invoices-1.1.5/invoices/management/__init__.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/management/commands/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2019-02-15 15:34:44.000000 django-mp-invoices-1.1.5/invoices/management/commands/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1577 2022-05-25 16:33:50.000000 django-mp-invoices-1.1.5/invoices/management/commands/sync_arrivals.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      387 2022-04-15 10:45:14.000000 django-mp-invoices-1.1.5/invoices/middleware.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4585 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1269 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/migrations/0002_invoice_creator.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      561 2021-03-13 06:00:05.000000 django-mp-invoices-1.1.5/invoices/migrations/0003_change_qty_to_float.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1187 2022-05-18 14:13:24.000000 django-mp-invoices-1.1.5/invoices/migrations/0004_auto_20220115_1231.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      619 2022-04-21 15:32:08.000000 django-mp-invoices-1.1.5/invoices/migrations/0005_arrival_supplier.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1035 2022-05-25 13:11:32.000000 django-mp-invoices-1.1.5/invoices/migrations/0006_invoice_currency.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      566 2022-07-24 08:17:09.000000 django-mp-invoices-1.1.5/invoices/migrations/0007_currency_rate.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      759 2022-11-20 07:46:02.000000 django-mp-invoices-1.1.5/invoices/migrations/0008_totals.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      776 2022-12-05 15:12:13.000000 django-mp-invoices-1.1.5/invoices/migrations/0009_auto_20221205_1712.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)    14016 2023-12-16 08:00:09.000000 django-mp-invoices-1.1.5/invoices/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4370 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.5/invoices/service.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/invoices/static/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/static/invoices/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1517 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/static/invoices/CategoryTree.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      937 2023-12-16 08:28:56.000000 django-mp-invoices-1.1.5/invoices/static/invoices/ContactChoiceField.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      501 2022-07-24 08:31:54.000000 django-mp-invoices-1.1.5/invoices/static/invoices/CurrencyRateInput.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      505 2022-05-25 13:11:32.000000 django-mp-invoices-1.1.5/invoices/static/invoices/CurrencySelect.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3635 2023-12-16 08:28:56.000000 django-mp-invoices-1.1.5/invoices/static/invoices/InvoiceList.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      464 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/static/invoices/InvoiceTotal.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      703 2022-04-23 13:05:23.000000 django-mp-invoices-1.1.5/invoices/static/invoices/SelectProductList.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      303 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/static/invoices/SelectServiceItemList.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)      680 2022-07-24 08:27:54.000000 django-mp-invoices-1.1.5/invoices/static/invoices/invoices.css
+-rwxrwxr-x   0 dev       (1000) dev       (1000)     8012 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/static/invoices/jquery.scannerdetection.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/templates/
+-rw-rw-r--   0 dev       (1000) dev       (1000)       33 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/accounting.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.910197 django-mp-invoices-1.1.5/invoices/templates/invoices/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      280 2022-05-22 07:56:13.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/contact-select.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2639 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/history.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1349 2021-03-13 06:57:34.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/index_page_section.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1332 2022-06-13 08:48:00.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/item.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      172 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/list_item_actions.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     9644 2022-12-05 15:19:27.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/manage.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      181 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/name_cell.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3414 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/print.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      579 2021-04-15 10:18:49.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/product-items.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3357 2022-05-24 12:10:30.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/product-select-list.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/invoices/templates/invoices/report/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      135 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/report/arrival-report.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5299 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/report/base.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1201 2022-12-14 14:54:05.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/report/report-item.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3469 2022-12-06 09:39:32.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/report/sale-report.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2927 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templates/invoices/service-select-list.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/invoices/templatetags/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-01-02 20:53:26.000000 django-mp-invoices-1.1.5/invoices/templatetags/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1977 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.5/invoices/templatetags/invoices.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1001 2022-11-03 18:38:52.000000 django-mp-invoices-1.1.5/invoices/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6952 2023-12-16 07:11:37.000000 django-mp-invoices-1.1.5/invoices/views.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/managers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      236 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/managers/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      124 2022-05-18 14:13:24.000000 django-mp-invoices-1.1.5/managers/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      633 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/managers/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/managers/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/managers/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/managers/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      823 2022-05-22 08:02:05.000000 django-mp-invoices-1.1.5/managers/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1172 2022-05-22 08:02:05.000000 django-mp-invoices-1.1.5/managers/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/managers/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      648 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.5/managers/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-01-24 08:16:12.000000 django-mp-invoices-1.1.5/managers/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      763 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/managers/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      454 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/products/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3222 2023-10-30 10:35:16.000000 django-mp-invoices-1.1.5/products/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1936 2023-10-30 10:35:55.000000 django-mp-invoices-1.1.5/products/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/products/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/products/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1948 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/products/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1378 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2444 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/locale/uk/LC_MESSAGES/django.po
+-rw-rw-r--   0 dev       (1000) dev       (1000)      358 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/managers.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3049 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      576 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/migrations/0002_tecdoc.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      418 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/migrations/0003_product_tecdoc_description.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      351 2022-06-18 06:32:22.000000 django-mp-invoices-1.1.5/products/migrations/0004_remove_product_tecdoc_description.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2153 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/products/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      892 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/querysets.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1691 2023-09-23 10:10:01.000000 django-mp-invoices-1.1.5/products/tasks.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/products/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/templates/products/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/products/templates/products/admin/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      379 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/templates/products/admin/changeform.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      725 2022-06-13 08:57:28.000000 django-mp-invoices-1.1.5/products/templates/products/admin/list_item_actions.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      176 2022-06-13 08:57:28.000000 django-mp-invoices-1.1.5/products/templates/products/admin/product_name.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2149 2022-06-13 09:26:27.000000 django-mp-invoices-1.1.5/products/templates/products/history.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      377 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/templates/products/print_bar_code.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      662 2022-06-13 08:55:39.000000 django-mp-invoices-1.1.5/products/templates/products/print_name.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      681 2022-06-20 10:35:46.000000 django-mp-invoices-1.1.5/products/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2947 2022-06-20 10:37:41.000000 django-mp-invoices-1.1.5/products/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      289 2024-04-07 06:40:00.000000 django-mp-invoices-1.1.5/requirements.txt
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/services/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      354 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.5/services/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      671 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1732 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.5/services/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/services/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/services/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/services/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4031 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/services/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/services/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2845 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5230 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/locale/uk/LC_MESSAGES/django.po
+-rw-rw-r--   0 dev       (1000) dev       (1000)      303 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/managers.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      387 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/middleware.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/services/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2775 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1114 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/migrations/0002_worker.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3975 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.5/services/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      561 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/querysets.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1250 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.5/services/service.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.906197 django-mp-invoices-1.1.5/services/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:41:58.914197 django-mp-invoices-1.1.5/services/templates/services/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2438 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/add-service-item.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      974 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/item.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5168 2023-12-16 08:29:51.000000 django-mp-invoices-1.1.5/services/templates/services/manage.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1457 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/print-service-items.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1057 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/print-services-table.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1722 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/print-services.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2728 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/report.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      459 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/templates/services/service-items.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      786 2022-11-19 14:02:57.000000 django-mp-invoices-1.1.5/services/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4118 2023-12-16 07:18:40.000000 django-mp-invoices-1.1.5/services/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)       38 2024-04-07 06:41:58.918197 django-mp-invoices-1.1.5/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      544 2024-04-07 06:40:09.000000 django-mp-invoices-1.1.5/setup.py
```

### Comparing `django-mp-invoices-1.1.4/customers/admin.py` & `django-mp-invoices-1.1.5/customers/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/forms.py` & `django-mp-invoices-1.1.5/customers/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/locale/uk/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/customers/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/locale/uk/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/customers/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/migrations/0001_initial.py` & `django-mp-invoices-1.1.5/customers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/models.py` & `django-mp-invoices-1.1.5/customers/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/templates/customers/detail.html` & `django-mp-invoices-1.1.5/customers/templates/customers/detail.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/customers/views.py` & `django-mp-invoices-1.1.5/customers/views.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/django_mp_invoices.egg-info/SOURCES.txt` & `django-mp-invoices-1.1.5/django_mp_invoices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/__init__.py` & `django-mp-invoices-1.1.5/invoices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/admin.py` & `django-mp-invoices-1.1.5/invoices/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/forms.py` & `django-mp-invoices-1.1.5/invoices/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/locale/ru/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/invoices/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/locale/ru/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/invoices/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/locale/uk/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/invoices/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/locale/uk/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/invoices/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/management/commands/sync_arrivals.py` & `django-mp-invoices-1.1.5/invoices/management/commands/sync_arrivals.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0001_initial.py` & `django-mp-invoices-1.1.5/invoices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0002_invoice_creator.py` & `django-mp-invoices-1.1.5/invoices/migrations/0002_invoice_creator.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0003_change_qty_to_float.py` & `django-mp-invoices-1.1.5/invoices/migrations/0003_change_qty_to_float.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0004_auto_20220115_1231.py` & `django-mp-invoices-1.1.5/invoices/migrations/0004_auto_20220115_1231.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0005_arrival_supplier.py` & `django-mp-invoices-1.1.5/invoices/migrations/0005_arrival_supplier.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0006_invoice_currency.py` & `django-mp-invoices-1.1.5/invoices/migrations/0006_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0007_currency_rate.py` & `django-mp-invoices-1.1.5/invoices/migrations/0007_currency_rate.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0008_totals.py` & `django-mp-invoices-1.1.5/invoices/migrations/0008_totals.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/migrations/0009_auto_20221205_1712.py` & `django-mp-invoices-1.1.5/invoices/migrations/0009_auto_20221205_1712.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/models.py` & `django-mp-invoices-1.1.5/invoices/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/service.py` & `django-mp-invoices-1.1.5/invoices/service.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/CategoryTree.js` & `django-mp-invoices-1.1.5/invoices/static/invoices/CategoryTree.js`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/ContactChoiceField.js` & `django-mp-invoices-1.1.5/invoices/static/invoices/ContactChoiceField.js`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/InvoiceList.js` & `django-mp-invoices-1.1.5/invoices/static/invoices/InvoiceList.js`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/SelectProductList.js` & `django-mp-invoices-1.1.5/invoices/static/invoices/SelectProductList.js`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/invoices.css` & `django-mp-invoices-1.1.5/invoices/static/invoices/invoices.css`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/static/invoices/jquery.scannerdetection.js` & `django-mp-invoices-1.1.5/invoices/static/invoices/jquery.scannerdetection.js`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/history.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/history.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/index_page_section.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/index_page_section.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/item.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/item.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/manage.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/manage.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/print.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/print.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/product-items.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/product-items.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/product-select-list.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/product-select-list.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/report/base.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/report/base.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/report/report-item.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/report/report-item.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/report/sale-report.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/report/sale-report.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templates/invoices/service-select-list.html` & `django-mp-invoices-1.1.5/invoices/templates/invoices/service-select-list.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/templatetags/invoices.py` & `django-mp-invoices-1.1.5/invoices/templatetags/invoices.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/urls.py` & `django-mp-invoices-1.1.5/invoices/urls.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/invoices/views.py` & `django-mp-invoices-1.1.5/invoices/views.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/managers/forms.py` & `django-mp-invoices-1.1.5/managers/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/managers/locale/uk/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/managers/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/managers/locale/uk/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/managers/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/managers/migrations/0001_initial.py` & `django-mp-invoices-1.1.5/managers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/managers/models.py` & `django-mp-invoices-1.1.5/managers/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/admin.py` & `django-mp-invoices-1.1.5/products/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/forms.py` & `django-mp-invoices-1.1.5/products/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/locale/ru/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/products/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/locale/ru/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/products/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/locale/uk/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/products/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/locale/uk/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/products/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/migrations/0001_initial.py` & `django-mp-invoices-1.1.5/products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/migrations/0002_tecdoc.py` & `django-mp-invoices-1.1.5/products/migrations/0002_tecdoc.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/models.py` & `django-mp-invoices-1.1.5/products/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/querysets.py` & `django-mp-invoices-1.1.5/products/querysets.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/tasks.py` & `django-mp-invoices-1.1.5/products/tasks.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/templates/products/admin/list_item_actions.html` & `django-mp-invoices-1.1.5/products/templates/products/admin/list_item_actions.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/templates/products/history.html` & `django-mp-invoices-1.1.5/products/templates/products/history.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/templates/products/print_name.html` & `django-mp-invoices-1.1.5/products/templates/products/print_name.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/urls.py` & `django-mp-invoices-1.1.5/products/urls.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/products/views.py` & `django-mp-invoices-1.1.5/products/views.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/admin.py` & `django-mp-invoices-1.1.5/services/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/forms.py` & `django-mp-invoices-1.1.5/services/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/locale/ru/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/services/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/locale/ru/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/services/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/locale/uk/LC_MESSAGES/django.mo` & `django-mp-invoices-1.1.5/services/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/locale/uk/LC_MESSAGES/django.po` & `django-mp-invoices-1.1.5/services/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/migrations/0001_initial.py` & `django-mp-invoices-1.1.5/services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/migrations/0002_worker.py` & `django-mp-invoices-1.1.5/services/migrations/0002_worker.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/models.py` & `django-mp-invoices-1.1.5/services/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/querysets.py` & `django-mp-invoices-1.1.5/services/querysets.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/service.py` & `django-mp-invoices-1.1.5/services/service.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/add-service-item.html` & `django-mp-invoices-1.1.5/services/templates/services/add-service-item.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/item.html` & `django-mp-invoices-1.1.5/services/templates/services/item.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/manage.html` & `django-mp-invoices-1.1.5/services/templates/services/manage.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/print-service-items.html` & `django-mp-invoices-1.1.5/services/templates/services/print-service-items.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/print-services-table.html` & `django-mp-invoices-1.1.5/services/templates/services/print-services-table.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/print-services.html` & `django-mp-invoices-1.1.5/services/templates/services/print-services.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/templates/services/report.html` & `django-mp-invoices-1.1.5/services/templates/services/report.html`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/urls.py` & `django-mp-invoices-1.1.5/services/urls.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/services/views.py` & `django-mp-invoices-1.1.5/services/views.py`

 * *Files identical despite different names*

### Comparing `django-mp-invoices-1.1.4/setup.py` & `django-mp-invoices-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 
-version = '1.1.4'
+version = '1.1.5'
 url = 'https://github.com/pmaigutyak/mp-invoices'
 
 
 setup(
     name='django-mp-invoices',
     version=version,
     description='Django invoices apps',
```

