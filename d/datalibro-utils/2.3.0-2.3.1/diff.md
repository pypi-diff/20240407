# Comparing `tmp/datalibro_utils-2.3.0.tar.gz` & `tmp/datalibro_utils-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_utils-2.3.0.tar", last modified: Fri Mar 22 02:43:35 2024, max compression
+gzip compressed data, was "datalibro_utils-2.3.1.tar", last modified: Sun Apr  7 05:56:42 2024, max compression
```

## Comparing `datalibro_utils-2.3.0.tar` & `datalibro_utils-2.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 02:43:35.277531 datalibro_utils-2.3.0/
--rw-rw-rw-   0        0        0      301 2024-03-22 02:43:35.277531 datalibro_utils-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 02:43:35.267038 datalibro_utils-2.3.0/datalibro_utils/
--rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.0/datalibro_utils/__init__.py
--rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.0/datalibro_utils/datalibro_auth.py
--rw-rw-rw-   0        0        0     6617 2024-02-02 10:06:27.000000 datalibro_utils-2.3.0/datalibro_utils/dlbi.py
--rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.0/datalibro_utils/email.py
--rw-rw-rw-   0        0        0    12697 2024-03-22 02:34:41.000000 datalibro_utils-2.3.0/datalibro_utils/mapping.py
--rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.0/datalibro_utils/openai.py
--rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.0/datalibro_utils/pet_sys.py
--rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.0/datalibro_utils/test.py
-drwxrwxrwx   0        0        0        0 2024-03-22 02:43:35.276522 datalibro_utils-2.3.0/datalibro_utils.egg-info/
--rw-rw-rw-   0        0        0      301 2024-03-22 02:43:34.000000 datalibro_utils-2.3.0/datalibro_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-03-22 02:43:35.000000 datalibro_utils-2.3.0/datalibro_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 02:43:34.000000 datalibro_utils-2.3.0/datalibro_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-22 02:43:34.000000 datalibro_utils-2.3.0/datalibro_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-22 02:43:34.000000 datalibro_utils-2.3.0/datalibro_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 02:43:35.278537 datalibro_utils-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-03-22 02:43:24.000000 datalibro_utils-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.250104 datalibro_utils-2.3.1/
+-rw-rw-rw-   0        0        0      301 2024-04-07 05:56:42.249112 datalibro_utils-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.241937 datalibro_utils-2.3.1/datalibro_utils/
+-rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.1/datalibro_utils/__init__.py
+-rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.1/datalibro_utils/datalibro_auth.py
+-rw-rw-rw-   0        0        0     6617 2024-02-02 10:06:27.000000 datalibro_utils-2.3.1/datalibro_utils/dlbi.py
+-rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.1/datalibro_utils/email.py
+-rw-rw-rw-   0        0        0    13183 2024-04-07 05:56:09.000000 datalibro_utils-2.3.1/datalibro_utils/mapping.py
+-rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.1/datalibro_utils/openai.py
+-rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.1/datalibro_utils/pet_sys.py
+-rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.1/datalibro_utils/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 05:56:42.249112 datalibro_utils-2.3.1/datalibro_utils.egg-info/
+-rw-rw-rw-   0        0        0      301 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-07 05:56:42.000000 datalibro_utils-2.3.1/datalibro_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 05:56:42.250104 datalibro_utils-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-04-07 05:56:25.000000 datalibro_utils-2.3.1/setup.py
```

### Comparing `datalibro_utils-2.3.0/README.md` & `datalibro_utils-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.0/datalibro_utils/datalibro_auth.py` & `datalibro_utils-2.3.1/datalibro_utils/datalibro_auth.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.0/datalibro_utils/dlbi.py` & `datalibro_utils-2.3.1/datalibro_utils/dlbi.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.0/datalibro_utils/email.py` & `datalibro_utils-2.3.1/datalibro_utils/email.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.0/datalibro_utils/mapping.py` & `datalibro_utils-2.3.1/datalibro_utils/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,33 +69,42 @@
     try:
         series = map_series.loc[map_series['Model']==model, 'Series'].iloc[0]
     except:
         series = ""
         miss_info = f'series of {sku} not found, please update!'
     return series, miss_info
 
-def get_sku_extra(df_ori, fields, return_miss=False):
+def get_sku_extra(df_ori, fields, return_miss=False,service_account_path=None):
     if fields == 'all':
         print('total fields...')
         fields_list = ['brand','product_line','product_type','sku_code','model', 'scu', 'app_supported', 'series']
     else:
         fields_list = fields
     df = df_ori.copy()
     print('loading mapping info...')
     if "product_line" in fields_list or "product_type" in fields_list :
-        df_map_sku_code = tm.gs_read_df(('Datalibro Mapping Master', 'sku_code'))
+        if service_account_path:
+            df_map_sku_code = tm.gs_read_df(('Datalibro Mapping Master', 'sku_code'),service_account_path)
+        else:
+            df_map_sku_code = tm.gs_read_df(('Datalibro Mapping Master', 'sku_code'))
         if "product_line" in fields_list:
             df["product_line"], list_miss_product_line = zip(*df['sku'].apply(sku_get_product_line, map_sku_code = df_map_sku_code))
         if "product_type" in fields_list:
             df["product_type"], list_miss_product_type = zip(*df['sku'].apply(sku_get_product_type, map_sku_code = df_map_sku_code))
     if "scu" in fields_list:
-        df_map_scu = tm.gs_read_df(('Datalibro Mapping Master', 'scu'))
+        if service_account_path:
+            df_map_scu = tm.gs_read_df(('Datalibro Mapping Master', 'scu'),service_account_path)
+        else:
+            df_map_scu = tm.gs_read_df(('Datalibro Mapping Master', 'scu'))
         df['scu'] = df['sku'].apply(sku_get_scu, map_scu=df_map_scu)
     if "series" in fields_list:
-        df_map_series = tm.gs_read_df(('Datalibro Mapping Master', 'series'))
+        if service_account_path:
+            df_map_series = tm.gs_read_df(('Datalibro Mapping Master', 'series'),service_account_path)
+        else:
+            df_map_series = tm.gs_read_df(('Datalibro Mapping Master', 'series'))
         df['series'], list_miss_series = zip(*df['sku'].apply(sku_get_series, map_series=df_map_series))
         df['series'] = df['series'].apply(lambda x: 'Infinity' if x == np.inf or x == -np.inf else x)
     if "brand" in fields_list:
         df['brand'] = df['sku'].apply(sku_get_brand)
     if ("model" in fields_list) | ("app_supported" in fields_list):
         df['model'] = df['sku'].apply(sku_get_model)
         # 检验是否有新增支持APP的model
```

### Comparing `datalibro_utils-2.3.0/datalibro_utils/openai.py` & `datalibro_utils-2.3.1/datalibro_utils/openai.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.0/datalibro_utils/pet_sys.py` & `datalibro_utils-2.3.1/datalibro_utils/pet_sys.py`

 * *Files identical despite different names*

