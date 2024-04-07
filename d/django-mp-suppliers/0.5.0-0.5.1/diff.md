# Comparing `tmp/django-mp-suppliers-0.5.0.tar.gz` & `tmp/django-mp-suppliers-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mp-suppliers-0.5.0.tar", last modified: Sat Sep 23 10:13:10 2023, max compression
+gzip compressed data, was "django-mp-suppliers-0.5.1.tar", last modified: Sun Apr  7 06:39:42 2024, max compression
```

## Comparing `django-mp-suppliers-0.5.0.tar` & `django-mp-suppliers-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2022-05-14 06:22:54.000000 django-mp-suppliers-0.5.0/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      323 2022-06-18 06:55:36.000000 django-mp-suppliers-0.5.0/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      117 2022-05-14 06:22:54.000000 django-mp-suppliers-0.5.0/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-09-23 10:13:10.000000 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     1056 2023-09-23 10:13:10.000000 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-09-23 10:13:10.000000 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       94 2023-09-23 10:13:10.000000 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       28 2023-09-23 10:13:10.000000 django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      115 2022-06-18 07:04:44.000000 django-mp-suppliers-0.5.0/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      548 2023-09-23 10:12:51.000000 django-mp-suppliers-0.5.0/setup.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/supplier_products/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1654 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/supplier_products/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1899 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/email.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1022 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/supplier_products/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/supplier_products/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/supplier_products/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/supplier_products/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1991 2022-06-18 07:13:18.000000 django-mp-suppliers-0.5.0/supplier_products/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2580 2022-06-18 07:13:05.000000 django-mp-suppliers-0.5.0/supplier_products/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 dev       (1000) dev       (1000)      328 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/managers.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/supplier_products/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     3667 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      641 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/migrations/0002_auto_20201007_1937.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.0/supplier_products/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4554 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/supplier_products/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1419 2022-05-25 16:34:44.000000 django-mp-suppliers-0.5.0/supplier_products/querysets.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3268 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/supplier_products/tasks.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      776 2022-05-19 10:08:41.000000 django-mp-suppliers-0.5.0/supplier_products/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4676 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/supplier_products/views.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/suppliers/
--rw-rw-r--   0 dev       (1000) dev       (1000)      489 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/suppliers/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      317 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/suppliers/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      615 2022-06-18 06:44:52.000000 django-mp-suppliers-0.5.0/suppliers/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      867 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/suppliers/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/suppliers/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/suppliers/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/suppliers/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1709 2022-06-18 07:13:32.000000 django-mp-suppliers-0.5.0/suppliers/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2265 2022-06-18 07:12:12.000000 django-mp-suppliers-0.5.0/suppliers/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-09-23 10:13:10.632793 django-mp-suppliers-0.5.0/suppliers/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2885 2022-06-18 06:44:52.000000 django-mp-suppliers-0.5.0/suppliers/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-04-21 15:31:08.000000 django-mp-suppliers-0.5.0/suppliers/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2613 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.0/suppliers/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      323 2022-06-18 06:55:36.000000 django-mp-suppliers-0.5.1/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      324 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      117 2022-05-14 06:22:54.000000 django-mp-suppliers-0.5.1/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      324 2024-04-07 06:39:42.000000 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1161 2024-04-07 06:39:42.000000 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2024-04-07 06:39:42.000000 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      125 2024-04-07 06:39:42.000000 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       28 2024-04-07 06:39:42.000000 django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      146 2024-04-07 06:38:23.000000 django-mp-suppliers-0.5.1/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       38 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      548 2024-04-07 06:39:17.000000 django-mp-suppliers-0.5.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/supplier_products/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1654 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.1/supplier_products/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1899 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/email.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1022 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.1/supplier_products/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/supplier_products/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/supplier_products/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/supplier_products/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1991 2022-06-18 07:13:18.000000 django-mp-suppliers-0.5.1/supplier_products/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2580 2022-06-18 07:13:05.000000 django-mp-suppliers-0.5.1/supplier_products/locale/uk/LC_MESSAGES/django.po
+-rw-rw-r--   0 dev       (1000) dev       (1000)      328 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/managers.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/supplier_products/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3667 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      641 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/migrations/0002_auto_20201007_1937.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-07-19 12:58:02.000000 django-mp-suppliers-0.5.1/supplier_products/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4554 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.1/supplier_products/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1419 2022-05-25 16:34:44.000000 django-mp-suppliers-0.5.1/supplier_products/querysets.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3268 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.1/supplier_products/tasks.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      776 2022-05-19 10:08:41.000000 django-mp-suppliers-0.5.1/supplier_products/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4676 2023-09-23 10:12:40.000000 django-mp-suppliers-0.5.1/supplier_products/views.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/suppliers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      519 2024-04-07 06:32:26.000000 django-mp-suppliers-0.5.1/suppliers/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      317 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      687 2024-04-07 06:31:36.000000 django-mp-suppliers-0.5.1/suppliers/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      867 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/suppliers/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.409709 django-mp-suppliers-0.5.1/suppliers/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/suppliers/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1709 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2265 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-07 06:39:42.413709 django-mp-suppliers-0.5.1/suppliers/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2885 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      816 2024-04-07 06:31:05.000000 django-mp-suppliers-0.5.1/suppliers/migrations/0002_supplier_order_alter_supplier_id_and_more.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      468 2024-04-07 06:34:38.000000 django-mp-suppliers-0.5.1/suppliers/migrations/0003_default_supplier_order.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2024-01-10 16:40:06.000000 django-mp-suppliers-0.5.1/suppliers/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2694 2024-04-07 06:31:52.000000 django-mp-suppliers-0.5.1/suppliers/models.py
```

### Comparing `django-mp-suppliers-0.5.0/django_mp_suppliers.egg-info/SOURCES.txt` & `django-mp-suppliers-0.5.1/django_mp_suppliers.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-LICENSE
 MANIFEST.in
 README.md
 requirements.txt
