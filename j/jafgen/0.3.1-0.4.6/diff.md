# Comparing `tmp/jafgen-0.3.1.tar.gz` & `tmp/jafgen-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jafgen-0.3.1.tar", last modified: Tue Jan 17 16:01:56 2023, max compression
+gzip compressed data, was "jafgen-0.4.6.tar", last modified: Sun Apr  7 21:25:27 2024, max compression
```

## Comparing `jafgen-0.3.1.tar` & `jafgen-0.4.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:56.381820 jafgen-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-01-17 16:01:40.000000 jafgen-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-17 16:01:56.381820 jafgen-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-17 16:01:40.000000 jafgen-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:56.377820 jafgen-0.3.1/jafgen/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:56.381820 jafgen-0.3.1/jafgen/customers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/customers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/customers/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/customers/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/customers/order_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:56.381820 jafgen-0.3.1/jafgen/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/stores/supply.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-17 16:01:40.000000 jafgen-0.3.1/jafgen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:01:56.377820 jafgen-0.3.1/jafgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-17 16:01:56.000000 jafgen-0.3.1/jafgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-17 16:01:40.000000 jafgen-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 16:01:56.381820 jafgen-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-01-17 16:01:40.000000 jafgen-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 21:25:16.000000 jafgen-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:25:27.604475 jafgen-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-07 21:25:16.000000 jafgen-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.600475 jafgen-0.4.6/jafgen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen/customers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/customers/order_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-07 21:25:16.000000 jafgen-0.4.6/jafgen/stores/supply.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/jafgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 21:25:27.000000 jafgen-0.4.6/jafgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 21:25:16.000000 jafgen-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:25:27.604475 jafgen-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 21:25:16.000000 jafgen-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:25:27.604475 jafgen-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 21:25:16.000000 jafgen-0.4.6/tests/test_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 21:25:16.000000 jafgen-0.4.6/tests/test_inventory.py
```

### Comparing `jafgen-0.3.1/LICENSE` & `jafgen-0.4.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
                                  Apache License
                            Version 2.0, January 2004
-                        https://www.apache.org/licenses/
+                        http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
       "License" shall mean the terms and conditions for use, reproduction,
       and distribution as defined by Sections 1 through 9 of this document.
@@ -174,28 +174,28 @@
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
    APPENDIX: How to apply the Apache License to your work.
 
       To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
+      boilerplate notice, with the fields enclosed by brackets "[]"
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
-       https://www.apache.org/licenses/LICENSE-2.0
+       http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `jafgen-0.3.1/jafgen/curves.py` & `jafgen-0.4.6/jafgen/curves.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,84 @@
 import datetime
-
+from abc import ABC, abstractmethod
 import numpy as np
 
 
-class Curve:
+class Curve(ABC):
+    @property
+    @abstractmethod
+    def Domain(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def TranslateDomain(self, date):
+        raise NotImplementedError
+
+    @abstractmethod
+    def Expr(self, x):
+        raise NotImplementedError
+
     @classmethod
     def eval(cls, date):
-        x = cls.TranslateDomain(date)
-        x_mod = x % len(cls.Domain)
-        x_translated = cls.Domain[x_mod]
-        return cls.Expr(x_translated)
+        instance = cls()
+        domain_value = instance.TranslateDomain(date)
+        domain_index = domain_value % len(instance.Domain)
+        translated_value = instance.Domain[domain_index]
+        return instance.Expr(translated_value)
 
 
 class AnnualCurve(Curve):
-    Domain = np.linspace(0, 2 * np.pi, 365)
-    TranslateDomain = lambda date: date.timetuple().tm_yday
-    Expr = lambda x: (np.cos(x) + 1) / 10 + 0.8
+    @property
+    def Domain(self):
+        return np.linspace(0, 2 * np.pi, 365)
+
+    def TranslateDomain(self, date):
+        return date.timetuple().tm_yday
+
+    def Expr(self, x):
+        return (np.cos(x) + 1) / 10 + 0.8
 
 
 class WeekendCurve(Curve):
-    Domain = tuple(range(6))
-    TranslateDomain = lambda date: date.weekday() - 1
-    Expr = lambda x: 0.6 if x >= 6 else 1
+    @property
+    def Domain(self):
+        return tuple(range(6))
+
+    def TranslateDomain(self, date):
+        return date.weekday() - 1
+
+    def Expr(self, x):
+        if x >= 6:
+            return 0.6
+        else:
+            return 1.0
 
 
 class GrowthCurve(Curve):
-    Domain = tuple(range(500))
-    TranslateDomain = lambda date: (date.year - 2016) * 12 + date.month
-    # ~ aim for ~20% growth/year
-    Expr = lambda x: 1 + (x / 12) * 0.2
+    @property
+    def Domain(self):
+        return tuple(range(500))
+
+    def TranslateDomain(self, date):
+        return (date.year - 2016) * 12 + date.month
+
+    def Expr(self, x):
+        # ~ aim for ~20% growth/year
+        return 1 + (x / 12) * 0.2
 
 
 class Day(object):
     EPOCH = datetime.datetime(year=2016, month=9, day=1)
     SEASONAL_MONTHLY_CURVE = AnnualCurve()
     WEEKEND_CURVE = WeekendCurve()
     GROWTH_CURVE = GrowthCurve()
 
     def __init__(self, date_index, minutes=0):
         self.date_index = date_index
         self.date = self.EPOCH + datetime.timedelta(days=date_index, minutes=minutes)
-
-        self.day_of_week = self._get_day_of_week(self.date)
-        self.is_weekend = self._is_weekend(self.date)
-        self.season = self._get_season(self.date)
-
         self.effects = [
             self.SEASONAL_MONTHLY_CURVE.eval(self.date),
             self.WEEKEND_CURVE.eval(self.date),
             self.GROWTH_CURVE.eval(self.date),
         ]
 
     def at_minute(self, minutes):
@@ -59,24 +89,27 @@
         for effect in self.effects:
             total = total * effect
         return total
 
         # weekend_effect = 0.8 if date.is_weekend else 1
         # summer_effect = 0.7 if date.season == 'summer' else 1
 
-    def _get_day_of_week(self, date):
-        return date.weekday()
+    @property
+    def day_of_week(self):
+        return self.date.weekday()
 
-    def _is_weekend(self, date):
+    @property
+    def is_weekend(self):
         # 5 + 6 are weekends
-        return date.weekday() >= 5
+        return self.date.weekday() >= 5
 
-    def _get_season(self, date):
-        month_no = date.month
-        day_no = date.day
+    @property
+    def season(self):
+        month_no = self.date.month
+        day_no = self.date.day
 
         if month_no in (1, 2) or (month_no == 3 and day_no < 21):
             return "winter"
         elif month_no in (3, 4, 5) or (month_no == 6 and day_no < 21):
             return "spring"
         elif month_no in (6, 7, 8) or (month_no == 9 and day_no < 21):
             return "summer"
```

