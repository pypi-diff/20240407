# Comparing `tmp/ts-soup-0.0.8.tar.gz` & `tmp/ts-soup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-oq12dazh\ts-soup-0.0.8.tar", last modified: Sat Apr  6 00:24:16 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-_ntpj_yd\ts-soup-0.0.9.tar", last modified: Sun Apr  7 06:47:24 2024, max compression
```

## Comparing `ts-soup-0.0.8.tar` & `ts-soup-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 00:24:16.975754 ts-soup-0.0.8/
--rw-rw-rw-   0        0        0     1028 2024-04-06 00:24:16.974753 ts-soup-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 00:24:16.975754 ts-soup-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-06 00:24:13.000000 ts-soup-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:24:16.966751 ts-soup-0.0.8/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.8/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts-soup-0.0.8/ts_soup/app.py
--rw-rw-rw-   0        0        0    18402 2024-04-06 00:21:59.000000 ts-soup-0.0.8/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:24:16.972751 ts-soup-0.0.8/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.8/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.8/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5796 2024-04-06 00:23:57.000000 ts-soup-0.0.8/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:24:16.973751 ts-soup-0.0.8/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-06 00:24:16.000000 ts-soup-0.0.8/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-06 00:24:16.000000 ts-soup-0.0.8/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 00:24:16.000000 ts-soup-0.0.8/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 00:24:16.000000 ts-soup-0.0.8/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.520920 ts-soup-0.0.9/
+-rw-rw-rw-   0        0        0     1028 2024-04-07 06:47:24.519919 ts-soup-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 06:47:24.520920 ts-soup-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-07 06:47:13.000000 ts-soup-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.506431 ts-soup-0.0.9/ts_soup/
+-rw-rw-rw-   0        0        0      307 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/app.py
+-rw-rw-rw-   0        0        0    18009 2024-04-07 06:46:03.000000 ts-soup-0.0.9/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.516559 ts-soup-0.0.9/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5793 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.518559 ts-soup-0.0.9/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.8/PKG-INFO` & `ts-soup-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.8
+Version: 0.0.9
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.8/README.md` & `ts-soup-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.8/setup.py` & `ts-soup-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.8",
+  version="0.0.9",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
-)
+)
```

### Comparing `ts-soup-0.0.8/ts_soup/app.py` & `ts-soup-0.0.9/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.8/ts_soup/common.py` & `ts-soup-0.0.9/ts_soup/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,17 +144,17 @@
         """
         :param db: 数据库名
         :param index_field: 数据源筛选日期的字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
         self.empty_check = empty_check
         if db:
-            self.db = USABLE_DBS.get(db)
+            self.db = USABLE_DBS[db]
         else:
-            self.db = USABLE_DBS.get('sources_default')
+            self.db = USABLE_DBS['sources_default']
         self.index_field = index_field
 
     @abstractmethod
     def build_source(self, to_update_date):
         pass
 
 
@@ -163,20 +163,20 @@
                  is_seperated):
         self.tb = tb
         self.user_def_pro = user_def_pro
         if user_def_pro is None:
             self.user_def_pro = []
 
         if db:
-            self.db = USABLE_DBS.get(db)
-            self.db_pym = USABLE_DBS.get(f'{db}_pym')
+            self.db = USABLE_DBS[db]
+            self.db_pym = USABLE_DBS[f'{db}_pym']
             self.db_str = db
         else:
-            self.db = USABLE_DBS.get('targets_default')
-            self.db_pym = USABLE_DBS.get('targets_default_pym')
+            self.db = USABLE_DBS['targets_default']
+            self.db_pym = USABLE_DBS['targets_default_pym']
             self.db_str = 'targets_default'
 
         self.is_seperated = is_seperated
         self.drop_axis = drop_axis
         self.drop_na_subset = drop_na_subset
         self.drop_na_thresh = drop_na_thresh
         self.has_unique_idx = has_unique_idx
@@ -203,15 +203,14 @@
         self.any_source_empty = False
         self.value = []
         self.sources = sources
         self.targets = targets
         self.source_data = []
         self.executed_table = executed_table
         self.to_update_date = self.__get_update_date()
-        self.index_map = None
         self.customized_updated_state = None
 
     def __get_update_date(self):
         return DATA_UPDATED_STATE.loc[~(DATA_UPDATED_STATE[self.executed_table] == 1), 'update_date']
 
     def make_source_data(self):
         """
