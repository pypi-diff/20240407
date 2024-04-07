# Comparing `tmp/phdu-2.3.2.tar.gz` & `tmp/phdu-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.2.tar", last modified: Fri Apr  5 12:19:18 2024, max compression
+gzip compressed data, was "phdu-2.3.3.tar", last modified: Sun Apr  7 07:24:07 2024, max compression
```

## Comparing `phdu-2.3.2.tar` & `phdu-2.3.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.652445 phdu-2.3.2/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.2/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-05 12:19:18.652445 phdu-2.3.2/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.2/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.600442 phdu-2.3.2/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.2/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/analysis.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.2/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.2/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/geometry.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.3.2/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.620443 phdu-2.3.2/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.2/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.2/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.2/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    22497 2024-04-05 12:18:43.000000 phdu-2.3.2/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.2/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.636444 phdu-2.3.2/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.2/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.2/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.2/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.2/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.2/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.2/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.644444 phdu-2.3.2/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.2/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.2/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.2/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.652445 phdu-2.3.2/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.2/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.2/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.2/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.2/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 12:19:18.612442 phdu-2.3.2/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-05 12:19:18.000000 phdu-2.3.2/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-05 12:19:18.000000 phdu-2.3.2/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-05 12:19:18.000000 phdu-2.3.2/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-05 12:19:18.000000 phdu-2.3.2/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-05 12:19:18.000000 phdu-2.3.2/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-05 12:19:18.656445 phdu-2.3.2/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-05 12:18:55.000000 phdu-2.3.2/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.022978 phdu-2.3.3/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.3.3/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-04-07 07:24:07.022978 phdu-2.3.3/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.3.3/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.019645 phdu-2.3.3/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.3.3/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.3.3/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.3.3/phdu/analysis.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.3.3/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.3.3/phdu/geometry.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.3.3/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     6224 2024-04-07 07:23:26.000000 phdu-2.3.3/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.022978 phdu-2.3.3/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.3.3/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    22497 2024-04-07 07:01:10.000000 phdu-2.3.3/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.022978 phdu-2.3.3/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    32282 2024-01-18 07:19:52.000000 phdu-2.3.3/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.022978 phdu-2.3.3/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.022978 phdu-2.3.3/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.3.3/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.3.3/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:24:07.019645 phdu-2.3.3/phdu.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-04-07 07:24:06.000000 phdu-2.3.3/phdu.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-04-07 07:24:06.000000 phdu-2.3.3/phdu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-07 07:24:06.000000 phdu-2.3.3/phdu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-04-07 07:24:06.000000 phdu-2.3.3/phdu.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-04-07 07:24:06.000000 phdu-2.3.3/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-04-07 07:24:07.022978 phdu-2.3.3/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1659 2024-04-07 07:23:37.000000 phdu-2.3.3/setup.py
```

### Comparing `phdu-2.3.2/LICENSE.md` & `phdu-2.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/PKG-INFO` & `phdu-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.2
+Version: 2.3.3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.2/README.md` & `phdu-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/__init__.py` & `phdu-2.3.3/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/_helper.py` & `phdu-2.3.3/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/analysis.py` & `phdu-2.3.3/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/clustering.py` & `phdu-2.3.3/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/decomposition.py` & `phdu-2.3.3/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/geometry.py` & `phdu-2.3.3/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/np_utils.py` & `phdu-2.3.3/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/pd_utils.py` & `phdu-2.3.3/phdu/pd_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 pandas utils
 """
 import pandas as pd
 import numpy as np
-from functools import reduce     
+from functools import reduce
 from .stats.rtopy import resample
 from .stats.test import permutation
 
 def latex_table(df, index=False, **kwargs):
     """Pandas DataFrame -> Latex table."""
     col_format = "c" if isinstance(df, pd.core.series.Series) else "c"*len(df.columns)
     if index:
         col_format += "c"
     table_replacements = (("\\toprule", "\\toprule "*2),
                           ("\\bottomrule", "\\bottomrule "*2)
     )
     text_replacements = (("\\textbackslash ", "\\"),
-                         ("\{", "{"), 
+                         ("\{", "{"),
                          ("\}", "}"),
                          ("\$", "$"),
                          ("\_", "_"),
                          ("\\textasciicircum ", "^")
     )
     table_formatter = lambda x:  reduce(lambda a, kv: a.replace(*kv), table_replacements, x)
     text_formatter = lambda x: reduce(lambda a, kv: a.replace(*kv), text_replacements, x)
@@ -28,62 +28,72 @@
     print(formatter(df.to_latex(index=index, column_format=col_format, **kwargs)))
     return
 
 def insert_level_sep(df, row_seps=1, col_seps=1):
     """
     Insert NaN rows and cols when the outer level of the MultiIndex changes.
     Example for three columns with col_seps=1:   c1, c2, c3    =>   c1, NANs, c2, NaNs, c3.