### Comparing `jafgen-0.3.1/jafgen/customers/customers.py` & `jafgen-0.4.6/jafgen/customers/customers.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/customers/order.py` & `jafgen-0.4.6/jafgen/customers/order.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/simulation.py` & `jafgen-0.4.6/jafgen/simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import uuid
 
 import pandas as pd
-from tqdm import tqdm
+from rich.progress import track
 
 from jafgen.curves import Day
-from jafgen.stores.inventory import Inventory
 from jafgen.stores.market import Market
 from jafgen.stores.stock import Stock
 from jafgen.stores.store import Store
 
 T_7AM = 60 * 7
 T_8AM = 60 * 8
 T_2PM = 60 * 14
@@ -53,29 +52,36 @@
             start, end = self.weekday_range
 
         for i in range(end - start):
             yield start + i
 
 
 class Simulation(object):
-    def __init__(self, years=2, prefix="raw"):
+    def __init__(self, years, prefix):
         self.years = years
         self.scale = 100
         self.prefix = prefix
         self.stores = [
             # id | name | popularity | opened | TAM | tax
             (str(uuid.uuid4()), "Philadelphia", 0.85, 0, 9 * self.scale, 0.06),
             (str(uuid.uuid4()), "Brooklyn", 0.95, 192, 14 * self.scale, 0.04),
             (str(uuid.uuid4()), "Chicago", 0.92, 605, 12 * self.scale, 0.0625),
             (str(uuid.uuid4()), "San Francisco", 0.87, 615, 11 * self.scale, 0.075),
             (str(uuid.uuid4()), "New Orleans", 0.92, 920, 8 * self.scale, 0.04),
         ]
 
         self.markets = []
