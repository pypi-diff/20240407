# Comparing `tmp/wellets_cli-1.9.4.tar.gz` & `tmp/wellets_cli-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellets_cli-1.9.4.tar", max compression
+gzip compressed data, was "wellets_cli-1.9.5.tar", max compression
```

## Comparing `wellets_cli-1.9.4.tar` & `wellets_cli-1.9.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1211 2024-04-06 16:47:16.964793 wellets_cli-1.9.4/LICENSE
--rw-r--r--   0        0        0      870 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/VERSION
--rw-r--r--   0        0        0       46 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/__init__.py
--rw-r--r--   0        0        0      137 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/__main__.py
--rw-r--r--   0        0        0    15790 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/api.py
--rw-r--r--   0        0        0     1243 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/auth.py
--rw-r--r--   0        0        0      335 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/base.py
--rw-r--r--   0        0        0     2875 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/chart.py
--rw-r--r--   0        0        0     1455 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/cli.py
--rw-r--r--   0        0        0        0 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/__init__.py
--rw-r--r--   0        0        0     8501 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/accumulation.py
--rw-r--r--   0        0        0    10476 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/asset.py
--rw-r--r--   0        0        0     1497 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/currency.py
--rw-r--r--   0        0        0     2000 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/investment.py
--rw-r--r--   0        0        0      688 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/login.py
--rw-r--r--   0        0        0    11798 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/portfolio.py
--rw-r--r--   0        0        0     1446 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/register.py
--rw-r--r--   0        0        0     6938 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/transaction.py
--rw-r--r--   0        0        0     3648 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/transfer.py
--rw-r--r--   0        0        0    12717 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/wallet.py
--rw-r--r--   0        0        0      246 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/commands/whoami.py
--rw-r--r--   0        0        0     1383 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/config.py
--rw-r--r--   0        0        0     4510 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/model.py
--rw-r--r--   0        0        0      479 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/prompt.py
--rw-r--r--   0        0        0     9218 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/question.py
--rw-r--r--   0        0        0     4250 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/util.py
--rw-r--r--   0        0        0     6677 2024-04-06 16:47:16.968793 wellets_cli-1.9.4/wellets_cli/validator.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 wellets_cli-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-07 19:47:52.172444 wellets_cli-1.9.5/LICENSE
+-rw-r--r--   0        0        0      870 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/VERSION
+-rw-r--r--   0        0        0       46 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/__main__.py
+-rw-r--r--   0        0        0    15790 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/api.py
+-rw-r--r--   0        0        0     1243 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/auth.py
+-rw-r--r--   0        0        0      335 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/base.py
+-rw-r--r--   0        0        0     2871 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/chart.py
+-rw-r--r--   0        0        0     1455 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8501 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/accumulation.py
+-rw-r--r--   0        0        0    10472 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/asset.py
+-rw-r--r--   0        0        0     1497 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/currency.py
+-rw-r--r--   0        0        0     2000 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/investment.py
+-rw-r--r--   0        0        0      688 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/login.py
+-rw-r--r--   0        0        0    11798 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/portfolio.py
+-rw-r--r--   0        0        0     1446 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/register.py
+-rw-r--r--   0        0        0     6938 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/transaction.py
+-rw-r--r--   0        0        0     3648 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/transfer.py
+-rw-r--r--   0        0        0    12717 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/wallet.py
+-rw-r--r--   0        0        0      246 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/commands/whoami.py
+-rw-r--r--   0        0        0     1347 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/config.py
+-rw-r--r--   0        0        0     4510 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/model.py
+-rw-r--r--   0        0        0      479 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/prompt.py
+-rw-r--r--   0        0        0     9218 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/question.py
+-rw-r--r--   0        0        0     4250 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/util.py
+-rw-r--r--   0        0        0     6677 2024-04-07 19:47:52.176444 wellets_cli-1.9.5/wellets_cli/validator.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 wellets_cli-1.9.5/PKG-INFO
```

### Comparing `wellets_cli-1.9.4/LICENSE` & `wellets_cli-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/pyproject.toml` & `wellets_cli-1.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wellets_cli"
-version = "1.9.4"
+version = "1.9.5"
 description = "wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control."
 authors = ["lparolari"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1"
 requests = "^2"
```

### Comparing `wellets_cli-1.9.4/wellets_cli/api.py` & `wellets_cli-1.9.5/wellets_cli/api.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/auth.py` & `wellets_cli-1.9.5/wellets_cli/auth.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/chart.py` & `wellets_cli-1.9.5/wellets_cli/chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     return fig
 
 
 def xdate_fmt(fig):
     from matplotlib.dates import DateFormatter
 
-    date_fmt = DateFormatter(settings.app.date_format)
+    date_fmt = DateFormatter(settings.date_format)
 
     fig.autofmt_xdate()
 
     ax = fig.gca()
     ax.xaxis.set_major_formatter(date_fmt)
 
     return fig
```

### Comparing `wellets_cli-1.9.4/wellets_cli/cli.py` & `wellets_cli-1.9.5/wellets_cli/cli.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/accumulation.py` & `wellets_cli-1.9.5/wellets_cli/commands/accumulation.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/asset.py` & `wellets_cli-1.9.5/wellets_cli/commands/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     }
 
     history = api.get_asset_history(params=params, headers=headers)
     asset = get_by_id(assets, asset_id)
 
     data = [
         {
-            "timestamp": h.timestamp.strftime(settings.app.date_format),
+            "timestamp": h.timestamp.strftime(settings.date_format),
             f"balance\n({asset.currency.acronym})": pp(h.balance, 8, fixed=False),
         }
         for h in history
     ]
 
     print(tabulate(data, headers="keys"))
```

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/currency.py` & `wellets_cli-1.9.5/wellets_cli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/investment.py` & `wellets_cli-1.9.5/wellets_cli/commands/investment.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/login.py` & `wellets_cli-1.9.5/wellets_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/portfolio.py` & `wellets_cli-1.9.5/wellets_cli/commands/portfolio.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/register.py` & `wellets_cli-1.9.5/wellets_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/transaction.py` & `wellets_cli-1.9.5/wellets_cli/commands/transaction.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/transfer.py` & `wellets_cli-1.9.5/wellets_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/commands/wallet.py` & `wellets_cli-1.9.5/wellets_cli/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/config.py` & `wellets_cli-1.9.5/wellets_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
     @property
     def datetime_format(self) -> str:
         return os.environ.get("WELLETS_DATETIME_FORMAT") or "%b %d, %Y %H:%M"
 
     @property
     def api_url(self) -> str:
-        return (
-            os.environ.get("WELLETS_API_URL") or "https://wellets-backend.herokuapp.com"
-        )
+        return os.environ.get("WELLETS_API_URL") or "http://lparolari.xyz:3333"
 
     @property
     def api_username(self) -> Optional[str]:
         return os.environ.get("WELLETS_API_USERNAME") or None
 
     @property
     def api_password(self) -> Optional[str]:
```

### Comparing `wellets_cli-1.9.4/wellets_cli/model.py` & `wellets_cli-1.9.5/wellets_cli/model.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/question.py` & `wellets_cli-1.9.5/wellets_cli/question.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/util.py` & `wellets_cli-1.9.5/wellets_cli/util.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/wellets_cli/validator.py` & `wellets_cli-1.9.5/wellets_cli/validator.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.9.4/PKG-INFO` & `wellets_cli-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellets_cli
-Version: 1.9.4
+Version: 1.9.5
 Summary: wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep your money under control.
 Author: lparolari
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8,<9)
 Requires-Dist: inquirerpy (>=0.3,<0.4)
```

