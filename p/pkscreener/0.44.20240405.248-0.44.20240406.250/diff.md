# Comparing `tmp/pkscreener-0.44.20240405.248.tar.gz` & `tmp/pkscreener-0.44.20240406.250.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240405.248.tar", last modified: Fri Apr  5 23:49:04 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240406.250.tar", last modified: Sat Apr  6 18:34:06 2024, max compression
```

## Comparing `pkscreener-0.44.20240405.248.tar` & `pkscreener-0.44.20240406.250.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/
--rw-rw-rw-   0        0        0     1086 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.244711 pkscreener-0.44.20240405.248/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27486 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    15888 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     7653 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48873 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   108935 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44525 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77220 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-05 23:48:55.000000 pkscreener-0.44.20240405.248/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   108550 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    16667 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 23:49:04.244711 pkscreener-0.44.20240405.248/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-05 23:49:04.000000 pkscreener-0.44.20240405.248/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-05 23:49:04.260328 pkscreener-0.44.20240405.248/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-05 23:43:53.000000 pkscreener-0.44.20240405.248/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:34:06.486237 pkscreener-0.44.20240406.250/
+-rw-rw-rw-   0        0        0     1086 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-06 18:34:06.486237 pkscreener-0.44.20240406.250/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 18:34:06.470615 pkscreener-0.44.20240406.250/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:34:06.486237 pkscreener-0.44.20240406.250/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27486 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    15888 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     7653 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    16886 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48873 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   108935 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77459 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-06 18:33:57.000000 pkscreener-0.44.20240406.250/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   108551 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    16667 2024-04-06 18:31:16.000000 pkscreener-0.44.20240406.250/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:34:06.470615 pkscreener-0.44.20240406.250/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-06 18:34:06.000000 pkscreener-0.44.20240406.250/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-06 18:34:06.486237 pkscreener-0.44.20240406.250/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-06 18:31:17.000000 pkscreener-0.44.20240406.250/setup.py
```

### Comparing `pkscreener-0.44.20240405.248/LICENSE` & `pkscreener-0.44.20240406.250/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/LICENSE-Others` & `pkscreener-0.44.20240406.250/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/PKG-INFO` & `pkscreener-0.44.20240406.250/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240405.248
+Version: 0.44.20240406.250
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240405.248.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240406.250.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240405.248/README.md` & `pkscreener-0.44.20240406.250/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240405.248/pkscreener/__init__.py` & `pkscreener-0.44.20240406.250/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,16 +545,19 @@
                         cellStyles, cellCleanValues = tools.getCellColors(
                             val, defaultCellFillColor=gridColor
                         )
                         valCounter = 0
                         for style in cellStyles:
                             cleanValue = cellCleanValues[valCounter]
                             valCounter += 1
-                            if columnNumber == 0:
-                                cleanValue = unstyledLine.split(column_separator)[1]
+                            if columnNumber == 0 and len(cleanValue.strip()) > 0:
+                                if column_separator in unstyledLine:
+                                    cleanValue = unstyledLine.split(column_separator)[1]
+                                if "\\" in cleanValue:
+                                    cleanValue = cleanValue.split("\\")[-1]
                                 # style = style if "%" in cleanValue else gridColor
                             if bgColor == "white" and style == "yellow":
                                 # Yellow on a white background is difficult to read
                                 style = "blue"
                             elif bgColor == "black" and style == "blue":
                                 # blue on a black background is difficult to read
                                 style = "yellow"
@@ -1445,11 +1448,11 @@
     def alertSound(beeps=3, delay=0.2):
         for i in range(beeps):
             print("\a")
             sleep(delay)
     
     def getMaxColumnWidths(df):
         columnWidths = [None]
-        addnlColumnWidths = [35 if (x in ["Trend(22Prds)"] or "-Pd" in x) else (20 if (x in ["Pattern"]) else None) for x in df.columns]
+        addnlColumnWidths = [40 if (x in ["Trend(22Prds)"] or "-Pd" in x) else (20 if (x in ["Pattern"]) else None) for x in df.columns]
         columnWidths.extend(addnlColumnWidths)
         columnWidths = columnWidths[:-1]
         return columnWidths
```

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/classes/keys.py` & `pkscreener-0.44.20240406.250/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/courbd.ttf` & `pkscreener-0.44.20240406.250/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/globals.py` & `pkscreener-0.44.20240406.250/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
             Utility.tools.clearScreen()
             return initPostLevel1Execution(indexOption, executeOption, retrial=True)
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
     try:
-        sortKey = ["%Chng"]
+        sortKey = ["Volume"]
         ascending = [False]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
                 sortKey = ["MFI"]
                 ascending = [reversalOption in [6,7]]
             elif reversalOption in [8,9]:
                 sortKey = ["FVDiff"]
```

### Comparing `pkscreener-0.44.20240405.248/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240406.250/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240406.250/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240406.250/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240406.250/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240405.248
+Version: 0.44.20240406.250
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240405.248.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240406.250.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240319.246/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240405.248/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240405.248/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240406.250/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240405.248/setup.py` & `pkscreener-0.44.20240406.250/setup.py`

 * *Files identical despite different names*

