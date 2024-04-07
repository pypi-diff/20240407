# Comparing `tmp/ml_backtest-0.1.1a0.tar.gz` & `tmp/ml_backtest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_backtest-0.1.1a0.tar", last modified: Wed Apr  3 19:48:03 2024, max compression
+gzip compressed data, was "ml_backtest-0.1.2.tar", last modified: Sun Apr  7 04:05:56 2024, max compression
```

## Comparing `ml_backtest-0.1.1a0.tar` & `ml_backtest-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/backtesting-with-machine-learning/
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/backtesting-with-machine-learning/machine-learning-class-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/backtesting-with-machine-learning/strategy-creation-class-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/backtest/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/data/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/interfaces/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/models/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/models/rfr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/bullishengulfing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/bullishharami.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/dragonflydoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/hammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/invertedhammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/morningstar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/morningstardoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/piercingpattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/tests/test_ml_backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.345187 ml_backtest-0.1.2/backtesting-with-machine-learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/backtesting-with-machine-learning/machine-learning-class-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/backtesting-with-machine-learning/strategy-creation-class-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.345187 ml_backtest-0.1.2/ml_backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/interfaces/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/models/rfr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/ml_backtest/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/bullishengulfing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/bullishharami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/dragonflydoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/hammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/invertedhammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/morningstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/morningstardoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/piercingpattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/ml_backtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/tests/test_ml_backtest.py
```

### Comparing `ml_backtest-0.1.1a0/LICENSE` & `ml_backtest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/PKG-INFO` & `ml_backtest-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,20 +18,14 @@
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
 Requires-Dist: TA-Lib~=0.4.0
 
----
-description: >-
-  Trading strategy backtesting with machine learning optimizing best exit point
-  (aka highest point of trade) for each trade, maximizing profit.
----
-
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -50,60 +44,61 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install -r requirements.txt
+pip install ml-backtest
 ```
 
 First you need to import all the required classes.
 
 ```python
+from ml_backtest import Backtest, MachineLearning
+from ml_backtest.machine_learning import CandleStickDataProcessing
+from ml_backtest.strategies import InvertedHammer
+from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
-from backtest.backtest import Backtest
-from strategies.invertedhammer import InvertedHammer
-from machine_learning.wrapper import MachineLearning
-from models.rfr import RandomForestRegressorTrainer
-from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
 ```
 
 After you have your data-frame prepped you can make an instance of the strategy you want and pass it into a Backtest instance.&#x20;
 
 ```python
 strategy = InvertedHammer()
 backtest = Backtest(df, strategy)
-print(backtest.results())
+print(backtest.get_results())
 ```
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
-                         df=df,
-                         results=backtest.get_trades())
-ml.run()
+                    df=df,
+                    results=backtest.get_trades(),
+                    rows=10,
+                    columns=['EMA_Diff', 'SMA_Diff', 'MACD_hist'])
+ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
-print(ml_backtest.results())
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+print(ml_backtest.get_results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1a0/README.md` & `ml_backtest-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,7 @@
----
-description: >-
-  Trading strategy backtesting with machine learning optimizing best exit point
-  (aka highest point of trade) for each trade, maximizing profit.
----
-
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -26,60 +20,61 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install -r requirements.txt
+pip install ml-backtest
 ```
 
 First you need to import all the required classes.
 
 ```python
+from ml_backtest import Backtest, MachineLearning
+from ml_backtest.machine_learning import CandleStickDataProcessing
+from ml_backtest.strategies import InvertedHammer
+from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
-from backtest.backtest import Backtest
-from strategies.invertedhammer import InvertedHammer
-from machine_learning.wrapper import MachineLearning
-from models.rfr import RandomForestRegressorTrainer
-from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
 ```
 
 After you have your data-frame prepped you can make an instance of the strategy you want and pass it into a Backtest instance.&#x20;
 
 ```python
 strategy = InvertedHammer()
 backtest = Backtest(df, strategy)
-print(backtest.results())
+print(backtest.get_results())
 ```
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
-                         df=df,
-                         results=backtest.get_trades())
-ml.run()
+                    df=df,
+                    results=backtest.get_trades(),
+                    rows=10,
+                    columns=['EMA_Diff', 'SMA_Diff', 'MACD_hist'])
+ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
-print(ml_backtest.results())
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+print(ml_backtest.get_results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1a0/backtesting-with-machine-learning/machine-learning-class-guide.md` & `ml_backtest-0.1.2/backtesting-with-machine-learning/machine-learning-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/backtesting-with-machine-learning/strategy-creation-class-guide.md` & `ml_backtest-0.1.2/backtesting-with-machine-learning/strategy-creation-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/backtest/backtest.py` & `ml_backtest-0.1.2/ml_backtest/backtest/backtest.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,18 @@
         self.__gross_loss = 0
         self.__start_time = None
         self.__end_time = None
         self.__model = model
         self.__columns = columns
         self.__rows = rows
         self.__cs_pattern = cs_pattern
+        self.__backtest = None
+
+        self.__run()
+        self.__results()
 
     def __run(self):
         dates = self.__data['date'].values
         lows = self.__data['low'].values
         highs = self.__data['high'].values
         close = self.__data['close'].values
         open = self.__data['open'].values
@@ -51,15 +55,15 @@
         if self.__columns is not None and self.__rows is not None and self.__model is not None:
             self.__strategy.set_ml(model=self.__model, columns=self.__columns, rows=self.__rows,
                                    df=self.__data, cs_pattern=self.__cs_pattern)
 
         for index in tqdm(range(len(dates)), total=len(dates)):
             # Assuming strategy.on_data can be adapted or is simplified for demonstration
             self.__strategy.on_data(index, lows[:index + 1], highs[:index + 1],
-                                  close[:index + 1], open[:index + 1], dates[:index + 1])
+                                    close[:index + 1], open[:index + 1], dates[:index + 1])
 
             for position in list(self.__strategy.positions):  # Iterate over a shallow copy if positions are modified
                 exit_price = None
 
                 if 'highest high' not in position or highs[index] > position['highest high']:
                     position['highest high'] = highs[index]
 
