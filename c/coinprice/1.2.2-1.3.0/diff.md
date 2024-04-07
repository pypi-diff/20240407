# Comparing `tmp/coinprice-1.2.2.tar.gz` & `tmp/coinprice-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinprice-1.2.2.tar", last modified: Fri Mar 29 15:11:15 2024, max compression
+gzip compressed data, was "coinprice-1.3.0.tar", last modified: Sun Apr  7 18:38:47 2024, max compression
```

## Comparing `coinprice-1.2.2.tar` & `coinprice-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:11:15.758847 coinprice-1.2.2/
--rw-rw-rw-   0        0        0     1063 2024-03-03 14:17:38.000000 coinprice-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3400 2024-03-29 15:11:15.756641 coinprice-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2609 2024-03-29 15:07:01.000000 coinprice-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 15:11:15.743609 coinprice-1.2.2/coinprice.egg-info/
--rw-rw-rw-   0        0        0     3400 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-29 15:11:15.000000 coinprice-1.2.2/coinprice.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-29 15:11:15.752758 coinprice-1.2.2/crypto_tracker/
--rw-rw-rw-   0        0        0        0 2024-03-15 18:04:57.000000 coinprice-1.2.2/crypto_tracker/__init__.py
--rw-rw-rw-   0        0        0     1243 2024-03-29 14:41:20.000000 coinprice-1.2.2/crypto_tracker/api.py
--rw-rw-rw-   0        0        0     7265 2024-03-29 14:44:06.000000 coinprice-1.2.2/crypto_tracker/main.py
--rw-rw-rw-   0        0        0       42 2024-03-29 15:11:15.758935 coinprice-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2024-03-29 15:08:46.000000 coinprice-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:38:47.253579 coinprice-1.3.0/
+-rw-rw-rw-   0        0        0     1063 2024-03-03 14:17:38.000000 coinprice-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3509 2024-04-07 18:38:47.252180 coinprice-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2024-04-07 18:09:54.000000 coinprice-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 18:38:47.241579 coinprice-1.3.0/coinprice.egg-info/
+-rw-rw-rw-   0        0        0     3509 2024-04-07 18:38:46.000000 coinprice-1.3.0/coinprice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-07 18:38:47.000000 coinprice-1.3.0/coinprice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:38:46.000000 coinprice-1.3.0/coinprice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-07 18:38:46.000000 coinprice-1.3.0/coinprice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 18:38:46.000000 coinprice-1.3.0/coinprice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-07 18:38:46.000000 coinprice-1.3.0/coinprice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 18:38:47.249140 coinprice-1.3.0/crypto_tracker/
+-rw-rw-rw-   0        0        0        0 2024-03-15 18:04:57.000000 coinprice-1.3.0/crypto_tracker/__init__.py
+-rw-rw-rw-   0        0        0     1243 2024-03-29 14:41:20.000000 coinprice-1.3.0/crypto_tracker/api.py
+-rw-rw-rw-   0        0        0     5541 2024-04-07 18:02:06.000000 coinprice-1.3.0/crypto_tracker/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 18:38:47.253579 coinprice-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2024-04-07 18:11:45.000000 coinprice-1.3.0/setup.py
```

### Comparing `coinprice-1.2.2/LICENSE` & `coinprice-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coinprice-1.2.2/PKG-INFO` & `coinprice-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinprice
-Version: 1.2.2
+Version: 1.3.0
 Summary: CryptoTracker is a command-line tool for tracking cryptocurrency prices across multiple exchanges.
 Author: Bohdan (7GitGuru)
 Author-email: Bohd4n@proton.me
 Project-URL: GitHub, https://github.com/7GitGuru/crypto-tracker/tree/cmd
 Project-URL: Documentation, https://github.com/7GitGuru/crypto-tracker/blob/cmd/README.md
 Project-URL: Website, https://cryptotrack3r.vercel.app/
 Keywords: cryptocurrency,crypto,bitcoin,ethereum,tracking,prices,finance,binance,okx,bybit,coinbase
