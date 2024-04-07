# Comparing `tmp/nablachem-24.4.tar.gz` & `tmp/nablachem-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nablachem-24.4.tar", max compression
+gzip compressed data, was "nablachem-24.5.tar", max compression
```

## Comparing `nablachem-24.4.tar` & `nablachem-24.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.4/LICENSE
--rw-r--r--   0        0        0      559 2024-01-22 10:02:27.526533 nablachem-24.4/README.md
--rw-r--r--   0        0        0      553 2024-04-04 14:23:12.466569 nablachem-24.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.4/src/nablachem/__init__.py
--rw-r--r--   0        0        0    12152 2024-04-04 14:19:27.006647 nablachem-24.4/src/nablachem/alchemy.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nablachem-24.4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.5/LICENSE
+-rw-r--r--   0        0        0      559 2024-01-22 10:02:27.526533 nablachem-24.5/README.md
+-rw-r--r--   0        0        0      553 2024-04-07 14:07:11.586964 nablachem-24.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.5/src/nablachem/__init__.py
+-rw-r--r--   0        0        0    16621 2024-04-07 14:00:22.947057 nablachem-24.5/src/nablachem/alchemy.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nablachem-24.5/PKG-INFO
```

### Comparing `nablachem-24.4/LICENSE` & `nablachem-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nablachem-24.4/README.md` & `nablachem-24.5/README.md`

 * *Files identical despite different names*

### Comparing `nablachem-24.4/pyproject.toml` & `nablachem-24.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nablachem"
-version = "24.4"
+version = "24.5"
 description = "Easy access to research code."
 authors = ["von Rudorff, Guido Falk <vonrudorff@uni-kassel.de>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://nablachem.org/code"
 repository = "https://github.com/NablaChem/nablachem"
```

### Comparing `nablachem-24.4/src/nablachem/alchemy.py` & `nablachem-24.5/src/nablachem/alchemy.py`

 * *Files 23% similar despite different names*

```diff
@@ -166,38 +166,131 @@
         ------
         ValueError
             Could not build stencil.
         ValueError
             Not enough points in the stencil for a given order.
         """
         offsets, ordering = shifted
-
         term_counter = collections.Counter(term)
         indices = tuple([term_counter[_] for _ in ordering])
+        order = len(term)
 
-        offsets = tuple(map(tuple, offsets))
-        try:
-            stencil = findiff.stencils.Stencil(
-                offsets, partials={indices: 1}, spacings=1
+        # shortcut for stencils similar to central differences
+        # often it is sufficient to have one value per combination of changes
+        # e.g. in 1D, select one point to the left, one to the right of the center
+        # e.g. in 2D, select one point from every quadrant, plus the center
+        shortcut = None
+        mask_center = np.all(offsets == 0, axis=1)
+        if len(set(term)) == 1:
+            column_mask = offsets[0, :] != offsets[0, :]
+            column_mask[ordering.index(term[0])] = True
+            shortcut = (offsets[:, column_mask] != 0).reshape(-1) & np.all(
+                offsets[:, ~column_mask] == 0, axis=1
             )
-        except:
-            raise ValueError(f"Could not build stencil for term {term}.")
-        if len(stencil.values) == 0:
-            raise ValueError(f"Not enough points for term {term}.")
-
-        for output in self._outputs:
-            weights = [stencil.values[_] if _ in stencil.values else 0 for _ in offsets]
-            values = self._filtered[output].values
-
-            self._monomials[output].append(
-                Monomial(
-                    prefactor=np.dot(weights, values),
-                    powers=dict(term_counter),
+            shortcut |= mask_center
+        if len(set(term)) > 0:
+            n_distinct_columns = len(set(term))
+            shortcut = mask_center
+            column_mask = np.array([False] * offsets.shape[1])
+            for column in term:
+                column_mask[ordering.index(column)] = True
+            other_columns_are_centered = np.all(offsets[:, ~column_mask] == 0, axis=1)
+            for hypercube in it.product((False, True), repeat=n_distinct_columns):
+                hypercube_mask = True
+                for sign, column in zip(hypercube, term):
+                    hypercube_mask &= (offsets[:, ordering.index(column)] > 0) == sign
+                hypercube_mask &= other_columns_are_centered
+                hypercube_mask &= ~mask_center
+
+                # keep only a few from this hypercube
+                # avoids slowdown because of very imbalanced data-sets
+                # parameter "extra" is free to choose (>0), should be generous
+                # choose closest to origin
+                extra = 3
+                all_selected = np.where(hypercube_mask)[0]
+                distance = np.linalg.norm(offsets[hypercube_mask, :], axis=1)
+                keep = order + extra
+                if len(distance) > keep:
+                    too_far = np.argpartition(distance, keep)[keep:]
+                    too_far = all_selected[too_far]
+                    hypercube_mask[too_far] = False
+
+                shortcut |= hypercube_mask
+
+            for this, count in term_counter.items():
+                if count < 2:
+                    continue
+
+                column_mask[True] = True
+                for column in term:
+                    column_mask[ordering.index(column)] = False
+                column_mask[ordering.index(this)] = True
+
+                higher_order_mask = np.all(offsets[:, column_mask] == 0, axis=1)
+                shortcut |= higher_order_mask
+
+        # auxiliary heuristics for viable subsets
+        relevant_indices = [i for i, v in enumerate(indices) if v != 0]
+        mask_changed = ~np.all(offsets[:, relevant_indices] == 0, axis=1)
+        base_mask = mask_changed | mask_center
+
+        mask_up_to_order = np.sum(offsets != 0, axis=1) <= order
+
+        # try with simple masks first
+        tries = [
+            shortcut,
+            base_mask & mask_up_to_order,
+            base_mask,
+            base_mask | ~base_mask,
+        ]
+        for mask in tries:
+            subset_offsets = offsets[mask, :]
+
+            # condense: drop all columns which are all zeros
+            non_zero_columns = np.where(~np.all(subset_offsets == 0, axis=0))[0]
+            subset_offsets = subset_offsets[:, non_zero_columns]
+
+            # make sure that no non-zero index is dropped
+            abort_mask = False
+            for i in range(len(indices)):
+                if indices[i] > 0 and i not in non_zero_columns:
+                    abort_mask = True
+                    break
+            if abort_mask:
+                continue
+
+            indices = tuple([indices[_] for _ in non_zero_columns])
+
+            subset_offsets = tuple(map(tuple, subset_offsets))
+            try:
+                stencil = findiff.stencils.Stencil(
+                    subset_offsets, partials={indices: 1}, spacings=1
                 )
-            )
+            except:
+                # Numerical issue -> next try
+                continue
+            # Did not find a stencil -> next try
+            if len(stencil.values) == 0:
+                continue
+
+            for output in self._outputs:
+                weights = [
+                    stencil.values[_] if _ in stencil.values else 0
+                    for _ in subset_offsets
+                ]
+                values = self._filtered[output].values[mask]
+
+                self._monomials[output].append(
+                    Monomial(
+                        prefactor=np.dot(weights, values),
+                        powers=dict(term_counter),
+                    )
+                )
+            return
+        raise ValueError(f"Could not build stencil for term {term}.")
 
     def _all_terms_up_to(self, order: int) -> tuple[tuple[str]]:
         """For all remaining input columns, find all possible terms entering a Taylor expansion.
 
         Parameters
         ----------
         order : int
@@ -212,21 +305,28 @@
         data_columns = [_ for _ in self._filtered.columns if _ not in self._outputs]
         data_columns = [_ for _ in data_columns if not _ in self._filter.keys()]
         for order in range(1, order + 1):
             for entry in it.combinations_with_replacement(data_columns, order):
                 terms.append(entry)
         return tuple(terms)
 
-    def build_model(self, orders: int):
-        """Sets up the model for a specific expansion order.
+    def build_model(self, orders: int, additional_terms: list[tuple[str]] = []):
+        """Sets up the model for a specific expansion order or list of terms.
 
         Parameters
         ----------
         orders : int
             All terms are included in the expansion up to this order.
+        additional_terms : list[tuple[str]]
+            The terms to ADDITIONALLY include, i.e. list of tuples of column names.
+
+            To only include d/dx, give [('x',)]
+            To only include d^2/dx^2, give [('x', 'x')]
+            To only include d^2/dxdy, give [('x', 'y')]
+            To include all three, give [('x',), ('x', 'x'), ('x', 'y')]
 
         Raises
         ------
         NotImplementedError
             Center needs to be given in dataframe.
         ValueError
             Center is not unique.
@@ -247,15 +347,15 @@
             self._filtered
         ):
             raise ValueError(f"Duplicate points in the dataset.")
 
         # setup constant term
         self._monomials = {k: [Monomial(center_row.iloc[0][k])] for k in self._outputs}
 
-        terms = self._all_terms_up_to(orders)
+        terms = tuple(list(self._all_terms_up_to(orders)) + list(additional_terms))
         if len(terms) > len(shifted[0]):
             raise ValueError(
                 f"Not enough points: {len(terms)} required, {len(shifted[0])} given."
             )
         for term in terms:
             self._build_monomials(term, shifted)
```

### Comparing `nablachem-24.4/PKG-INFO` & `nablachem-24.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nablachem
-Version: 24.4
+Version: 24.5
 Summary: Easy access to research code.
 Home-page: https://nablachem.org/code
 License: LGPL
 Author: von Rudorff, Guido Falk
 Author-email: vonrudorff@uni-kassel.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

