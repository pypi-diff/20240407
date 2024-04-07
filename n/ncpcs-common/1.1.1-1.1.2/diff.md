# Comparing `tmp/ncpcs_common-1.1.1.tar.gz` & `tmp/ncpcs_common-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ncpcs_common-1.1.1.tar", last modified: Tue Mar 26 05:29:54 2024, max compression
+gzip compressed data, was "dist/ncpcs_common-1.1.2.tar", last modified: Sun Apr  7 01:43:58 2024, max compression
```

## Comparing `ncpcs_common-1.1.1.tar` & `ncpcs_common-1.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.586616 ncpcs_common-1.1.1/
--rw-r--r--   0 chen       (501) staff       (20)      137 2024-03-26 05:29:54.586304 ncpcs_common-1.1.1/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-01 03:19:06.000000 ncpcs_common-1.1.1/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.553616 ncpcs_common-1.1.1/common/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/__init__.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.554762 ncpcs_common-1.1.1/common/constants/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/constants/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      296 2024-03-11 01:42:08.000000 ncpcs_common-1.1.1/common/constants/database_config.py
--rw-r--r--   0 chen       (501) staff       (20)    75666 2024-03-20 07:35:17.000000 ncpcs_common-1.1.1/common/constants/level_dict.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.556178 ncpcs_common-1.1.1/common/entity/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/entity/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      742 2024-03-14 03:04:23.000000 ncpcs_common-1.1.1/common/entity/relation_key.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.557764 ncpcs_common-1.1.1/common/service/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1433 2024-02-22 00:30:19.000000 ncpcs_common-1.1.1/common/service/iccc3.py
--rw-r--r--   0 chen       (501) staff       (20)     3502 2024-03-14 03:08:51.000000 ncpcs_common-1.1.1/common/service/medical_text.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.569943 ncpcs_common-1.1.1/common/tests/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/tests/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1621 2024-03-13 00:54:29.000000 ncpcs_common-1.1.1/common/tests/test_date_util.py
--rw-r--r--   0 chen       (501) staff       (20)      493 2024-03-11 01:56:01.000000 ncpcs_common-1.1.1/common/tests/test_encrypt_util.py
--rw-r--r--   0 chen       (501) staff       (20)      990 2024-02-22 00:30:19.000000 ncpcs_common-1.1.1/common/tests/test_iccc3.py
--rw-r--r--   0 chen       (501) staff       (20)      259 2024-03-08 06:32:33.000000 ncpcs_common-1.1.1/common/tests/test_id_card_util.py
--rw-r--r--   0 chen       (501) staff       (20)      238 2024-02-22 00:30:19.000000 ncpcs_common-1.1.1/common/tests/test_list_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1776 2024-03-14 03:09:57.000000 ncpcs_common-1.1.1/common/tests/test_medical_text.py
--rw-r--r--   0 chen       (501) staff       (20)      196 2024-03-08 06:32:33.000000 ncpcs_common-1.1.1/common/tests/test_phone_util.py
--rw-r--r--   0 chen       (501) staff       (20)      248 2024-03-14 03:02:47.000000 ncpcs_common-1.1.1/common/tests/test_relation_key.py
--rw-r--r--   0 chen       (501) staff       (20)     2331 2024-03-08 07:52:02.000000 ncpcs_common-1.1.1/common/tests/test_sql_util.py
--rw-r--r--   0 chen       (501) staff       (20)     4194 2024-03-14 08:10:50.000000 ncpcs_common-1.1.1/common/tests/test_string_util.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.583578 ncpcs_common-1.1.1/common/util/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.1/common/util/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      316 2024-03-08 07:12:56.000000 ncpcs_common-1.1.1/common/util/csv_util.py
--rw-r--r--   0 chen       (501) staff       (20)     2200 2024-03-11 01:54:24.000000 ncpcs_common-1.1.1/common/util/database_connection_util.py
--rw-r--r--   0 chen       (501) staff       (20)     9442 2024-03-25 08:45:23.000000 ncpcs_common-1.1.1/common/util/date_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1133 2024-03-11 01:01:54.000000 ncpcs_common-1.1.1/common/util/encrypt_util.py
--rw-r--r--   0 chen       (501) staff       (20)      185 2024-03-07 08:57:18.000000 ncpcs_common-1.1.1/common/util/excel_util.py
--rw-r--r--   0 chen       (501) staff       (20)     3829 2024-03-08 06:13:07.000000 ncpcs_common-1.1.1/common/util/id_card_util.py
--rw-r--r--   0 chen       (501) staff       (20)      889 2024-03-20 01:13:40.000000 ncpcs_common-1.1.1/common/util/linux_util.py
--rw-r--r--   0 chen       (501) staff       (20)      131 2024-02-01 05:44:53.000000 ncpcs_common-1.1.1/common/util/list_util.py
--rw-r--r--   0 chen       (501) staff       (20)      238 2024-03-08 06:33:15.000000 ncpcs_common-1.1.1/common/util/phone_util.py
--rw-r--r--   0 chen       (501) staff       (20)     7430 2024-03-08 07:32:28.000000 ncpcs_common-1.1.1/common/util/sql_util.py
--rw-r--r--   0 chen       (501) staff       (20)     3279 2024-03-26 05:24:15.000000 ncpcs_common-1.1.1/common/util/string_util.py
--rw-r--r--   0 chen       (501) staff       (20)      497 2024-02-02 06:22:13.000000 ncpcs_common-1.1.1/common/util/timer_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1315 2024-03-08 06:08:27.000000 ncpcs_common-1.1.1/common/util/zip_util.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-03-26 05:29:54.585929 ncpcs_common-1.1.1/ncpcs_common.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      137 2024-03-26 05:29:54.000000 ncpcs_common-1.1.1/ncpcs_common.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     1168 2024-03-26 05:29:54.000000 ncpcs_common-1.1.1/ncpcs_common.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2024-03-26 05:29:54.000000 ncpcs_common-1.1.1/ncpcs_common.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       51 2024-03-26 05:29:54.000000 ncpcs_common-1.1.1/ncpcs_common.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)        7 2024-03-26 05:29:54.000000 ncpcs_common-1.1.1/ncpcs_common.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2024-03-26 05:29:54.586723 ncpcs_common-1.1.1/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      263 2024-03-26 05:29:52.000000 ncpcs_common-1.1.1/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.050715 ncpcs_common-1.1.2/
+-rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-07 01:43:58.050174 ncpcs_common-1.1.2/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-01 03:19:06.000000 ncpcs_common-1.1.2/README.md
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.008852 ncpcs_common-1.1.2/common/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/__init__.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.010582 ncpcs_common-1.1.2/common/constants/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/constants/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      296 2024-03-11 01:42:08.000000 ncpcs_common-1.1.2/common/constants/database_config.py
+-rw-r--r--   0 chen       (501) staff       (20)    76279 2024-04-07 01:40:35.000000 ncpcs_common-1.1.2/common/constants/level_dict.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.012672 ncpcs_common-1.1.2/common/entity/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/entity/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      742 2024-03-14 03:04:23.000000 ncpcs_common-1.1.2/common/entity/relation_key.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.014702 ncpcs_common-1.1.2/common/service/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/service/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1433 2024-02-22 00:30:19.000000 ncpcs_common-1.1.2/common/service/iccc3.py
+-rw-r--r--   0 chen       (501) staff       (20)     3502 2024-03-14 03:08:51.000000 ncpcs_common-1.1.2/common/service/medical_text.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.028925 ncpcs_common-1.1.2/common/tests/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/tests/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1621 2024-03-13 00:54:29.000000 ncpcs_common-1.1.2/common/tests/test_date_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      493 2024-03-11 01:56:01.000000 ncpcs_common-1.1.2/common/tests/test_encrypt_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      990 2024-02-22 00:30:19.000000 ncpcs_common-1.1.2/common/tests/test_iccc3.py
+-rw-r--r--   0 chen       (501) staff       (20)      259 2024-03-08 06:32:33.000000 ncpcs_common-1.1.2/common/tests/test_id_card_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      238 2024-02-22 00:30:19.000000 ncpcs_common-1.1.2/common/tests/test_list_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1776 2024-03-14 03:09:57.000000 ncpcs_common-1.1.2/common/tests/test_medical_text.py
+-rw-r--r--   0 chen       (501) staff       (20)      196 2024-03-08 06:32:33.000000 ncpcs_common-1.1.2/common/tests/test_phone_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      248 2024-03-14 03:02:47.000000 ncpcs_common-1.1.2/common/tests/test_relation_key.py
+-rw-r--r--   0 chen       (501) staff       (20)     2705 2024-03-27 06:49:32.000000 ncpcs_common-1.1.2/common/tests/test_sql_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     4194 2024-03-14 08:10:50.000000 ncpcs_common-1.1.2/common/tests/test_string_util.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.046035 ncpcs_common-1.1.2/common/util/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.2/common/util/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      316 2024-03-08 07:12:56.000000 ncpcs_common-1.1.2/common/util/csv_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     2200 2024-03-11 01:54:24.000000 ncpcs_common-1.1.2/common/util/database_connection_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     9442 2024-03-25 08:45:23.000000 ncpcs_common-1.1.2/common/util/date_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1133 2024-03-11 01:01:54.000000 ncpcs_common-1.1.2/common/util/encrypt_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      185 2024-03-07 08:57:18.000000 ncpcs_common-1.1.2/common/util/excel_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     3829 2024-03-08 06:13:07.000000 ncpcs_common-1.1.2/common/util/id_card_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      889 2024-03-20 01:13:40.000000 ncpcs_common-1.1.2/common/util/linux_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      131 2024-02-01 05:44:53.000000 ncpcs_common-1.1.2/common/util/list_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      238 2024-03-08 06:33:15.000000 ncpcs_common-1.1.2/common/util/phone_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     7451 2024-03-27 00:35:28.000000 ncpcs_common-1.1.2/common/util/sql_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     3279 2024-03-26 05:24:15.000000 ncpcs_common-1.1.2/common/util/string_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      497 2024-02-02 06:22:13.000000 ncpcs_common-1.1.2/common/util/timer_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1315 2024-03-08 06:08:27.000000 ncpcs_common-1.1.2/common/util/zip_util.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:43:58.049477 ncpcs_common-1.1.2/ncpcs_common.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-07 01:43:57.000000 ncpcs_common-1.1.2/ncpcs_common.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)     1168 2024-04-07 01:43:57.000000 ncpcs_common-1.1.2/ncpcs_common.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2024-04-07 01:43:57.000000 ncpcs_common-1.1.2/ncpcs_common.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       51 2024-04-07 01:43:57.000000 ncpcs_common-1.1.2/ncpcs_common.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)        7 2024-04-07 01:43:57.000000 ncpcs_common-1.1.2/ncpcs_common.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2024-04-07 01:43:58.050861 ncpcs_common-1.1.2/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      263 2024-04-07 01:41:56.000000 ncpcs_common-1.1.2/setup.py
```

### Comparing `ncpcs_common-1.1.1/common/constants/level_dict.py` & `ncpcs_common-1.1.2/common/constants/level_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,30 @@
                             "nc_allergy_history", "nc_exposure_history", "nc_mother_fertile_history", "nc_feed_history",
                             "nc_growth_history", "nc_physical_exam"],
     "nc_fist_disease_course": ["nc_case_characteristics", "nc_primary_diagnosis", "nc_primary_diagnosis_basis",
                                "nc_differential_diagnosis", "nc_diagnosis_treatment_plan"],
     "nc_daily_disease_course": ["nc_course_detail"],
     "nc_discharge_record": ["nc_discharge_condition", 'nc_diagnosis_process', 'nc_discharge_order'],
     "nc_pathology_info": ["nc_clinical_diagnosis", 'nc_gross_findings', 'nc_pathology_diagnosis'],