@@ -125,37 +129,40 @@
         # Add any statistics to the completed trades
         position['exit price'] = current_price
         position['size'] = 1
         position['pnl'] = profit_loss
         self.__completed_trades.append(position)
         self.__strategy.in_position = False
 
-    def results(self) -> pd.DataFrame:
-        self.__run()
+    def __results(self) -> pd.DataFrame:
 
         wins = self.__short_wins + self.__long_wins
         loses = self.__short_loses + self.__long_loses
-        backtest_result = [{'start time': self.__start_time,
-                            'end time': self.__end_time,
-                            '# of trades': self.__trade_counter,
-                            '# of wins': wins,
-                            '# of loses': loses,
-                            'win rate': f'{np.around((wins / (wins + loses)) * 100, decimals=2)}%',
-                            '# of long wins': self.__long_wins,
-                            '# of long loses': self.__long_loses,
-                            '# of long evens': self.__long_evens,
-                            '# of short wins': self.__short_wins,
-                            '# of short loses': self.__short_loses,
-                            '# of short evens': self.__short_evens,
-                            'net profit': np.around(self.__gross_profit + self.__gross_loss, decimals=2),
-                            'max drawdown': f'-{np.around(self.__max_drawdown, decimals=2)}',
-                            'gross profit': np.around(self.__gross_profit, decimals=2),
-                            'gross loss': np.around(self.__gross_loss, decimals=2),
-                            'profit factor': np.around(self.__gross_profit / abs(self.__gross_loss), decimals=2)}]
-
-        backtest_df = pd.DataFrame(backtest_result)
-        backtest_df = backtest_df.T
-        return backtest_df
+        self.__backtest_result = [{'start time': self.__start_time,
+                                   'end time': self.__end_time,
+                                   '# of trades': self.__trade_counter,
+                                   '# of wins': wins,
+                                   '# of loses': loses,
+                                   'win rate': f'{np.around((wins / (wins + loses)) * 100, decimals=2)}%',
+                                   '# of long wins': self.__long_wins,
+                                   '# of long loses': self.__long_loses,
+                                   '# of long evens': self.__long_evens,
+                                   '# of short wins': self.__short_wins,
+                                   '# of short loses': self.__short_loses,
+                                   '# of short evens': self.__short_evens,
+                                   'net profit': np.around(self.__gross_profit + self.__gross_loss, decimals=2),
+                                   'max drawdown': f'-{np.around(self.__max_drawdown, decimals=2)}',
+                                   'gross profit': np.around(self.__gross_profit, decimals=2),
+                                   'gross loss': np.around(self.__gross_loss, decimals=2),
+                                   'profit factor': np.around(self.__gross_profit / abs(self.__gross_loss),
+                                                              decimals=2)}]
+
+        self.__backtest_df = pd.DataFrame(self.__backtest_result)
+        self.__backtest_df = self.__backtest_df.T
+        return self.__backtest_df
 
     def get_trades(self) -> pd.DataFrame:
         completed_trades_df = pd.DataFrame(self.__completed_trades)
         return completed_trades_df