-    
+
     This is useful when plotting a matrix and you want to visually separate different groups.
     """
     df_c = df.copy()
     col_levels = df.columns.get_level_values(0).unique() # respect the order
     row_levels = df.index.get_level_values(0).unique()
     for l in col_levels[:-1]:
         for k in range(col_seps):
-            df_c[(l, " "*k)] = np.NaN 
+            df_c[(l, " "*k)] = np.NaN
     for l in row_levels[:-1]:
         for k in range(row_seps):
             df_c.loc[(l, " "*k), :] = np.NaN
     return df_c[col_levels].loc[row_levels]
 
 def expand_sequences(df, dt=1, maxlen=None):
     """
     Input: DataFrame. Each element is an array and all arrays start at the same time and have the same time step dt.
-    
+
     Returns: MultiColumn DataFrame: (df.index,  (df.columns, time_steps))
     """
     if df.isna().values.any():
         if maxlen is None:
             maxlen = int(df.applymap(lambda x: x.size if isinstance(x, np.ndarray) else np.NaN).max().max())
         df_padded = df.applymap(lambda x: np.hstack((x, np.NaN*np.empty((maxlen-x.size)))) if isinstance(x, np.ndarray) else np.NaN*np.empty((maxlen)))
     else:
         if maxlen is None:
             maxlen = int(df.applymap(lambda x: x.size).values.max())
         df_padded = df.applymap(lambda x: np.hstack((x, np.NaN*np.empty((maxlen-x.size)))))
     df_padded_arr = np.stack([np.vstack(x) for x in df_padded.values]) # shape (df.shape[0], df.shape[1], time_steps)
-    return pd.DataFrame(df_padded_arr.reshape((df.shape[0], -1)), 
-                        index = df.index, 
+    return pd.DataFrame(df_padded_arr.reshape((df.shape[0], -1)),
+                        index = df.index,
                         columns = pd.MultiIndex.from_product([df.columns, dt*np.arange(maxlen)]))
 
 def tuple_wise(*dfs):
-    """Returns dataframe where each element is a tuple containing the elements from other dataframes."""
+    """
+    Attributes: Dataframes with same indices and columns. If the input are Series, they are converted to DataFrames.
+
+    Returns dataframe where each element is a tuple containing the elements from other dataframes.
+    """
+    for df in dfs:
+        if isinstance(df, pd.Series):
+            df = df.to_frame()
     df = dfs[0]
     assert all(df.index.intersection(df2.index).size == df.shape[0] for df2 in dfs[1:])
     assert all(df.columns.intersection(df2.columns).size == df.shape[1] for df2 in dfs[1:])
-    return pd.DataFrame(np.rec.fromarrays(tuple(df.values for df in dfs)).tolist(), 
+    return pd.DataFrame(np.rec.fromarrays(tuple(df.values for df in dfs)).tolist(),
                         columns=df.columns,
                         index=df.index)
 
 def vstack_wise(*dfs):
     """
