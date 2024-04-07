# Comparing `tmp/django-telethon-1.3.2.tar.gz` & `tmp/django-telethon-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-telethon-1.3.2.tar", last modified: Sat Mar 30 21:57:28 2024, max compression
+gzip compressed data, was "django-telethon-1.3.3.tar", last modified: Sun Apr  7 14:55:55 2024, max compression
```

## Comparing `django-telethon-1.3.2.tar` & `django-telethon-1.3.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.753544 django-telethon-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-30 21:57:25.000000 django-telethon-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-30 21:57:25.000000 django-telethon-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-03-30 21:57:28.753544 django-telethon-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-30 21:57:25.000000 django-telethon-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.749544 django-telethon-1.3.2/django_telethon/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.749544 django-telethon-1.3.2/django_telethon/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.749544 django-telethon-1.3.2/django_telethon/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/management/commands/runtelegram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.749544 django-telethon-1.3.2/django_telethon/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.753544 django-telethon-1.3.2/django_telethon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/sentfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/models/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-30 21:57:25.000000 django-telethon-1.3.2/django_telethon/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:57:28.753544 django-telethon-1.3.2/django_telethon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-03-30 21:57:28.000000 django-telethon-1.3.2/django_telethon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-30 21:57:28.000000 django-telethon-1.3.2/django_telethon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:57:28.000000 django-telethon-1.3.2/django_telethon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-30 21:57:28.000000 django-telethon-1.3.2/django_telethon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-30 21:57:28.000000 django-telethon-1.3.2/django_telethon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-30 21:57:25.000000 django-telethon-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:57:28.753544 django-telethon-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-30 21:57:26.000000 django-telethon-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.808309 django-telethon-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-07 14:55:52.000000 django-telethon-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-07 14:55:52.000000 django-telethon-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-07 14:55:55.808309 django-telethon-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-07 14:55:52.000000 django-telethon-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.804309 django-telethon-1.3.3/django_telethon/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.804309 django-telethon-1.3.3/django_telethon/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.804309 django-telethon-1.3.3/django_telethon/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/management/commands/runtelegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.804309 django-telethon-1.3.3/django_telethon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.808309 django-telethon-1.3.3/django_telethon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/sentfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/models/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-07 14:55:52.000000 django-telethon-1.3.3/django_telethon/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:55:55.808309 django-telethon-1.3.3/django_telethon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-07 14:55:55.000000 django-telethon-1.3.3/django_telethon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-07 14:55:55.000000 django-telethon-1.3.3/django_telethon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:55:55.000000 django-telethon-1.3.3/django_telethon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-07 14:55:55.000000 django-telethon-1.3.3/django_telethon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 14:55:55.000000 django-telethon-1.3.3/django_telethon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-07 14:55:52.000000 django-telethon-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:55:55.808309 django-telethon-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-07 14:55:53.000000 django-telethon-1.3.3/setup.py
```

### Comparing `django-telethon-1.3.2/LICENSE` & `django-telethon-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/PKG-INFO` & `django-telethon-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.3.2
+Version: 1.3.3
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-telethon-1.3.2/README.md` & `django-telethon-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/admin.py` & `django-telethon-1.3.3/django_telethon/admin.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/default_settings.py` & `django-telethon-1.3.3/django_telethon/default_settings.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/management/commands/runtelegram.py` & `django-telethon-1.3.3/django_telethon/management/commands/runtelegram.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/migrations/0001_initial.py` & `django-telethon-1.3.3/django_telethon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/models/entities.py` & `django-telethon-1.3.3/django_telethon/models/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,10 @@
         auto_now_add=True,
         verbose_name=_('Date'),
     )
 
     class Meta:
         verbose_name = _('Entity')
         verbose_name_plural = _('Entities')
+
+    def __str__(self):
+        return f'{self.entity_id} - {self.username} - {self.name}'
```

### Comparing `django-telethon-1.3.2/django_telethon/models/login.py` & `django-telethon-1.3.3/django_telethon/models/login.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/models/sentfiles.py` & `django-telethon-1.3.3/django_telethon/models/sentfiles.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/models/sessions.py` & `django-telethon-1.3.3/django_telethon/models/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/models/states.py` & `django-telethon-1.3.3/django_telethon/models/states.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/rabbitmq.py` & `django-telethon-1.3.3/django_telethon/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/receivers.py` & `django-telethon-1.3.3/django_telethon/receivers.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/sessions.py` & `django-telethon-1.3.3/django_telethon/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/utils.py` & `django-telethon-1.3.3/django_telethon/utils.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon/views.py` & `django-telethon-1.3.3/django_telethon/views.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/django_telethon.egg-info/PKG-INFO` & `django-telethon-1.3.3/django_telethon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.3.2
+Version: 1.3.3
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-telethon-1.3.2/django_telethon.egg-info/SOURCES.txt` & `django-telethon-1.3.3/django_telethon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/pyproject.toml` & `django-telethon-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-telethon-1.3.2/setup.py` & `django-telethon-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-telethon',
-    version='v1.3.2',
+    version='v1.3.3',
     packages=find_packages(),
     include_package_data=True,
     license='BSD License',
     description='Telethon for django',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ali-zahedi/django-telethon',
```