+
+    def get_results(self) -> pd.DataFrame:
+        return self.__backtest_df
```

### Comparing `ml_backtest-0.1.1a0/ml_backtest/data/data.py` & `ml_backtest-0.1.2/ml_backtest/data/data.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/interfaces/interface.py` & `ml_backtest-0.1.2/ml_backtest/interfaces/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pandas as pd
 from ml_backtest.machine_learning import DataProcessing
 from datetime import datetime
 from typing import final
 from sklearn.base import BaseEstimator
-from typing import Optional
+from typing import Optional, List
 import numpy as np
 
 
 class MachineLearningInterface:
 
-    def __init__(self, data: pd.DataFrame):
+    def __init__(self, data: pd.DataFrame,
+                 rows: Optional[int] = None,
+                 columns: Optional[List[str]] = None):
 
         if type(self).get_model != MachineLearningInterface.get_model:
             raise TypeError("get_model method should not be overridden")
 
         if isinstance(data, pd.DataFrame):
             self.data = data
             self.model = None
             self.predictions = None
-            self.get_rows = 10
-            self.get_columns = ['Close']
+            self.get_rows = rows if rows is not None else 10
+            self.get_columns = columns if columns is not None else ['close']
 
         else:
             print('Data being passed into MachineLearningWorker is not a list of type DataContainer.')
 
     def feature_engineer(self):
         """
         Create new features or change current ones. Method will be called
@@ -55,14 +57,15 @@
         :param y_train:
         :param x_test:
         :param y_test:
         :return:
         """
         raise NotImplementedError("This method must be implemented by a subclass")
 
+    @final
     def get_model(self):
         """
         Returns the model used in training.
 
         :return: model
         """
         return self.model
```

### Comparing `ml_backtest-0.1.1a0/ml_backtest/machine_learning/data.py` & `ml_backtest-0.1.2/ml_backtest/machine_learning/data.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/machine_learning/wrapper.py` & `ml_backtest-0.1.2/ml_backtest/machine_learning/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import numpy as np
 from joblib import dump
 from ml_backtest.interfaces import MachineLearningInterface, TargetInterface
 from sklearn.model_selection import train_test_split
 from ml_backtest.machine_learning import DataProcessing
-from typing import Type
+from typing import Type, List, Optional
 import pandas as pd
 import os
 
 
 class MachineLearning:
 
     def __init__(self, ml_class: Type[MachineLearningInterface],
                  df: pd.DataFrame, results: pd.DataFrame,
-                 target_class: Type[TargetInterface] = None):
+                 target_class: Type[TargetInterface] = None,
+                 rows: Optional[int] = None,
+                 columns: Optional[List[str]] = None):
         self.__df = df
         self.__results = results
+
         if target_class is not None:
             self.__target_class = target_class(trades=self.__results, data=self.__df)
             self.__target_class.target_engineer()
             self.__results = self.__target_class.trades
-        self.__ml = ml_class(self.__df)
+        if rows is not None and columns is not None:
+            self.__ml = ml_class(data=self.__df, rows=rows, columns=columns)
+        else:
+            self.__ml = ml_class(data=self.__df)
 
     def run(self, dp_pattern=None) -> None:
         self.__ml.feature_engineer()
 
         dp = DataProcessing(df=self.__df, results=self.__results,
                             rows=self.__ml.get_rows, columns=self.__ml.get_columns)
```

### Comparing `ml_backtest-0.1.1a0/ml_backtest/models/rfr.py` & `ml_backtest-0.1.2/ml_backtest/models/rfr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from ml_backtest.interfaces import MachineLearningInterface, TargetInterface
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import mean_squared_error
 import pandas as pd
 import talib
+from typing import Optional, List
 
 
 class RandomForestRegressorTrainer(MachineLearningInterface):
 
-    def __init__(self, data: pd.DataFrame):
-        super().__init__(data)
-        # this is the number of rows before each target you want trained
-        self.get_rows = 10
-        # these are the columns you want trained, in my case I want the column
-        # that is already there and a column I am adding in the feature_engineer()
-        # method
+    def __init__(self, data: pd.DataFrame, rows: Optional[int] = None,
+                 columns: Optional[List[str]] = None):
+        super().__init__(data,  rows, columns)
+        # Additional initialization specific to RandomForestRegressorTrainer can go here.
+        # For example, setting up model-specific parameters or preprocessing steps.
+        # self.model_specific_param = some_value
 
