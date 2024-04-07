# Comparing `tmp/istari-0.0.7.tar.gz` & `tmp/istari-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.0.7.tar", last modified: Sat Apr  6 04:13:44 2024, max compression
+gzip compressed data, was "istari-0.0.8.tar", last modified: Sun Apr  7 02:22:23 2024, max compression
```

## Comparing `istari-0.0.7.tar` & `istari-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.169639 istari-0.0.7/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:13:44.169445 istari-0.0.7/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.7/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.166957 istari-0.0.7/istari/
--rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-06 04:12:29.000000 istari-0.0.7/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167646 istari-0.0.7/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.7/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.0.7/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167971 istari-0.0.7/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     1450 2024-04-05 21:17:27.000000 istari-0.0.7/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.7/istari/cli/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.168502 istari-0.0.7/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.7/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      929 2024-04-06 02:58:34.000000 istari-0.0.7/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      629 2024-04-06 02:20:21.000000 istari-0.0.7/istari/commands/startproject.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.168926 istari-0.0.7/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.7/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.7/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.7/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.169099 istari-0.0.7/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 02:02:06.000000 istari-0.0.7/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     2639 2024-04-06 02:36:09.000000 istari-0.0.7/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167468 istari-0.0.7/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      490 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-06 04:13:44.169675 istari-0.0.7/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.7/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.720847 istari-0.0.8/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-07 02:22:23.720641 istari-0.0.8/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.8/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.716097 istari-0.0.8/istari/
+-rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-07 02:21:02.000000 istari-0.0.8/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.718297 istari-0.0.8/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.8/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.0.8/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.718765 istari-0.0.8/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     1446 2024-04-06 19:50:45.000000 istari-0.0.8/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.8/istari/cli/base.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.719188 istari-0.0.8/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.8/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      967 2024-04-07 01:21:57.000000 istari-0.0.8/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      723 2024-04-07 01:21:42.000000 istari-0.0.8/istari/commands/startproject.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.719588 istari-0.0.8/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.8/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.8/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.8/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.719887 istari-0.0.8/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.0.8/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     4262 2024-04-07 02:13:43.000000 istari-0.0.8/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.720351 istari-0.0.8/istari/templates/plugins/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.0.8/istari/templates/plugins/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      611 2024-04-06 21:28:02.000000 istari-0.0.8/istari/templates/plugins/base.py
+-rw-r--r--   0 jay        (501) staff       (20)     1669 2024-04-07 02:17:49.000000 istari-0.0.8/istari/templates/plugins/editable.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-07 02:22:23.717939 istari-0.0.8/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-07 02:22:23.000000 istari-0.0.8/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      593 2024-04-07 02:22:23.000000 istari-0.0.8/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-07 02:22:23.000000 istari-0.0.8/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-07 02:22:23.000000 istari-0.0.8/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-07 02:22:23.000000 istari-0.0.8/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-07 02:22:23.720888 istari-0.0.8/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.8/setup.py
```

### Comparing `istari-0.0.7/istari/auth/models.py` & `istari-0.0.8/istari/auth/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.7/istari/cli/__init__.py` & `istari-0.0.8/istari/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import pkgutil
 from argparse import ArgumentParser
 
-from istari.cli.commands import BaseCommand
+from istari.cli.base import BaseCommand
 
 
 class IstariCLI:
     def __init__(self):
         self.parser = ArgumentParser()
         self.subparsers = self.parser.add_subparsers(title='commands', dest='command_name')
         self.subparsers.required = True
```

### Comparing `istari-0.0.7/istari/commands/startapp.py` & `istari-0.0.8/istari/commands/startapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class Command(TemplateCommand):
     template_name = 'app_template'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('app_name')
+        super().add_arguments(parser)
 
     def handle(self, **options):
         options['target_dir'] = Path.cwd()
         options['variables'] = {
             'app_name': options['app_name'],
         }
```

### Comparing `istari-0.0.7/istari/commands/startproject.py` & `istari-0.0.8/istari/commands/startproject.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from argparse import ArgumentParser
 
-from istari import SECRET_KEY_INSECURE_PREFIX, get_random_secret_key
+from istari import __version__, SECRET_KEY_INSECURE_PREFIX, get_random_secret_key
 from istari.templates.commands import TemplateCommand
 
 
 class Command(TemplateCommand):
     template_name = 'project_template'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('project_name')
+        super().add_arguments(parser)
     
     def handle(self, **options):
         options['variables'] = {
             'docs_version': '5.0',
+            'istari_version': __version__,
             'project_name': options['project_name'],
             'secret_key': SECRET_KEY_INSECURE_PREFIX + get_random_secret_key(),
         }
         return super().handle(**options)
```

### Comparing `istari-0.0.7/istari/db/fields.py` & `istari-0.0.8/istari/db/fields.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.7/istari/db/models.py` & `istari-0.0.8/istari/db/models.py`

 * *Files identical despite different names*

