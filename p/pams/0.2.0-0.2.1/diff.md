# Comparing `tmp/pams-0.2.0.tar.gz` & `tmp/pams-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pams-0.2.0.tar", max compression
+gzip compressed data, was "pams-0.2.1.tar", max compression
```

## Comparing `pams-0.2.0.tar` & `pams-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11585 2023-09-22 13:59:29.636843 pams-0.2.0/LICENSE
--rw-r--r--   0        0        0     2244 2023-09-22 13:59:29.636843 pams-0.2.0/README.md
--rw-r--r--   0        0        0      594 2023-09-22 13:59:29.640843 pams-0.2.0/pams/__init__.py
--rw-r--r--   0        0        0      292 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/__init__.py
--rw-r--r--   0        0        0     6689 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/arbitrage_agent.py
--rw-r--r--   0        0        0     8620 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/base.py
--rw-r--r--   0        0        0     9663 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/fcn_agent.py
--rw-r--r--   0        0        0      363 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/high_frequency_agent.py
--rw-r--r--   0        0        0     4903 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/market_maker_agent.py
--rw-r--r--   0        0        0     1656 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/market_share_fcn_agent.py
--rw-r--r--   0        0        0     2323 2023-09-22 13:59:29.640843 pams-0.2.0/pams/agents/test_agent.py
--rw-r--r--   0        0        0      257 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/__init__.py
--rw-r--r--   0        0        0     9916 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/base.py
--rw-r--r--   0        0        0     3832 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/fundamental_price_shock.py
--rw-r--r--   0        0        0     4677 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/order_mistake_shock.py
--rw-r--r--   0        0        0     4833 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/price_limit_rule.py
--rw-r--r--   0        0        0     6163 2023-09-22 13:59:29.640843 pams-0.2.0/pams/events/trading_halt_rule.py
--rw-r--r--   0        0        0    10298 2023-09-22 13:59:29.640843 pams-0.2.0/pams/fundamentals.py
--rw-r--r--   0        0        0     6379 2023-09-22 13:59:29.640843 pams-0.2.0/pams/index_market.py
--rw-r--r--   0        0        0      447 2023-09-22 13:59:29.640843 pams-0.2.0/pams/logs/__init__.py
--rw-r--r--   0        0        0    13673 2023-09-22 13:59:29.640843 pams-0.2.0/pams/logs/base.py
--rw-r--r--   0        0        0     1465 2023-09-22 13:59:29.640843 pams-0.2.0/pams/logs/market_step_loggers.py
--rw-r--r--   0        0        0    33164 2023-09-22 13:59:29.640843 pams-0.2.0/pams/market.py
--rw-r--r--   0        0        0    10140 2023-09-22 13:59:29.640843 pams-0.2.0/pams/order.py
--rw-r--r--   0        0        0     6151 2023-09-22 13:59:29.640843 pams-0.2.0/pams/order_book.py
--rw-r--r--   0        0        0       66 2023-09-22 13:59:29.640843 pams-0.2.0/pams/runners/__init__.py
--rw-r--r--   0        0        0     3848 2023-09-22 13:59:29.640843 pams-0.2.0/pams/runners/base.py
--rw-r--r--   0        0        0    27935 2023-09-22 13:59:29.640843 pams-0.2.0/pams/runners/sequential.py
--rw-r--r--   0        0        0     6187 2023-09-22 13:59:29.640843 pams-0.2.0/pams/session.py
--rw-r--r--   0        0        0    18386 2023-09-22 13:59:29.640843 pams-0.2.0/pams/simulator.py
--rw-r--r--   0        0        0      147 2023-09-22 13:59:29.640843 pams-0.2.0/pams/utils/__init__.py
--rw-r--r--   0        0        0     1353 2023-09-22 13:59:29.640843 pams-0.2.0/pams/utils/class_finder.py
--rw-r--r--   0        0        0     2312 2023-09-22 13:59:29.640843 pams-0.2.0/pams/utils/json_extends.py
--rw-r--r--   0        0        0     7435 2023-09-22 13:59:29.640843 pams-0.2.0/pams/utils/json_random.py
--rw-r--r--   0        0        0       22 2023-09-22 13:59:29.640843 pams-0.2.0/pams/version.py
--rw-r--r--   0        0        0     1332 2023-09-22 13:59:29.640843 pams-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 pams-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11585 2024-04-07 10:27:18.190654 pams-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2246 2024-04-07 10:27:18.190654 pams-0.2.1/README.md
+-rw-r--r--   0        0        0      594 2024-04-07 10:27:18.194654 pams-0.2.1/pams/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/__init__.py
+-rw-r--r--   0        0        0     6689 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/arbitrage_agent.py
+-rw-r--r--   0        0        0     8620 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/base.py
+-rw-r--r--   0        0        0     9663 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/fcn_agent.py
+-rw-r--r--   0        0        0      363 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/high_frequency_agent.py
+-rw-r--r--   0        0        0     4903 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/market_maker_agent.py
+-rw-r--r--   0        0        0     1656 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/market_share_fcn_agent.py
+-rw-r--r--   0        0        0     2323 2024-04-07 10:27:18.194654 pams-0.2.1/pams/agents/test_agent.py
+-rw-r--r--   0        0        0      257 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/__init__.py
+-rw-r--r--   0        0        0     9916 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/base.py
+-rw-r--r--   0        0        0     3832 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/fundamental_price_shock.py
+-rw-r--r--   0        0        0     4677 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/order_mistake_shock.py
+-rw-r--r--   0        0        0     4833 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/price_limit_rule.py
+-rw-r--r--   0        0        0     6163 2024-04-07 10:27:18.194654 pams-0.2.1/pams/events/trading_halt_rule.py
+-rw-r--r--   0        0        0    10298 2024-04-07 10:27:18.194654 pams-0.2.1/pams/fundamentals.py
+-rw-r--r--   0        0        0     6379 2024-04-07 10:27:18.194654 pams-0.2.1/pams/index_market.py
+-rw-r--r--   0        0        0      479 2024-04-07 10:27:18.194654 pams-0.2.1/pams/logs/__init__.py
+-rw-r--r--   0        0        0    15419 2024-04-07 10:27:18.194654 pams-0.2.1/pams/logs/base.py
+-rw-r--r--   0        0        0     1465 2024-04-07 10:27:18.194654 pams-0.2.1/pams/logs/market_step_loggers.py
+-rw-r--r--   0        0        0    33801 2024-04-07 10:27:18.194654 pams-0.2.1/pams/market.py
+-rw-r--r--   0        0        0    10140 2024-04-07 10:27:18.194654 pams-0.2.1/pams/order.py
+-rw-r--r--   0        0        0     6992 2024-04-07 10:27:18.194654 pams-0.2.1/pams/order_book.py
+-rw-r--r--   0        0        0       66 2024-04-07 10:27:18.194654 pams-0.2.1/pams/runners/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-07 10:27:18.194654 pams-0.2.1/pams/runners/base.py
+-rw-r--r--   0        0        0    27935 2024-04-07 10:27:18.194654 pams-0.2.1/pams/runners/sequential.py
+-rw-r--r--   0        0        0     6187 2024-04-07 10:27:18.194654 pams-0.2.1/pams/session.py
+-rw-r--r--   0        0        0    18386 2024-04-07 10:27:18.198654 pams-0.2.1/pams/simulator.py
+-rw-r--r--   0        0        0      147 2024-04-07 10:27:18.198654 pams-0.2.1/pams/utils/__init__.py
+-rw-r--r--   0        0        0     1353 2024-04-07 10:27:18.198654 pams-0.2.1/pams/utils/class_finder.py
+-rw-r--r--   0        0        0     2312 2024-04-07 10:27:18.198654 pams-0.2.1/pams/utils/json_extends.py
+-rw-r--r--   0        0        0     7435 2024-04-07 10:27:18.198654 pams-0.2.1/pams/utils/json_random.py
+-rw-r--r--   0        0        0       22 2024-04-07 10:27:18.198654 pams-0.2.1/pams/version.py
+-rw-r--r--   0        0        0     1332 2024-04-07 10:27:18.198654 pams-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 pams-0.2.1/PKG-INFO
```

### Comparing `pams-0.2.0/LICENSE` & `pams-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/README.md` & `pams-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 $ python
 >> import pams
 ```
 
 ## Citation
 If you consider cite our work, please use the following [arxiv entry](https://arxiv.org/abs/2309.10729):
 ```bibtex
