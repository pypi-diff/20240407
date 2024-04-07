# Comparing `tmp/lumibot-3.2.9.tar.gz` & `tmp/lumibot-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.2.9.tar", last modified: Tue Mar 19 07:32:01 2024, max compression
+gzip compressed data, was "lumibot-3.3.1.tar", last modified: Sun Apr  7 08:27:22 2024, max compression
```

## Comparing `lumibot-3.2.9.tar` & `lumibot-3.3.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.837088 lumibot-3.2.9/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.2.9/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5468 2024-03-19 07:32:01.837020 lumibot-3.2.9/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.2.9/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.814554 lumibot-3.2.9/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.817036 lumibot-3.2.9/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30909 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.818941 lumibot-3.2.9/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42333 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    29800 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    23394 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.822260 lumibot-3.2.9/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    14998 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2573 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     8133 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6744 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.825157 lumibot-3.2.9/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9345 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28584 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.826957 lumibot-3.2.9/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2469 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.827663 lumibot-3.2.9/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53399 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   146885 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39624 2024-03-19 07:27:52.000000 lumibot-3.2.9/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.831068 lumibot-3.2.9/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21342 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26055 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19634 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15215 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.831612 lumibot-3.2.9/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.832493 lumibot-3.2.9/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.2.9/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.836654 lumibot-3.2.9/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5468 2024-03-19 07:32:01.000000 lumibot-3.2.9/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-03-19 07:32:01.000000 lumibot-3.2.9/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-03-19 07:32:01.000000 lumibot-3.2.9/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      573 2024-03-19 07:32:01.000000 lumibot-3.2.9/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-03-19 07:32:01.000000 lumibot-3.2.9/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.2.9/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-03-19 07:32:01.837438 lumibot-3.2.9/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-19 07:29:47.000000 lumibot-3.2.9/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.835174 lumibot-3.2.9/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-19 07:32:01.836484 lumibot-3.2.9/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4301 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20205 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.2.9/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.100086 lumibot-3.3.1/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.1/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-07 08:27:22.100020 lumibot-3.3.1/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.1/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.085300 lumibot-3.3.1/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.086993 lumibot-3.3.1/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30919 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.088010 lumibot-3.3.1/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42446 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.1/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27024 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.089924 lumibot-3.3.1/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.1/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.1/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6744 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.091278 lumibot-3.3.1/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28584 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.093448 lumibot-3.3.1/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2469 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.094091 lumibot-3.3.1/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.1/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149829 2024-04-07 08:26:01.000000 lumibot-3.3.1/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39624 2024-03-19 07:27:52.000000 lumibot-3.3.1/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.095746 lumibot-3.3.1/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.1/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26137 2024-03-31 03:38:08.000000 lumibot-3.3.1/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.1/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15215 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.096047 lumibot-3.3.1/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.096486 lumibot-3.3.1/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.1/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.099601 lumibot-3.3.1/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-07 08:27:22.000000 lumibot-3.3.1/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-07 08:27:22.000000 lumibot-3.3.1/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-07 08:27:22.000000 lumibot-3.3.1/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-07 08:27:22.000000 lumibot-3.3.1/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-07 08:27:22.000000 lumibot-3.3.1/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.1/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-07 08:27:22.100399 lumibot-3.3.1/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-07 08:26:01.000000 lumibot-3.3.1/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.098597 lumibot-3.3.1/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-07 08:27:22.099425 lumibot-3.3.1/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4301 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20670 2024-04-07 08:26:01.000000 lumibot-3.3.1/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.1/tests/test_tradingfee.py
```

### Comparing `lumibot-3.2.9/LICENSE` & `lumibot-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/PKG-INFO` & `lumibot-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.2.9
+Version: 3.3.1
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,24 +30,24 @@
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
 Requires-Dist: scipy==1.10.1
 Requires-Dist: ipython
-Requires-Dist: quantstats-lumi>=0.1.10
+Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
-Requires-Dist: ccxt==4.2.50
+Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
 Requires-Dist: appdirs
 Requires-Dist: pyarrow
 Requires-Dist: tqdm
-Requires-Dist: lumiwealth-tradier>=0.1.6
+Requires-Dist: lumiwealth-tradier>=0.1.7
 Requires-Dist: pytz
 Requires-Dist: psycopg2-binary
 Requires-Dist: exchange_calendars>=4.5.2
 Requires-Dist: duckdb
 Requires-Dist: uuid
 Requires-Dist: tabulate
```

### Comparing `lumibot-3.2.9/README.md` & `lumibot-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/__init__.py` & `lumibot-3.3.1/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.3.1/lumibot/backtesting/backtesting_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
         self.stream.dispatch(
             self.NEW_ORDER,
             wait_until_complete=True,
             order=order,
         )
         return order
 
-    def submit_orders(self, orders):
+    def submit_orders(self, orders, **kwargs):
         results = []
         for order in orders:
             results.append(self.submit_order(order))
         return results
 
     def cancel_order(self, order):
         """Cancel an order"""
