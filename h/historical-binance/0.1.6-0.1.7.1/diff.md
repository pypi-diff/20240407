# Comparing `tmp/historical_binance-0.1.6-py3-none-any.whl.zip` & `tmp/historical_binance-0.1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9617 bytes, number of entries: 6
--rw-r--r--  2.0 unx    19086 b- defN 24-Apr-06 08:36 historical_binance.py
--rw-r--r--  2.0 unx     7048 b- defN 24-Apr-06 08:39 historical_binance-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2735 b- defN 24-Apr-06 08:39 historical_binance-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 08:39 historical_binance-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-06 08:39 historical_binance-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      520 b- defN 24-Apr-06 08:39 historical_binance-0.1.6.dist-info/RECORD
-6 files, 29500 bytes uncompressed, 8669 bytes compressed:  70.6%
+Zip file size: 9454 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    17797 b- defN 24-Apr-07 06:28 historical_binance.py
+-rw-r--r--  2.0 unx     7048 b- defN 24-Apr-07 06:30 historical_binance-0.1.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2737 b- defN 24-Apr-07 06:30 historical_binance-0.1.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:30 historical_binance-0.1.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-07 06:30 historical_binance-0.1.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 24-Apr-07 06:30 historical_binance-0.1.7.1.dist-info/RECORD
+6 files, 28223 bytes uncompressed, 8486 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: historical_binance.py
 Comment: 
 
-Filename: historical_binance-0.1.6.dist-info/LICENSE
+Filename: historical_binance-0.1.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: historical_binance-0.1.6.dist-info/METADATA
+Filename: historical_binance-0.1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: historical_binance-0.1.6.dist-info/WHEEL
+Filename: historical_binance-0.1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: historical_binance-0.1.6.dist-info/top_level.txt
+Filename: historical_binance-0.1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: historical_binance-0.1.6.dist-info/RECORD
+Filename: historical_binance-0.1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## historical_binance.py

