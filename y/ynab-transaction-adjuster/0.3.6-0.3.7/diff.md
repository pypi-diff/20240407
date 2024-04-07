# Comparing `tmp/ynab_transaction_adjuster-0.3.6.tar.gz` & `tmp/ynab_transaction_adjuster-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-0.3.6.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-0.3.7.tar", max compression
```

## Comparing `ynab_transaction_adjuster-0.3.6.tar` & `ynab_transaction_adjuster-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35148 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/LICENSE
--rw-r--r--   0        0        0     3481 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/README.md
--rw-r--r--   0        0        0      680 2024-04-07 07:55:50.616488 ynab_transaction_adjuster-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     1942 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2481 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0      903 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      358 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0     3209 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0      602 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originalsubtransaction.py
--rw-r--r--   0        0        0     2865 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originaltransaction.py
--rw-r--r--   0        0        0      586 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0     1244 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     1860 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/transactionmodifier.py
--rw-r--r--   0        0        0       72 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1918 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1723 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     4337 2024-04-07 07:55:36.876569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/ynabtransactionadjuster.py
--rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-07 08:02:34.526925 ynab_transaction_adjuster-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3462 2024-04-07 08:02:34.526925 ynab_transaction_adjuster-0.3.7/README.md
+-rw-r--r--   0        0        0      680 2024-04-07 08:02:49.139138 ynab_transaction_adjuster-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2481 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0      903 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      358 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0     3209 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0      602 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originalsubtransaction.py
+-rw-r--r--   0        0        0     2865 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originaltransaction.py
+-rw-r--r--   0        0        0      586 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0     1244 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     1860 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/transactionmodifier.py
+-rw-r--r--   0        0        0       72 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1918 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1723 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     4337 2024-04-07 08:02:34.530925 ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/ynabtransactionadjuster.py
+-rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.7/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-0.3.6/LICENSE` & `ynab_transaction_adjuster-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/README.md` & `ynab_transaction_adjuster-0.3.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,58 +20,59 @@
 ```bash
 pip install ynab-transaction-adjuster
 ```
 
 ## Usage
 A detailed documentation is available at https://ynab-transaction-adjuster.readthedocs.io
 
-### Fetch transactions
-Fetch current transactions from YNAB backend with all available information and check for useful values. All records 
-come with two additional attributes (`import_payee_name` and `import_payee_name_original`) which are not shown in the user 
-interface.
+# Basic Usage
 
+### Create an Adjuster
+Create a child class of `YnabTransactionAdjuster`.
+This class needs to implement a `filter()` and an `adjust()` method which contain the intended logic. The `filter()`
+method receives a list of `OriginalTransaction` objects which can be filtered before 
+adjustement. The `adjust()` method receives a singular `OriginalTransaction` and a 
+`TransactionModifier`. The latter is prefilled with values from the original transaction. 
+Its attributes can be modified, and it needs to be returned at the end of the function. 
+Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section for explanations how to change different attributes.
 ```py
 from ynabtransactionadjuster import YnabTransactionAdjuster
-
-ynab_transaction_adjuster = YnabTransactionAdjuster(token='<token>', budget='<budget>', account='<account>')
-orig_transactions = ynab_transaction_adjuster.fetch()
-```
-
-### Create a `AdjusterFactory` child class
-This class is for implementing your actual logic. It needs to implement a `run()` method which receives on runtime 
-the `OriginalTransaction` and a `TransactionModifier`. The 
-latter is prefilled with values from the original transaction. Its attributes can be modified and it needs to be 
-returned at the end of the function.
-
-```py
-from ynabtransactionadjuster import AdjusterFactory
 from ynabtransactionadjuster.models import OriginalTransaction, TransactionModifier
 
 
-class MyAdjusterFactory(AdjusterFactory):
-
-	def run(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
-		# your implementation
+class MyAdjuster(YnabTransactionAdjuster):
+    
+    def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
+        # your implementation
+        
+        # return the filtered list of transactions
+        return transactions
+        
+    def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
+        # your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
-### Test your Factory class
-Test the factory on records fetched via the `fetch()`method. If only a subset of these transactions should
-get adjusted, filter them before handing the list over to the `adjust()` method. The method returns a list 
-of `ModifiedTransaction` objects which can be inspected for the changed properties.
-
+### Initialize
+Initalize the adjuster with `token`, `budget` and `account` from YNAB
 ```py