-@misc{Hirano2023-pams
+@misc{Hirano2023-pams,
     title={{PAMS: Platform for Artificial Market Simulations}},
-    autors={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
+    author={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
     year={2023},
     doi = {10.48550/arXiv.2309.10729}
 }
 ```
 https://arxiv.org/abs/2309.10729
 
 If you prefer to cite this package directly, please use the following bibtex entry:
 ```bibtex
-@misc{Hirano2022-pams
+@misc{Hirano2022-pams,
     title={{PAMS: Platform for Artificial Market Simulations}},
-    autors={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
+    author={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
     year={2022},
     url = {https://github.com/masanorihirano/pams}
 }
 ```
 
 ## Issues and Contribution
 About issues (bugs):
```

### Comparing `pams-0.2.0/pams/__init__.py` & `pams-0.2.1/pams/__init__.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/arbitrage_agent.py` & `pams-0.2.1/pams/agents/arbitrage_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/base.py` & `pams-0.2.1/pams/agents/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/fcn_agent.py` & `pams-0.2.1/pams/agents/fcn_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/market_maker_agent.py` & `pams-0.2.1/pams/agents/market_maker_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/market_share_fcn_agent.py` & `pams-0.2.1/pams/agents/market_share_fcn_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/agents/test_agent.py` & `pams-0.2.1/pams/agents/test_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/events/base.py` & `pams-0.2.1/pams/events/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/events/fundamental_price_shock.py` & `pams-0.2.1/pams/events/fundamental_price_shock.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/events/order_mistake_shock.py` & `pams-0.2.1/pams/events/order_mistake_shock.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/events/price_limit_rule.py` & `pams-0.2.1/pams/events/price_limit_rule.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/events/trading_halt_rule.py` & `pams-0.2.1/pams/events/trading_halt_rule.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/fundamentals.py` & `pams-0.2.1/pams/fundamentals.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/index_market.py` & `pams-0.2.1/pams/index_market.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/logs/base.py` & `pams-0.2.1/pams/logs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,59 @@
         self.kind: OrderKind = kind
         self.price: Optional[float] = price
         self.volume: int = volume
         self.ttl: Optional[int] = ttl
         # TODO: Type validation
 
 
+class ExpirationLog(Log):
+    """Expiration type log class.
+
+    This log is usually generated when an order is expired on markets.
+    """
+
+    def __init__(
+        self,
+        order_id: Optional[int],
+        market_id: int,
+        time: int,
+        order_time: Optional[int],
+        agent_id: int,
+        is_buy: bool,
+        kind: OrderKind,
+        volume: int,
+        price: Optional[float] = None,
+        ttl: Optional[int] = None,
+    ):
+        """initialize
+
+        Args:
+            order_id (int): order ID.
+            market_id (int): market ID.
+            time (int): time.
+            order_time (int): time to order.
+            agent_id (int): agent ID.
+            is_buy (bool): whether it is a buy order or not.
+            kind (:class:`pams.order.OrderKind`): kind of order.
+            volume (int): order volume.
+            price (float, Optional): order price.
+            ttl (int, Optional): time to order expiration.
+        """
+        self.order_id: Optional[int] = order_id
+        self.market_id: int = market_id
+        self.time: int = time
+        self.order_time: Optional[int] = order_time
+        self.agent_id: int = agent_id
+        self.is_buy: bool = is_buy
+        self.kind: OrderKind = kind
+        self.price: Optional[float] = price
+        self.volume: int = volume
+        self.ttl: Optional[int] = ttl
+
+
 class ExecutionLog(Log):
     """Execution type log class.
 
     This log is usually generated when an order is executed on markets.
     """
 
     def __init__(
@@ -348,14 +393,16 @@
             None
         """
         for log in logs:
             if isinstance(log, OrderLog):
                 self.process_order_log(log=log)
             elif isinstance(log, CancelLog):
                 self.process_cancel_log(log=log)
+            elif isinstance(log, ExpirationLog):
+                self.process_expiration_log(log=log)
             elif isinstance(log, ExecutionLog):
                 self.process_execution_log(log=log)
             elif isinstance(log, SimulationBeginLog):
                 self.process_simulation_begin_log(log=log)
             elif isinstance(log, SimulationEndLog):
                 self.process_simulation_end_log(log=log)
             elif isinstance(log, SessionBeginLog):
@@ -386,14 +433,25 @@
             log (:class:`pams.logs.CancelLog`]): cancel log
 
         Returns:
             None
         """
         pass
 
+    def process_expiration_log(self, log: "ExpirationLog") -> None:
+        """process expiration log. Called from :func:`process`.
+
+        Args:
+            log (:class:`pams.logs.ExpirationLog`]): expiration log
+
+        Returns:
+            None
+        """
+        pass
+
     def process_execution_log(self, log: "ExecutionLog") -> None:
         """process execution log. Called from :func:`process`.
 
         Args:
             log (:class:`pams.logs.ExecutionLog`]): execution log
 
         Returns:
```

### Comparing `pams-0.2.0/pams/logs/market_step_loggers.py` & `pams-0.2.1/pams/logs/market_step_loggers.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/market.py` & `pams-0.2.1/pams/market.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 from typing import cast
 
 from .logs.base import CancelLog
 from .logs.base import ExecutionLog
+from .logs.base import ExpirationLog
 from .logs.base import Log
 from .logs.base import Logger
 from .logs.base import OrderLog
 from .order import Cancel
 from .order import Order
 from .order_book import OrderBook
 
@@ -547,16 +548,22 @@
             time (int): time step.
             next_fundamental_price (float): next fundamental price.
 
         Returns:
             None
         """
         self.time = time
-        self.buy_order_book._set_time(time)
-        self.sell_order_book._set_time(time)
+        logs: List[ExpirationLog] = self.buy_order_book._set_time(time)
+        if self.logger is not None:
+            for log in logs:
+                log.read_and_write(logger=self.logger)
+        logs_: List[ExpirationLog] = self.sell_order_book._set_time(time)
+        if self.logger is not None:
+            for log_ in logs_:
+                log_.read_and_write(logger=self.logger)
         self._fill_until(time=time)
         self._fundamental_prices[self.time] = next_fundamental_price
         if self.time > 0:
             executed_prices: List[float] = cast(
                 List[float],
                 list(
                     filter(
@@ -595,16 +602,22 @@
         Args:
             next_fundamental_price (float): next fundamental price.
 
         Returns:
             None
         """
         self.time += 1
-        self.buy_order_book._set_time(self.time)
-        self.sell_order_book._set_time(self.time)
+        logs: List[ExpirationLog] = self.buy_order_book._set_time(self.time)
+        if self.logger is not None:
+            for log in logs:
+                log.read_and_write(logger=self.logger)
+        logs_: List[ExpirationLog] = self.sell_order_book._set_time(self.time)
+        if self.logger is not None:
+            for log_ in logs_:
+                log_.read_and_write(logger=self.logger)
         self._fill_until(time=self.time)
         self._fundamental_prices[self.time] = next_fundamental_price
         if self.time > 0:
             self._last_executed_prices[self.time] = self._last_executed_prices[
                 self.time - 1
             ]
             self._mid_prices[self.time] = self._mid_prices[self.time - 1]
```

### Comparing `pams-0.2.0/pams/order.py` & `pams-0.2.1/pams/order.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/runners/base.py` & `pams-0.2.1/pams/runners/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/runners/sequential.py` & `pams-0.2.1/pams/runners/sequential.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/session.py` & `pams-0.2.1/pams/session.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/simulator.py` & `pams-0.2.1/pams/simulator.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/utils/class_finder.py` & `pams-0.2.1/pams/utils/class_finder.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/utils/json_extends.py` & `pams-0.2.1/pams/utils/json_extends.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pams/utils/json_random.py` & `pams-0.2.1/pams/utils/json_random.py`

 * *Files identical despite different names*

### Comparing `pams-0.2.0/pyproject.toml` & `pams-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pams"
-version = "0.2.0"
+version = "0.2.1"
 description = "PAMS: Platform for Artificial Market Simulations"
 authors = ["Masanori HIRANO <masa.hirano.1996@gmail.com>", "Ryosuke TAKATA <ryos427@yahoo.co.jp>", "Kiyoshi IZUMI"]
 license = "epl-1.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `pams-0.2.0/PKG-INFO` & `pams-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pams
-Version: 0.2.0
+Version: 0.2.1
 Summary: PAMS: Platform for Artificial Market Simulations
 License: EPL-1.0
 Author: Masanori HIRANO
 Author-email: masa.hirano.1996@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Eclipse Public License 1.0 (EPL-1.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: scipy (>=1.9.2,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pams
 PAMS: Platform for Artificial Market Simulations
@@ -38,28 +39,28 @@
 $ python
 >> import pams
 ```
 
 ## Citation
 If you consider cite our work, please use the following [arxiv entry](https://arxiv.org/abs/2309.10729):
 ```bibtex
-@misc{Hirano2023-pams
+@misc{Hirano2023-pams,
     title={{PAMS: Platform for Artificial Market Simulations}},
-    autors={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
+    author={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
     year={2023},
     doi = {10.48550/arXiv.2309.10729}
 }
 ```
 https://arxiv.org/abs/2309.10729
 
 If you prefer to cite this package directly, please use the following bibtex entry:
 ```bibtex
-@misc{Hirano2022-pams
+@misc{Hirano2022-pams,
     title={{PAMS: Platform for Artificial Market Simulations}},
-    autors={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
+    author={Masanori HIRANO, Ryosuke TAKATA, Kiyoshi IZUMI},
     year={2022},
     url = {https://github.com/masanorihirano/pams}
 }
 ```
 
 ## Issues and Contribution
 About issues (bugs):
```