-        for store_id, store_name, popularity, opened_date, market_size, tax in self.stores:
+        for (
+            store_id,
+            store_name,
+            popularity,
+            opened_date,
+            market_size,
+            tax,
+        ) in self.stores:
             market = Market(
                 Store(
                     store_id=store_id,
                     name=store_name,
                     base_popularity=popularity,
                     hours_of_operation=HoursOfOperation(
                         weekday_range=(T_7AM, T_8PM),
@@ -89,62 +95,45 @@
             self.markets.append(market)
 
         self.customers = {}
         self.orders = []
         self.sim_days = 365 * self.years
 
     def run_simulation(self):
-
-        for i in tqdm(range(self.sim_days), desc="[SIM]"):
-
+        for i in track(
+            range(self.sim_days), description="🥪 Pressing fresh jaffles..."
+        ):
             for market in self.markets:
                 day = Day(i)
                 for order in (o for o in market.sim_day(day) if o is not None):
                     self.orders.append(order)
                     if order.customer.customer_id not in self.customers:
                         self.customers[order.customer.customer_id] = order.customer
 
     def save_results(self):
-        df_customers = pd.DataFrame.from_dict(
-            customer.to_dict() for customer in self.customers.values()
-        )
-        df_orders = pd.DataFrame.from_dict(order.to_dict() for order in self.orders)
-        df_items = pd.DataFrame.from_dict(
-            item.to_dict() for order in self.orders for item in order.items
-        )
-        df_stores = pd.DataFrame.from_dict(market.store.to_dict() for market in self.markets)
-        df_products = pd.DataFrame.from_dict(Inventory.to_dict())
-        df_supplies = pd.DataFrame.from_dict(Stock.to_dict())
-        # ask Drew about what the heck is up with the to_dict generator stuff
-
+        stock: Stock = Stock()
+        entities: dict[str, pd.DataFrame] = {
+            "customers": pd.DataFrame.from_dict(
+                (customer.to_dict() for customer in self.customers.values())
+            ),
+            "orders": pd.DataFrame.from_dict(
+                (order.to_dict() for order in self.orders)
+            ),
+            "items": pd.DataFrame.from_dict(
+                (item.to_dict() for order in self.orders for item in order.items)
+            ),
+            "stores": pd.DataFrame.from_dict(
+                (market.store.to_dict() for market in self.markets)
+            ),
+            "supplies": pd.DataFrame.from_dict(stock.to_dict()),
+        }
         if not os.path.exists("./jaffle-data"):
             os.makedirs("./jaffle-data")
-
         # save output
-        df_customers.to_csv(
-            f"./jaffle-data/{self.prefix}_customers.csv",
-            header=df_customers.columns.to_list(),
-            index=False,
-        )
-        df_items.to_csv(
-            f"./jaffle-data/{self.prefix}_items.csv", header=df_items.columns.to_list(), index=False
-        )
-        df_orders.to_csv(
-            f"./jaffle-data/{self.prefix}_orders.csv",
-            header=df_orders.columns.to_list(),
-            index=False,
-        )
-        df_products.to_csv(
-            f"./jaffle-data/{self.prefix}_products.csv",
-            header=df_products.columns.to_list(),
-            index=False,
-        )
-        df_stores.to_csv(
-            f"./jaffle-data/{self.prefix}_stores.csv",
-            header=df_stores.columns.to_list(),
-            index=False,
-        )
-        df_supplies.to_csv(
-            f"./jaffle-data/{self.prefix}_supplies.csv",
-            header=df_supplies.columns.to_list(),
-            index=False,
-        )
+        for entity, df in track(
+            entities.items(), description="🚚 Delivering jaffles..."
+        ):
+            df.to_csv(
+                f"./jaffle-data/{self.prefix}_{entity}.csv",
+                header=df.columns.to_list(),
+                index=False,
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jafgen-0.3.1/jafgen/stores/inventory.py` & `jafgen-0.4.6/jafgen/stores/inventory.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/stores/item.py` & `jafgen-0.4.6/jafgen/stores/item.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/stores/market.py` & `jafgen-0.4.6/jafgen/stores/market.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/stores/stock.py` & `jafgen-0.4.6/jafgen/stores/stock.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/stores/store.py` & `jafgen-0.4.6/jafgen/stores/store.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen/stores/supply.py` & `jafgen-0.4.6/jafgen/stores/supply.py`

 * *Files identical despite different names*

### Comparing `jafgen-0.3.1/jafgen.egg-info/SOURCES.txt` & `jafgen-0.4.6/jafgen.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 jafgen/__init__.py
+jafgen/cli.py
 jafgen/curves.py
-jafgen/main.py
-jafgen/py.typed
 jafgen/simulation.py
-jafgen/version.py
 jafgen.egg-info/PKG-INFO
 jafgen.egg-info/SOURCES.txt
 jafgen.egg-info/dependency_links.txt
 jafgen.egg-info/entry_points.txt
 jafgen.egg-info/requires.txt
 jafgen.egg-info/top_level.txt
 jafgen/customers/__init__.py
@@ -20,8 +18,10 @@
 jafgen/customers/order_item.py
 jafgen/stores/__init__.py
 jafgen/stores/inventory.py
 jafgen/stores/item.py
 jafgen/stores/market.py
 jafgen/stores/stock.py
 jafgen/stores/store.py
-jafgen/stores/supply.py
+jafgen/stores/supply.py
+tests/test_days.py
+tests/test_inventory.py
```

