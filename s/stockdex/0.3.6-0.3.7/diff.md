# Comparing `tmp/stockdex-0.3.6.tar.gz` & `tmp/stockdex-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdex-0.3.6.tar", last modified: Wed Mar 20 01:39:22 2024, max compression
+gzip compressed data, was "stockdex-0.3.7.tar", last modified: Sun Apr  7 10:05:58 2024, max compression
```

## Comparing `stockdex-0.3.6.tar` & `stockdex-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:22.160804 stockdex-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-20 01:39:22.160804 stockdex-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-20 01:39:11.000000 stockdex-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 01:39:22.160804 stockdex-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-20 01:39:11.000000 stockdex-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:22.160804 stockdex-0.3.6/stockdex/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/ticker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/ticker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:11.000000 stockdex-0.3.6/stockdex/ticker_etf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:22.160804 stockdex-0.3.6/stockdex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-20 01:39:22.000000 stockdex-0.3.6/stockdex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-20 01:39:22.000000 stockdex-0.3.6/stockdex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 01:39:22.000000 stockdex-0.3.6/stockdex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-20 01:39:22.000000 stockdex-0.3.6/stockdex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-20 01:39:22.000000 stockdex-0.3.6/stockdex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:22.160804 stockdex-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 01:39:11.000000 stockdex-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-20 01:39:11.000000 stockdex-0.3.6/tests/test_justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-20 01:39:11.000000 stockdex-0.3.6/tests/test_nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-20 01:39:11.000000 stockdex-0.3.6/tests/test_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-03-20 01:39:11.000000 stockdex-0.3.6/tests/test_ticker_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:05:58.093271 stockdex-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 10:05:50.000000 stockdex-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:05:58.093271 stockdex-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-07 10:05:50.000000 stockdex-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.089271 stockdex-0.3.7/stockdex/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/selenium_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_etf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/stockdex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_ticker_api.py
```

### Comparing `stockdex-0.3.6/PKG-INFO` & `stockdex-0.3.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.6
+Version: 0.3.7
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -86,14 +86,34 @@
 top_institutional_holders = ticker.top_institutional_holders
 top_mutual_fund_holders = ticker.top_mutual_fund_holders
 
 # Main statistics
 statistics = ticker.statistics 
 ```
 
+## ETF data from justETF website:
+```python
+
+# build the ETF object, make sure to pass the ETF ISIN and use security_type to "etf"
+etf = Ticker('IE00B4L5Y983', security_type='etf')
+
+etf_general_info = etf.etf_general_info
+etf_wkn = etf.etf_wkn
+etf_description = etf.etf_description
+
+# Basic data about the ETF
+etf_basics = etf.etf_basics
+
+# Holdings of the ETF by company, country and sector
+etf_holdings_companies = etf.etf_holdings_companies
+etf_holdings_countries = etf.etf_holdings_countries
+etf_holdings_sectors = etf.etf_holdings_sectors
+```
+
+
 ## Historical dividends data
 
 All dividends paid by the company returned as a pandas DataFrame.
 
 ```python
 dividend = ticker.dividend
 ```
```

### Comparing `stockdex-0.3.6/README.md` & `stockdex-0.3.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -74,14 +74,34 @@
 top_institutional_holders = ticker.top_institutional_holders
 top_mutual_fund_holders = ticker.top_mutual_fund_holders
 
 # Main statistics
 statistics = ticker.statistics 
 ```
 
+## ETF data from justETF website:
+```python
+
+# build the ETF object, make sure to pass the ETF ISIN and use security_type to "etf"
+etf = Ticker('IE00B4L5Y983', security_type='etf')
+
+etf_general_info = etf.etf_general_info
+etf_wkn = etf.etf_wkn
+etf_description = etf.etf_description
+
+# Basic data about the ETF
+etf_basics = etf.etf_basics
+
+# Holdings of the ETF by company, country and sector
+etf_holdings_companies = etf.etf_holdings_companies
+etf_holdings_countries = etf.etf_holdings_countries
+etf_holdings_sectors = etf.etf_holdings_sectors
+```
+
+
 ## Historical dividends data
 
 All dividends paid by the company returned as a pandas DataFrame.
 
 ```python
 dividend = ticker.dividend
 ```
```

