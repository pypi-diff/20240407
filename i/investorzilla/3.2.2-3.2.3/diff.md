# Comparing `tmp/investorzilla-3.2.2.tar.gz` & `tmp/investorzilla-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investorzilla-3.2.2.tar", last modified: Wed Mar 27 20:53:26 2024, max compression
+gzip compressed data, was "investorzilla-3.2.3.tar", last modified: Sun Apr  7 10:49:38 2024, max compression
```

## Comparing `investorzilla-3.2.2.tar` & `investorzilla-3.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:26.000000 investorzilla-3.2.2/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-22 08:46:03.000000 investorzilla-3.2.2/LICENSE
--rw-r--r--   0 aviram    (1000) aviram    (1000)    46321 2024-03-27 20:53:26.000000 investorzilla-3.2.2/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4470 2023-12-12 11:07:53.000000 investorzilla-3.2.2/README.md
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:24.000000 investorzilla-3.2.2/investorzilla/
--rw-r--r--   0 aviram    (1000) aviram    (1000)      582 2024-03-10 10:12:17.000000 investorzilla-3.2.2/investorzilla/__init__.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1324 2023-11-22 08:43:50.000000 investorzilla-3.2.2/investorzilla/__main__.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:25.000000 investorzilla-3.2.2/investorzilla/currency/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2944 2023-12-15 20:49:46.000000 investorzilla-3.2.2/investorzilla/currency/brasil_banco_central.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2374 2023-11-22 08:44:44.000000 investorzilla-3.2.2/investorzilla/currency/cryptocompare.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    12863 2024-02-10 08:46:46.000000 investorzilla-3.2.2/investorzilla/datacache.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    68186 2024-03-27 19:54:05.000000 investorzilla-3.2.2/investorzilla/fund.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     9272 2024-02-10 09:20:56.000000 investorzilla-3.2.2/investorzilla/investor.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:25.000000 investorzilla-3.2.2/investorzilla/marketindex/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     3913 2023-11-20 22:28:04.000000 investorzilla-3.2.2/investorzilla/marketindex/brasil_banco_central.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1464 2023-11-22 08:44:43.000000 investorzilla-3.2.2/investorzilla/marketindex/federal_reserve.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2906 2023-12-16 08:53:09.000000 investorzilla-3.2.2/investorzilla/marketindex/yahoo_finance.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    11871 2023-12-16 08:31:42.000000 investorzilla-3.2.2/investorzilla/monetary_time_series.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    16852 2024-03-27 19:52:35.000000 investorzilla-3.2.2/investorzilla/portfolio.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:26.000000 investorzilla-3.2.2/investorzilla/portfolios/
--rw-r--r--   0 aviram    (1000) aviram    (1000)      515 2023-11-22 08:44:43.000000 investorzilla-3.2.2/investorzilla/portfolios/app-credentials-for-google-sheets.json
--rw-r--r--   0 aviram    (1000) aviram    (1000)    12780 2024-03-27 19:39:50.000000 investorzilla-3.2.2/investorzilla/portfolios/google_sheets.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     8472 2024-03-27 19:41:19.000000 investorzilla-3.2.2/investorzilla/portfolios/uri.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    27732 2024-03-27 20:23:21.000000 investorzilla-3.2.2/investorzilla/streamlit_ui.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-03-27 20:53:24.000000 investorzilla-3.2.2/investorzilla.egg-info/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    46321 2024-03-27 20:53:19.000000 investorzilla-3.2.2/investorzilla.egg-info/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)      841 2024-03-27 20:53:20.000000 investorzilla-3.2.2/investorzilla.egg-info/SOURCES.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-03-27 20:53:19.000000 investorzilla-3.2.2/investorzilla.egg-info/dependency_links.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       62 2024-03-27 20:53:19.000000 investorzilla-3.2.2/investorzilla.egg-info/entry_points.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)      159 2024-03-27 20:53:19.000000 investorzilla-3.2.2/investorzilla.egg-info/requires.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2024-03-27 20:53:19.000000 investorzilla-3.2.2/investorzilla.egg-info/top_level.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1496 2024-03-27 20:52:01.000000 investorzilla-3.2.2/pyproject.toml
--rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-03-27 20:53:26.000000 investorzilla-3.2.2/setup.cfg
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:37.000000 investorzilla-3.2.3/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-22 08:46:03.000000 investorzilla-3.2.3/LICENSE
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    46321 2024-04-07 10:49:37.000000 investorzilla-3.2.3/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     4470 2023-12-12 11:07:53.000000 investorzilla-3.2.3/README.md
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:35.000000 investorzilla-3.2.3/investorzilla/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      582 2024-03-10 10:12:17.000000 investorzilla-3.2.3/investorzilla/__init__.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1324 2023-11-22 08:43:50.000000 investorzilla-3.2.3/investorzilla/__main__.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:36.000000 investorzilla-3.2.3/investorzilla/currency/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2944 2023-12-15 20:49:46.000000 investorzilla-3.2.3/investorzilla/currency/brasil_banco_central.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2374 2023-11-22 08:44:44.000000 investorzilla-3.2.3/investorzilla/currency/cryptocompare.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    12863 2024-02-10 08:46:46.000000 investorzilla-3.2.3/investorzilla/datacache.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    68186 2024-03-27 19:54:05.000000 investorzilla-3.2.3/investorzilla/fund.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     9784 2024-04-07 10:26:30.000000 investorzilla-3.2.3/investorzilla/investor.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:37.000000 investorzilla-3.2.3/investorzilla/marketindex/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     3913 2023-11-20 22:28:04.000000 investorzilla-3.2.3/investorzilla/marketindex/brasil_banco_central.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1464 2023-11-22 08:44:43.000000 investorzilla-3.2.3/investorzilla/marketindex/federal_reserve.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2906 2023-12-16 08:53:09.000000 investorzilla-3.2.3/investorzilla/marketindex/yahoo_finance.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    11871 2023-12-16 08:31:42.000000 investorzilla-3.2.3/investorzilla/monetary_time_series.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    16852 2024-03-27 19:52:35.000000 investorzilla-3.2.3/investorzilla/portfolio.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:37.000000 investorzilla-3.2.3/investorzilla/portfolios/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      515 2023-11-22 08:44:43.000000 investorzilla-3.2.3/investorzilla/portfolios/app-credentials-for-google-sheets.json
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    12780 2024-03-27 19:39:50.000000 investorzilla-3.2.3/investorzilla/portfolios/google_sheets.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     8472 2024-03-27 19:41:19.000000 investorzilla-3.2.3/investorzilla/portfolios/uri.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    27749 2024-04-07 10:34:29.000000 investorzilla-3.2.3/investorzilla/streamlit_ui.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 10:49:35.000000 investorzilla-3.2.3/investorzilla.egg-info/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    46321 2024-04-07 10:49:31.000000 investorzilla-3.2.3/investorzilla.egg-info/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      841 2024-04-07 10:49:32.000000 investorzilla-3.2.3/investorzilla.egg-info/SOURCES.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-04-07 10:49:31.000000 investorzilla-3.2.3/investorzilla.egg-info/dependency_links.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       62 2024-04-07 10:49:31.000000 investorzilla-3.2.3/investorzilla.egg-info/entry_points.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      159 2024-04-07 10:49:31.000000 investorzilla-3.2.3/investorzilla.egg-info/requires.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2024-04-07 10:49:31.000000 investorzilla-3.2.3/investorzilla.egg-info/top_level.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1496 2024-04-07 10:49:03.000000 investorzilla-3.2.3/pyproject.toml
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-04-07 10:49:37.000000 investorzilla-3.2.3/setup.cfg
```

### Comparing `investorzilla-3.2.2/LICENSE` & `investorzilla-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/PKG-INFO` & `investorzilla-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investorzilla
-Version: 3.2.2
+Version: 3.2.3
 Summary: Manage your investments like a data scientist
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `investorzilla-3.2.2/README.md` & `investorzilla-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/__init__.py` & `investorzilla-3.2.3/investorzilla/__init__.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/__main__.py` & `investorzilla-3.2.3/investorzilla/__main__.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/currency/brasil_banco_central.py` & `investorzilla-3.2.3/investorzilla/currency/brasil_banco_central.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/currency/cryptocompare.py` & `investorzilla-3.2.3/investorzilla/currency/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/datacache.py` & `investorzilla-3.2.3/investorzilla/datacache.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/fund.py` & `investorzilla-3.2.3/investorzilla/fund.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/investor.py` & `investorzilla-3.2.3/investorzilla/investor.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,19 +177,27 @@
 
 
     def augmentDomains(self):
         """
         Fabricate more benchmarks from currency converters, as specified by
         YAML config file.
 
-        Entries such as the following from the YAML file will be engineered:
+        Entries such as the following from the YAML file will be handled:
 
         benchmarks:
             - kind: from_currency_converter
               from_to: BRLUSD
+
+        For the config entry above, result is two benchmarks:
+        - [BRL] USDBRL: expressed in BRL, or how USD performed in comparison to BRL
+        - [USD] BRLUSD: expressed in USD, or how BRL performed in comparison to USD
+
+        As the “[USD] S&P500” bechmark conveys what would happen if I converted
+        my USD into assets of the S&P500 set, the fabricated “[BRL] USDBRL”
+        benchmark shows what would happen if I converted my BRL in USD.
         """
 
         for item in self.config['benchmarks']:
             if 'kind' in item and item['kind'] == 'from_currency_converter':
                 curFrom = item['from_to'][:3]
                 curTo   = item['from_to'][3:]
 
@@ -199,19 +207,20 @@
                 )
 
                 # Delete old MarketIndex previously created by a CurrencyConverter
                 self.benchmarks = [b for b in self.benchmarks if b['obj'].id!=curFrom+curTo]
 
                 # Scan all currency converters we have to find a match
                 for cc in self.currency_converters:
-                    if curFrom == cc['obj'].currencyFrom and curTo == cc['obj'].currencyTo:
-                        item['obj']=MarketIndex().fromCurrencyConverter(cc['obj'])
+                    current_cc=cc['obj']
+                    if curFrom == current_cc.currencyFrom and curTo == current_cc.currencyTo:
+                        item['obj']=MarketIndex().fromCurrencyConverter(current_cc)
                         break
-                    elif curTo == cc['obj'].currencyFrom and curFrom == cc['obj'].currencyTo:
-                        item['obj']=MarketIndex().fromCurrencyConverter(cc['obj'].invert())
+                    elif curTo == current_cc.currencyFrom and curFrom == current_cc.currencyTo:
+                        item['obj']=MarketIndex().fromCurrencyConverter(current_cc.invert())
                         break
 
                 if 'obj' in item:
                     self.benchmarks.append(item)
                 else:
                     raise Exception(f'Can’t find "{item.kind}" CurrencyConverter to make a MarketIndex from.')
```

