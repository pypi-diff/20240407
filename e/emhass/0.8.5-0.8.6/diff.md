# Comparing `tmp/emhass-0.8.5.tar.gz` & `tmp/emhass-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emhass-0.8.5.tar", last modified: Mon Apr  1 21:38:57 2024, max compression
+gzip compressed data, was "emhass-0.8.6.tar", last modified: Sun Apr  7 11:53:22 2024, max compression
```

## Comparing `emhass-0.8.5.tar` & `emhass-0.8.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.183555 emhass-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-01 21:38:53.000000 emhass-0.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-01 21:38:53.000000 emhass-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-01 21:38:53.000000 emhass-0.8.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 21:38:53.000000 emhass-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:38:53.000000 emhass-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-01 21:38:57.183555 emhass-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33584 2024-04-01 21:38:53.000000 emhass-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.171555 emhass-0.8.5/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_load_cost_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_load_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_prod_price_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_train_load_clustering.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_train_load_forecast.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-01 21:38:53.000000 emhass-0.8.5/data/data_weather_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_latest.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_cost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_profit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-04-01 21:38:53.000000 emhass-0.8.5/data/opt_res_perfect_optim_self-consumption.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_df_final.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_get_data_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_scrapper_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_solarforecast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-01 21:38:53.000000 emhass-0.8.5/data/test_response_solcast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-01 21:38:53.000000 emhass-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:38:57.183555 emhass-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-01 21:38:53.000000 emhass-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.167555 emhass-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.175555 emhass-0.8.5/src/emhass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37462 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.175555 emhass-0.8.5/src/emhass/data/
--rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/data/cec_inverters.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/data/cec_modules.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)    43796 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    37197 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/advanced.html
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/basic.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/emhass_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/emhass_logo_short.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/img/feather-sprite.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/script.js
--rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/src/emhass/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (127)    42394 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-01 21:38:53.000000 emhass-0.8.5/src/emhass/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.183555 emhass-0.8.5/src/emhass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:38:57.000000 emhass-0.8.5/src/emhass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:38:57.179556 emhass-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29703 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-01 21:38:53.000000 emhass-0.8.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-07 11:53:19.000000 emhass-0.8.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-07 11:53:19.000000 emhass-0.8.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 11:53:19.000000 emhass-0.8.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 11:53:19.000000 emhass-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 11:53:19.000000 emhass-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-07 11:53:22.849832 emhass-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33584 2024-04-07 11:53:19.000000 emhass-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.841832 emhass-0.8.6/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_load_cost_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_load_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_prod_price_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_train_load_clustering.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_train_load_forecast.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 11:53:19.000000 emhass-0.8.6/data/data_weather_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_latest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_cost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_profit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-04-07 11:53:19.000000 emhass-0.8.6/data/opt_res_perfect_optim_self-consumption.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_df_final.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_get_data_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_scrapper_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_solarforecast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-07 11:53:19.000000 emhass-0.8.6/data/test_response_solcast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-07 11:53:19.000000 emhass-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:53:22.849832 emhass-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-07 11:53:19.000000 emhass-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.837832 emhass-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.841832 emhass-0.8.6/src/emhass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37580 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/data/cec_inverters.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/data/cec_modules.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)    45704 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37197 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/advanced.html
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/basic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/emhass_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/emhass_logo_short.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/img/feather-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.845832 emhass-0.8.6/src/emhass/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42394 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-07 11:53:19.000000 emhass-0.8.6/src/emhass/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/src/emhass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 11:53:22.000000 emhass-0.8.6/src/emhass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:53:22.849832 emhass-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30769 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-07 11:53:19.000000 emhass-0.8.6/tests/test_utils.py
```

### Comparing `emhass-0.8.5/CHANGELOG.md` & `emhass-0.8.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.8.6 - 2024-04-07
+### Fix
+- Fixed bug from forecast out method related to issue 240
+- Fix patch for some issues with package file paths
+
 ## 0.8.5 - 2024-04-01
 ### Improvement
 - Simplified fetch urls to relatives
 - Improved code for passed forecast data error handling in utils.py
 - Added new tests for forecast longer than 24h by changing parameter `delta_forecast`
 - Added new files for updated PV modules and inverters database for use with PVLib
 - Added a new webapp to help configuring modules and inverters: [https://emhass-pvlib-database.streamlit.app/](https://emhass-pvlib-database.streamlit.app/)
```

### Comparing `emhass-0.8.5/CODE_OF_CONDUCT.md` & `emhass-0.8.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/CONTRIBUTING.md` & `emhass-0.8.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/LICENSE` & `emhass-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/PKG-INFO` & `emhass-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.5
+Version: 0.8.6
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.5 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.8.6 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
```

### Comparing `emhass-0.8.5/README.md` & `emhass-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_load_cost_forecast.csv` & `emhass-0.8.6/data/data_load_cost_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_load_forecast.csv` & `emhass-0.8.6/data/data_load_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_prod_price_forecast.csv` & `emhass-0.8.6/data/data_prod_price_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_train_load_clustering.pkl` & `emhass-0.8.6/data/data_train_load_clustering.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_train_load_forecast.pkl` & `emhass-0.8.6/data/data_train_load_forecast.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/data_weather_forecast.csv` & `emhass-0.8.6/data/data_weather_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/opt_res_latest.csv` & `emhass-0.8.6/data/opt_res_latest.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/opt_res_perfect_optim_cost.csv` & `emhass-0.8.6/data/opt_res_perfect_optim_cost.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/opt_res_perfect_optim_profit.csv` & `emhass-0.8.6/data/opt_res_perfect_optim_profit.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/opt_res_perfect_optim_self-consumption.csv` & `emhass-0.8.6/data/opt_res_perfect_optim_self-consumption.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/test_df_final.pkl` & `emhass-0.8.6/data/test_df_final.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/test_response_get_data_get_method.pbz2` & `emhass-0.8.6/data/test_response_get_data_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/test_response_scrapper_get_method.pbz2` & `emhass-0.8.6/data/test_response_scrapper_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/test_response_solarforecast_get_method.pbz2` & `emhass-0.8.6/data/test_response_solarforecast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/data/test_response_solcast_get_method.pbz2` & `emhass-0.8.6/data/test_response_solcast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/setup.py` & `emhass-0.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='emhass',  # Required
-    version='0.8.5',  # Required
+    version='0.8.6',  # Required
     description='An Energy Management System for Home Assistant',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/davidusb-geek/emhass',  # Optional
     author='David HERNANDEZ',  # Optional
     author_email='davidusb@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `emhass-0.8.5/src/emhass/command_line.py` & `emhass-0.8.6/src/emhass/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,20 @@
         if get_data_from_file:
             with open(pathlib.Path(base_path) / 'data' / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
         else:
             days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             if not rh.get_data(days_list, var_list,
-                        minimal_response=False, significant_changes_only=False):
+                               minimal_response=False, significant_changes_only=False):
                 return False 
         if not rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
-                        set_zero_min = retrieve_hass_conf['set_zero_min'], 
-                        var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
-                        var_interp = retrieve_hass_conf['var_interp']):
+                               set_zero_min = retrieve_hass_conf['set_zero_min'], 
+                               var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
+                               var_interp = retrieve_hass_conf['var_interp']):
             return False
         df_input_data = rh.df_final.copy()
         # What we don't need for this type of action
         P_PV_forecast, P_load_forecast, df_input_data_dayahead = None, None, None
     elif set_type == "dayahead-optim":
         # Get PV and load forecasts
         df_weather = fcst.get_weather_forecast(method=optim_conf['weather_forecast_method'])