-    Attributes: Dataframes where elements are arrays with equal length and have same indices and columns.
-    
+    Attributes: Dataframes where elements are arrays with equal length and have same indices and columns. If the input are Series, they are converted to DataFrames.
+
     Returns: DataFrame where df_ij = np.vstack((df1_ij, df2_ij, ...))
     """
+    for df in dfs:
+        if isinstance(df, pd.Series):
+            df = df.to_frame()
     R = np.rec.fromarrays(tuple(df.values for df in dfs))
     df1_df2 = pd.Series([np.vstack(i) if all(isinstance(j, np.ndarray) for j in i) else np.NaN for i in R.flatten()], dtype=object,
                         index=dfs[0].stack(dropna=False).index).unstack()
     return df1_df2
 
 def column_diffs(df, mode="to", mod_col=lambda x: "".join(np.array([*x])[[0, -1]])):
     """
@@ -92,15 +102,15 @@
     """
     N = df.shape[1]
     data = {}
     if mode == "-":
         label = lambda col1, col2: f"{col2} - {col1}"
     elif mode == "to":
         if callable(mod_col):
-            label = lambda col1, col2: r"$\Huge {{{}}} \to {{{}}}$".format(mod_col(col1.replace(" ", "\ ")), mod_col(col2.replace(" ", "\ ")))            
+            label = lambda col1, col2: r"$\Huge {{{}}} \to {{{}}}$".format(mod_col(col1.replace(" ", "\ ")), mod_col(col2.replace(" ", "\ ")))
         else:
             label = lambda col1, col2: r"$\Huge {{{}}} \to {{{}}}$".format(col1.replace(" ", "\ "), col2.replace(" ", "\ "))
     for i, col1 in enumerate(df.columns):
         if i < N:
             for col2 in df.columns[i+1:]:
                 data[label(col1, col2)] = df[col2] - df[col1]
     return pd.DataFrame(data)
@@ -112,25 +122,25 @@
             x[np.isnan(x)] = fillna
             return x
         CI = CI.apply(aux)
     if return_sample_stat:
         return CI, getattr(df, stat)()
     else:
         return CI
-    
+
 def permtest_by_col(df, alternative, stat="mean", paired=True, diff=True, label="c", **kwargs):
     """
-    Test directionality accross columns. 
-        col_i  (direction in [<, >, !=])  col_j     
-        
+    Test directionality accross columns.
+        col_i  (direction in [<, >, !=])  col_j
+
     Attributes:
         alternative:    'less', 'greater', 'two-sided'.
     """
     P = {}
     N = df.shape[1]
     is_paired = "paired" if paired else "not_paired"
     is_diff = "diff" if diff else ""
     for i in range(N):
         for j in range(i+1, N):
             yi, yj = df.iloc[:, [i,j]].dropna().values.T
             P[r"$\Huge {}_{{{}{}}}$".format(label, i+1, j+1)] = getattr(permutation, f"permutation_test_2sample_{is_paired}_{is_diff}{stat}")(yi, yj, alternative=alternative, **kwargs)
-    return pd.Series(P)
+    return pd.Series(P)
```

### Comparing `phdu-2.3.2/phdu/plots/base.py` & `phdu-2.3.3/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/plots/plotly_utils.py` & `phdu-2.3.3/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/script_fmt.py` & `phdu-2.3.3/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/_integration.py` & `phdu-2.3.3/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/_plots.py` & `phdu-2.3.3/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/bootstrap.py` & `phdu-2.3.3/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/conf_interval.py` & `phdu-2.3.3/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/corr.py` & `phdu-2.3.3/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/rtopy/_helper.py` & `phdu-2.3.3/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/rtopy/resample.py` & `phdu-2.3.3/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/stats/test/permutation.py` & `phdu-2.3.3/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu/storage.py` & `phdu-2.3.3/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/phdu.egg-info/PKG-INFO` & `phdu-2.3.3/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.2
+Version: 2.3.3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.2/phdu.egg-info/SOURCES.txt` & `phdu-2.3.3/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.2/setup.py` & `phdu-2.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.2',
+    version='2.3.3',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