-    "nc_death_record": ["nc_chief_complaint", 'nc_admission_condition', 'nc_diagnosis_process', 'nc_death_reason', 'nc_death_detail']
+    "nc_death_record": ["nc_chief_complaint", 'nc_admission_condition', 'nc_diagnosis_process', 'nc_death_reason', 'nc_death_detail'],
+    'nc_readmission_record': ["nc_past_admission_record", "nc_chief_complaint", "nc_present_illness_history", 'nc_primary_diagnosis'],
+    'nc_24hours_admission_discharge_info': ['nc_chief_complaint', 'nc_admission_condition', 'nc_admission_diagnosis', 'nc_diagnosis_process', 'nc_discharge_condition', 'nc_discharge_diagnosis', 'nc_discharge_order']
 }
 
 
 NAME_MAP = {
+    "nc_readmission_record": "再入院记录",
+    "nc_24hours_admission_discharge_info": "24小时入出院记录",
     "nc_pathology_diagnosis_name": "病理诊断名称",
     "nc_main_diagnosis_name": "出院主要诊断名称",
     "nc_other_diagnosis_name": "出院其他诊断名称",
     'nc_admission_record': '入院记录',
+    "nc_past_admission_record": "既往疾病史",
+    "nc_admission_diagnosis": "入院诊断",
+    "nc_discharge_diagnosis": "出院诊断",
     'nc_present_illness_history': '现病史',
     'nc_chief_complaint': '主诉',
     'nc_family_history': '家族史',
     'nc_past_medical_history': '既往疾病史',
     'nc_tumo_rgenetic_history': '肿瘤遗传史',
     'nc_personal_history': '个人史',
     'nc_marital_history': '婚育史',
```

### Comparing `ncpcs_common-1.1.1/common/entity/relation_key.py` & `ncpcs_common-1.1.2/common/entity/relation_key.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/service/iccc3.py` & `ncpcs_common-1.1.2/common/service/iccc3.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/service/medical_text.py` & `ncpcs_common-1.1.2/common/service/medical_text.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/tests/test_date_util.py` & `ncpcs_common-1.1.2/common/tests/test_date_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/tests/test_iccc3.py` & `ncpcs_common-1.1.2/common/tests/test_iccc3.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/tests/test_medical_text.py` & `ncpcs_common-1.1.2/common/tests/test_medical_text.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/tests/test_sql_util.py` & `ncpcs_common-1.1.2/common/tests/test_sql_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,18 +9,22 @@
         assert transfer_database_name_to_hump("nc_admission_record") == 'ncAdmissionRecord'
 
     def test_transfer_hump_to_database_name(self):
         assert transfer_hump_to_database_name("ncAddTime") == 'nc_add_time'
         assert transfer_hump_to_database_name("ncAdmissionRecord") == 'nc_admission_record'
 
     def test_generate_select_sql(self):
-        print(generate_select_sql('ncpcs_tool', 'nc_report_medical_info'))
+        print(generate_select_sql('ncpcs_medical_data_analyze', 'nc_tumor_desc'))
 
     def test_generate_insert_sql(self):
-        print(generate_insert_sql('ncpcs_tool', 'nc_report_medical_info'))
+        # print(generate_insert_sql('ncpcs_tool', 'nc_report_medical_info'))
+        print("select distinct nc_iccc3_code, nc_level from nc_tumor_desc UNION " \
+                          "select distinct nc_iccc3_code, nc_level from nc_tumor_gtm union select distinct " \
+                          "nc_iccc3_code, nc_level from nc_tumor_subtype UNION select distinct nc_iccc3_code, " \
+                          "nc_level from nc_tumor_tnm")
 
     def test_generate_batch_insert_sql(self):
         print(generate_batch_insert_sql('ncpcs_tool', 'nc_report_medical_info'))
 
     def test_generate_common_query_sql(self):
         print(generate_common_query_sql('ncpcs_tool', 'nc_report_medical_info'))
```

### Comparing `ncpcs_common-1.1.1/common/tests/test_string_util.py` & `ncpcs_common-1.1.2/common/tests/test_string_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/database_connection_util.py` & `ncpcs_common-1.1.2/common/util/database_connection_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/date_util.py` & `ncpcs_common-1.1.2/common/util/date_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/encrypt_util.py` & `ncpcs_common-1.1.2/common/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/id_card_util.py` & `ncpcs_common-1.1.2/common/util/id_card_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/linux_util.py` & `ncpcs_common-1.1.2/common/util/linux_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/sql_util.py` & `ncpcs_common-1.1.2/common/util/sql_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 
 def get_insert_columns_and_values(data):
     return _get_insert_columns(data.keys()), _get_insert_values(data.values())
 
 
 def _get_col_list(schema, table_name):
-    conn = get_connection_by_schema(schema)
+    conn = get_connection_by_schema(b'my pleasure lord', schema)
     cursor = conn.cursor()
     CHECK_COL_SQL_FORMAT = "SELECT COLUMN_NAME, DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME = '{}' AND TABLE_SCHEMA = '{}'"
     ITEM_FORMAT = "#[item.{}]"
     cursor.execute(CHECK_COL_SQL_FORMAT.format(table_name, schema))
     col_name_list = []
     item_name_list = []
     for ele in cursor.fetchall():
```

### Comparing `ncpcs_common-1.1.1/common/util/string_util.py` & `ncpcs_common-1.1.2/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/common/util/zip_util.py` & `ncpcs_common-1.1.2/common/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.1/ncpcs_common.egg-info/SOURCES.txt` & `ncpcs_common-1.1.2/ncpcs_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