```

### Comparing `lumibot-3.2.9/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.3.1/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/brokers/alpaca.py` & `lumibot-3.3.1/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/brokers/broker.py` & `lumibot-3.3.1/lumibot/brokers/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,18 @@
 
     def sync_positions(self, strategy):
         """
         Sync the broker positions with the lumibot positions. Remove any lumibot positions that are not at the broker.
         """
         positions_broker = self._pull_positions(strategy)
         for position in positions_broker:
+            # Check if the position is None
+            if position is None:
+                continue
+
             # Check against existing position.
             position_lumi = [
                 pos_lumi
                 for pos_lumi in self._filled_positions.get_list()
                 if pos_lumi.asset == position.asset
             ]
             position_lumi = position_lumi[0] if len(position_lumi) > 0 else None
@@ -825,15 +829,15 @@
         result = self._parse_broker_orders(response, strategy_name, strategy_object=strategy_object)
         return result
 
     def submit_order(self, order):
         """Submit an order for an asset"""
         self._orders_queue.put(order)
 
-    def submit_orders(self, orders):
+    def submit_orders(self, orders, **kwargs):
         """Submit orders"""
         self._orders_queue.put(orders)
 
     def wait_for_order_registration(self, order):
         """Wait for the order to be registered by the broker"""
         order.wait_to_be_registered()
```

### Comparing `lumibot-3.2.9/lumibot/brokers/ccxt.py` & `lumibot-3.3.1/lumibot/brokers/ccxt.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,16 +171,25 @@
         into a position object"""
 
         symbol = position["currency"]
         hold = position["used"]
         available = position["free"]
         quantity = Decimal(position["total"])
 
-        if self.api.exchangeId == "binance":
+        # Check if symbol is in the currencies list
+        if symbol not in self.api.currencies:
+            logging.error(
+                f"The symbol {symbol} is not in the currencies list. "
+                f"Please check the symbol and the exchange currencies list."
+            )
+            precision = None
+        
+        elif self.api.exchangeId == "binance":
             precision = str(10 ** -self.api.currencies[symbol]["precision"])
+            
         else:
             precision = str(self.api.currencies[symbol]["precision"])
 
         asset = Asset(
             symbol=symbol,
             asset_type="crypto",
             precision=precision,
@@ -235,16 +244,20 @@
             )
 
     def _parse_broker_positions(self, broker_positions, strategy):
         """parse a list of broker positions into a
         list of position objects"""
         result = []
         for broker_position in broker_positions:
-            result.append(self._parse_broker_position(broker_position, strategy))
+            new_pos = self._parse_broker_position(broker_position, strategy)
 
+            # Check if the position is not None
+            if new_pos is not None:
+                result.append(new_pos)
+                
         return result
 
     def _pull_positions(self, strategy):
         """Get the account positions. return a list of
         position objects"""
         response = self._pull_broker_positions(strategy)
         result = self._parse_broker_positions(response, strategy.name)
@@ -465,18 +478,19 @@
 
         # Convert the price to Decimal.
         for price_type in [
             "limit_price",
             "stop_price",
         ]:
             if hasattr(order, price_type) and getattr(order, price_type) is not None:
+                precision_price = Decimal(str(10 ** -precision["price"])) if self.api.exchangeId == "binance" else precision["price"]
                 setattr(
                     order,
                     price_type,
-                    Decimal(getattr(order, price_type)).quantize(Decimal(str(precision["price"]))),
+                    Decimal(getattr(order, price_type)).quantize(Decimal(str(precision_price))),
                 )
             else:
                 continue
 
             try:
                 if limits["price"]["min"] is not None:
                     assert getattr(order, price_type) >= limits["price"]["min"]
```

### Comparing `lumibot-3.2.9/lumibot/brokers/interactive_brokers.py` & `lumibot-3.3.1/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/brokers/tradier.py` & `lumibot-3.3.1/lumibot/brokers/tradier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import traceback
 
 import pandas as pd
 from lumiwealth_tradier import Tradier as _Tradier
 from lumiwealth_tradier.base import TradierApiError
+from lumiwealth_tradier.orders import OrderLeg
 from termcolor import colored
 
 from lumibot.brokers import Broker
 from lumibot.data_sources.tradier_data import TradierData
 from lumibot.entities import Asset, Order, Position
 from lumibot.tools.helpers import create_options_symbol
 from lumibot.trading_builtins import PollingStream
@@ -102,14 +103,102 @@
 
         if not order.identifier:
             raise ValueError("Order identifier is not set, unable to cancel order. Did you remember to submit it?")
 
         # Cancel the order
         self.tradier.orders.cancel(order.identifier)
 
+    def submit_orders(self, orders, is_multileg=False, order_type="market", duration="day", price=None, tag=None):
+        """
+        Submit multiple orders to the broker. This function will submit the orders in the order they are provided.
+        If any order fails to submit, the function will stop submitting orders and return the last successful order.
+        """
+        # Check if the orders are empty
+        if not orders:
+            return
+        
+        # Check if it is a multi-leg order
+        if is_multileg:
+            # Submit the multi-leg order
+            return self._submit_multileg_order(orders, order_type, duration, price, tag)
+
+        # Submit each order
+        for order in orders:
+            self.submit_order(order)
+
+    def _submit_multileg_order(self, orders, order_type="market", duration="day", price=None, tag=None):
+        """
+        Submit a multi-leg order to Tradier. This function will submit the multi-leg order to Tradier.
+
+        Parameters
+        ----------
+        orders: list[Order]
+            List of orders to submit
+        order_type: str
+            The type of multi-leg order to submit. Valid values are ('market', 'debit', 'credit', 'even'). Default is 'market'.
+        duration: str
+            The duration of the order. Valid values are ('day', 'gtc', 'pre', 'post'). Default is 'day'.
+        price: float
+            The limit price for the order. Required for 'debit' and 'credit' order types.
+        tag: str
+            The tag to associate with the order.
+
+        Returns
+        -------
+            list of Order objects
+                List of processed order objects.
+        """
+
+        # Check if the order type is valid
+        if order_type not in ["market", "debit", "credit", "even"]:
+            raise ValueError(f"Invalid order type '{order_type}' for multi-leg order.")
+        
+        # Check if the duration is valid
+        if duration not in ["day", "gtc", "pre", "post"]:   
+            raise ValueError(f"Invalid duration {duration} for multi-leg order.")
+        
+        # Check if the price is required
+        if order_type in ["debit", "credit"] and price is None:
+            raise ValueError(f"Price is required for '{order_type}' order type.")
+
+        # Check that all the order objects have the same symbol
+        if len(set([order.asset.symbol for order in orders])) > 1:
+            raise ValueError("All orders in a multi-leg order must have the same symbol.")
+        
+        # Get the symbol from the first order
+        symbol = orders[0].asset.symbol
+
+        # Create the legs for the multi-leg order
+        legs = []
+        for order in orders:
+            # Create the options symbol
+            option_symbol = create_options_symbol(
+                order.asset.symbol, order.asset.expiration, order.asset.right, order.asset.strike
+            )
+
+            # Example leg: leg1 = OrderLeg(option_symbol=option_symbol_1, quantity=1, side='buy_to_open')
+            leg = OrderLeg(
+                option_symbol=option_symbol,
+                quantity=int(order.quantity), # Quantity for Tradier must be a positive integer
+                side=self._lumi_side2tradier(order),
+            )
+            legs.append(leg)
+
+        # Example assuming order_type and duration are required and correctly set
+        result = self.tradier.orders.multileg_order(
+            symbol=symbol,
+            order_type=order_type,
+            duration=duration,
+            legs=legs,
+            price=price,
+            tag=tag,
+        )
+
+        return result
+        
     def _submit_order(self, order: Order):
         """
         Do checking and input sanitization, then submit the order to the broker.
         Parameters
         ----------
         order: Order
             Order to submit to the broker