-transations = ynab_transaction_adjuster.fetch()
-# optionally filter transactions before passing them to method below
-mod_transactions = ynab_transaction_adjuster.adjust(transactions=transactions, factory_class=MyAdjusterFactory)
+my_adjuster = MyAdjuster(token='<token>', budget='<budget>', account='<account>')
 ```
 
-### Update records in YNAB
-If you are satisfied with your parsing results you can pass the list of the 
-`ModifedTransaction` objects to the `update()` method. It will update  
-the changed transactions in YNAB and return an integer with the number of successfully updated records.
+### Test
+Test the adjuster on records fetched via the `test()`method. The method fetches and executes the 
+adjustments but doesn't write the results back to YNAB. Instead it returns a list of 
+the changed transactions which can be inspected for the changed properties.
+
+```py
+mod_transactions = my_adjuster.test()
+```
 
+### Run
+If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
+adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
+successfully updated records.
 ```py
-count = ynab_transaction_adjuster.update(transactions=mod_transactions)
+count_of_updated_transactions = my_adjuster.run()
 ```
```

### Comparing `ynab_transaction_adjuster-0.3.6/pyproject.toml` & `ynab_transaction_adjuster-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "0.3.6"
+version = "0.3.7"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/adjuster.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/client.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/exceptions.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/modifiedtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originalsubtransaction.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originalsubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originaltransaction.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/originaltransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/transactionmodifier.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/models/transactionmodifier.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/ynabtransactionadjuster.py` & `ynab_transaction_adjuster-0.3.7/ynabtransactionadjuster/ynabtransactionadjuster.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.6/PKG-INFO` & `ynab_transaction_adjuster-0.3.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 0.3.6
+Version: 0.3.7
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,59 +41,60 @@
 ```bash
 pip install ynab-transaction-adjuster
 ```
 
 ## Usage
 A detailed documentation is available at https://ynab-transaction-adjuster.readthedocs.io
 
-### Fetch transactions
-Fetch current transactions from YNAB backend with all available information and check for useful values. All records 
-come with two additional attributes (`import_payee_name` and `import_payee_name_original`) which are not shown in the user 
-interface.
+# Basic Usage
 
+### Create an Adjuster
+Create a child class of `YnabTransactionAdjuster`.
+This class needs to implement a `filter()` and an `adjust()` method which contain the intended logic. The `filter()`
+method receives a list of `OriginalTransaction` objects which can be filtered before 
+adjustement. The `adjust()` method receives a singular `OriginalTransaction` and a 
+`TransactionModifier`. The latter is prefilled with values from the original transaction. 
+Its attributes can be modified, and it needs to be returned at the end of the function. 
+Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section for explanations how to change different attributes.
 ```py
 from ynabtransactionadjuster import YnabTransactionAdjuster
-
-ynab_transaction_adjuster = YnabTransactionAdjuster(token='<token>', budget='<budget>', account='<account>')
-orig_transactions = ynab_transaction_adjuster.fetch()
-```
-
-### Create a `AdjusterFactory` child class
-This class is for implementing your actual logic. It needs to implement a `run()` method which receives on runtime 
-the `OriginalTransaction` and a `TransactionModifier`. The 
-latter is prefilled with values from the original transaction. Its attributes can be modified and it needs to be 
-returned at the end of the function.
-
-```py
-from ynabtransactionadjuster import AdjusterFactory
 from ynabtransactionadjuster.models import OriginalTransaction, TransactionModifier
 
 
-class MyAdjusterFactory(AdjusterFactory):
-
-	def run(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
-		# your implementation
+class MyAdjuster(YnabTransactionAdjuster):
+    
+    def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
+        # your implementation
+        
+        # return the filtered list of transactions
+        return transactions
+        
+    def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
+        # your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
-### Test your Factory class
-Test the factory on records fetched via the `fetch()`method. If only a subset of these transactions should
-get adjusted, filter them before handing the list over to the `adjust()` method. The method returns a list 
-of `ModifiedTransaction` objects which can be inspected for the changed properties.
-
+### Initialize
+Initalize the adjuster with `token`, `budget` and `account` from YNAB
 ```py
-transations = ynab_transaction_adjuster.fetch()
-# optionally filter transactions before passing them to method below
-mod_transactions = ynab_transaction_adjuster.adjust(transactions=transactions, factory_class=MyAdjusterFactory)
+my_adjuster = MyAdjuster(token='<token>', budget='<budget>', account='<account>')
 ```
 
-### Update records in YNAB
-If you are satisfied with your parsing results you can pass the list of the 
-`ModifedTransaction` objects to the `update()` method. It will update  
-the changed transactions in YNAB and return an integer with the number of successfully updated records.
+### Test
+Test the adjuster on records fetched via the `test()`method. The method fetches and executes the 
+adjustments but doesn't write the results back to YNAB. Instead it returns a list of 
+the changed transactions which can be inspected for the changed properties.
+
+```py
+mod_transactions = my_adjuster.test()
+```
 
+### Run
+If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
+adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
+successfully updated records.
 ```py
-count = ynab_transaction_adjuster.update(transactions=mod_transactions)
+count_of_updated_transactions = my_adjuster.run()
 ```
```

