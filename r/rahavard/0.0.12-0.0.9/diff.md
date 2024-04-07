# Comparing `tmp/rahavard-0.0.12.tar.gz` & `tmp/rahavard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rahavard-0.0.12.tar", last modified: Sun Apr  7 13:37:37 2024, max compression
+gzip compressed data, was "rahavard-0.0.9.tar", last modified: Thu Mar 21 13:06:07 2024, max compression
```

## Comparing `rahavard-0.0.12.tar` & `rahavard-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-07 13:37:37.923967 rahavard-0.0.12/
--rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.12/LICENSE
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-07 13:37:37.920633 rahavard-0.0.12/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.12/README.md
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-07 13:37:37.920633 rahavard-0.0.12/rahavard/
--rw-r--r--   0 nino      (1000) nino      (1000)      333 2024-03-21 10:39:33.000000 rahavard-0.0.12/rahavard/__init__.py
--rw-r--r--   0 nino      (1000) nino      (1000)     8197 2024-04-07 13:36:04.000000 rahavard-0.0.12/rahavard/utils.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-07 13:37:37.920633 rahavard-0.0.12/rahavard.egg-info/
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-07 13:37:37.000000 rahavard-0.0.12/rahavard.egg-info/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-04-07 13:37:37.000000 rahavard-0.0.12/rahavard.egg-info/SOURCES.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-04-07 13:37:37.000000 rahavard-0.0.12/rahavard.egg-info/dependency_links.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-04-07 13:37:37.000000 rahavard-0.0.12/rahavard.egg-info/requires.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-04-07 13:37:37.000000 rahavard-0.0.12/rahavard.egg-info/top_level.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-04-07 13:37:37.923967 rahavard-0.0.12/setup.cfg
--rw-r--r--   0 nino      (1000) nino      (1000)     1182 2024-04-07 13:36:54.000000 rahavard-0.0.12/setup.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.104723 rahavard-0.0.9/
+-rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.9/LICENSE
+-rw-r--r--   0 nino      (1000) nino      (1000)      698 2024-03-21 13:06:07.104723 rahavard-0.0.9/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.9/README.md
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.101390 rahavard-0.0.9/rahavard/
+-rw-r--r--   0 nino      (1000) nino      (1000)      333 2024-03-21 10:39:33.000000 rahavard-0.0.9/rahavard/__init__.py
+-rw-r--r--   0 nino      (1000) nino      (1000)     7560 2024-03-21 13:03:58.000000 rahavard-0.0.9/rahavard/utils.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.104723 rahavard-0.0.9/rahavard.egg-info/
+-rw-r--r--   0 nino      (1000) nino      (1000)      698 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/SOURCES.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/dependency_links.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/requires.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/top_level.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-03-21 13:06:07.104723 rahavard-0.0.9/setup.cfg
+-rw-r--r--   0 nino      (1000) nino      (1000)     1181 2024-03-21 13:05:38.000000 rahavard-0.0.9/setup.py
```

### Comparing `rahavard-0.0.12/LICENSE` & `rahavard-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rahavard-0.0.12/PKG-INFO` & `rahavard-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.12
+Version: 0.0.9
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rahavard-0.0.12/rahavard/utils.py` & `rahavard-0.0.9/rahavard/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from django.http import HttpResponse
-
 from math import floor, log as math_log, pow as math_pow
 from os import path, listdir, getenv
 from re import match, sub
 from uuid import uuid4
 
 from convert_numbers import english_to_persian
 from jdatetime import datetime as jdt
@@ -62,21 +60,21 @@
 def convert_second(seconds, verbose=True):
     seconds = int(seconds)
 
     if seconds == 0:
         if verbose:
             return '0'
         else:
-            return '0:00'
+            return '0:00:00'
 
     if seconds < 1:
         if verbose:
             return '~0'
         else:
-            return '~0:00'
+            return '~0:00:00'
 
     ss = f'{int(seconds % 60):02}'
     mi = f'{int(seconds / 60 % 60):02}'
     hh = f'{int(seconds / 3600 % 24):02}'
     dd = f'{int(seconds / 3600 / 24 % 30):02}'
     mo = f'{int(seconds / 3600 / 24 / 30 % 12):02}'
     yy = f'{int(seconds / 3600 / 24 / 30 / 12):02}'
@@ -181,15 +179,15 @@
     return conn.execute(f'''
         SELECT MAX(id) FROM "{table_name}";
     ''').fetchone()[0] \
     or 0  ## added 'or 0' because max id may sometimes be None
 
 
 def get_percent(smaller_number, total_number, to_persian=False):
-    if smaller_number == 0 or total_number == 0:
+    if smaller_number == 0:
         if to_persian:
             return '۰'
         return '0'
 
     _perc = (smaller_number * 100) / total_number
 
     if int(_perc) == 0:
@@ -236,24 +234,7 @@
 
 
 def to_tilda(text):
     '''/home/USERNAME/... -> ~/...'''
     return sub(getenv('HOME'), '~', text)
 
 
-
-def get_date_time_live():
-    jdatetime.set_locale('fa_IR')
-
-    jdt_now = jdt.now()
-
-    _year  = english_to_persian(jdt_now.strftime('%Y'))  ## ۱۴۰۱
-    _day   = english_to_persian(jdt_now.strftime('%d'))  ## ۱۷
-    _month = english_to_persian(jdt_now.strftime('%m'))  ## ۰۱
-
-    _hour = english_to_persian(jdt_now.strftime('%H'))
-    _min  = english_to_persian(jdt_now.strftime('%M'))
-    # _sec  = english_to_persian(jdt_now.strftime('%S'))
-
-    # _weekday = jdt_now.strftime('%A')  ## چهارشنبه
-
-    return HttpResponse(f'{_year}/{_month}/{_day} {_hour}:{_min}')
```

### Comparing `rahavard-0.0.12/rahavard.egg-info/PKG-INFO` & `rahavard-0.0.9/rahavard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.12
+Version: 0.0.9
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rahavard-0.0.12/setup.py` & `rahavard-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 here = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(here, 'README.md'), encoding='utf-8') as opened:
     long_description = '\n' + opened.read()
 
 
-VERSION = '0.0.12'
+VERSION = '0.0.9'
 DESCRIPTION = 'Re-Usable Utils'
 LONG_DESCRIPTION = 'Re-Usable Utils to Be Used on Our Django Projects'
 
 setup(
     name='rahavard',
     version=VERSION,
     author='Davoud Arsalani',
```