```

### Comparing `lumibot-3.2.9/lumibot/data_sources/alpaca_data.py` & `lumibot-3.3.1/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.3.1/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.3.1/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/ccxt_data.py` & `lumibot-3.3.1/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/data_source.py` & `lumibot-3.3.1/lumibot/data_sources/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,24 +108,30 @@
         float
             The last known price of the asset.
         """
         pass
 
     # ========Python datetime helpers======================
 
-    def get_datetime(self):
+    def get_datetime(self, adjust_for_delay=False):
         """
         Returns the current datetime in the default timezone
 
+        Parameters
+        ----------
+        adjust_for_delay : bool
+            Whether to adjust the current time for the delay. This is useful for paper trading data sources that
+            provide delayed data.
+
         Returns
         -------
         datetime
         """
         current_time = self.to_default_timezone(datetime.now())
-        if self._delay:
+        if adjust_for_delay and self._delay:
             current_time -= self._delay
         return current_time
 
     def get_timestamp(self):
         """
         Returns the current timestamp in the default timezone
         Returns
```

### Comparing `lumibot-3.2.9/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.3.1/lumibot/data_sources/data_source_backtesting.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,28 @@
         # Subtract one minute from the datetime_end so that the strategy stops right before the datetime_end
         self.datetime_end -= timedelta(minutes=1)
 
         # Legacy strategy.backtest code will always pass in a config even for DataSources that don't need it, so
         # catch it here and ignore it in this class. Child classes that need it should error check it themselves.
         self._config = config
 
