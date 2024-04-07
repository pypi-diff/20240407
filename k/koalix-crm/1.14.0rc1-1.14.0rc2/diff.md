# Comparing `tmp/koalix-crm-1.14.0rc1.tar.gz` & `tmp/koalix-crm-1.14.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koalix-crm-1.14.0rc1.tar", last modified: Sat Apr  6 11:47:58 2024, max compression
+gzip compressed data, was "koalix-crm-1.14.0rc2.tar", last modified: Sun Apr  7 09:40:32 2024, max compression
```

## Comparing `koalix-crm-1.14.0rc1.tar` & `koalix-crm-1.14.0rc2.tar`

### file list

```diff
@@ -1,456 +1,455 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/koalix_crm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-04-06 11:47:58.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 11:47:57.000000 koalix-crm-1.14.0rc1/koalix_crm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.019991 koalix-crm-1.14.0rc1/koalixcrm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.019991 koalix-crm-1.14.0rc1/koalixcrm/accounting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/accounting_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/booking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/product_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/const/accountTypeChoices.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/factories/factory_product_category.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.023991 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0011_auto_20240329_2207.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/account_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/accounting_period_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/booking_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/product_categorie_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/restinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/
--rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/test_accountingModelTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/accounting/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/crm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.027991 koalix-crm-1.14.0rc1/koalixcrm/crm/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/country.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/postaladdressprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/const/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.031991 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/call.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_billing_cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/email_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/phone_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/postal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/contact/supplier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.031991 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/delivery_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/payment_reminder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/pdf_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_confirmation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.039991 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_billing_cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_delivery_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_project_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_task_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_human_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_payment_reminder.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_postal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_price.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_purchase_confirmation.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_purchase_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_price.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_work.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/inlinemixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.039991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    45333 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.011991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.043991 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/middleware/timezoneMiddleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.055992 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    53282 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
--rw-r--r--   0 runner    (1001) docker     (127)    42385 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
--rw-r--r--   0 runner    (1001) docker     (127)    41477 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0021_purchaseorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0034_genericprojectlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0044_reportingperiod_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0047_work_worked_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
--rw-r--r--   0 runner    (1001) docker     (127)    17512 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0059_auto_20240329_2207.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.055992 koalix-crm-1.14.0rc1/koalixcrm/crm/product/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/customer_group_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/price.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.059991 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_project_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_task_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/human_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    26915 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.063991 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_status_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_type_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/contact_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/currency_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_billing_cycle_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_group_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_status_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/human_resource_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/product_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_status_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_status_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_manager_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_price_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_type_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/restinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_status_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/tax_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/unit_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/rest/work_rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.067992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/
--rw-r--r--   0 runner    (1001) docker     (127)    50507 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50540 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/invoice.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    30645 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/project_report.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/quote.xsl
--rwxr-xr-x   0 runner    (1001) docker     (127)    27411 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/work_report.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.067992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/
--rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50599 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/invoice.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    50630 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/quote.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.071992 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/
--rw-r--r--   0 runner    (1001) docker     (127)   704128 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   756072 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   122303 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
--rw-r--r--   0 runner    (1001) docker     (127)   156738 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/logo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.071992 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/create_work_report.html
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/exception.html
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/register_payment.html
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/set_timezone.html
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/time_reporting.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.075991 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_calculations_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_delete_of_empty_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_admin_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_effective_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_planned_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_supplier_admin_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_effort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_effort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_update_last_status_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_time_tracking_add_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_user_is_not_human_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_version_increase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_view_work_entry_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_work_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/crm/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_work_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/newdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/pdfexport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/range_selection_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/reporting_period_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/set_timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/template_set_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/time_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_extension_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_is_not_human_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_formset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.079991 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/const/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_document_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_template_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.083992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/document_template_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/template_set_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/document_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/template_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/user_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/global_support_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/const/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/subscriptions/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.087992 koalix-crm-1.14.0rc1/koalixcrm/test/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/UITests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/test/test_support_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/koalixcrm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.015991 koalix-crm-1.14.0rc1/projectsettings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/projectsettings/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/base_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/development_docker_sqlite_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/projectsettings/settings/production_docker_postgres_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:47:58.091992 koalix-crm-1.14.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-06 11:47:54.000000 koalix-crm-1.14.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.569444 koalix-crm-1.14.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-07 09:40:32.569444 koalix-crm-1.14.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.569444 koalix-crm-1.14.0rc2/koalix_crm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 09:40:32.000000 koalix-crm-1.14.0rc2/koalix_crm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.501444 koalix-crm-1.14.0rc2/koalixcrm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.501444 koalix-crm-1.14.0rc2/koalixcrm/accounting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/accounting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/booking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/product_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/const/accountTypeChoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/factories/factory_product_category.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.505444 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0003_remove_account_originalamount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0011_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/account_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/accounting_period_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/booking_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/product_categorie_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/restinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/accounting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/tests/test_accountingModelTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/accounting/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/crm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.509444 koalix-crm-1.14.0rc2/koalixcrm/crm/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/const/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/const/postaladdressprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/const/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/const/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.513444 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer_billing_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/email_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/phone_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/contact/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.513444 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/delivery_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/payment_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/pdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/purchase_confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/purchase_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/sales_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/documents/sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_agreement_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_agreement_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_currency_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer_billing_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer_group_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_delivery_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_estimation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_generic_project_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_generic_task_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_payment_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_product_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_project_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_purchase_confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_purchase_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_reporting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_reporting_period_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_sales_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_unit_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/inlinemixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    45333 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.493444 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.521444 koalix-crm-1.14.0rc2/koalixcrm/crm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/middleware/timezoneMiddleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.533444 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    53282 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0002_auto_20170927_2042.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42385 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0003_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0004_auto_20171009_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41477 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0005_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0006_auto_20171210_1805.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0007_auto_20171210_2126.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0008_auto_20180104_2042.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0009_auto_20180104_2111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0010_auto_20180104_2138.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0011_auto_20180104_2152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0012_auto_20180105_1840.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0013_auto_20180105_2159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0014_auto_20180108_2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0015_auto_20180111_2043.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0016_auto_20180111_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0017_auto_20180111_2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0018_auto_20180111_2031.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0019_auto_20180112_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0020_auto_20180116_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0021_purchaseorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0022_auto_20180117_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0023_auto_20180119_2102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0024_auto_20180122_2121.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0025_auto_20180413_1937.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0026_auto_20180507_1957.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0027_auto_20180606_2034.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0028_auto_20180611_1835.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0029_auto_20180611_1903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0030_auto_20180611_1930.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0031_auto_20180612_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0032_auto_20180612_1925.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0033_auto_20180612_1936.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0034_genericprojectlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0035_auto_20180619_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0036_auto_20180626_2059.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0037_auto_20180701_2128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0038_auto_20180702_1628.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0039_auto_20180702_1635.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0040_auto_20180724_1657.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0041_auto_20180724_1657.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0042_auto_20180724_1816.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0043_reportingperiodstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0044_reportingperiod_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0045_auto_20180805_2047.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0046_auto_20180805_2051.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0047_work_worked_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0048_auto_20181012_2056.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0049_auto_20181014_2258.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0050_auto_20181014_2300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0051_auto_20181014_2302.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0052_auto_20181014_2304.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17512 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0053_auto_20181014_2305.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0054_auto_20181020_1845.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0055_auto_20181022_1937.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0056_auto_20181216_2224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0056_auto_20190102_2230.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0057_merge_20190106_1510.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0058_auto_20190401_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0059_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.533444 koalix-crm-1.14.0rc2/koalixcrm/crm/product/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/currency_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/customer_group_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/product_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/product/unit_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.537444 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/estimation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/generic_project_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/generic_task_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26915 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/reporting_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/reporting_period_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.541444 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_type_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/contact_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/currency_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_billing_cycle_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_group_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/estimation_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/estimation_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/human_resource_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/product_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/project_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/project_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/reporting_period_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/reporting_period_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_manager_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_price_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_type_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/restinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/task_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/task_status_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/tax_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/unit_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/rest/work_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/crm/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.545444 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    50507 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50540 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/invoice.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    30645 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/project_report.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/quote.xsl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27411 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/work_report.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.545444 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50599 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/invoice.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50534 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50629 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    50630 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/quote.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.549444 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)   704128 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   756072 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   122303 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   156738 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/dejavusans.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/fontconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.549444 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/create_work_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/exception.html
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/register_payment.html
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/set_timezone.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/time_reporting.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.553444 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_calculations_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_delete_of_empty_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_incomplete_sales_document_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_admin_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_effective_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_planned_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_supplier_admin_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_effort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_effort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_update_last_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_time_tracking_add_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_user_is_not_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_version_increase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_view_work_entry_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_work_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.557444 koalix-crm-1.14.0rc2/koalixcrm/crm/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/create_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/create_work_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/newdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/pdfexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/range_selection_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/reporting_period_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/set_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/template_set_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/time_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/user_extension_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/user_is_not_human_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/work_entry_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/crm/views/work_entry_formset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.557444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.557444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/const/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.561444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/factory_document_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/factory_template_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/factory_user_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.561444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.561444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.561444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.561444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/document_template_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/template_set_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/user_extension_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/user_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/document_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/template_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/user_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/global_support_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/const/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/subscriptions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.565444 koalix-crm-1.14.0rc2/koalixcrm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/test/UITests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/test/test_support_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/koalixcrm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.497444 koalix-crm-1.14.0rc2/projectsettings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:32.569444 koalix-crm-1.14.0rc2/projectsettings/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/projectsettings/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/projectsettings/settings/base_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/projectsettings/settings/development_docker_sqlite_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:40:32.569444 koalix-crm-1.14.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-07 09:40:28.000000 koalix-crm-1.14.0rc2/setup.py
```

### Comparing `koalix-crm-1.14.0rc1/LICENSE` & `koalix-crm-1.14.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/PKG-INFO` & `koalix-crm-1.14.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koalix-crm
-Version: 1.14.0rc1
+Version: 1.14.0rc2
 Summary: koalixcrm is a tiny and easy to use Customer-Relationship-Management Software (CRM) including tiny and easy to use Accounting Software
 Home-page: http://github.com/scaphilo/koalixcrm
 Author: Aaron Riedener
 Author-email: aaron.riedener@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: koalix-crm Version: 1.14.0rc1 Summary: koalixcrm is