### Comparing `stockdex-0.3.6/setup.py` & `stockdex-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/stockdex/config.py` & `stockdex-0.3.7/stockdex/config.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/stockdex/lib.py` & `stockdex-0.3.7/stockdex/lib.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/stockdex/nasdaq_interface.py` & `stockdex-0.3.7/stockdex/nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/stockdex/ticker.py` & `stockdex-0.3.7/stockdex/ticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,52 @@
 """
 Moduel for the Ticker class
 """
 
+from typing import Literal
+
 import pandas as pd
 from bs4 import BeautifulSoup
 
+from stockdex.justetf import JustETF
 from stockdex.ticker_api import TickerAPI
 
 
-class Ticker(TickerAPI):
+class Ticker(TickerAPI, JustETF):
     """
     Class for the Ticker
     """
 
-    def __init__(self, ticker: str) -> None:
-        self.ticker = ticker.upper()
+    def __init__(
+        self,
+        ticker: str = "",
+        isin: str = "",
+        security_type: str = Literal["stock", "etf"],
+    ) -> None:
+        """
+        Initialize the Ticker class
+
+        Args:
+        ticker (str): The ticker of the stock
+        isin (str): The ISIN of the etf
+        security_type (str): The security type of the ticker
+            default is "stock"
+        """
+
+        self.ticker = ticker
+        self.isin = isin
+        self.security_type = security_type if security_type else "stock"
+
+        if not ticker and not isin:
+            raise Exception("Please provide either a ticker or an ISIN")
+
+        if security_type == "etf":
+            super().__init__(isin=isin)
+        else:
+            super().__init__(ticker=ticker)
 
     @property
     def summary(self) -> pd.DataFrame:
         """
         Get data for the ticker
 
         Returns:
@@ -324,14 +352,16 @@
         """
         Get the description of the ticker
 
         Returns:
         str: A string including the description of the ticker
         visible in the Yahoo Finance profile page for the ticker
         """
+        if self.security_type == "etf":
+            return self.etf_description
 
         # URL of the website to scrape
         url = f"https://finance.yahoo.com/quote/{self.ticker}/profile"
         response = self.get_response(url)
 
         # Parse the HTML content of the website
         soup = BeautifulSoup(response.content, "html.parser")
```

### Comparing `stockdex-0.3.6/stockdex/ticker_api.py` & `stockdex-0.3.7/stockdex/ticker_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,23 @@
 import pandas as pd
 
 from stockdex import config
 from stockdex.ticker_base import TickerBase
 
 
 class TickerAPI(TickerBase):
-    # current_timestamp = int(pd.Timestamp("now").timestamp())
-    # five_years_ago = int(pd.Timestamp("now").timestamp()) - 5 * 365 * 24 * 60 * 60
+    def __init__(
+        self,
+        ticker: str = "",
+        isin: str = "",
+        security_type: str = Literal["stock", "etf"],
+    ) -> None:
+        self.ticker = ticker
+        self.isin = isin
+        self.security_type = security_type
 
     today = datetime.today()
     five_years_ago = today.replace(year=today.year - 5)
 
     def price(
         self,
         range: Literal[
@@ -40,19 +47,24 @@
             "3mo",
         ] = "1m",
     ) -> pd.DataFrame:
         """
         Get the price data for the stock
 
         Args:
+        ----------------
         range (str): The range of the price data to retrieve
         valid values are "1d", "5d", "1mo", "3mo", "6mo", "1y", "2y", "5y", "10y", "ytd", "max"
 
         dataGranularity (str): The granularity of the data to retrieve (interval)
         valid values are "1m", "2m", "5m", "15m", "30m", "60m", "90m", "1h", "1d", "5d", "1wk", "1mo", "3mo""  # noqa: E501
+
+        Returns:
+        ----------------
+        pd.DataFrame: The price data
         """
 
         url = f"{config.BASE_URL}/chart/{self.ticker}?range={range}&interval={dataGranularity}"
         response = self.get_response(url)
 
         meta = response.json()["chart"]["result"][0]["meta"]
         currency = meta["currency"]
@@ -127,27 +139,32 @@
         period1: datetime = five_years_ago,
         period2: datetime = today,
     ) -> pd.DataFrame:
         """
         Get the income statement for the stock
 
         Args:
+        ----------------
         frequency (str): The frequency of the data to retrieve
         valid values are "annual", "quarterly"
 
         format (str): The format of the data to retrieve
         valid values are "fmt", "raw"
         if "fmt" is used, the data will be in a human readable format, e.g. 1B
         if "raw" is used, the data will be in a raw format, e.g. 1000000000
 
         period1 (datetime): The start date of the data to retrieve
         default is five years ago as that is the maximum period the API supports data retrieval for
 
         period2 (datetime): The end date of the data to retrieve
         default is the current date
+
+        Returns:
+        ----------------
+        pd.DataFrame: The income statement data
         """
         url = self.build_url(frequency, period1, period2, "income_statement")
 
         response = self.get_response(url).json()["timeseries"]["result"]
 
         return self.extract_dataframe(response, format)
 
@@ -158,27 +175,32 @@
         period1: datetime = five_years_ago,
         period2: datetime = today,
     ) -> pd.DataFrame:
         """
         Get the cash flow statement for the stock
 
         Args:
+        ----------------
         frequency (str): The frequency of the data to retrieve
         valid values are "annual", "quarterly"
 
         format (str): The format of the data to retrieve
         valid values are "fmt", "raw"
         if "fmt" is used, the data will be in a human readable format, e.g. 1B
         if "raw" is used, the data will be in a raw format, e.g. 1000000000
 
         period1 (datetime): The start date of the data to retrieve
         default is five years ago as that is the maximum period the API supports data retrieval for
 
         period2 (datetime): The end date of the data to retrieve
         default is the current date
+
+        Returns:
+        ----------------
+        pd.DataFrame: The cash flow statement data
         """
         url = self.build_url(frequency, period1, period2, "cash_flow")
 
         response = self.get_response(url).json()["timeseries"]["result"]
 
         return self.extract_dataframe(response, format)
 
@@ -189,27 +211,32 @@
         period1: datetime = five_years_ago,
         period2: datetime = today,
     ) -> pd.DataFrame:
         """
         Get the balance sheet for the stock
 
         Args:
+        ----------------
         frequency (str): The frequency of the data to retrieve
         valid values are "annual", "quarterly"
 
         format (str): The format of the data to retrieve
         valid values are "fmt", "raw"
         if "fmt" is used, the data will be in a human readable format, e.g. 1B
         if "raw" is used, the data will be in a raw format, e.g. 1000000000
 
         period1 (datetime): The start date of the data to retrieve
         default is five years ago as that is the maximum period the API supports data retrieval for
 
         period2 (datetime): The end date of the data to retrieve
         default is the current date
+
+        Returns:
+        ----------------
+        pd.DataFrame: The balance sheet data
         """
         url = self.build_url(frequency, period1, period2, "balance_sheet")
 
         response = self.get_response(url).json()["timeseries"]["result"]
 
         return self.extract_dataframe(response, format)
 
@@ -220,27 +247,32 @@
         period1: datetime = five_years_ago,
         period2: datetime = today,
     ) -> pd.DataFrame:
         """
         Get the financials for the stock
 
         Args:
+        ----------------
         frequency (str): The frequency of the data to retrieve
         valid values are "annual", "quarterly"
 
         format (str): The format of the data to retrieve
         valid values are "fmt", "raw"
         if "fmt" is used, the data will be in a human readable format, e.g. 1B
         if "raw" is used, the data will be in a raw format, e.g. 1000000000
 
         period1 (datetime): The start date of the data to retrieve
         default is five years ago as that is the maximum period the API supports data retrieval for
 
         period2 (datetime): The end date of the data to retrieve
         default is the current date
+
+        Returns:
+        ----------------
+        pd.DataFrame: The financials data
         """
         url = self.build_url(frequency, period1, period2, "financials")
 
         response = self.get_response(url).json()["timeseries"]["result"]
 
         return self.extract_dataframe(response, format)
 
@@ -249,14 +281,29 @@
         frequency: str,
         period1: datetime,
         period2: datetime,
         desired_entity: str,
     ) -> str:
         """
         Build the URL for the income statement, balance sheet, and cash flow statement