```diff
@@ -1,17 +1,17 @@
 import asyncio
 import httpx
-import tqdm
 import zipfile
 from io import BytesIO
 from datetime import datetime, timedelta, date
 import polars as pl
 from dateutil.relativedelta import relativedelta
 import os
 from pytz import UTC
+from utils.logging import logger
 
 
 class BinanceDataProvider:
     TICKER_DIR = None
     TICKER_NAME = None
     data_downloader = None
     pairlist = None
@@ -119,16 +119,15 @@
                     if earliest_date.replace(tzinfo=UTC) > fallback_starting_date:
                         download_from = fallback_starting_date
                 else:
                     download_from = fallback_starting_date
 
                 # Download new data and merge with existing data
                 task = (asyncio.create_task(
-                    self.data_downloader.download_one_ticker(ticker, download_from, today_datetime, timeframe,
-                                                             tqdm_position=len(tasks) - 1)))
+                    self.data_downloader.download_one_ticker(ticker, download_from, today_datetime, timeframe)))
                 tasks.append(task)
         for coroutine in asyncio.as_completed(tasks):
             try:
                 ticker, timeframe, new_data = await coroutine
             except Exception as e:
                 print(e)
                 new_data = None
@@ -159,20 +158,19 @@
         self.timeframes = timeframes
         self.cached_dataframes = {}
 
 
 class BinanceDataDownloader:
     downloadable_ticker_information = {}
     pbars = None
-    use_pbar = True
+    # use_pbar = True
     __minimum_achieved_date = None
     ignore = []
 
-    async def download_and_process(self, session, url: str, ticker: str, date_of_cycle: datetime, is_csv=True,
-                                   tqdm_position=0):
+    async def download_and_process(self, session, url: str, ticker: str, date_of_cycle: datetime, is_csv=True):
         DEFAULT_COLUMNS = ['open_time', 'open', 'high', 'low', 'close', 'volume',
                            'close_time', 'quote_volume', 'count', 'taker_buy_volume',
                            'taker_buy_quote_volume', 'ignore']
         retry_count = 0
         while retry_count < self.max_retry_count:
             try:
                 response = await session.get(url)
@@ -196,48 +194,35 @@
                         del data
                         df.columns = DEFAULT_COLUMNS
                     df = df.with_columns((pl.col(coln).cast(pl.Float64) for coln in DEFAULT_COLUMNS if
                                           not coln in ["open_time", "close_time"])).filter(
                         pl.col("ignore") == 0).rename({"open_time": "date"}).drop(
                         ["close_time", "ignore", "quote_volume", "taker_buy_quote_volume"] + self.ignore).with_columns(
                         (pl.col("date").cast(pl.Datetime(time_unit="ms")).dt.replace_time_zone("UTC").alias("date")))
-                    # print(df)
-                    if tqdm_position in self.pbars:
-                        self.pbars[tqdm_position].update(1)
                     if self.__minimum_achieved_date is None or date_of_cycle < self.__minimum_achieved_date:
                         self.__minimum_achieved_date = date_of_cycle
                     del response
                     return df
                 else:
                     raise ConnectionError(response.status_code)
             except Exception as e:
                 # del response
                 retry_count += 1
-                if self.pbars[tqdm_position] is not None:
-                    if self.__minimum_achieved_date is not None and (
-                            not date.today() == date_of_cycle.date()) and self.__minimum_achieved_date < date_of_cycle:
-                        self.pbars[tqdm_position].write(
-                            f"A hole in the cycle has been found, minimum achieved date is {self.__minimum_achieved_date}, url: {url.split('/klines')[1]}, {e}")
-                        if retry_count == self.max_retry_count:
-                            raise Exception(
-                                f"Hole in the data {self.__minimum_achieved_date}/{date_of_cycle}, url: {url.split('/klines')[1]}, {e}")
-                    self.pbars[tqdm_position].write(
-                        f"Error({retry_count}/{self.max_retry_count} retries): {url.split('/klines')[1]}, {e}")
-                    self.pbars[tqdm_position].update(1)
-                    if not hasattr(self.pbars[tqdm_position], "error_count"):
-                        self.pbars[tqdm_position].error_count = 1
-                    else:
-                        self.pbars[tqdm_position].error_count += 1
-                    self.pbars[tqdm_position].set_postfix_str(f"Error Count: {self.pbars[tqdm_position].error_count}")
-                else:
-                    print(f"Error: Failed to download data for {ticker} from {url}")
+                logger.warning(f"Error({retry_count}/{self.max_retry_count} retries): {url.split('/klines')[1]}, {e}")
+                if self.__minimum_achieved_date is not None and (
+                        not date.today() == date_of_cycle.date()) and self.__minimum_achieved_date < date_of_cycle:
+                    logger.error(
+                        f"A hole in the cycle has been found, minimum achieved date is {self.__minimum_achieved_date}, url: {url.split('/klines')[1]}, {e}")
+                    if retry_count == self.max_retry_count:
+                        raise Exception(
+                            f"Hole in the data {self.__minimum_achieved_date}/{date_of_cycle}, url: {url.split('/klines')[1]}, {e}")
         return pl.DataFrame()
 
     async def download_one_ticker(self, ticker, start_date: datetime, end_date: datetime, timeframe, spot=False,
-                                  max_retry_count=5, tqdm_position=0):
+                                  max_retry_count=5):
         if self.downloadable_ticker_information is None:
             self.downloadable_ticker_information = await self.__fetch_downloadable_tickers()
         self.max_retry_count = max_retry_count
         # Write some code to ensure that start_date is smaller than end_date and make them both timezone-aware using UTC
         start_date = start_date.replace(tzinfo=UTC)
         end_date = end_date.replace(tzinfo=UTC)
         end_date_plus_one = end_date + timedelta(days=1)
@@ -259,50 +244,45 @@
                     start_time = current_date.timestamp() * 1000
                     end_time = (current_date + timedelta(minutes=1000)).timestamp() * 1000
                     if spot:
                         url = f"https://data-api.binance.vision/api/v3/klines?symbol={ticker}&interval={timeframe}&limit=1000&startTime={start_time}&endTime={end_time}"
                     else:
                         url = f"https://fapi.binance.com/fapi/v1/klines?symbol={ticker}&interval={timeframe}&limit=1000&startTime={start_time}&endTime={end_time}"
                     task = asyncio.create_task(
-                        self.download_and_process(session, url, ticker, current_date, False, tqdm_position))
+                        self.download_and_process(session, url, ticker, current_date, False))
                     tasks.append(task)
                     current_date += timedelta(minutes=1000)
                 elif current_date.month == end_date.month and current_date.year == end_date.year:
                     # Download daily data for the ending month
                     url = f"https://data.binance.vision/data/{prefix}/daily/klines/{ticker}/{timeframe}/{ticker}-{timeframe}-{year}-{month:02d}-{day:02d}.zip"
                     task = asyncio.create_task(
-                        self.download_and_process(session, url, ticker, current_date, True, tqdm_position))
+                        self.download_and_process(session, url, ticker, current_date, True))
                     tasks.append(task)
                     current_date += timedelta(days=1)
 
                 else:
                     # Download monthly data for full months
                     url = f"https://data.binance.vision/data/{prefix}/monthly/klines/{ticker}/{timeframe}/{ticker}-{timeframe}-{year}-{month:02d}.zip"
                     task = asyncio.create_task(
-                        self.download_and_process(session, url, ticker, current_date, True, tqdm_position))
+                        self.download_and_process(session, url, ticker, current_date, True))
                     tasks.append(task)
                     # add one month to the current date setting the day to be the first day of the month
                     current_date = current_date.replace(day=1) + relativedelta(months=1)
-            if self.use_pbar:
-                self.pbars[tqdm_position] = tqdm.tqdm(total=len(tasks), position=tqdm_position,
-                                                      desc=f'DOWN {ticker}-{timeframe}, {start_date.date()} to {end_date.date()}')
+            logger.info(f'DOWN {ticker}-{timeframe}, {start_date.date()} to {end_date.date()}')
             combined_df = None
             for cor in asyncio.as_completed(tasks):
                 df = await cor
                 if combined_df is None:
                     combined_df = df
                 else:
                     combined_df = pl.concat([combined_df, df], how="vertical")
             combined_df = combined_df.unique(subset=["date"]).sort("date")
 
             if combined_df.shape[0] == 0:
                 raise Exception(f"No data found for {ticker} between {start_date} and {end_date}")
-            if self.use_pbar:
-                self.pbars[tqdm_position].close()
-                del self.pbars[tqdm_position]
             return ticker, timeframe, combined_df
 
     async def __fetch_downloadable_tickers(self):
         async with httpx.AsyncClient() as session:
             headers = {
                 'authority': 'www.binance.com',
                 'accept': '*/*',
@@ -326,14 +306,14 @@
                 'https://www.binance.com/bapi/bigdata/v1/public/bigdata/finance/exchange/listDownloadOptions',
                 headers=headers, json=data)
             result = response.json()
             if result["code"] != '000000' or not result["success"]:
                 raise Exception(f"Failed to fetch downloadable tickers, {result}")
             return result["data"]
 
-    def __init__(self, use_pbar=True, ignore_extras=True):
+    def __init__(self, use_pbar=False, ignore_extras=True):
         if ignore_extras:
             self.ignore = ["taker_buy_volume", "count"]
         self.max_retry_count = None
-        self.use_pbar = use_pbar
-        self.pbars = {}
+        logger.info("TEST")
+        print("TEST")
         self.downloadable_ticker_information = None
```

## Comparing `historical_binance-0.1.6.dist-info/LICENSE` & `historical_binance-0.1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `historical_binance-0.1.6.dist-info/METADATA` & `historical_binance-0.1.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historical-binance
-Version: 0.1.6
+Version: 0.1.7.1
 Summary: A very fast downloader for Binance historical data
 Author: Denkik
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