@@ -42,15 +42,17 @@
 - Flexible Command-line Usage.
 - Customizable.
 - Set a custom interval for price updates.
 - Open-source project.
 
 --- 
 
-![image](https://github.com/7GitGuru/crypto-tracker/assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da)
+![demo](https://github.com/7GitGuru/crypto-tracker/assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf)
+![demo2](https://github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-6941ecdf4f76)
+
 
 ----
 
 ## Installation
 
 You can install Crypto Tracker using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coinprice Version: 1.2.2 Summary: CryptoTracker is
+Metadata-Version: 2.1 Name: coinprice Version: 1.3.0 Summary: CryptoTracker is
 a command-line tool for tracking cryptocurrency prices across multiple
 exchanges. Author: Bohdan (7GitGuru) Author-email: Bohd4n@proton.me Project-
 URL: GitHub, https://github.com/7GitGuru/crypto-tracker/tree/cmd Project-URL:
 Documentation, https://github.com/7GitGuru/crypto-tracker/blob/cmd/README.md
 Project-URL: Website, https://cryptotrack3r.vercel.app/ Keywords:
 cryptocurrency,crypto,bitcoin,ethereum,tracking,prices,finance,binance,okx,bybit,coinbase
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -18,27 +18,29 @@
  project/coinprice/) [![Downloads](https://static.pepy.tech/badge/coinprice)]
  (https://pepy.tech/project/coinprice) [![PyPI format](https://img.shields.io/
    pypi/format/coinprice.svg)](https://pypi.org/project/coinprice/) [![PyPI
  version](https://img.shields.io/pypi/v/coinprice)](https://pypi.org/project/
                                   coinprice/)
 --- ## Features - Track the prices of various cryptocurrencies. - Flexible
 Command-line Usage. - Customizable. - Set a custom interval for price updates.
-- Open-source project. --- ![image](https://github.com/7GitGuru/crypto-tracker/
-assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da) ---- ## Installation You
-can install Crypto Tracker using pip: ``` pip install coinprice ``` ## Usage To
-track the price of a cryptocurrency, simply run the following command: **[Here
-you can find a list of all cryptocurrencies you can use.](https://github.com/
-7GitGuru/crypto-tracker/blob/main/coin-names.json)** ``` price [--interval
-time] ``` Replace `` with the cryptocurrency you want to track (e.g., bitcoin,
-ethereum). You can optionally specify the interval (in seconds) for price
-updates using the `--interval` flag. By default, the interval is set to 15
-seconds. Example usage: ``` price btc Track the price of Bitcoin from all
-exchanges. price eth --binance Track the price of Bitcoin from Binance. price
-ltc --bybit --interval 10 Track the price of Litecoin from Bybit with a check
-interval of 10 seconds. ``` ### [Check out Telegram version!](https://
-github.com/7GitGuru/crypto-tracker/tree/telegram) ## Contributing Contributions
-to Crypto Tracker are welcome! If you find any bugs or have suggestions for new
-features, please open an issue or submit a [pull request](https://github.com/
-7GitGuru/crypto-tracker/pulls) on GitHub. ## License Crypto Tracker is released
-under the MIT License. See [LICENSE](https://github.com/7GitGuru/crypto-
-tracker/blob/main/LICENSE) for details.
+- Open-source project. --- ![demo](https://github.com/7GitGuru/crypto-tracker/
+assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf) ![demo2](https://
+github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-
+6941ecdf4f76) ---- ## Installation You can install Crypto Tracker using pip:
+``` pip install coinprice ``` ## Usage To track the price of a cryptocurrency,
+simply run the following command: **[Here you can find a list of all
+cryptocurrencies you can use.](https://github.com/7GitGuru/crypto-tracker/blob/
+main/coin-names.json)** ``` price [--interval time] ``` Replace `` with the
+cryptocurrency you want to track (e.g., bitcoin, ethereum). You can optionally
+specify the interval (in seconds) for price updates using the `--interval`
+flag. By default, the interval is set to 15 seconds. Example usage: ``` price
+btc Track the price of Bitcoin from all exchanges. price eth --binance Track
+the price of Bitcoin from Binance. price ltc --bybit --interval 10 Track the
+price of Litecoin from Bybit with a check interval of 10 seconds. ``` ###
+[Check out Telegram version!](https://github.com/7GitGuru/crypto-tracker/tree/
+telegram) ## Contributing Contributions to Crypto Tracker are welcome! If you
+find any bugs or have suggestions for new features, please open an issue or
+submit a [pull request](https://github.com/7GitGuru/crypto-tracker/pulls) on
+GitHub. ## License Crypto Tracker is released under the MIT License. See
+[LICENSE](https://github.com/7GitGuru/crypto-tracker/blob/main/LICENSE) for
+details.
            ********** [[DDoonnaattee]]((hhttttppss::////wwwwww..bbuuyymmeeaaccooffffeeee..ccoomm//bboohhdd44nn)) **********
```

### Comparing `coinprice-1.2.2/README.md` & `coinprice-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 - Flexible Command-line Usage.
 - Customizable.
 - Set a custom interval for price updates.
 - Open-source project.
 
 --- 
 
-![image](https://github.com/7GitGuru/crypto-tracker/assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da)
+![demo](https://github.com/7GitGuru/crypto-tracker/assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf)
+![demo2](https://github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-6941ecdf4f76)
+
 
 ----
 
 ## Installation
 
 You can install Crypto Tracker using pip:
```

#### html2text {}

```diff
@@ -7,27 +7,29 @@
  project/coinprice/) [![Downloads](https://static.pepy.tech/badge/coinprice)]
  (https://pepy.tech/project/coinprice) [![PyPI format](https://img.shields.io/
    pypi/format/coinprice.svg)](https://pypi.org/project/coinprice/) [![PyPI
  version](https://img.shields.io/pypi/v/coinprice)](https://pypi.org/project/
                                   coinprice/)
 --- ## Features - Track the prices of various cryptocurrencies. - Flexible
 Command-line Usage. - Customizable. - Set a custom interval for price updates.
-- Open-source project. --- ![image](https://github.com/7GitGuru/crypto-tracker/
-assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da) ---- ## Installation You
-can install Crypto Tracker using pip: ``` pip install coinprice ``` ## Usage To
-track the price of a cryptocurrency, simply run the following command: **[Here
-you can find a list of all cryptocurrencies you can use.](https://github.com/
-7GitGuru/crypto-tracker/blob/main/coin-names.json)** ``` price [--interval
-time] ``` Replace `` with the cryptocurrency you want to track (e.g., bitcoin,
-ethereum). You can optionally specify the interval (in seconds) for price
-updates using the `--interval` flag. By default, the interval is set to 15
-seconds. Example usage: ``` price btc Track the price of Bitcoin from all
-exchanges. price eth --binance Track the price of Bitcoin from Binance. price
-ltc --bybit --interval 10 Track the price of Litecoin from Bybit with a check
-interval of 10 seconds. ``` ### [Check out Telegram version!](https://
-github.com/7GitGuru/crypto-tracker/tree/telegram) ## Contributing Contributions
-to Crypto Tracker are welcome! If you find any bugs or have suggestions for new
-features, please open an issue or submit a [pull request](https://github.com/
-7GitGuru/crypto-tracker/pulls) on GitHub. ## License Crypto Tracker is released
-under the MIT License. See [LICENSE](https://github.com/7GitGuru/crypto-
-tracker/blob/main/LICENSE) for details.
+- Open-source project. --- ![demo](https://github.com/7GitGuru/crypto-tracker/
+assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf) ![demo2](https://
+github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-
+6941ecdf4f76) ---- ## Installation You can install Crypto Tracker using pip:
+``` pip install coinprice ``` ## Usage To track the price of a cryptocurrency,
+simply run the following command: **[Here you can find a list of all
+cryptocurrencies you can use.](https://github.com/7GitGuru/crypto-tracker/blob/
+main/coin-names.json)** ``` price [--interval time] ``` Replace `` with the
+cryptocurrency you want to track (e.g., bitcoin, ethereum). You can optionally
+specify the interval (in seconds) for price updates using the `--interval`
+flag. By default, the interval is set to 15 seconds. Example usage: ``` price
+btc Track the price of Bitcoin from all exchanges. price eth --binance Track
+the price of Bitcoin from Binance. price ltc --bybit --interval 10 Track the
+price of Litecoin from Bybit with a check interval of 10 seconds. ``` ###
+[Check out Telegram version!](https://github.com/7GitGuru/crypto-tracker/tree/
+telegram) ## Contributing Contributions to Crypto Tracker are welcome! If you
+find any bugs or have suggestions for new features, please open an issue or
+submit a [pull request](https://github.com/7GitGuru/crypto-tracker/pulls) on
+GitHub. ## License Crypto Tracker is released under the MIT License. See
+[LICENSE](https://github.com/7GitGuru/crypto-tracker/blob/main/LICENSE) for
+details.
            ********** [[DDoonnaattee]]((hhttttppss::////wwwwww..bbuuyymmeeaaccooffffeeee..ccoomm//bboohhdd44nn)) **********
```

### Comparing `coinprice-1.2.2/coinprice.egg-info/PKG-INFO` & `coinprice-1.3.0/coinprice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinprice
-Version: 1.2.2
+Version: 1.3.0
 Summary: CryptoTracker is a command-line tool for tracking cryptocurrency prices across multiple exchanges.
 Author: Bohdan (7GitGuru)
 Author-email: Bohd4n@proton.me
 Project-URL: GitHub, https://github.com/7GitGuru/crypto-tracker/tree/cmd
 Project-URL: Documentation, https://github.com/7GitGuru/crypto-tracker/blob/cmd/README.md
 Project-URL: Website, https://cryptotrack3r.vercel.app/
 Keywords: cryptocurrency,crypto,bitcoin,ethereum,tracking,prices,finance,binance,okx,bybit,coinbase
@@ -42,15 +42,17 @@
 - Flexible Command-line Usage.
 - Customizable.
 - Set a custom interval for price updates.
 - Open-source project.
 
 --- 
 
-![image](https://github.com/7GitGuru/crypto-tracker/assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da)
+![demo](https://github.com/7GitGuru/crypto-tracker/assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf)
+![demo2](https://github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-6941ecdf4f76)
+
 
 ----
 
 ## Installation
 
 You can install Crypto Tracker using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coinprice Version: 1.2.2 Summary: CryptoTracker is
+Metadata-Version: 2.1 Name: coinprice Version: 1.3.0 Summary: CryptoTracker is
 a command-line tool for tracking cryptocurrency prices across multiple
 exchanges. Author: Bohdan (7GitGuru) Author-email: Bohd4n@proton.me Project-
 URL: GitHub, https://github.com/7GitGuru/crypto-tracker/tree/cmd Project-URL:
 Documentation, https://github.com/7GitGuru/crypto-tracker/blob/cmd/README.md
 Project-URL: Website, https://cryptotrack3r.vercel.app/ Keywords:
 cryptocurrency,crypto,bitcoin,ethereum,tracking,prices,finance,binance,okx,bybit,coinbase
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -18,27 +18,29 @@
  project/coinprice/) [![Downloads](https://static.pepy.tech/badge/coinprice)]
  (https://pepy.tech/project/coinprice) [![PyPI format](https://img.shields.io/
    pypi/format/coinprice.svg)](https://pypi.org/project/coinprice/) [![PyPI
  version](https://img.shields.io/pypi/v/coinprice)](https://pypi.org/project/
                                   coinprice/)
 --- ## Features - Track the prices of various cryptocurrencies. - Flexible
 Command-line Usage. - Customizable. - Set a custom interval for price updates.
-- Open-source project. --- ![image](https://github.com/7GitGuru/crypto-tracker/
-assets/154711952/d5386490-30ca-4bdd-85ec-c0f936cfd5da) ---- ## Installation You
-can install Crypto Tracker using pip: ``` pip install coinprice ``` ## Usage To
-track the price of a cryptocurrency, simply run the following command: **[Here
-you can find a list of all cryptocurrencies you can use.](https://github.com/
-7GitGuru/crypto-tracker/blob/main/coin-names.json)** ``` price [--interval
-time] ``` Replace `` with the cryptocurrency you want to track (e.g., bitcoin,
-ethereum). You can optionally specify the interval (in seconds) for price
-updates using the `--interval` flag. By default, the interval is set to 15
-seconds. Example usage: ``` price btc Track the price of Bitcoin from all
-exchanges. price eth --binance Track the price of Bitcoin from Binance. price
-ltc --bybit --interval 10 Track the price of Litecoin from Bybit with a check
-interval of 10 seconds. ``` ### [Check out Telegram version!](https://
-github.com/7GitGuru/crypto-tracker/tree/telegram) ## Contributing Contributions
-to Crypto Tracker are welcome! If you find any bugs or have suggestions for new
-features, please open an issue or submit a [pull request](https://github.com/
-7GitGuru/crypto-tracker/pulls) on GitHub. ## License Crypto Tracker is released
-under the MIT License. See [LICENSE](https://github.com/7GitGuru/crypto-
-tracker/blob/main/LICENSE) for details.
+- Open-source project. --- ![demo](https://github.com/7GitGuru/crypto-tracker/
+assets/154711952/0df38415-6b97-4d06-ba31-e6a421d520bf) ![demo2](https://
+github.com/7GitGuru/crypto-tracker/assets/154711952/908a0b26-f6ce-41ae-9a6b-
+6941ecdf4f76) ---- ## Installation You can install Crypto Tracker using pip:
+``` pip install coinprice ``` ## Usage To track the price of a cryptocurrency,
+simply run the following command: **[Here you can find a list of all
+cryptocurrencies you can use.](https://github.com/7GitGuru/crypto-tracker/blob/
+main/coin-names.json)** ``` price [--interval time] ``` Replace `` with the
+cryptocurrency you want to track (e.g., bitcoin, ethereum). You can optionally
+specify the interval (in seconds) for price updates using the `--interval`
+flag. By default, the interval is set to 15 seconds. Example usage: ``` price
+btc Track the price of Bitcoin from all exchanges. price eth --binance Track
+the price of Bitcoin from Binance. price ltc --bybit --interval 10 Track the
+price of Litecoin from Bybit with a check interval of 10 seconds. ``` ###
+[Check out Telegram version!](https://github.com/7GitGuru/crypto-tracker/tree/
+telegram) ## Contributing Contributions to Crypto Tracker are welcome! If you
+find any bugs or have suggestions for new features, please open an issue or
+submit a [pull request](https://github.com/7GitGuru/crypto-tracker/pulls) on
+GitHub. ## License Crypto Tracker is released under the MIT License. See
+[LICENSE](https://github.com/7GitGuru/crypto-tracker/blob/main/LICENSE) for
+details.
            ********** [[DDoonnaattee]]((hhttttppss::////wwwwww..bbuuyymmeeaaccooffffeeee..ccoomm//bboohhdd44nn)) **********
```

### Comparing `coinprice-1.2.2/crypto_tracker/api.py` & `coinprice-1.3.0/crypto_tracker/api.py`

 * *Files identical despite different names*

### Comparing `coinprice-1.2.2/setup.py` & `coinprice-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='coinprice',
-    version='1.2.2',
+    version='1.3.0',
     author='Bohdan (7GitGuru)',
     author_email='Bohd4n@proton.me',
     description='CryptoTracker is a command-line tool for tracking cryptocurrency prices across multiple exchanges.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