-setup.cfg
 setup.py
 django_mp_suppliers.egg-info/PKG-INFO
 django_mp_suppliers.egg-info/SOURCES.txt
 django_mp_suppliers.egg-info/dependency_links.txt
 django_mp_suppliers.egg-info/requires.txt
 django_mp_suppliers.egg-info/top_level.txt
 supplier_products/__init__.py
@@ -28,8 +26,10 @@
 suppliers/actions.py
 suppliers/admin.py
 suppliers/forms.py
 suppliers/models.py
 suppliers/locale/uk/LC_MESSAGES/django.mo
 suppliers/locale/uk/LC_MESSAGES/django.po
 suppliers/migrations/0001_initial.py
+suppliers/migrations/0002_supplier_order_alter_supplier_id_and_more.py
+suppliers/migrations/0003_default_supplier_order.py
 suppliers/migrations/__init__.py
```

### Comparing `django-mp-suppliers-0.5.0/setup.py` & `django-mp-suppliers-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup, find_packages
 
 
-version = '0.5.0'
+version = '0.5.1'
 url = 'https://github.com/pmaigutyak/mp-suppliers'
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 setup(
     name='django-mp-suppliers',
```

### Comparing `django-mp-suppliers-0.5.0/supplier_products/admin.py` & `django-mp-suppliers-0.5.1/supplier_products/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/email.py` & `django-mp-suppliers-0.5.1/supplier_products/email.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/forms.py` & `django-mp-suppliers-0.5.1/supplier_products/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/locale/uk/LC_MESSAGES/django.mo` & `django-mp-suppliers-0.5.1/supplier_products/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/locale/uk/LC_MESSAGES/django.po` & `django-mp-suppliers-0.5.1/supplier_products/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/migrations/0001_initial.py` & `django-mp-suppliers-0.5.1/supplier_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/migrations/0002_auto_20201007_1937.py` & `django-mp-suppliers-0.5.1/supplier_products/migrations/0002_auto_20201007_1937.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/models.py` & `django-mp-suppliers-0.5.1/supplier_products/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/querysets.py` & `django-mp-suppliers-0.5.1/supplier_products/querysets.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/tasks.py` & `django-mp-suppliers-0.5.1/supplier_products/tasks.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/urls.py` & `django-mp-suppliers-0.5.1/supplier_products/urls.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/supplier_products/views.py` & `django-mp-suppliers-0.5.1/supplier_products/views.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/suppliers/admin.py` & `django-mp-suppliers-0.5.1/suppliers/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from django.contrib import admin
 
 from suppliers.models import Supplier
 from suppliers.actions import clean_products
 from suppliers.forms import SupplierWarehouseInline
+from adminsortable2.admin import SortableAdminMixin
 
 
 @admin.register(Supplier)
-class SupplierAdmin(admin.ModelAdmin):
+class SupplierAdmin(SortableAdminMixin, admin.ModelAdmin):
 
     list_display = [
         'id', 'name', 'short_name', 'code', 'currency', 'discount',
         'markup', 'is_visible_for_unregistered_users', 'country',
         'warehouse_count', 'price_updated'
     ]
```

### Comparing `django-mp-suppliers-0.5.0/suppliers/forms.py` & `django-mp-suppliers-0.5.1/suppliers/forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/suppliers/locale/uk/LC_MESSAGES/django.mo` & `django-mp-suppliers-0.5.1/suppliers/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/suppliers/locale/uk/LC_MESSAGES/django.po` & `django-mp-suppliers-0.5.1/suppliers/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/suppliers/migrations/0001_initial.py` & `django-mp-suppliers-0.5.1/suppliers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-suppliers-0.5.0/suppliers/models.py` & `django-mp-suppliers-0.5.1/suppliers/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,27 +30,30 @@
 
     price_updated = models.DateTimeField(
         _('Price updated date'), blank=True, editable=False, null=True)
 
     is_visible_for_unregistered_users = models.BooleanField(
         _('Is visible for unregistered users'), default=True)
 
+    order = models.PositiveIntegerField(default=0)
+
     @property
     def warehouse_count(self):
         return self.warehouses.count()
 
     warehouse_count.fget.short_description = _('Warehouse count')
 
     def __str__(self):
         return self.name
 
     def clean_products(self):
         return self.products.all().delete()
 
     class Meta:
+        ordering = ['order']
         verbose_name = _('Supplier')
         verbose_name_plural = _('Suppliers')
 
 
 class SupplierWarehouse(OrderedModel):
 
     supplier = models.ForeignKey(
```

