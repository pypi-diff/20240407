# Comparing `tmp/istari-0.0.6.tar.gz` & `tmp/istari-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.0.6.tar", last modified: Sat Apr  6 04:08:32 2024, max compression
+gzip compressed data, was "istari-0.0.7.tar", last modified: Sat Apr  6 04:13:44 2024, max compression
```

## Comparing `istari-0.0.6.tar` & `istari-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.970513 istari-0.0.6/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:08:32.970333 istari-0.0.6/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.6/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.967738 istari-0.0.6/istari/
--rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-06 04:07:26.000000 istari-0.0.6/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.968433 istari-0.0.6/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.6/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3027 2024-04-06 04:06:32.000000 istari-0.0.6/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.968756 istari-0.0.6/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     1450 2024-04-05 21:17:27.000000 istari-0.0.6/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.6/istari/cli/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.969332 istari-0.0.6/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.6/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      929 2024-04-06 02:58:34.000000 istari-0.0.6/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      629 2024-04-06 02:20:21.000000 istari-0.0.6/istari/commands/startproject.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.969819 istari-0.0.6/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.6/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.6/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.6/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.969993 istari-0.0.6/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 02:02:06.000000 istari-0.0.6/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     2639 2024-04-06 02:36:09.000000 istari-0.0.6/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:08:32.968221 istari-0.0.6/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:08:32.000000 istari-0.0.6/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      490 2024-04-06 04:08:32.000000 istari-0.0.6/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-06 04:08:32.000000 istari-0.0.6/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-06 04:08:32.000000 istari-0.0.6/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-06 04:08:32.000000 istari-0.0.6/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-06 04:08:32.970543 istari-0.0.6/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.6/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.169639 istari-0.0.7/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:13:44.169445 istari-0.0.7/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.0.7/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.166957 istari-0.0.7/istari/
+-rw-r--r--   0 jay        (501) staff       (20)      292 2024-04-06 04:12:29.000000 istari-0.0.7/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167646 istari-0.0.7/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.0.7/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.0.7/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167971 istari-0.0.7/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     1450 2024-04-05 21:17:27.000000 istari-0.0.7/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.0.7/istari/cli/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.168502 istari-0.0.7/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.0.7/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      929 2024-04-06 02:58:34.000000 istari-0.0.7/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      629 2024-04-06 02:20:21.000000 istari-0.0.7/istari/commands/startproject.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.168926 istari-0.0.7/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.0.7/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.0.7/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.0.7/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.169099 istari-0.0.7/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 02:02:06.000000 istari-0.0.7/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     2639 2024-04-06 02:36:09.000000 istari-0.0.7/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-06 04:13:44.167468 istari-0.0.7/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      490 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-06 04:13:44.000000 istari-0.0.7/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-06 04:13:44.169675 istari-0.0.7/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.0.7/setup.py
```

### Comparing `istari-0.0.6/istari/auth/models.py` & `istari-0.0.7/istari/auth/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,9 @@
         username = slugify(name)
         while self.__class__.objects.filter(username=username).exists():
             username = f'{username}-{get_random_string(length=4)}'
         return username
     
     def save(self, *args, **kwargs):
         if self.username is None:
-            self._generate_username()
+            self.username = self._generate_username()
         super().save(*args, **kwargs)
```

### Comparing `istari-0.0.6/istari/cli/__init__.py` & `istari-0.0.7/istari/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.6/istari/commands/startapp.py` & `istari-0.0.7/istari/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.6/istari/commands/startproject.py` & `istari-0.0.7/istari/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.6/istari/db/fields.py` & `istari-0.0.7/istari/db/fields.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.6/istari/db/models.py` & `istari-0.0.7/istari/db/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.0.6/istari/templates/commands.py` & `istari-0.0.7/istari/templates/commands.py`

 * *Files identical despite different names*