@@ -109,20 +109,20 @@
         if get_data_from_file:
             with open(pathlib.Path(base_path) / 'data' / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
         else:
             days_list = utils.get_days_list(1)
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             if not rh.get_data(days_list, var_list,
-                        minimal_response=False, significant_changes_only=False):
+                               minimal_response=False, significant_changes_only=False):
                 return False
         if not rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
-                        set_zero_min = retrieve_hass_conf['set_zero_min'], 
-                        var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
-                        var_interp = retrieve_hass_conf['var_interp']):
+                               set_zero_min = retrieve_hass_conf['set_zero_min'], 
+                               var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
+                               var_interp = retrieve_hass_conf['var_interp']):
             return False
         df_input_data = rh.df_final.copy()
         # Get PV and load forecasts
         df_weather = fcst.get_weather_forecast(method=optim_conf['weather_forecast_method'])
         P_PV_forecast = fcst.get_power_from_weather(df_weather, set_mix_forecast=True, df_now=df_input_data)
         P_load_forecast = fcst.get_load_forecast(method=optim_conf['load_forecast_method'], set_mix_forecast=True, df_now=df_input_data)
         df_input_data_dayahead = pd.concat([P_PV_forecast, P_load_forecast], axis=1)
@@ -197,17 +197,19 @@
     :rtype: pd.DataFrame
 
     """
     logger.info("Performing perfect forecast optimization")
     # Load cost and prod price forecast
     df_input_data = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data'], 
-        method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'])
+        method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'],
+        list_and_perfect=True)
     df_input_data = input_data_dict['fcst'].get_prod_price_forecast(
-        df_input_data, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'])
+        df_input_data, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'],
+        list_and_perfect=True)
     opt_res = input_data_dict['opt'].perform_perfect_forecast_optim(df_input_data, input_data_dict['days_list'])
     # Save CSV file for analysis
     if save_data_to_file:
         filename = 'opt_res_perfect_optim_'+input_data_dict['costfun']+'.csv'
     else: # Just save the latest optimization results
         filename = 'opt_res_latest.csv'
     if not debug:
```

### Comparing `emhass-0.8.5/src/emhass/data/cec_inverters.pbz2` & `emhass-0.8.6/src/emhass/data/cec_inverters.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/data/cec_modules.pbz2` & `emhass-0.8.6/src/emhass/data/cec_modules.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/forecast.py` & `emhass-0.8.6/src/emhass/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pvlib.location import Location
 from pvlib.modelchain import ModelChain
 from pvlib.temperature import TEMPERATURE_MODEL_PARAMETERS
 from pvlib.irradiance import disc
 
 from emhass.retrieve_hass import RetrieveHass
 from emhass.machine_learning_forecaster import MLForecaster
-from emhass.utils import get_days_list, get_root
+from emhass.utils import get_days_list, get_root, set_df_index_freq
 
 
 class Forecast(object):
     r"""
     Generate weather, load and costs forecasts needed as inputs to the optimization.
     
     In EMHASS we have basically 4 forecasts to deal with:
@@ -483,16 +483,17 @@
                                            freq=self.freq).round(self.freq, ambiguous='infer', nonexistent='shift_forward')
         if self.params is not None:
             if 'prediction_horizon' in list(self.params['passed_data'].keys()):
                 if self.params['passed_data']['prediction_horizon'] is not None:
                     forecast_dates_csv = forecast_dates_csv[0:self.params['passed_data']['prediction_horizon']]
         return forecast_dates_csv
     
-    def get_forecast_out_from_csv(self, df_final: pd.DataFrame, forecast_dates_csv: pd.date_range,
-                                  csv_path: str, data_list: Optional[list] = None) -> pd.DataFrame:
+    def get_forecast_out_from_csv_or_list(self, df_final: pd.DataFrame, forecast_dates_csv: pd.date_range,
+                                          csv_path: str, data_list: Optional[list] = None, 
+                                          list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
         r"""
         Get the forecast data as a DataFrame from a CSV file. 
         
         The data contained in the CSV file should be a 24h forecast with the same frequency as 
         the main 'freq' parameter in the configuration file. The timestamp will not be used and 
         a new DateTimeIndex is generated to fit the timestamp index of the input data in 'df_final'.
         
@@ -502,42 +503,75 @@
         :type forecast_dates_csv: pd.date_range
         :param csv_path: The path to the CSV file
         :type csv_path: str
         :return: The data from the CSV file
         :rtype: pd.DataFrame
 
         """
-        days_list = df_final.index.day.unique().tolist()
         if csv_path is None:
             data_dict = {'ts':forecast_dates_csv, 'yhat':data_list}
             df_csv = pd.DataFrame.from_dict(data_dict)
             df_csv.index = forecast_dates_csv
             df_csv.drop(['ts'], axis=1, inplace=True)
+            df_csv = set_df_index_freq(df_csv)
+            if list_and_perfect:
+                days_list = df_final.index.day.unique().tolist()
+            else:
+                days_list = df_csv.index.day.unique().tolist()
         else:
             load_csv_file_path = self.root + csv_path
             df_csv = pd.read_csv(load_csv_file_path, header=None, names=['ts', 'yhat'])
             df_csv.index = forecast_dates_csv
             df_csv.drop(['ts'], axis=1, inplace=True)
+            df_csv = set_df_index_freq(df_csv)
+            days_list = df_final.index.day.unique().tolist()
         forecast_out = pd.DataFrame()
         for day in days_list:
-            first_elm_index = [i for i, x in enumerate(df_final.index.day == day) if x][0]
-            last_elm_index = [i for i, x in enumerate(df_final.index.day == day) if x][-1]
-            fcst_index = pd.date_range(start=df_final.index[first_elm_index],
-                                       end=df_final.index[last_elm_index], 
-                                       freq=df_final.index.freq)
-            first_hour = str(df_final.index[first_elm_index].hour)+":"+str(df_final.index[first_elm_index].minute)
-            last_hour = str(df_final.index[last_elm_index].hour)+":"+str(df_final.index[last_elm_index].minute)
+            if csv_path is None:
+                if list_and_perfect:
+                    df_tmp = copy.deepcopy(df_final)
+                else:
+                    df_tmp = copy.deepcopy(df_csv)
+            else:
+                df_tmp = copy.deepcopy(df_final)
+            first_elm_index = [i for i, x in enumerate(df_tmp.index.day == day) if x][0]
+            last_elm_index = [i for i, x in enumerate(df_tmp.index.day == day) if x][-1]
+            fcst_index = pd.date_range(start=df_tmp.index[first_elm_index],
+                                    end=df_tmp.index[last_elm_index], 
+                                    freq=df_tmp.index.freq)
+            first_hour = str(df_tmp.index[first_elm_index].hour)+":"+str(df_tmp.index[first_elm_index].minute)
+            last_hour = str(df_tmp.index[last_elm_index].hour)+":"+str(df_tmp.index[last_elm_index].minute)
             if len(forecast_out) == 0:
-                forecast_out = pd.DataFrame(
-                    df_csv.between_time(first_hour, last_hour).values,
-                    index=fcst_index)
-            else:
-                forecast_tp = pd.DataFrame(
-                    df_csv.between_time(first_hour, last_hour).values,
-                    index=fcst_index)
+                if csv_path is None:
+                    if list_and_perfect:
+                        forecast_out = pd.DataFrame(
+                            df_csv.between_time(first_hour, last_hour).values,
+                            index=fcst_index)
+                    else:
+                        forecast_out = pd.DataFrame(
+                            df_csv.loc[fcst_index,:].between_time(first_hour, last_hour).values,
+                            index=fcst_index)
+                else:
+                    forecast_out = pd.DataFrame(
+                        df_csv.between_time(first_hour, last_hour).values,
+                        index=fcst_index)
+            else:
+                if csv_path is None:
+                    if list_and_perfect:
+                        forecast_tp = pd.DataFrame(
+                            df_csv.between_time(first_hour, last_hour).values,
+                            index=fcst_index)
+                    else:
+                        forecast_tp = pd.DataFrame(
+                            df_csv.loc[fcst_index,:].between_time(first_hour, last_hour).values,
+                            index=fcst_index)
+                else:
+                    forecast_tp = pd.DataFrame(
+                        df_csv.between_time(first_hour, last_hour).values,
+                        index=fcst_index)
                 forecast_out = pd.concat([forecast_out, forecast_tp], axis=0)
         return forecast_out
     
     def get_load_forecast(self, days_min_load_forecast: Optional[int] = 3, method: Optional[str] = 'naive',
                           csv_path: Optional[str] = "/data/data_load_forecast.csv",
                           set_mix_forecast:Optional[bool] = False, df_now:Optional[pd.DataFrame] = pd.DataFrame(),
                           use_last_window: Optional[bool] = True, mlf: Optional[MLForecaster] = None,
@@ -664,15 +698,16 @@
         if set_mix_forecast:
             P_Load_forecast = Forecast.get_mix_forecast(
                 df_now, P_Load_forecast, 
                 self.params['passed_data']['alpha'], self.params['passed_data']['beta'], self.var_load_new)
         return P_Load_forecast
     
     def get_load_cost_forecast(self, df_final: pd.DataFrame, method: Optional[str] = 'hp_hc_periods',
-                               csv_path: Optional[str] = "data_load_cost_forecast.csv") -> pd.DataFrame:
+                               csv_path: Optional[str] = "data_load_cost_forecast.csv",
+                               list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
         r"""
         Get the unit cost for the load consumption based on multiple tariff \
         periods. This is the cost of the energy from the utility in a vector \
         sampled at the fixed freq value.
         
         :param df_final: The DataFrame containing the input data.
         :type df_final: pd.DataFrame
@@ -694,39 +729,40 @@
             for key, period_hp in self.optim_conf['list_hp_periods'].items():
                 list_df_hp.append(df_final[self.var_load_cost].between_time(
                     period_hp[0]['start'], period_hp[1]['end']))
             for df_hp in list_df_hp:
                 df_final.loc[df_hp.index, self.var_load_cost] = self.optim_conf['load_cost_hp']
         elif method == 'csv':
             forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
-            forecast_out = self.get_forecast_out_from_csv(
+            forecast_out = self.get_forecast_out_from_csv_or_list(
                 df_final, forecast_dates_csv, csv_path)
             df_final[self.var_load_cost] = forecast_out
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['load_cost_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
             else:
                 # Ensure correct length
                 data_list = data_list[0:len(self.forecast_dates)]
                 # Define the correct dates
                 forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
-                forecast_out = self.get_forecast_out_from_csv(
-                    df_final, forecast_dates_csv, None, data_list=data_list)
+                forecast_out = self.get_forecast_out_from_csv_or_list(
+                    df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_load_cost] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
             
         return df_final
     
     def get_prod_price_forecast(self, df_final: pd.DataFrame, method: Optional[str] = 'constant',
-                               csv_path: Optional[str] = "/data/data_prod_price_forecast.csv") -> pd.DataFrame:
+                                csv_path: Optional[str] = "/data/data_prod_price_forecast.csv",
+                                list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
         r"""
         Get the unit power production price for the energy injected to the grid.\
         This is the price of the energy injected to the utility in a vector \
         sampled at the fixed freq value.
         
         :param df_input_data: The DataFrame containing all the input data retrieved
             from hass
@@ -743,31 +779,31 @@
         :rtype: pd.DataFrame
 
         """
         if method == 'constant':
             df_final[self.var_prod_price] = self.optim_conf['prod_sell_price']
         elif method == 'csv':
             forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
-            forecast_out = self.get_forecast_out_from_csv(df_final,
+            forecast_out = self.get_forecast_out_from_csv_or_list(df_final,
                                                           forecast_dates_csv,
                                                           csv_path)
             df_final[self.var_prod_price] = forecast_out
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['prod_price_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
             else:
                 # Ensure correct length
                 data_list = data_list[0:len(self.forecast_dates)]
                 # Define the correct dates
                 forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
-                forecast_out = self.get_forecast_out_from_csv(
-                    df_final, forecast_dates_csv, None, data_list=data_list)
+                forecast_out = self.get_forecast_out_from_csv_or_list(
+                    df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_prod_price] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
             
         return df_final
```

### Comparing `emhass-0.8.5/src/emhass/machine_learning_forecaster.py` & `emhass-0.8.6/src/emhass/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/optimization.py` & `emhass-0.8.6/src/emhass/optimization.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/retrieve_hass.py` & `emhass-0.8.6/src/emhass/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/advanced.html` & `emhass-0.8.6/src/emhass/static/advanced.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/basic.html` & `emhass-0.8.6/src/emhass/static/basic.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/img/emhass_icon.png` & `emhass-0.8.6/src/emhass/static/img/emhass_icon.png`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/img/emhass_logo_short.svg` & `emhass-0.8.6/src/emhass/static/img/emhass_logo_short.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/img/feather-sprite.svg` & `emhass-0.8.6/src/emhass/static/img/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/script.js` & `emhass-0.8.6/src/emhass/static/script.js`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/static/style.css` & `emhass-0.8.6/src/emhass/static/style.css`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/templates/index.html` & `emhass-0.8.6/src/emhass/templates/index.html`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/utils.py` & `emhass-0.8.6/src/emhass/utils.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass/web_server.py` & `emhass-0.8.6/src/emhass/web_server.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/src/emhass.egg-info/PKG-INFO` & `emhass-0.8.6/src/emhass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.8.5
+Version: 0.8.6
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.8.5 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.8.6 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
```

### Comparing `emhass-0.8.5/src/emhass.egg-info/SOURCES.txt` & `emhass-0.8.6/src/emhass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/tests/test_command_line_utils.py` & `emhass-0.8.6/tests/test_command_line_utils.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/tests/test_forecast.py` & `emhass-0.8.6/tests/test_forecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 import _pickle as cPickle
 
 from emhass.retrieve_hass import RetrieveHass
 from emhass.command_line import set_input_data_dict
 from emhass.machine_learning_forecaster import MLForecaster
 from emhass.forecast import Forecast
 from emhass.optimization import Optimization
-from emhass.utils import get_root, get_logger, get_yaml_parse, treat_runtimeparams, get_days_list
+from emhass import utils
 
 # the root folder
-root = str(get_root(__file__, num_parent=2))
+root = str(utils.get_root(__file__, num_parent=2))
 # create logger
-logger, ch = get_logger(__name__, root, save_to_file=False)
+logger, ch = utils.get_logger(__name__, root, save_to_file=False)
 
 class TestForecast(unittest.TestCase):
     
     @staticmethod
     def get_test_params():
         with open(root+'/config_emhass.yaml', 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
@@ -37,25 +37,25 @@
             }
             })
         return params
 
     def setUp(self):
         self.get_data_from_file = True
         params = None
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root) / 'config_emhass.yaml', use_secrets=False)
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root) / 'config_emhass.yaml', use_secrets=False)
         self.retrieve_hass_conf, self.optim_conf, self.plant_conf = \
             retrieve_hass_conf, optim_conf, plant_conf
         self.rh = RetrieveHass(self.retrieve_hass_conf['hass_url'], self.retrieve_hass_conf['long_lived_token'], 
                                self.retrieve_hass_conf['freq'], self.retrieve_hass_conf['time_zone'],
                                params, root, logger)
         if self.get_data_from_file:
             with open(pathlib.Path(root) / 'data' / 'test_df_final.pkl', 'rb') as inp:
                 self.rh.df_final, self.days_list, self.var_list = pickle.load(inp)
         else:
-            self.days_list = get_days_list(self.retrieve_hass_conf['days_to_retrieve'])
+            self.days_list = utils.get_days_list(self.retrieve_hass_conf['days_to_retrieve'])
             self.var_list = [self.retrieve_hass_conf['var_load'], self.retrieve_hass_conf['var_PV']]
             self.rh.get_data(self.days_list, self.var_list,
                             minimal_response=False, significant_changes_only=False)
         self.rh.prepare_data(self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
                              set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
                              var_replace_zero = self.retrieve_hass_conf['var_replace_zero'], 
                              var_interp = self.retrieve_hass_conf['var_interp'])
@@ -188,28 +188,28 @@
             'load_power_forecast':[i+1 for i in range(48)],
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
-        params, retrieve_hass_conf, optim_conf, plant_conf = treat_runtimeparams(
+        params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
                           retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'],
                           params, root, logger)
         if self.get_data_from_file:
             with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
         else:
-            days_list = get_days_list(retrieve_hass_conf['days_to_retrieve'])
+            days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
@@ -255,46 +255,59 @@
                 'time_zone': 'Europe/Paris',
                 'lat': 45.83,
                 'lon': 6.86,
                 'alt': 4807.8
             }
             })
         runtimeparams = {
-            'pv_power_forecast':[i+1 for i in range(2*48)],
-            'load_power_forecast':[i+1 for i in range(2*48)],
-            'load_cost_forecast':[i+1 for i in range(2*48)],
-            'prod_price_forecast':[i+1 for i in range(2*48)]
+            'pv_power_forecast':[i+1 for i in range(3*48)],
+            'load_power_forecast':[i+1 for i in range(3*48)],
+            'load_cost_forecast':[i+1 for i in range(3*48)],
+            'prod_price_forecast':[i+1 for i in range(3*48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
-                                                                    use_secrets=False, params=params_json)
-        optim_conf['delta_forecast'] = pd.Timedelta(days=2)
-        params, retrieve_hass_conf, optim_conf, plant_conf = treat_runtimeparams(
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+                                                                          use_secrets=False, params=params_json)
+        optim_conf['delta_forecast'] = pd.Timedelta(days=3)
+        params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf, 
-                        params_json, root, logger, opt_time_delta=48, get_data_from_file=True)
+                        params_json, root, logger, get_data_from_file=True)
         P_PV_forecast = fcst.get_weather_forecast(method='list')
         self.assertIsInstance(P_PV_forecast, type(pd.DataFrame()))
         self.assertIsInstance(P_PV_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_PV_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_PV_forecast.index.tz, fcst.time_zone)
         self.assertTrue(fcst.start_forecast < ts for ts in P_PV_forecast.index)
         self.assertTrue(P_PV_forecast.values[0][0] == 1)
-        self.assertTrue(P_PV_forecast.values[-1][0] == 2*48)
+        self.assertTrue(P_PV_forecast.values[-1][0] == 3*48)
         P_load_forecast = fcst.get_load_forecast(method='list')
         self.assertIsInstance(P_load_forecast, pd.core.series.Series)
         self.assertIsInstance(P_load_forecast.index, pd.core.indexes.datetimes.DatetimeIndex)
         self.assertIsInstance(P_load_forecast.index.dtype, pd.core.dtypes.dtypes.DatetimeTZDtype)
         self.assertEqual(P_load_forecast.index.tz, fcst.time_zone)
         self.assertEqual(len(P_PV_forecast), len(P_load_forecast))
         self.assertTrue(P_load_forecast.values[0] == 1)
-        self.assertTrue(P_load_forecast.values[-1] == 2*48)
+        self.assertTrue(P_load_forecast.values[-1] == 3*48)
+        df_input_data_dayahead = pd.concat([P_PV_forecast, P_load_forecast], axis=1)
+        df_input_data_dayahead = utils.set_df_index_freq(df_input_data_dayahead)
+        df_input_data_dayahead.columns = ['P_PV_forecast', 'P_load_forecast']
+        df_input_data_dayahead = fcst.get_load_cost_forecast(df_input_data_dayahead, method='list')
+        self.assertTrue(fcst.var_load_cost in df_input_data_dayahead.columns)
+        self.assertTrue(df_input_data_dayahead.isnull().sum().sum()==0)
+        self.assertTrue(df_input_data_dayahead[fcst.var_load_cost].iloc[0] == 1)
+        self.assertTrue(df_input_data_dayahead[fcst.var_load_cost].iloc[-1] == 3*48)
+        df_input_data_dayahead = fcst.get_prod_price_forecast(df_input_data_dayahead, method='list')
+        self.assertTrue(fcst.var_prod_price in df_input_data_dayahead.columns)
+        self.assertTrue(df_input_data_dayahead.isnull().sum().sum()==0)
+        self.assertTrue(df_input_data_dayahead[fcst.var_prod_price].iloc[0] == 1)
+        self.assertTrue(df_input_data_dayahead[fcst.var_prod_price].iloc[-1] == 3*48)
         
     def test_get_forecasts_with_lists_special_case(self):
         with open(root+'/config_emhass.yaml', 'r') as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
         params.update({
             'params_secrets': {
                 'hass_url': 'http://supervisor/core/api',
@@ -308,28 +321,28 @@
         runtimeparams = {
             'load_cost_forecast':[i+1 for i in range(48)],
             'prod_price_forecast':[i+1 for i in range(48)]
         }
         runtimeparams_json = json.dumps(runtimeparams)
         params['passed_data'] = runtimeparams
         params_json = json.dumps(params)
-        retrieve_hass_conf, optim_conf, plant_conf = get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
+        retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(pathlib.Path(root+'/config_emhass.yaml'), 
                                                                     use_secrets=False, params=params_json)
         set_type = "dayahead-optim"
-        params, retrieve_hass_conf, optim_conf, plant_conf = treat_runtimeparams(
+        params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
             runtimeparams_json, params_json, retrieve_hass_conf, 
             optim_conf, plant_conf, set_type, logger)
         rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
                           retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'],
                           params, root, logger)
         if self.get_data_from_file:
             with open(pathlib.Path(root+'/data/test_df_final.pkl'), 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
         else:
-            days_list = get_days_list(retrieve_hass_conf['days_to_retrieve'])
+            days_list = utils.get_days_list(retrieve_hass_conf['days_to_retrieve'])
             var_list = [retrieve_hass_conf['var_load'], retrieve_hass_conf['var_PV']]
             rh.get_data(days_list, var_list,
                         minimal_response=False, significant_changes_only=False)
         rh.prepare_data(retrieve_hass_conf['var_load'], load_negative = retrieve_hass_conf['load_negative'],
                         set_zero_min = retrieve_hass_conf['set_zero_min'], 
                         var_replace_zero = retrieve_hass_conf['var_replace_zero'], 
                         var_interp = retrieve_hass_conf['var_interp'])
```

### Comparing `emhass-0.8.5/tests/test_machine_learning_forecaster.py` & `emhass-0.8.6/tests/test_machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/tests/test_optimization.py` & `emhass-0.8.6/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/tests/test_retrieve_hass.py` & `emhass-0.8.6/tests/test_retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `emhass-0.8.5/tests/test_utils.py` & `emhass-0.8.6/tests/test_utils.py`

 * *Files identical despite different names*