-    def get_datetime(self):
+    def get_datetime(self, adjust_for_delay=False):
+        """
+        Get the current datetime of the backtest.
+
+        Parameters
+        ----------
+        adjust_for_delay: bool
+            Not used for backtesting data sources.  This parameter is only used for live data sources.
+
+        Returns
+        -------
+        datetime
+            The current datetime of the backtest.
+        """
         return self._datetime
 
     def get_datetime_range(self, length, timestep="minute", timeshift=None):
         backtesting_timeshift = datetime.now() - self._datetime
         if timeshift:
             backtesting_timeshift += timeshift
```

### Comparing `lumibot-3.2.9/lumibot/data_sources/exceptions.py` & `lumibot-3.3.1/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.3.1/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/pandas_data.py` & `lumibot-3.3.1/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/data_sources/tradier_data.py` & `lumibot-3.3.1/lumibot/data_sources/tradier_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -193,17 +193,20 @@
         return bars
 
     def get_last_price(self, asset, quote=None, exchange=None):
         """
         This function returns the last price of an asset.
         Parameters
         ----------
-        asset
-        quote
-        exchange
+        asset: Asset
+            The asset to get the last price for
+        quote: Asset
+            The quote asset to get the last price for (currently not used for Tradier)
+        exchange: str
+            The exchange to get the last price for (currently not used for Tradier)
 
         Returns
         -------
         float
            Price of the asset
         """
 
@@ -216,14 +219,54 @@
             )
         else:
             symbol = asset.symbol
 
         price = self.tradier.market.get_last_price(symbol)
         return price
 
+    def get_quote(self, asset, quote=None, exchange=None):
+        """
+        This function returns the quote of an asset.
+        Parameters
+        ----------
+        asset: Asset
+            The asset to get the quote for
+        quote: Asset
+            The quote asset to get the quote for (currently not used for Tradier)
+        exchange: str
+            The exchange to get the quote for (currently not used for Tradier)
+
+        Returns
+        -------
+        dict
+           Quote of the asset
+        """
+
+        if asset.asset_type == "option":
+            symbol = create_options_symbol(
+                asset.symbol,
+                asset.expiration,
+                asset.right,
+                asset.strike,
+            )
+        else:
+            symbol = asset.symbol
+
+        quotes_df = self.tradier.market.get_quotes([symbol])
+
+        # If the dataframe is empty, return an empty dictionary
+        if quotes_df is None or quotes_df.empty:
+            return {}
+        
+        # Get the quote from the dataframe and convert it to a dictionary
+        quote = quotes_df.iloc[0].to_dict()
+
+        # Return the quote
+        return quote
+
     def query_greeks(self, asset: Asset):
         """
         This function returns the greeks of an option as reported by the Tradier API.
 
         Parameters
         ----------
         asset : Asset
```

### Comparing `lumibot-3.2.9/lumibot/data_sources/yahoo_data.py` & `lumibot-3.3.1/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/asset.py` & `lumibot-3.3.1/lumibot/entities/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,19 +259,14 @@
             if self.expiration is None:
                 return False
             if self.strike is None:
                 return False
             if self.right is None:
                 return False
 
-        # If it's a future it should have an expiration date
-        if self.asset_type == "future":
-            if self.expiration is None:
-                return False
-
         return True
 
 
 class AssetsMapping(UserDict):
     def __init__(self, mapping):
         UserDict.__init__(self, mapping)
         symbols_mapping = {k.symbol: v for k, v in mapping.items()}
```

### Comparing `lumibot-3.2.9/lumibot/entities/bar.py` & `lumibot-3.3.1/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/bars.py` & `lumibot-3.3.1/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/data.py` & `lumibot-3.3.1/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/order.py` & `lumibot-3.3.1/lumibot/entities/order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/position.py` & `lumibot-3.3.1/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/entities/trading_fee.py` & `lumibot-3.3.1/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.3.1/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.3.1/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.3.1/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.3.1/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/stock_oco.py` & `lumibot-3.3.1/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/example_strategies/strangle.py` & `lumibot-3.3.1/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/strategies/_strategy.py` & `lumibot-3.3.1/lumibot/strategies/_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
 
         return result
 
     def _set_cash_position(self, cash: float):
         # Check if cash is in the list of positions yet
         for x in range(len(self.broker._filled_positions.get_list())):
             position = self.broker._filled_positions[x]
-            if position.asset == self.quote_asset:
+            if position is not None and position.asset == self.quote_asset:
                 position.quantity = cash
                 self.broker._filled_positions[x] = position
                 return
 
         # If not in positions, create a new position for cash
         position = Position(
             self._name,
@@ -683,23 +683,31 @@
 
         if show_tearsheet:
             save_tearsheet = True
 
         if self._strategy_returns_df is None:
             self.logger.warning("Cannot create a tearsheet because the strategy returns are missing")
         else:
+            # Get the strategy parameters
+            strategy_parameters = self.parameters
+
+            # Remove pandas_data from the strategy parameters if it exists
+            if "pandas_data" in strategy_parameters:
+                del strategy_parameters["pandas_data"]
+
             strat_name = self._name if self._name is not None else "Strategy"
             create_tearsheet(
                 self._strategy_returns_df,
                 strat_name,
                 tearsheet_file,
                 self._benchmark_returns_df,
                 self._benchmark_asset,
                 show_tearsheet,
                 risk_free_rate=self.risk_free_rate,
+                strategy_parameters=strategy_parameters,
             )
 
     @classmethod
     def run_backtest(
         cls,
         *args,
         minutes_before_closing=5,
```

### Comparing `lumibot-3.2.9/lumibot/strategies/strategy.py` & `lumibot-3.3.1/lumibot/strategies/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1489,29 +1489,47 @@
             self.logger.error(
                 "Cannot submit a None order, please check to make sure that you have actually created an order before submitting."
             )
             return
 
         return self.broker.submit_order(order)
 
-    def submit_orders(self, orders):
+    def submit_orders(self, orders, **kwargs):
         """Submit a list of orders
 
         Submits a list of orders for processing by the active broker.
 
         Parameters
         ---------
         orders : list of orders
             A list of order objects containing the asset and
             instructions for the orders.
