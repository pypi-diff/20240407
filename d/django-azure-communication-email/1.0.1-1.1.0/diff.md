# Comparing `tmp/django_azure_communication_email-1.0.1.tar.gz` & `tmp/django_azure_communication_email-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_communication_email-1.0.1.tar", max compression
+gzip compressed data, was "django_azure_communication_email-1.1.0.tar", max compression
```

## Comparing `django_azure_communication_email-1.0.1.tar` & `django_azure_communication_email-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/LICENSE
--rw-r--r--   0        0        0     2060 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/README.md
--rw-r--r--   0        0        0      238 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/__init__.py
--rw-r--r--   0        0        0     2342 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/attachment.py
--rw-r--r--   0        0        0     5445 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/backend.py
--rw-r--r--   0        0        0      526 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/django_azure_communication_email/settings.py
--rw-r--r--   0        0        0      818 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/django_azure_communication_email/utils.py
--rw-r--r--   0        0        0     2003 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 django_azure_communication_email-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2060 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/README.md
+-rw-r--r--   0        0        0      238 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/django_azure_communication_email/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/django_azure_communication_email/attachment.py
+-rw-r--r--   0        0        0     5445 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/django_azure_communication_email/backend.py
+-rw-r--r--   0        0        0      526 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/django_azure_communication_email/settings.py
+-rw-r--r--   0        0        0      818 2024-04-06 22:48:56.344710 django_azure_communication_email-1.1.0/django_azure_communication_email/utils.py
+-rw-r--r--   0        0        0     2092 2024-04-06 22:48:56.348710 django_azure_communication_email-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 django_azure_communication_email-1.1.0/PKG-INFO
```

### Comparing `django_azure_communication_email-1.0.1/LICENSE` & `django_azure_communication_email-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/README.md` & `django_azure_communication_email-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/django_azure_communication_email/attachment.py` & `django_azure_communication_email-1.1.0/django_azure_communication_email/attachment.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/django_azure_communication_email/backend.py` & `django_azure_communication_email-1.1.0/django_azure_communication_email/backend.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/django_azure_communication_email/settings.py` & `django_azure_communication_email-1.1.0/django_azure_communication_email/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/django_azure_communication_email/utils.py` & `django_azure_communication_email-1.1.0/django_azure_communication_email/utils.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.1/pyproject.toml` & `django_azure_communication_email-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "django-azure-communication-email"
-version = "1.0.1"
+version = "1.1.0"
 description = "A Django email backend for Azure Communication Email service."
-authors = ["Dmitrii Azarenko <dmitrii@retechlabs.com>"]
+authors = ["Dmitrii Azarenko <dmitrii.azarenko@symphonyai.com>"]
 maintainers = []
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/rebotics/django-azure-communication-email"
+repository = "https://github.com/retech-us/django-azure-communication-email"
 packages = [{include = "django_azure_communication_email"}]
 keywords = ["django", "email", "azure"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
@@ -18,40 +18,42 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Framework :: Django',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/rebotics/django-azure-communication-email/issues"
+"Bug Tracker" = "https://github.com/retech-us/django-azure-communication-email/issues"
 "Company Website" = "https://retechlabs.com"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-Django = ">=2.2,<4.3"
-azure-identity = "~1.13"
+python = ">=3.8,<3.13"
+Django = ">=2.2,<5.1"
+azure-identity = "~1.15"
 azure-communication-email = "~1.0"
 
 [tool.poetry.group.dev.dependencies]
-isort = "^5.1.0"
-tox = "^4.6.4"
+isort = "^5.13"
+tox = "^4.14"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
-py_version = 311
+py_version = 312
 default_section = "THIRDPARTY"
 known_first_party = ["django_azure_communication_email"]
 known_django = "django"
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "DJANGO", "FIRSTPARTY", "LOCALFOLDER"]
 combine_as_imports = true
 sort_reexports = true
 multi_line_output = 5
```

### Comparing `django_azure_communication_email-1.0.1/PKG-INFO` & `django_azure_communication_email-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: django-azure-communication-email
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Django email backend for Azure Communication Email service.
-Home-page: https://github.com/rebotics/django-azure-communication-email
+Home-page: https://github.com/retech-us/django-azure-communication-email
 License: Apache-2.0
 Keywords: django,email,azure
 Author: Dmitrii Azarenko
-Author-email: dmitrii@retechlabs.com
-Requires-Python: >=3.8,<3.12
+Author-email: dmitrii.azarenko@symphonyai.com
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Django (>=2.2,<4.3)
+Requires-Dist: Django (>=2.2,<5.1)
 Requires-Dist: azure-communication-email (>=1.0,<1.1)
-Requires-Dist: azure-identity (>=1.13,<1.14)
-Project-URL: Bug Tracker, https://github.com/rebotics/django-azure-communication-email/issues
+Requires-Dist: azure-identity (>=1.15,<1.16)
+Project-URL: Bug Tracker, https://github.com/retech-us/django-azure-communication-email/issues
 Project-URL: Company Website, https://retechlabs.com
-Project-URL: Repository, https://github.com/rebotics/django-azure-communication-email
+Project-URL: Repository, https://github.com/retech-us/django-azure-communication-email
 Description-Content-Type: text/markdown
 
 # Django Azure Communication Email
 
 [![Unit tests](https://github.com/rebotics/django-azure-communication-email/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/rebotics/django-azure-communication-email/actions/workflows/ci.yml)
 [![PyPI version](https://badge.fury.io/py/django-azure-communication-email.svg)](https://badge.fury.io/py/django-azure-communication-email)
 [![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://img.shields.io/badge/python-3.8+-blue)
```