+Metadata-Version: 2.1 Name: koalix-crm Version: 1.14.0rc2 Summary: koalixcrm is
 a tiny and easy to use Customer-Relationship-Management Software (CRM)
 including tiny and easy to use Accounting Software Home-page: http://
 github.com/scaphilo/koalixcrm Author: Aaron Riedener Author-email:
 aaron.riedener@gmail.com License: BSD Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python :: 3.10 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 Django==3.2.25 Requires-Dist: django-filebrowser==3.14.3 Requires-Dist:
```

### Comparing `koalix-crm-1.14.0rc1/README.md` & `koalix-crm-1.14.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalix_crm.egg-info/PKG-INFO` & `koalix-crm-1.14.0rc2/koalix_crm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koalix-crm
-Version: 1.14.0rc1
+Version: 1.14.0rc2
 Summary: koalixcrm is a tiny and easy to use Customer-Relationship-Management Software (CRM) including tiny and easy to use Accounting Software
 Home-page: http://github.com/scaphilo/koalixcrm
 Author: Aaron Riedener
 Author-email: aaron.riedener@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: koalix-crm Version: 1.14.0rc1 Summary: koalixcrm is
+Metadata-Version: 2.1 Name: koalix-crm Version: 1.14.0rc2 Summary: koalixcrm is
 a tiny and easy to use Customer-Relationship-Management Software (CRM)
 including tiny and easy to use Accounting Software Home-page: http://
 github.com/scaphilo/koalixcrm Author: Aaron Riedener Author-email:
 aaron.riedener@gmail.com License: BSD Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python :: 3.10 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 Django==3.2.25 Requires-Dist: django-filebrowser==3.14.3 Requires-Dist:
```

### Comparing `koalix-crm-1.14.0rc1/koalix_crm.egg-info/SOURCES.txt` & `koalix-crm-1.14.0rc2/koalix_crm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -379,9 +379,8 @@
 koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py
 koalixcrm/subscriptions/migrations/__init__.py
 koalixcrm/test/UITests.py
 koalixcrm/test/__init__.py
 koalixcrm/test/test_support_functions.py
 projectsettings/settings/__init__.py
 projectsettings/settings/base_settings.py
-projectsettings/settings/development_docker_sqlite_settings.py
-projectsettings/settings/production_docker_postgres_settings.py
+projectsettings/settings/development_docker_sqlite_settings.py
```

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/account.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/account.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/accounting_period.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/accounting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/booking.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/booking.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/accounting/product_category.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/accounting/product_category.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/admin.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/exceptions.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0001_initial.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0002_auto_20170705_1702.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0004_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0006_auto_20180422_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0007_auto_20180422_2105.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0008_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0009_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0010_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/migrations/0011_auto_20240329_2207.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/migrations/0011_auto_20240329_2207.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/account_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/account_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/accounting_period_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/accounting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/booking_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/booking_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/product_categorie_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/product_categorie_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/rest/restinterface.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/de/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/de/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/en/balancesheet.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/static/default_templates/en/profitlossstatement.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/tests/test_accountingModelTest.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/tests/test_accountingModelTest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/accounting/views.py` & `koalix-crm-1.14.0rc2/koalixcrm/accounting/views.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/admin.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/const/country.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/const/country.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/const/purpose.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/const/purpose.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/const/status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/const/status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/call.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/call.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/contact.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/contact.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_billing_cycle.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer_billing_cycle.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/customer_group.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/customer_group.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/person.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/person.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/postal_address.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/postal_address.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/contact/supplier.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/contact/supplier.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/calculations.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/calculations.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/contract.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/delivery_note.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/delivery_note.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/invoice.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/invoice.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/payment_reminder.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/payment_reminder.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/pdf_export.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/pdf_export.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_confirmation.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/purchase_confirmation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/purchase_order.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/purchase_order.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/quote.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/quote.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/sales_document.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/documents/sales_document_position.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/documents/sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/exceptions.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_agreement_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_agreement_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_contract.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_currency.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_currency_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_currency_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_customer_group_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_customer_group_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_estimation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_estimation_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_estimation_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_project_link.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_generic_project_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_generic_task_link.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_generic_task_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_human_resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_price.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_product_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_product_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_product_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_project.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_project_link_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_project_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_reporting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_reporting_period_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_reporting_period_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_resource_price.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_resource_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_sales_document.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_sales_document_position.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_link_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_task_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_task_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_unit.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_unit_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_unit_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_user.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_user.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/factories/factory_work.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/factories/factory_work.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/inlinemixin.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/inlinemixin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/crm/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/crm/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/management/commands/koalixcrm_install_defaulttemplates.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0001_initial.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0002_auto_20170927_2042.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0002_auto_20170927_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0003_auto_20171009_1949.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0003_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0004_auto_20171009_2008.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0004_auto_20171009_2008.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0005_auto_20171110_1732.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0005_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0006_auto_20171210_1805.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0006_auto_20171210_1805.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0007_auto_20171210_2126.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0007_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0008_auto_20180104_2042.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0008_auto_20180104_2042.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0009_auto_20180104_2111.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0009_auto_20180104_2111.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0011_auto_20180104_2152.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0011_auto_20180104_2152.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0012_auto_20180105_1840.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0012_auto_20180105_1840.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0013_auto_20180105_2159.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0013_auto_20180105_2159.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0014_auto_20180108_2048.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0014_auto_20180108_2048.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0015_auto_20180111_2043.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0015_auto_20180111_2043.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0016_auto_20180111_2011.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0016_auto_20180111_2011.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0017_auto_20180111_2022.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0017_auto_20180111_2022.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0018_auto_20180111_2031.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0018_auto_20180111_2031.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0019_auto_20180112_2020.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0019_auto_20180112_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0020_auto_20180116_2056.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0020_auto_20180116_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0021_purchaseorder.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0021_purchaseorder.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0022_auto_20180117_2020.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0022_auto_20180117_2020.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0024_auto_20180122_2121.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0024_auto_20180122_2121.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0025_auto_20180413_1937.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0025_auto_20180413_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0026_auto_20180507_1957.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0026_auto_20180507_1957.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0027_auto_20180606_2034.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0027_auto_20180606_2034.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0028_auto_20180611_1835.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0028_auto_20180611_1835.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0029_auto_20180611_1903.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0029_auto_20180611_1903.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0030_auto_20180611_1930.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0030_auto_20180611_1930.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0031_auto_20180612_1924.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0031_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0032_auto_20180612_1925.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0032_auto_20180612_1925.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0033_auto_20180612_1936.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0033_auto_20180612_1936.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0034_genericprojectlink.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0034_genericprojectlink.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0035_auto_20180619_1924.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0035_auto_20180619_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0036_auto_20180626_2059.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0036_auto_20180626_2059.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0038_auto_20180702_1628.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0038_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0039_auto_20180702_1635.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0039_auto_20180702_1635.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0040_auto_20180724_1657.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0040_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0041_auto_20180724_1657.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0041_auto_20180724_1657.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0042_auto_20180724_1816.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0042_auto_20180724_1816.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0043_reportingperiodstatus.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0043_reportingperiodstatus.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0044_reportingperiod_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0044_reportingperiod_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0045_auto_20180805_2047.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0045_auto_20180805_2047.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0047_work_worked_hours.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0047_work_worked_hours.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0048_auto_20181012_2056.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0048_auto_20181012_2056.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0049_auto_20181014_2258.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0049_auto_20181014_2258.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0050_auto_20181014_2300.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0050_auto_20181014_2300.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0051_auto_20181014_2302.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0051_auto_20181014_2302.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0052_auto_20181014_2304.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0052_auto_20181014_2304.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0053_auto_20181014_2305.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0053_auto_20181014_2305.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0055_auto_20181022_1937.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0055_auto_20181022_1937.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20181216_2224.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0056_auto_20181216_2224.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0056_auto_20190102_2230.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0056_auto_20190102_2230.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/migrations/0059_auto_20240329_2207.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/migrations/0059_auto_20240329_2207.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/models.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/models.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/currency.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/currency_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/currency_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/customer_group_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/customer_group_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/price.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_price.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/product_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/product_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/product_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/tax.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/tax.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/unit.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/product/unit_transform.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/product/unit_transform.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/agreement_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/agreement_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/estimation.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/estimation_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/estimation_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_project_link.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/generic_project_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/generic_task_link.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/generic_task_link.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/human_resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_link_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/project_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/project_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/reporting_period.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/reporting_period_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/reporting_period_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_manager.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_manager.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_price.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_price.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/resource_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/resource_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_link_type.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task_link_type.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/task_status.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/task_status.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/urls.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/urls.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/reporting/work.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/reporting/work.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_status_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/agreement_type_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/agreement_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/contact_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/contact_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_billing_cycle_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_billing_cycle_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_group_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_group_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/customer_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/customer_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/estimation_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/estimation_status_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/estimation_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/human_resource_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/human_resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/product_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/product_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/project_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/project_status_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/project_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/reporting_period_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/reporting_period_status_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/reporting_period_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_manager_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_manager_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_price_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_price_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/resource_type_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/resource_type_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/restinterface.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/restinterface.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/task_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/task_status_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/task_status_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/tax_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/tax_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/unit_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/unit_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/rest/work_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/rest/work_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/invoice.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/project_report.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/project_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/quote.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/de/work_report.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/de/work_report.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/deliveryorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/invoice.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/invoice.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/purchaseconfirmation.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/purchaseorder.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/en/quote.xsl` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/en/quote.xsl`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/dejavusans-bold.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/dejavusans.xml` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/dejavusans.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/fontconfig.xml` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/fontconfig.xml`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/static/default_templates/generic/logo.jpg` & `koalix-crm-1.14.0rc2/koalixcrm/crm/static/default_templates/generic/logo.jpg`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/create_work_report.html` & `koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/create_work_report.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/exception.html` & `koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/exception.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/register_payment.html` & `koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/register_payment.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/set_timezone.html` & `koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/set_timezone.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/templates/crm/admin/time_reporting.html` & `koalix-crm-1.14.0rc2/koalixcrm/crm/templates/crm/admin/time_reporting.html`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_calculations_document.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_calculations_document.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_contract.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_contract.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_invoice.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_sales_document_from_quote.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_sales_document_from_quote.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_create_task.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_create_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_delete_of_empty_row.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_delete_of_empty_row.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_incomplete_sales_document_position.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_incomplete_sales_document_position.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_admin_view.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_admin_view.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_effective_costs.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_effective_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_project_planned_costs.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_project_planned_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_supplier_admin_view.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_supplier_admin_view.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_constructor.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_constructor.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_costs_no_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_costs_with_agreement.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_duration.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_duration.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_effective_effort.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_effective_effort.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_costs.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_costs.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_duration.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_duration.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_planned_effort.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_planned_effort.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_task_update_last_status_update.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_task_update_last_status_update.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_time_tracking_add_row.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_time_tracking_add_row.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_user_is_not_human_resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_user_is_not_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_version_increase.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_version_increase.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_view_work_entry_form.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_view_work_entry_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/tests/test_work_delete.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/tests/test_work_delete.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_task.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/create_task.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/create_work_report.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/create_work_report.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/newdocument.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/newdocument.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/pdfexport.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/pdfexport.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/range_selection_form.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/range_selection_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/renderer.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/renderer.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/reporting_period_missing.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/reporting_period_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/template_set_missing.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/template_set_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/time_tracking.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/time_tracking.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_extension_missing.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/user_extension_missing.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/user_is_not_human_resource.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/user_is_not_human_resource.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_form.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/work_entry_form.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/crm/views/work_entry_formset.py` & `koalix-crm-1.14.0rc2/koalixcrm/crm/views/work_entry_formset.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/admin.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/exceptions.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/exceptions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_document_template.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/factory_document_template.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/factories/factory_user_extension.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/factories/factory_user_extension.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0001_initial.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0004_auto_20171210_2126.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0005_auto_20180612_1924.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0006_auto_20180701_2128.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0007_auto_20180702_1628.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/migrations/0008_auto_20240329_2207.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/document_template_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/document_template_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/template_set_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/template_set_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/rest/user_extension_rest.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/rest/user_extension_rest.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/document_template.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/document_template.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/template_set.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/template_set.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/text_paragraph.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/djangoUserExtension/user_extension/user_extension.py` & `koalix-crm-1.14.0rc2/koalixcrm/djangoUserExtension/user_extension/user_extension.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/global_support_functions.py` & `koalix-crm-1.14.0rc2/koalixcrm/global_support_functions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/plugin.py` & `koalix-crm-1.14.0rc2/koalixcrm/plugin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/admin.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/admin.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0001_initial.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0002_auto_20171009_1949.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0003_auto_20171110_1732.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0004_auto_20181013_2213.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0005_auto_20181013_2228.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/migrations/0006_auto_20240329_2207.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/subscriptions/models.py` & `koalix-crm-1.14.0rc2/koalixcrm/subscriptions/models.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/test/UITests.py` & `koalix-crm-1.14.0rc2/koalixcrm/test/UITests.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/koalixcrm/test/test_support_functions.py` & `koalix-crm-1.14.0rc2/koalixcrm/test/test_support_functions.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/projectsettings/settings/base_settings.py` & `koalix-crm-1.14.0rc2/projectsettings/settings/base_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,23 +90,23 @@
 USE_L10N = True
 USE_TZ = True
 
 STATIC_URL = '/static/'
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')
 
 MEDIA_URL = "/media/"
-MEDIA_ROOT = os.path.join(BASE_DIR)
+MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
 
 PROJECT_ROOT = BASE_DIR
 
 # Settings specific for koalixcrm
 PDF_OUTPUT_ROOT = os.path.join(STATIC_ROOT, 'pdf')
 
 # Settings specific for filebrowser
-FILEBROWSER_DIRECTORY = 'media/uploads/'
+FILEBROWSER_DIRECTORY = 'uploads/'
 FILEBROWSER_EXTENSIONS = {
     'XML': ['.xml'],
     'XSL': ['.xsl'],
     'JPG': ['.jpg'],
     'PNG': ['.png'],
     'GIF': ['.gif'],
     'TTF': ['.ttf'],
```

### Comparing `koalix-crm-1.14.0rc1/projectsettings/settings/development_docker_sqlite_settings.py` & `koalix-crm-1.14.0rc2/projectsettings/settings/development_docker_sqlite_settings.py`

 * *Files identical despite different names*

### Comparing `koalix-crm-1.14.0rc1/setup.py` & `koalix-crm-1.14.0rc2/setup.py`

 * *Files identical despite different names*