+
+        Args:
+        ----------------
+        frequency (str): The frequency of the data to retrieve
+        valid values are "annual", "quarterly"
+
+        period1 (datetime): The start date of the data to retrieve
+
+        period2 (datetime): The end date of the data to retrieve
+
+        desired_entity (str): The entity to retrieve the data for
+
+        Returns:
+        ----------------
+        str: The URL to retrieve the data from
         """
         # convert period1 and period2 to timestamps
         period1 = int(pd.Timestamp(period1).timestamp())
         period2 = int(pd.Timestamp(period2).timestamp())
 
         columns = ",".join(getattr(config, f"{desired_entity.upper()}_COLUMNS"))
 
@@ -266,14 +313,24 @@
         url += f"&type={columns}"
         url += f"&period1={period1}&period2={period2}"
         return url
 
     def extract_dataframe(self, response, format="fmt") -> pd.DataFrame:
         """
         Extract the dataframes from the response
+
+        Args:
+        ----------------
+        response (dict): The response from the API
+
+        format (str): The format of the data to retrieve
+
+        Returns:
+        ----------------
+        pd.DataFrame: The data in a dataframe
         """
         row = {}
         for item in response:
             column = item["meta"]["type"][0]
 
             # skip if there is no data for in the response
             if column not in item:
```

### Comparing `stockdex-0.3.6/stockdex/ticker_base.py` & `stockdex-0.3.7/stockdex/ticker_base.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/stockdex.egg-info/PKG-INFO` & `stockdex-0.3.7/stockdex.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.6
+Version: 0.3.7
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -86,14 +86,34 @@
 top_institutional_holders = ticker.top_institutional_holders
 top_mutual_fund_holders = ticker.top_mutual_fund_holders
 
 # Main statistics
 statistics = ticker.statistics 
 ```
 
+## ETF data from justETF website:
+```python
+
+# build the ETF object, make sure to pass the ETF ISIN and use security_type to "etf"
+etf = Ticker('IE00B4L5Y983', security_type='etf')
+
+etf_general_info = etf.etf_general_info
+etf_wkn = etf.etf_wkn
+etf_description = etf.etf_description
+
+# Basic data about the ETF
+etf_basics = etf.etf_basics
+
+# Holdings of the ETF by company, country and sector
+etf_holdings_companies = etf.etf_holdings_companies
+etf_holdings_countries = etf.etf_holdings_countries
+etf_holdings_sectors = etf.etf_holdings_sectors
+```
+
+
 ## Historical dividends data
 
 All dividends paid by the company returned as a pandas DataFrame.
 
 ```python
 dividend = ticker.dividend
 ```
```

### Comparing `stockdex-0.3.6/tests/test_nasdaq_interface.py` & `stockdex-0.3.7/tests/test_nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/tests/test_ticker.py` & `stockdex-0.3.7/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.6/tests/test_ticker_api.py` & `stockdex-0.3.7/tests/test_ticker_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     assert len(price) > 0
 
 
 @pytest.mark.parametrize(
     "ticker",
     [
         ("AAPL"),
+        ("ASML"),
     ],
 )
 def test_current_trading_period(ticker):
     """
     Test the price property of the TickerAPI class
     """
 
@@ -59,21 +60,25 @@
 
     assert current_trading_period.columns.tolist() == [
         "pre",
         "regular",
         "post",
     ]
     assert len(current_trading_period) == 4
-    assert current_trading_period.index.tolist() == [
+
+    expected_columns = [
         "timezone",
         "start",
         "end",
         "gmtoffset",
     ]
 
+    for column in expected_columns:
+        assert column in current_trading_period.index.tolist()
+
 
 @pytest.mark.parametrize(
     "ticker, frequency, format, period1, period2",
     [
         ("AAPL", "quarterly", "fmt", datetime(2020, 1, 1), datetime.today()),
         ("GOOGL", "quarterly", "fmt", datetime(2021, 1, 1), datetime.today()),
         ("MSFT", "quarterly", "fmt", datetime(2023, 1, 1), datetime(2024, 1, 1)),
```

