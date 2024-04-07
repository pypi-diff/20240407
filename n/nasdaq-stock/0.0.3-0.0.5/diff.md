# Comparing `tmp/nasdaq_stock-0.0.3.tar.gz` & `tmp/nasdaq_stock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nasdaq_stock-0.0.3.tar", last modified: Mon Apr  9 22:41:26 2018, max compression
+gzip compressed data, was "nasdaq_stock-0.0.5.tar", last modified: Sun Apr  7 02:43:40 2024, max compression
```

## Comparing `nasdaq_stock-0.0.3.tar` & `nasdaq_stock-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxrwx   0        0        0        0 2018-04-09 22:41:26.000000 nasdaq_stock-0.0.3/
-drwxrwxrwx   0        0        0        0 2018-04-09 22:41:26.000000 nasdaq_stock-0.0.3/nasdaq_stock/
--rw-rw-rw-   0        0        0     3992 2018-04-09 05:39:00.000000 nasdaq_stock-0.0.3/nasdaq_stock/nasdaq_stock.py
--rw-rw-rw-   0        0        0        0 2018-04-09 05:44:19.000000 nasdaq_stock-0.0.3/nasdaq_stock/__init__.py
--rw-rw-rw-   0        0        0     1687 2018-04-09 22:41:26.000000 nasdaq_stock-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       40 2018-04-01 17:33:07.000000 nasdaq_stock-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1729 2018-04-09 22:40:24.000000 nasdaq_stock-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:43:40.014967 nasdaq_stock-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2024-04-07 02:26:14.000000 nasdaq_stock-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1303 2024-04-07 02:43:40.015968 nasdaq_stock-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-07 02:42:23.000000 nasdaq_stock-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 02:43:40.011968 nasdaq_stock-0.0.5/nasdaq_stock/
+-rw-rw-rw-   0        0        0       29 2024-04-07 02:26:14.000000 nasdaq_stock-0.0.5/nasdaq_stock/__init__.py
+-rw-rw-rw-   0        0        0     4944 2024-04-07 02:30:32.000000 nasdaq_stock-0.0.5/nasdaq_stock/nasdaq_stock.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:43:40.014967 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/
+-rw-rw-rw-   0        0        0     1303 2024-04-07 02:43:39.000000 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-07 02:43:39.000000 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:43:39.000000 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-07 02:43:39.000000 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-07 02:43:39.000000 nasdaq_stock-0.0.5/nasdaq_stock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2024-04-07 02:43:40.015968 nasdaq_stock-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      547 2024-04-07 02:43:35.000000 nasdaq_stock-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nasdaq_stock-0.0.3/PKG-INFO` & `nasdaq_stock-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nasdaq_stock
-Version: 0.0.3
+Version: 0.0.5
 Summary: nasdaq stock retriever
 Home-page: https://github.com/georgejs/nasdaq_stock
+Download-URL: https://github.com/georgejs/nasdaq_stock/archive/0.0.5.tar.gz
 Author: George Shen
 Author-email: georgejs.arch@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/georgejs/nasdaq_stock/archive/0.0.3.tar.gz
-Description: Nasdaq Stock: Stock data retriever
-         =========================                  
-         How to use                                 
-         ---------------                            
-         >>>from nasdaq_stock import nasdaq_stock as ns
-         or
-         >>>from nasdaq_stock import nasdaq_stock   
-         >>>nasdaq_stock.stock(‘spyd’)              
-         or
-         >>>spyd = nasdaq_stock.stock(‘spyd’)       
-         
-         This will return string data and a dictionary of that data.
-         Current data fields are:                   
-         ticker: The stock or id of that ticker.    
-         date: The date when the stock was queried. 
-         time: The time when the stock was taken. This can be helpful if you are trying to do minute by minute data gathering
-         price: The current price or bid price      
-         ask: The current ask price                 
-         high: The high of the day                  
-         low: The low of the day                    
-         previous_close: The previous closing form the last day. Not to be confused with last ask price
-         volume: Volume of shares for the current day. 
-         market_cap: Market cap of the stock. i.e. dollar amount currently vested in stock
-         
 Keywords: stock,nasdaq,stock retriever,nasdaq stock
-Platform: UNKNOWN
+License-File: LICENSE
+
+# nasdaq_stock
+nasdaq stock pull down
+
+# How to use
+```
+>>>from nasdaq_stock import nasdaq_stock as ns
+```
+or
+```
+>>>from nasdaq_stock import nasdaq_stock   
+>>>nasdaq_stock.stock(â€˜spydâ€™)              
+```
+or
+```
+>>>spyd = nasdaq_stock.stock(â€˜spydâ€™)       
+```
+
+This will return string data and a dictionary of that data.
+Current data fields are:                   
+ticker: The stock or id of that ticker.    
+date: The date when the stock was queried. 
+time: The time when the stock was taken. This can be helpful if you are trying to do minute-by-minute data gathering
+price: The current price or bid price      
+ask: The current ask price                 
+high: The high of the day                  
+low: The low of the day                    
+previous_close: The previous closing form the last day. Not to be confused with last ask price
+volume: Volume of shares for the current day.
```