-
+        is_multileg : bool
+            Tradier only.
+            A boolean value to indicate if the orders are part of one multileg order.
+            Currently this is only available for Tradier.
+        order_type : str
+            Tradier only.
+            The order type for the multileg order. Possible values are:
+            ('market', 'debit', 'credit', 'even'). Default is 'market'.
+        duration : str
+            Tradier only.
+            The duration for the multileg order. Possible values are:
+            ('day', 'gtc', 'pre', 'post'). Default is 'day'.
+        price : float
+            Tradier only.
+            The limit price for the multileg order. Required for 'debit' and 'credit' order types.
+        tag : str
+            Tradier only.
+            A tag for the multileg order.
+        
         Returns
         -------
-        list of orders
-            List of processed order object.
+        list of Order objects
+            List of processed order objects.
 
         Example
         -------
         >>> # For 2 market buy orders
         >>> order1 = self.create_order("SPY", 100, "buy")
         >>> order2 = self.create_order("TLT", 200, "buy")
         >>> self.submit_orders([order1, order2])
@@ -1600,15 +1618,15 @@
         >>> order2 = self.create_order(asset_ETH, 10, "buy", quote=asset_quote)
         >>> self.submit_order([order1, order2])
         >>> or...
         >>> order1 = self.create_order((asset_BTC, asset_quote), 0.1, "buy")
         >>> order2 = self.create_order((asset_ETH, asset_quote), 10, "buy")
         >>> self.submit_order([order1, order2])
         """
-        return self.broker.submit_orders(orders)
+        return self.broker.submit_orders(orders, **kwargs)
 
     def wait_for_order_registration(self, order):
         """Wait for the order to be registered by the broker
 
         Parameters
         ----------
         order : Order object
@@ -1882,14 +1900,39 @@
                 exchange=exchange,
                 # should_use_last_close=should_use_last_close,
             )
         except Exception as e:
             self.log_message(f"Could not get last price for {asset}", color="red")
             self.log_message(f"{e}")
             return None
+        
+    def get_quote(self, asset):
+        """Get a quote for the asset.
+
+        NOTE: This currently only works with Tradier. It does not work with backtetsing or other brokers.
+        
+        Parameters
+        ----------
+        asset : Asset object
+            The asset for which the quote is needed.
+            
+        Returns
+        -------
+        dict
+            A dictionary with the quote information, eg. bid, ask, etc.
+        """
+
+        asset = self._sanitize_user_asset(asset)
+
+        # Check if the broker has the get_quote method (not all brokers do)
+        if not hasattr(self.broker.data_source, "get_quote"):
+            self.log_message("Broker does not have a get_quote method.")
+            return None
+
+        return self.broker.data_source.get_quote(asset)
 
     def get_tick(self, asset):
         """Takes an Asset and returns the last known price"""
         # TODO: Should this function be depricated? This appears to be an IBKR-only thing.
         asset = self._sanitize_user_asset(asset)
         return self.broker._get_tick(asset)
 
@@ -1980,14 +2023,41 @@
         -------
         >>> # Will return the option chains for SPY
         >>> asset = "SPY"
         >>> chains = self.get_chains(asset)
         """
         asset = self._sanitize_user_asset(asset)
         return self.broker.get_chains(asset)
+    
+    def get_next_trading_day(self, date, exchange='NYSE'):
+        """
+        Finds the next trading day for the given date and exchange.
+        
+        Parameters:
+            date (str): The date from which to find the next trading day, in 'YYYY-MM-DD' format.
+            exchange (str): The exchange calendar to use, default is 'NYSE'.
+            
+        Returns:
+            next_trading_day (datetime.date): The next trading day after the given date.
+        """
+        
+        # Load the specified market calendar
+        calendar = mcal.get_calendar(exchange)
+        
+        # Convert the input string date to pandas Timestamp
+        date_timestamp = pd.Timestamp(date)
+        
+        # Get the next trading day. The schedule is inclusive of the start_date when the market is open on this day.
+        # Hence, we add 1 day to the start_date to ensure we start checking from the day after.
+        schedule = calendar.schedule(start_date=date_timestamp + pd.Timedelta(days=1), end_date=date_timestamp + pd.Timedelta(days=10))
+        
+        # The next trading day is the first entry in the schedule
+        next_trading_day = schedule.index[0].date()
+        
+        return next_trading_day
 
     def get_chain(self, chains, exchange="SMART"):
         """Returns option chain for a particular exchange.
 
         Takes in a full set of chains for all the exchanges and returns
         on chain for a given exchange. The full chains are returned
         from `get_chains` method.
