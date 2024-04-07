# Comparing `tmp/tablemaster-1.1.4.tar.gz` & `tmp/tablemaster-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.1.4.tar", last modified: Wed Oct 25 10:22:38 2023, max compression
+gzip compressed data, was "tablemaster-1.1.5.tar", last modified: Sun Apr  7 03:24:13 2024, max compression
```

## Comparing `tablemaster-1.1.4.tar` & `tablemaster-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-10-25 10:22:38.746260 tablemaster-1.1.4/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.4/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-10-25 10:22:38.746080 tablemaster-1.1.4/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     1729 2023-07-04 07:26:19.000000 tablemaster-1.1.4/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-10-25 10:22:38.746304 tablemaster-1.1.4/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      559 2023-10-25 10:22:09.000000 tablemaster-1.1.4/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-10-25 10:22:38.745059 tablemaster-1.1.4/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      615 2023-10-25 10:17:27.000000 tablemaster-1.1.4/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1716 2023-10-25 10:16:44.000000 tablemaster-1.1.4/tablemaster/feishu.py
--rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.4/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3334 2023-06-19 10:02:57.000000 tablemaster-1.1.4/tablemaster/local.py
--rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.4/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.4/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-10-25 10:22:38.745883 tablemaster-1.1.4/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-10-25 10:22:38.000000 tablemaster-1.1.4/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      332 2023-10-25 10:22:38.000000 tablemaster-1.1.4/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-10-25 10:22:38.000000 tablemaster-1.1.4/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)      108 2023-10-25 10:22:38.000000 tablemaster-1.1.4/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2023-10-25 10:22:38.000000 tablemaster-1.1.4/tablemaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 03:24:13.202820 tablemaster-1.1.5/
+-rw-rw-rw-   0        0        0    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-07 03:24:13.201814 tablemaster-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1729 2023-07-04 07:26:19.000000 tablemaster-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 03:24:13.202820 tablemaster-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      559 2024-04-07 03:20:15.000000 tablemaster-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:24:13.194588 tablemaster-1.1.5/tablemaster/
+-rw-rw-rw-   0        0        0      615 2023-10-25 10:17:27.000000 tablemaster-1.1.5/tablemaster/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-10-25 10:16:44.000000 tablemaster-1.1.5/tablemaster/feishu.py
+-rw-rw-rw-   0        0        0     1137 2024-04-07 03:20:05.000000 tablemaster-1.1.5/tablemaster/gspread.py
+-rw-rw-rw-   0        0        0     3334 2023-06-19 10:02:57.000000 tablemaster-1.1.5/tablemaster/local.py
+-rw-rw-rw-   0        0        0     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.5/tablemaster/mysql.py
+-rw-rw-rw-   0        0        0      810 2023-03-29 11:23:27.000000 tablemaster-1.1.5/tablemaster/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:24:13.201814 tablemaster-1.1.5/tablemaster.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-07 03:24:12.000000 tablemaster-1.1.5/tablemaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-07 03:24:13.000000 tablemaster-1.1.5/tablemaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 03:24:12.000000 tablemaster-1.1.5/tablemaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-07 03:24:12.000000 tablemaster-1.1.5/tablemaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 03:24:12.000000 tablemaster-1.1.5/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.1.4/LICENSE` & `tablemaster-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/README.md` & `tablemaster-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/setup.py` & `tablemaster-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.1.4',
+    version='1.1.5',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy==1.4.46',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.1.4/tablemaster/__init__.py` & `tablemaster-1.1.5/tablemaster/__init__.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/tablemaster/feishu.py` & `tablemaster-1.1.5/tablemaster/feishu.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/tablemaster/gspread.py` & `tablemaster-1.1.5/tablemaster/gspread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import gspread
 import pandas as pd
 
-def gs_read_df(map):
+def gs_read_df(map,service_account_path=None):
     print('...reading google sheets...')
-    gc = gspread.service_account()
+    if service_account_path:
+        gc = gspread.service_account(service_account_path)
+    else:
+        gc = gspread.service_account()
     wks = gc.open(map[0]).worksheet(map[1])
     df = pd.DataFrame(wks.get_all_records())
     print('...have read google sheets!...')
     print(df.head())
     return df
 
 def gs_write_df(map, df, loc='A1'):
```

### Comparing `tablemaster-1.1.4/tablemaster/local.py` & `tablemaster-1.1.5/tablemaster/local.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/tablemaster/mysql.py` & `tablemaster-1.1.5/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.4/tablemaster/utils.py` & `tablemaster-1.1.5/tablemaster/utils.py`

 * *Files identical despite different names*

