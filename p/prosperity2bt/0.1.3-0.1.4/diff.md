# Comparing `tmp/prosperity2bt-0.1.3.tar.gz` & `tmp/prosperity2bt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.1.3.tar", last modified: Sat Apr  6 00:11:53 2024, max compression
+gzip compressed data, was "prosperity2bt-0.1.4.tar", last modified: Sun Apr  7 00:22:48 2024, max compression
```

## Comparing `prosperity2bt-0.1.3.tar` & `prosperity2bt-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:53.048480 prosperity2bt-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-06 00:11:53.048480 prosperity2bt-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:53.044480 prosperity2bt-0.1.3/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:53.044480 prosperity2bt-0.1.3/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:53.044480 prosperity2bt-0.1.3/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-06 00:11:46.000000 prosperity2bt-0.1.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:53.048480 prosperity2bt-0.1.3/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 00:11:53.000000 prosperity2bt-0.1.3/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-06 00:11:50.000000 prosperity2bt-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:53.048480 prosperity2bt-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-07 00:22:42.000000 prosperity2bt-0.1.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 00:22:48.000000 prosperity2bt-0.1.4/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 00:22:45.000000 prosperity2bt-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:22:48.375306 prosperity2bt-0.1.4/setup.cfg
```

### Comparing `prosperity2bt-0.1.3/LICENSE` & `prosperity2bt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/PKG-INFO` & `prosperity2bt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.1.3/README.md` & `prosperity2bt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt/core.py` & `prosperity2bt-0.1.4/prosperity2bt/core.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt/data.py` & `prosperity2bt-0.1.4/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt/datamodel.py` & `prosperity2bt-0.1.4/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt/main.py` & `prosperity2bt-0.1.4/prosperity2bt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,21 @@
     http_handler = partial(HTTPRequestHandler, directory=output_file.parent)
     http_server = HTTPServer(("localhost", 0), http_handler)
 
     webbrowser.open(f"https://jmerle.github.io/imc-prosperity-2-visualizer/?open=http://localhost:{http_server.server_port}/{output_file.name}")
     http_server.handle_request()
     http_server.handle_request()
 
+def format_path(path: Path) -> str:
+    cwd = Path.cwd()
+    if path.is_relative_to(cwd):
+        return str(path.relative_to(cwd))
+    else:
+        return str(path)
+
 def main() -> None:
     parser = ArgumentParser(prog="prosperity2bt", description="Run a backtest.")
     parser.add_argument("algorithm", type=str, help="path to the Python file containing the algoritm to backtest")
     parser.add_argument("days", type=str, nargs="+", help="the days to backtest on (<round>-<day> for a single day, <round> for all days in a round)")
     parser.add_argument("--merge-pnl", action="store_true", help="merge profit and loss across days")
     parser.add_argument("--vis", action="store_true", help="open backtest result in visualizer when done")
     parser.add_argument("--out", type=str, help="path to save output log to (defaults to backtests/<timestamp>.log)")
@@ -152,11 +159,11 @@
     merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
 
     write_output(output_file, merged_results)
 
     if len(days) > 1:
         print_overall_summary(results)
 
-    print(f"Successfully saved backtest results to {output_file}")
+    print(f"Successfully saved backtest results to {format_path(output_file)}")
 
     if args.vis:
         open_visualizer(output_file)
```

### Comparing `prosperity2bt-0.1.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.1.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.1.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.1.4/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.1.3/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.1.4/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.1.3/pyproject.toml` & `prosperity2bt-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