@@ -2315,29 +2385,29 @@
         -------
         >>> # Will return the pytz object of the data source
         >>> pytz = self.pytz
         >>> self.log_message(f"pytz: {pytz}")
         """
         return self.broker.data_source.DEFAULT_PYTZ
 
-    def get_datetime(self):
+    def get_datetime(self, adjust_for_delay=False):
         """Returns the current datetime according to the data source. In a backtest this will be the current bar's datetime. In live trading this will be the current datetime on the exchange.
 
         Returns
         -------
         datetime.datetime
             The current datetime.
 
         Example
         -------
         >>> # Will return the current datetime
         >>> datetime = self.get_datetime()
         >>> self.log_message(f"The current datetime is {datetime}")
         """
-        return self.broker.data_source.get_datetime()
+        return self.broker.data_source.get_datetime(adjust_for_delay=adjust_for_delay)
 
     def get_timestamp(self):
         """Returns the current timestamp according to the data source. In a backtest this will be the current bar's timestamp. In live trading this will be the current timestamp on the exchange.
 
         Returns
         -------
         int
@@ -3719,40 +3789,41 @@
         if response.status_code == 200 or response.status_code == 204:
             self.logger.info("Discord message sent successfully.")
         else:
             self.logger.error(
                 f"Failed to send message to Discord. Status code: {response.status_code}, message: {response.text}"
             )
 
-    def send_spark_chart_to_discord(self, stats_df, portfolio_value, now):
+    def send_spark_chart_to_discord(self, stats_df, portfolio_value, now, days=180):
         # Check if we are in backtesting mode, if so, don't send the message
         if self.is_backtesting:
             return
 
-        # Only keep the stats for the past week
-        stats_df = stats_df.loc[stats_df["datetime"] >= (now - pd.Timedelta(days=7))]
+        # Only keep the stats for the past X days
+        stats_df = stats_df.loc[stats_df["datetime"] >= (now - pd.Timedelta(days=days))]
 
         # Set the default color
         color = "black"
 
         # Check what return we made over the past week
         if stats_df.shape[0] > 0:
             # Resanple the stats dataframe to daily but keep the datetime column
             stats_df = stats_df.resample("D", on="datetime").last().reset_index()
 
             # Remove nan values
             stats_df = stats_df.dropna()
 
-            # Get the portfolio value 7 days ago
-            portfolio_value_7_days_ago = stats_df.iloc[0]["portfolio_value"]
+            # Get the portfolio value at the beginning of the dataframe
+            portfolio_value_start = stats_df.iloc[0]["portfolio_value"]
+
             # Calculate the return over the past 7 days
-            return_7_days = ((portfolio_value / portfolio_value_7_days_ago) - 1) * 100
+            total_return = ((portfolio_value / portfolio_value_start) - 1) * 100
 
             # Check if we made a positive return, if so, set the color to green, otherwise set it to red
-            if return_7_days > 0:
+            if total_return > 0:
                 color = "green"
             else:
                 color = "red"
 
         # Plotting the DataFrame
         plt.figure()
```

### Comparing `lumibot-3.2.9/lumibot/strategies/strategy_executor.py` & `lumibot-3.3.1/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/__init__.py` & `lumibot-3.3.1/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/black_scholes.py` & `lumibot-3.3.1/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/ccxt_data_store.py` & `lumibot-3.3.1/lumibot/tools/ccxt_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             timeframe (str): 1m, 1d etc.
         """
         cache_file = self.get_cache_file_name(symbol, timeframe)
 
         with duckdb.connect(cache_file) as con:
             con.execute("""CREATE TABLE IF NOT EXISTS candles (
                             datetime DATETIME,
-                            open FLOAT, high FLOAT, low FLOAT, close FLOAT, volume INTEGER, missing INTEGER)""")
+                            open DECIMAL, high DECIMAL, low DECIMAL, close DECIMAL, volume DECIMAL, missing INTEGER)""")
 
             # cache ranges table
             con.execute("""CREATE TABLE  IF NOT EXISTS cache_dt_ranges (
                             id STRING ,
                             start_dt DATETIME ,
                             end_dt DATETIME)""")
             # insert df to cache db
