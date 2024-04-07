# Comparing `tmp/ynab_transaction_adjuster-0.3.5.tar.gz` & `tmp/ynab_transaction_adjuster-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-0.3.5.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-0.3.6.tar", max compression
```

## Comparing `ynab_transaction_adjuster-0.3.5.tar` & `ynab_transaction_adjuster-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35148 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/LICENSE
--rw-r--r--   0        0        0     3481 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/README.md
--rw-r--r--   0        0        0      680 2024-03-27 06:10:30.514125 ynab_transaction_adjuster-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       84 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     1942 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2481 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0      903 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      358 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0     4090 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0      602 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/originalsubtransaction.py
--rw-r--r--   0        0        0     2856 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/originaltransaction.py
--rw-r--r--   0        0        0      586 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0     1244 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     1860 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/transactionmodifier.py
--rw-r--r--   0        0        0       72 2024-03-27 06:10:12.729881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1918 2024-03-27 06:10:12.733881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1723 2024-03-27 06:10:12.733881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     4337 2024-03-27 06:10:12.733881 ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/ynabtransactionadjuster.py
--rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3481 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/README.md
+-rw-r--r--   0        0        0      680 2024-04-07 07:55:50.616488 ynab_transaction_adjuster-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2481 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0      903 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      358 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0     3209 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0      602 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originalsubtransaction.py
+-rw-r--r--   0        0        0     2865 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originaltransaction.py
+-rw-r--r--   0        0        0      586 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0     1244 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     1860 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/transactionmodifier.py
+-rw-r--r--   0        0        0       72 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1918 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1723 2024-04-07 07:55:36.872569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     4337 2024-04-07 07:55:36.876569 ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/ynabtransactionadjuster.py
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.6/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-0.3.5/LICENSE` & `ynab_transaction_adjuster-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/README.md` & `ynab_transaction_adjuster-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/pyproject.toml` & `ynab_transaction_adjuster-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "0.3.5"
+version = "0.3.6"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/adjuster.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/client.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/exceptions.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/ynabtransactionadjuster.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,93 @@
-from datetime import datetime
+from abc import abstractmethod
+from typing import List
 
