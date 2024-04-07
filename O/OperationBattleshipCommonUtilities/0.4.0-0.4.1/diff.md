# Comparing `tmp/OperationBattleshipCommonUtilities-0.4.0.tar.gz` & `tmp/OperationBattleshipCommonUtilities-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.0.tar", last modified: Mon Apr  1 23:38:51 2024, max compression
+gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.1.tar", last modified: Sun Apr  7 21:20:50 2024, max compression
```

## Comparing `OperationBattleshipCommonUtilities-0.4.0.tar` & `OperationBattleshipCommonUtilities-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:38:51.812222 OperationBattleshipCommonUtilities-0.4.0/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 OperationBattleshipCommonUtilities-0.4.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 23:38:51.812222 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-04-01 23:38:51.000000 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-01 23:38:51.000000 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:38:51.000000 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-01 23:38:51.000000 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-01 23:38:51.000000 OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-04-01 23:38:51.812222 OperationBattleshipCommonUtilities-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 OperationBattleshipCommonUtilities-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 23:38:51.812222 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 21:51:05.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0    18758 2024-04-01 23:37:28.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     2758 2024-03-19 02:54:10.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-01 23:38:51.812222 OperationBattleshipCommonUtilities-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-01 23:20:31.000000 OperationBattleshipCommonUtilities-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.570362 OperationBattleshipCommonUtilities-0.4.1/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 OperationBattleshipCommonUtilities-0.4.1/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.563144 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/
+-rw-rw-rw-   0        0        0     3177 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3177 2024-04-07 21:20:50.565142 OperationBattleshipCommonUtilities-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 OperationBattleshipCommonUtilities-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.561141 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/
+-rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 21:51:05.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CompanyDao.py
+-rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/FailureLogger.py
+-rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GeographyHelper.py
+-rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-rw-rw-   0        0        0    18787 2024-04-07 21:12:06.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobPostingDao.py
+-rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/NomicAICaller.py
+-rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/OpenAICaller.py
+-rw-rw-rw-   0        0        0     2758 2024-03-19 02:54:10.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 21:20:50.571368 OperationBattleshipCommonUtilities-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-07 21:13:34.000000 OperationBattleshipCommonUtilities-0.4.1/setup.py
```

### Comparing `OperationBattleshipCommonUtilities-0.4.0/LICENSE` & `OperationBattleshipCommonUtilities-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.0
+Version: 0.4.1
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.0/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.0
+Version: 0.4.1
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.0/README.md` & `OperationBattleshipCommonUtilities-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/ApifyJobsCaller.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/CompanyDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CompanyDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/FailureLogger.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/FailureLogger.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/GeographyHelper.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobKeyWordsDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobPostingDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobPostingDao.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,14 +472,15 @@
         job_ids = dataframeOfJobIds['job_posting_id'].tolist()
 
         job_ids_tuple = tuple(job_ids)
 
         sql_query = f"""
         SELECT
             c.company_name,
+            c.linkedin_url,
             jp.job_title,
             jp.posting_url,
             jp.full_posting_description,
             jp.job_description,
             jp.is_ai,
             jp.is_genai,
             jp.salary_low,
```

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobSkillsDao.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/NomicAICaller.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/OpenAICaller.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.0/setup.py` & `OperationBattleshipCommonUtilities-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.4.0',
+    version='0.4.1',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