@@ -502,8 +502,8 @@
     # cache ranges updated
     start = datetime(2023, 3, 9)
     end = datetime(2023, 3, 17)
     df = cache.download_ohlcv(symbol,timeframe,start,end)
     print(f"data length: {len(df)}")
 
     df = cache.get_data_from_cache("SOL/USDT","1m",datetime(2000,1,1),datetime(2025,1,1))
-    print(f"total data length: {len(df)}")
+    print(f"total data length: {len(df)}")
```

### Comparing `lumibot-3.2.9/lumibot/tools/decorators.py` & `lumibot-3.3.1/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/helpers.py` & `lumibot-3.3.1/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/indicators.py` & `lumibot-3.3.1/lumibot/tools/indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,14 +635,15 @@
     strategy_df: pd.DataFrame,
     strat_name: str,
     tearsheet_file: str,
     benchmark_df: pd.DataFrame,
     benchmark_asset,  # This is causing a circular import: Asset,
     show_tearsheet: bool,
     risk_free_rate: float,
+    strategy_parameters: dict = None,
 ):
     # If show tearsheet is False, then we don't want to open the tearsheet in the browser
     if not show_tearsheet:
         print("show_tearsheet is False, not creating the tearsheet file.")
         return
 
     print("\nCreating tearsheet...")
@@ -713,14 +714,15 @@
         qs.reports.html(
             df_final["strategy"],
             df_final["benchmark"],
             title=title,
             output=tearsheet_file,
             download_filename=tearsheet_file,  # Consider if you need a different name for clarity
             rf=risk_free_rate,
+            parameters=strategy_parameters,
         )
 
     if show_tearsheet:
         url = "file://" + os.path.abspath(str(tearsheet_file))
         webbrowser.open(url)