### Comparing `investorzilla-3.2.2/investorzilla/marketindex/brasil_banco_central.py` & `investorzilla-3.2.3/investorzilla/marketindex/brasil_banco_central.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/marketindex/federal_reserve.py` & `investorzilla-3.2.3/investorzilla/marketindex/federal_reserve.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/marketindex/yahoo_finance.py` & `investorzilla-3.2.3/investorzilla/marketindex/yahoo_finance.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/monetary_time_series.py` & `investorzilla-3.2.3/investorzilla/monetary_time_series.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/portfolio.py` & `investorzilla-3.2.3/investorzilla/portfolio.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/portfolios/app-credentials-for-google-sheets.json` & `investorzilla-3.2.3/investorzilla/portfolios/app-credentials-for-google-sheets.json`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/portfolios/google_sheets.py` & `investorzilla-3.2.3/investorzilla/portfolios/google_sheets.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/portfolios/uri.py` & `investorzilla-3.2.3/investorzilla/portfolios/uri.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/investorzilla/streamlit_ui.py` & `investorzilla-3.2.3/investorzilla/streamlit_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             streamlit.session_state.investor=investorzilla.Investor(
                 'investorzilla.yaml',
                 self.refreshMap
             )
 
         # Make a preliminary internal fund from the portfolio for display purposes
         streamlit.session_state.investor.portfolio.makeInternalFund(
-            streamlit.session_state.investor.exchange
+            currencyExchange=streamlit.session_state.investor.exchange
         )
 
         with streamlit.sidebar:
             # Put controls in the sidebar
             self.interact_assets()
             self.interact_exclude_assets()
             self.interact_start_end()
```

### Comparing `investorzilla-3.2.2/investorzilla.egg-info/PKG-INFO` & `investorzilla-3.2.3/investorzilla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investorzilla
-Version: 3.2.2
+Version: 3.2.3
 Summary: Manage your investments like a data scientist
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `investorzilla-3.2.2/investorzilla.egg-info/SOURCES.txt` & `investorzilla-3.2.3/investorzilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investorzilla-3.2.2/pyproject.toml` & `investorzilla-3.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "investorzilla"
-version = '3.2.2'
+version = '3.2.3'
 description = "Manage your investments like a data scientist"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