-from pydantic import BaseModel, model_validator
-
-from ynabtransactionadjuster.models.originaltransaction import OriginalTransaction
-from ynabtransactionadjuster.models.transactionmodifier import TransactionModifier
-
-
-class ModifiedTransaction(BaseModel):
-	original_transaction: OriginalTransaction
-	transaction_modifier: TransactionModifier
-
-	def is_changed(self) -> bool:
-		"""Helper function to determine if transaction has been altered as compared to original one
-
-		:returns: True if values from original transaction have been altered, False otherwise
+from ynabtransactionadjuster.adjuster import Adjuster
+from ynabtransactionadjuster.client import Client
+from ynabtransactionadjuster.models import OriginalTransaction, ModifiedTransaction
+from ynabtransactionadjuster.models import TransactionModifier
+from ynabtransactionadjuster.repos import CategoryRepo
+from ynabtransactionadjuster.repos import PayeeRepo
+
+
+class YnabTransactionAdjuster:
+	"""Abstract class which modifies transactions according to concrete implementation. You need to create your own
+	child class and implement the `filter()`and `adjust()` method in it according to your needs. It has attributes
+	which allow you to lookup categories and payees from your budget.
+
+	:param budget: The YNAB budget id to use
+	:param account: The YNAB account id to use
+	:param token: The YNAB token to use
+
+	:ivar categories: Collection of current categories in YNAB budget
+	:ivar payees: Collection of current payees in YNAB budget
+	"""
+	def __init__(self, budget: str, account: str, token: str) -> None:
+		self._budget = budget
+		self._account = account
+		self._client = Client(token=token, budget=budget, account=account)
+		self.categories: CategoryRepo = CategoryRepo(self._client.fetch_categories())
+		self.payees: PayeeRepo = PayeeRepo(self._client.fetch_payees())
+
+	def run(self) -> int:
+		"""Run the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
+		implementation of the two methods and push the updated transactions back to YNAB
+
+		:return: count of adjusted transactions which have been updated in YNAB
+		:raises AdjustError: if there is any error during the adjust process
+		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		"""
+		transactions = self._client.fetch_transactions()
+		filtered_transactions = self.filter(transactions)
+		adjuster = Adjuster(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
+		modified_transactions = adjuster.run()
+		updated = self._client.update_transactions(modified_transactions)
+		return updated
+
+	def test(self) -> List[dict]:
+		"""Tests the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
+		implementation of the two methods. This function doesn't update records in YNAB but returns the modified
+		transactions so that they can be inspected. `#! select * from source`
+
+		The returned dicts have the following structure:
+
+			{
+				"original": "<OriginalTransaction>",
+			 	"changes": {
+			 		"<Attribute>": {
+			 			"original": "<Original Value>",
+			 			"changed": "<Changed Value>"
+			 			}
+					}
+				}
+
+		:return: List of modified transactions in the format
+		:raises AdjustError: if there is any error during the adjust process
+		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		"""
+		transactions = self._client.fetch_transactions()
+		filtered_transactions = self.filter(transactions)
+		sa = Adjuster(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
+		modified_transactions = [{'original': mt.original_transaction, 'changes': mt.changed_attributes()} for mt in sa.run()]
+		return modified_transactions
+
+	@abstractmethod
+	def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
+		"""Function which implements filtering for the list of transactions from YNAB account. It receives a list of
+		the original transactions which can be filtered. Must return the filtered list or just the list if no filtering
+		is intended.
+
+		:param transactions: List of original transactions from YNAB
+		:return: Method needs to return a list of filtered transactions"""
+		pass
+
+	@abstractmethod
+	def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
+		"""Function which implements the actual modification of a transaction. It receives the original transaction from
+		YNAB and a prefilled modifier. The modifier can be altered and must be returned.
+
+		:param original: Original transaction
+		:param modifier: Transaction modifier prefilled with values from original transaction. All attributes can be
+		changed and will modify the transaction
+		:returns: Method needs to return the transaction modifier after modification
 		"""
-		if self.changed_attributes():
-			return True
-		return False
-
-	def as_dict(self) -> dict:
-		"""Returns a dictionary representation of the transaction which is used for the update call to YNAB"""
-		t_dict = dict(id=self.original_transaction.id,
-					payee_name=self.transaction_modifier.payee.name,
-					payee_id=self.transaction_modifier.payee.id,
-					date=datetime.strftime(self.transaction_modifier.transaction_date, '%Y-%m-%d'),
-					approved=self.transaction_modifier.approved,
-					cleared=self.transaction_modifier.cleared)
-		if len(self.transaction_modifier.subtransactions) > 0:
-			t_dict['subtransactions'] = [s.as_dict() for s in self.transaction_modifier.subtransactions]
-		if self.transaction_modifier.category:
-			t_dict['category_id'] = self.transaction_modifier.category.id
-		if self.transaction_modifier.flag_color:
-			t_dict['flag_color'] = self.transaction_modifier.flag_color
-		if self.transaction_modifier.memo:
-			t_dict['memo'] = self.transaction_modifier.memo
-
-		return t_dict
-
-	def changed_attributes(self) -> dict:
-		"""Returns a dictionary representation of the modified values and the original transaction"""
-		changed_attributes = {}
-		if self.transaction_modifier.payee != self.original_transaction.payee:
-			changed_attributes['payee'] = dict(original=self.original_transaction.payee,
-											   changed=self.transaction_modifier.payee)
-		if (self.transaction_modifier.transaction_date.isocalendar() !=
-				self.original_transaction.transaction_date.isocalendar()):
-			changed_attributes['transaction_date'] = dict(original=self.original_transaction.transaction_date,
-														  changed=self.transaction_modifier.transaction_date)
-		if (self.transaction_modifier.category and
-				self.transaction_modifier.category.id != self.original_transaction.category.id):
-			changed_attributes['category'] = dict(original=self.original_transaction.category,
-												  changed=self.transaction_modifier.category)
-		if self.transaction_modifier.memo != self.original_transaction.memo:
-			changed_attributes['memo'] = dict(original=self.original_transaction.memo,
-											  changed=self.transaction_modifier.memo)
-		if self.transaction_modifier.flag_color != self.original_transaction.flag_color:
-			changed_attributes['flag_color'] = dict(original=self.original_transaction.flag_color,
-													changed=self.transaction_modifier.flag_color)
-		if len(self.transaction_modifier.subtransactions) > 0:
-			changed_attributes['subtransactions'] = dict(original=[],
-														 changed=self.transaction_modifier.subtransactions)
-		if self.transaction_modifier.approved != self.original_transaction.approved:
-			changed_attributes['approved'] = dict(original=self.original_transaction.approved,
-												  changed=self.transaction_modifier.approved)
-		if self.transaction_modifier.cleared != self.original_transaction.cleared:
-			changed_attributes['cleared'] = dict(original=self.original_transaction.cleared,
-												 changed=self.transaction_modifier.cleared)
-		return changed_attributes
-
-	@model_validator(mode='after')
-	def check_values(self):
-		if len(self.transaction_modifier.subtransactions) > 1:
-			if len(self.original_transaction.subtransactions) > 1:
-				raise ValueError(f"Existing Subtransactions can not be updated")
-			if sum(a.amount for a in self.transaction_modifier.subtransactions) != self.original_transaction.amount:
-				raise ValueError('Amount of subtransactions needs to be equal to amount of original transaction')
-		return self
+		pass
```

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/originalsubtransaction.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originalsubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/originaltransaction.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/originaltransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Literal, Optional, Tuple
 
 from ynabtransactionadjuster.models.category import Category
 from ynabtransactionadjuster.models.payee import Payee
 from ynabtransactionadjuster.models.originalsubtransaction import OriginalSubTransaction
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, eq=True)
 class OriginalTransaction:
 	"""Represents original transaction from YNAB
 
 	:ivar id: The original transaction id
 	:ivar amount: The transaction amount in milliunits format
 	:ivar category: The category of the original transaction
 	:ivar transaction_date: The date of the original transaction
```

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/models/transactionmodifier.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/models/transactionmodifier.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-0.3.6/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.5/PKG-INFO` & `ynab_transaction_adjuster-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 0.3.5
+Version: 0.3.6
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