-        # 'EMA_Diff', 'SMA_Diff', 'RSI', 'MACD', 'MACD_signal', 'MACD_hist'
-        self.get_columns = ['EMA_Diff', 'SMA_Diff', 'MACD_hist']
+        # If there's additional setup required for the RandomForest model,
+        # that doesn't fit the pattern provided by MachineLearningInterface,
+        # it can be performed here.
 
     def feature_engineer(self):
         # here is where you can add addition columns of features you want to be used in training
         # just make sure you edit the 'self.data' with the features you want as that is the dataframe being
         # used in training
         self.data['SMA'] = self.data['close'].rolling(window=10).mean()
         self.data['EMA'] = talib.EMA(self.data['close'], timeperiod=10)
```

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishengulfing.py` & `ml_backtest-0.1.2/ml_backtest/strategies/bullishengulfing.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishharami.py` & `ml_backtest-0.1.2/ml_backtest/strategies/bullishharami.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/dragonflydoji.py` & `ml_backtest-0.1.2/ml_backtest/strategies/dragonflydoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/hammer.py` & `ml_backtest-0.1.2/ml_backtest/strategies/hammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/invertedhammer.py` & `ml_backtest-0.1.2/ml_backtest/strategies/invertedhammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstar.py` & `ml_backtest-0.1.2/ml_backtest/strategies/morningstar.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstardoji.py` & `ml_backtest-0.1.2/ml_backtest/strategies/morningstardoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest/strategies/piercingpattern.py` & `ml_backtest-0.1.2/ml_backtest/strategies/piercingpattern.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/ml_backtest.egg-info/PKG-INFO` & `ml_backtest-0.1.2/ml_backtest.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,20 +18,14 @@
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
 Requires-Dist: TA-Lib~=0.4.0
 
----
-description: >-
-  Trading strategy backtesting with machine learning optimizing best exit point
-  (aka highest point of trade) for each trade, maximizing profit.
----
-
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -50,60 +44,61 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install -r requirements.txt
+pip install ml-backtest
 ```
 
 First you need to import all the required classes.
 
 ```python
+from ml_backtest import Backtest, MachineLearning
+from ml_backtest.machine_learning import CandleStickDataProcessing
+from ml_backtest.strategies import InvertedHammer
+from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
-from backtest.backtest import Backtest
-from strategies.invertedhammer import InvertedHammer
-from machine_learning.wrapper import MachineLearning
-from models.rfr import RandomForestRegressorTrainer
-from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
 ```
 
 After you have your data-frame prepped you can make an instance of the strategy you want and pass it into a Backtest instance.&#x20;
 
 ```python
 strategy = InvertedHammer()
 backtest = Backtest(df, strategy)
-print(backtest.results())
+print(backtest.get_results())
 ```
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
-                         df=df,
-                         results=backtest.get_trades())
-ml.run()
+                    df=df,
+                    results=backtest.get_trades(),
+                    rows=10,
+                    columns=['EMA_Diff', 'SMA_Diff', 'MACD_hist'])
+ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
-print(ml_backtest.results())
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+print(ml_backtest.get_results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1a0/ml_backtest.egg-info/SOURCES.txt` & `ml_backtest-0.1.2/ml_backtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/setup.py` & `ml_backtest-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1a0/tests/test_ml_backtest.py` & `ml_backtest-0.1.2/tests/test_ml_backtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import pandas as pd
 from ml_backtest import Backtest, MachineLearning
 from ml_backtest.strategies import InvertedHammer
 from ml_backtest.models import RandomForestRegressorTrainer
 from ml_backtest.machine_learning import CandleStickDataProcessing
 from ml_backtest.data import Data
 
 
 def test_backtesting_with_machine_learning():
     strategy = InvertedHammer()
 
     backtest = Backtest(Data.data(), strategy)
-    backtest_results = backtest.results()
+    backtest_results = backtest.get_results()
     assert backtest_results is not None
 
     ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
                          df=Data.data(),
                          results=backtest.get_trades())
     ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
 
     model, columns, rows = ml.get_util()
     assert model is not None
 
     data = ml.get_data()
     assert not data.empty
 
     ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
-    ml_backtest_results = ml_backtest.results()
+    ml_backtest_results = ml_backtest.get_results()
     assert ml_backtest_results is not None
```