@@ -254,33 +253,29 @@
         update_state_date = None
         func_update_flag = True
         for index, target in enumerate(self.targets):
             cur_result = self.value[index]
 
             if len(target.user_def_pro) > 0:  # 获取在funcs里传入的额外属性（target未定义的）
                 for pro in target.user_def_pro:
-                    exec(f"target.{pro} = self.{pro}")
-            # target.index_map = self.index_map
+                    setattr(target, pro, getattr(self, pro))
 
             """
              处理返回值整个为none，如有一个返回结果为none，则整个方法的 这段to_update_date时间都应视为无数据，防止下文
              转str和合并索引时产生keyError
              """
             if cur_result is None:
                 func_update_flag = False
                 print(f'{target.tb} 无数据同步')
                 continue
 
             # 处理返回值部分为空的情况
-            params = {'axis': target.drop_axis, 'how': 'all'}
+            params = {'axis': target.drop_axis, 'how': 'all', 'thresh': target.drop_na_thresh}
             if target.drop_na_subset:
                 params['subset'] = target.drop_na_subset
-            if target.drop_na_thresh:
-                params['thresh'] = target.drop_na_thresh
-                del params['how']
             cur_result = cur_result.dropna(**params)
 
             # 处理经过dropna以后如果全为空的情况，视为全为空，原理同上
             if cur_result.empty:
                 func_update_flag = False
                 print(f'{target.tb} 无数据同步')
                 continue
@@ -298,24 +293,22 @@
 
             # 调用统一接口完成成果产出
             target.build_output(cur_result)
 
             # 如果未传入自定义更新日期，则取数据日期作为 处理操作表的更新日期，取各数据结果交集
             if (update_state_date is not None) and (self.customized_updated_state is None):
                 update_state_date = update_state_date.merge(
-                    cur_result[[target.index_field]].drop_duplicates().apply(
-                        lambda x: self.index_map[x] if self.index_map is not None else x),
+                    cur_result[[target.index_field]].drop_duplicates(),
                     left_on='update_date',
                     right_on=target.index_field,
                     how='inner'
                 )[['update_date']]
             elif (update_state_date is None) and (self.customized_updated_state is None):
                 update_state_date = pd.DataFrame(
-                    cur_result[target.index_field].drop_duplicates().apply(
-                        lambda x: self.index_map[x] if self.index_map is not None else x).values,
+                    cur_result[target.index_field].drop_duplicates().values,
                     columns=['update_date']
                 )
 
         # 将方法的操作记录写入数据库
         if func_update_flag:
             if update_state_date is not None and not update_state_date.empty:
                 self.__handle_insert_update_state(update_state_date)
```

### Comparing `ts-soup-0.0.8/ts_soup/workers/sources.py` & `ts-soup-0.0.9/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.8/ts_soup/workers/targets.py` & `ts-soup-0.0.9/ts_soup/workers/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from dateutil.relativedelta import relativedelta
 import datetime
 
 
 class TargetTable(BaseTarget):
     def __init__(self, tb, db: str = None, index_field: str = 'date', is_seperated=False, drop_axis=0,
-                 drop_na_subset=None, drop_na_thresh=None, tag=None, has_unique_idx=False, user_def_pro: list = None):
+                 drop_na_subset=None, drop_na_thresh=2, tag=None, has_unique_idx=False, user_def_pro: list = None):
         """
         目标表信息，如果该表需要分表，则tb传入没有分表年份的表名，年份在写入时会自动加入，同时is_seperated设置为True
         :param tb:表名，
         :param db:数据库，配置里的source_name，默认使用去向表第一个库
         :param index_field:
         :param is_seperated:是否是分表的表
         :param drop_axis:如果存在空数据，drop_na的轴
```

### Comparing `ts-soup-0.0.8/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.0.9/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.8
+Version: 0.0.9
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