```

### Comparing `lumibot-3.2.9/lumibot/tools/lumibot_time.py` & `lumibot-3.3.1/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/pandas.py` & `lumibot-3.3.1/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/polygon_helper.py` & `lumibot-3.3.1/lumibot/tools/polygon_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
     If the list of splits for a stock have changed then we need to invalidate its cache
     because all of the prices will have changed (because we're using split adjusted prices).
     Get the splits data from Polygon only once per day per stock.
     Use the timestamp on the splits feather file to determine if we need to get the splits again.
     When invalidating we delete the cache file and return force_cache_update=True too.
     """
-    if asset.asset_type != Asset.AssetType.STOCK:
+    if asset.asset_type not in [Asset.AssetType.STOCK, Asset.AssetType.OPTION]:
         return force_cache_update
     cached_splits = pd.DataFrame()
     splits_file_stale = True
     splits_file_path = Path(str(cache_file).rpartition(".feather")[0] + "_splits.feather")
     if splits_file_path.exists():
         splits_file_stale = datetime.fromtimestamp(splits_file_path.stat().st_mtime).date() != date.today()
         if splits_file_stale:
```

### Comparing `lumibot-3.2.9/lumibot/tools/types.py` & `lumibot-3.3.1/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/tools/yahoo_helper.py` & `lumibot-3.3.1/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/traders/trader.py` & `lumibot-3.3.1/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.3.1/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot/trading_builtins/safe_list.py` & `lumibot-3.3.1/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot.egg-info/PKG-INFO` & `lumibot-3.3.1/lumibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.2.9
+Version: 3.3.1
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,24 +30,24 @@
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
 Requires-Dist: scipy==1.10.1
 Requires-Dist: ipython
-Requires-Dist: quantstats-lumi>=0.1.10
+Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
-Requires-Dist: ccxt==4.2.50
+Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
 Requires-Dist: appdirs
 Requires-Dist: pyarrow
 Requires-Dist: tqdm
-Requires-Dist: lumiwealth-tradier>=0.1.6
+Requires-Dist: lumiwealth-tradier>=0.1.7
 Requires-Dist: pytz
 Requires-Dist: psycopg2-binary
 Requires-Dist: exchange_calendars>=4.5.2
 Requires-Dist: duckdb
 Requires-Dist: uuid
 Requires-Dist: tabulate
```

### Comparing `lumibot-3.2.9/lumibot.egg-info/SOURCES.txt` & `lumibot-3.3.1/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/lumibot.egg-info/requires.txt` & `lumibot-3.3.1/lumibot.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 flask-security
 marshmallow-sqlalchemy
 email_validator
 bcrypt
 pytest
 scipy==1.10.1
 ipython
-quantstats-lumi>=0.1.10
+quantstats-lumi>=0.2.0
 python-dotenv
-ccxt==4.2.50
+ccxt==4.2.85
 termcolor
 jsonpickle
 apscheduler==3.10.4
 appdirs
 pyarrow
 tqdm
-lumiwealth-tradier>=0.1.6
+lumiwealth-tradier>=0.1.7
 pytz
 psycopg2-binary
 exchange_calendars>=4.5.2
 duckdb
 uuid
 tabulate
```

### Comparing `lumibot-3.2.9/pyproject.toml` & `lumibot-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/setup.cfg` & `lumibot-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/setup.py` & `lumibot-3.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.2.9",
+    version="3.3.1",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
@@ -33,24 +33,24 @@
         "flask-security",
         "marshmallow-sqlalchemy",
         "email_validator",
         "bcrypt",
         "pytest",
         "scipy==1.10.1",  # Newer versions of scipy are currently causing issues
         "ipython",  # required for quantstats, but not in their dependency list for some reason
-        "quantstats-lumi>=0.1.10",
+        "quantstats-lumi>=0.2.0",
         "python-dotenv",  # Secret Storage
-        "ccxt==4.2.50",
+        "ccxt==4.2.85",
         "termcolor",
         "jsonpickle",
         "apscheduler==3.10.4",
         "appdirs",
         "pyarrow",
         "tqdm",
-        "lumiwealth-tradier>=0.1.6",
+        "lumiwealth-tradier>=0.1.7",
         "pytz",
         "psycopg2-binary",
         "exchange_calendars>=4.5.2",
         "duckdb",
         "uuid",
         "tabulate",
     ],
```

### Comparing `lumibot-3.2.9/tests/backtest/test_example_strategies.py` & `lumibot-3.3.1/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.3.1/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/backtest/test_polygon.py` & `lumibot-3.3.1/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/backtest/test_strategy_executor.py` & `lumibot-3.3.1/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/backtest/test_yahoo.py` & `lumibot-3.3.1/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_alpaca.py` & `lumibot-3.3.1/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_alpaca_old.py` & `lumibot-3.3.1/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_asset.py` & `lumibot-3.3.1/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_backtesting_broker.py` & `lumibot-3.3.1/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_ccxt.py` & `lumibot-3.3.1/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_ccxt_store.py` & `lumibot-3.3.1/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_interactive_brokers.py` & `lumibot-3.3.1/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_order.py` & `lumibot-3.3.1/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_polygon_helper.py` & `lumibot-3.3.1/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_strategy_methods.py` & `lumibot-3.3.1/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.2.9/tests/test_tradier.py` & `lumibot-3.3.1/tests/test_tradier.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 @pytest.mark.apitest
 class TestTradierDataAPI:
     """
     API Tests skipped by default. To run all API tests, use the following command:
     python -m pytest -m apitest
     """
     def test_basics(self):
-        tdata = TradierData(account_number="1234", access_token="a1b2c3", paper=True)
-        assert tdata._account_number == "1234"
+        tdata = TradierData(account_number=TRADIER_ACCOUNT_ID_PAPER, access_token=TRADIER_TOKEN_PAPER, paper=True)
+        assert tdata._account_number == TRADIER_ACCOUNT_ID_PAPER
 
     def test_get_last_price(self, tradier_ds):
         asset = Asset("AAPL")
         price = tradier_ds.get_last_price(asset)
         assert isinstance(price, float)
         assert price > 0.0
-
+               
     def test_get_chains(self, tradier_ds):
         asset = Asset("SPY")
         chain = tradier_ds.get_chains(asset)
         assert isinstance(chain, dict)
         assert 'Chains' in chain
         assert "CALL" in chain['Chains']
         assert len(chain['Chains']['CALL']) > 0
@@ -61,14 +61,27 @@
         option_asset = Asset(asset.symbol, asset_type='option', expiration=expir_date, strike=strike, right='CALL')
         greeks = tradier_ds.query_greeks(option_asset)
         assert greeks
         assert 'delta' in greeks
         assert 'gamma' in greeks
         assert greeks['delta'] > 0
 
+    def test_get_quote(self, tradier_ds):
+        asset = Asset("AAPL")
+        quote = tradier_ds.get_quote(asset)
+        assert isinstance(quote, dict)
+        assert 'last' in quote
+        assert 'bid' in quote
+        assert 'ask' in quote
+        assert 'volume' in quote
+        assert 'open' in quote
+        assert 'high' in quote
+        assert 'low' in quote
+        assert 'close' in quote
+
 
 @pytest.mark.apitest
 class TestTradierBrokerAPI:
     """
     API Tests skipped by default. To run all API tests, use the following command:
     python -m pytest -m apitest
     """
@@ -85,15 +98,14 @@
         assert submitted_order.status == "submitted"
         assert submitted_order.identifier > 0
 
         # Cancel the testing order once we are done
         # How do we check this? Who changes the Lumibot order status to "canceled"?
         tradier.cancel_order(submitted_order)
 
-
 class TestTradierBroker:
     """
     Unit tests for the Tradier broker. These tests do not require any API calls.
     """
     def test_basics(self):
         broker = Tradier(account_number="1234", access_token="a1b2c3", paper=True)
         assert broker.name == "Tradier"
```

