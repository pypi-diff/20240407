# Comparing `tmp/autobean-refactor-0.2.4.tar.gz` & `tmp/autobean-refactor-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-refactor-0.2.4.tar", last modified: Sat Jul  1 13:45:40 2023, max compression
+gzip compressed data, was "autobean-refactor-0.2.5.tar", last modified: Sun Apr  7 17:17:50 2024, max compression
```

## Comparing `autobean-refactor-0.2.4.tar` & `autobean-refactor-0.2.5.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     1065 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/LICENSE
--rw-r--r--   0        0        0      865 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/__init__.py
--rw-r--r--   0        0        0     8351 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/beancount.lark
--rw-r--r--   0        0        0     2328 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/editor.py
--rw-r--r--   0        0        0     1397 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/__init__.py
--rw-r--r--   0        0        0      163 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/account.py
--rw-r--r--   0        0        0       32 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/amount.py
--rw-r--r--   0        0        0       33 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/balance.py
--rw-r--r--   0        0        0     6114 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/base.py
--rw-r--r--   0        0        0     2923 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/block_comment.py
--rw-r--r--   0        0        0      438 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/bool.py
--rw-r--r--   0        0        0       31 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/close.py
--rw-r--r--   0        0        0       35 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/commodity.py
--rw-r--r--   0        0        0       41 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/compound_amount.py
--rw-r--r--   0        0        0     1047 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost.py
--rw-r--r--   0        0        0      336 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost_component.py
--rw-r--r--   0        0        0    11370 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/cost_spec.py
--rw-r--r--   0        0        0      159 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/currency.py
--rw-r--r--   0        0        0     4933 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/custom.py
--rw-r--r--   0        0        0      476 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/date.py
--rw-r--r--   0        0        0     2000 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/document.py
--rw-r--r--   0        0        0     1438 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/escaped_string.py
--rw-r--r--   0        0        0       31 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/event.py
--rw-r--r--   0        0        0      433 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/file.py
--rw-r--r--   0        0        0        0 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/__init__.py
--rw-r--r--   0        0        0     3407 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/amount.py
--rw-r--r--   0        0        0    14881 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/balance.py
--rw-r--r--   0        0        0    11726 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/close.py
--rw-r--r--   0        0        0    11801 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/commodity.py
--rw-r--r--   0        0        0     5834 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/compound_amount.py
--rw-r--r--   0        0        0     2147 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/cost_spec.py
--rw-r--r--   0        0        0    11712 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/custom.py
--rw-r--r--   0        0        0    12638 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/document.py
--rw-r--r--   0        0        0    12716 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/event.py
--rw-r--r--   0        0        0     3763 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/file.py
--rw-r--r--   0        0        0     5480 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/ignored_line.py
--rw-r--r--   0        0        0     8227 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/include.py
--rw-r--r--   0        0        0     9314 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/meta_item.py
--rw-r--r--   0        0        0    12562 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/note.py
--rw-r--r--   0        0        0     2414 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_expr.py
--rw-r--r--   0        0        0     3924 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_paren_expr.py
--rw-r--r--   0        0        0     3055 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/number_unary_expr.py
--rw-r--r--   0        0        0    14245 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/open.py
--rw-r--r--   0        0        0     8947 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/option.py
--rw-r--r--   0        0        0    12819 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pad.py
--rw-r--r--   0        0        0     9249 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/plugin.py
--rw-r--r--   0        0        0     8045 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/popmeta.py
--rw-r--r--   0        0        0     8008 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/poptag.py
--rw-r--r--   0        0        0    15938 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/posting.py
--rw-r--r--   0        0        0    12604 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/price.py
--rw-r--r--   0        0        0     9260 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pushmeta.py
--rw-r--r--   0        0        0     8020 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/pushtag.py
--rw-r--r--   0        0        0    12744 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/query.py
--rw-r--r--   0        0        0     3203 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/tolerance.py
--rw-r--r--   0        0        0     4346 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/total_cost.py
--rw-r--r--   0        0        0     4720 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/total_price.py
--rw-r--r--   0        0        0    15435 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/transaction.py
--rw-r--r--   0        0        0     4152 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_cost.py
--rw-r--r--   0        0        0     4703 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_price.py
--rw-r--r--   0        0        0      162 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/ignored.py
--rw-r--r--   0        0        0       38 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/ignored_line.py
--rw-r--r--   0        0        0       33 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/include.py
--rw-r--r--   0        0        0      423 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/inline_comment.py
--rw-r--r--   0        0        0      318 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/__init__.py
--rw-r--r--   0        0        0      921 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/base_property.py
--rw-r--r--   0        0        0     2213 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/base_token_models.py
--rw-r--r--   0        0        0     7991 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/fields.py
--rw-r--r--   0        0        0      441 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/indexes.py
--rw-r--r--   0        0        0     8020 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/interleaving_comments.py
--rw-r--r--   0        0        0      250 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/placeholder.py
--rw-r--r--   0        0        0    14206 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/properties.py
--rw-r--r--   0        0        0      435 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/registry.py
--rw-r--r--   0        0        0     2810 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/repeated.py
--rw-r--r--   0        0        0     3159 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/spacing_accessors.py
--rw-r--r--   0        0        0     3180 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/surrounding_comments.py
--rw-r--r--   0        0        0      825 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/token_models.py
--rw-r--r--   0        0        0    12620 2023-07-01 13:45:22.514656 autobean-refactor-0.2.4/autobean_refactor/models/internal/value_properties.py
--rw-r--r--   0        0        0      334 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/link.py
--rw-r--r--   0        0        0       35 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_item.py
--rw-r--r--   0        0        0    10447 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_item_internal.py
--rw-r--r--   0        0        0      346 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_key.py
--rw-r--r--   0        0        0      603 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_value.py
--rw-r--r--   0        0        0     2074 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/meta_value_internal.py
--rw-r--r--   0        0        0     1958 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/note.py
--rw-r--r--   0        0        0      170 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/null.py
--rw-r--r--   0        0        0      425 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number.py
--rw-r--r--   0        0        0     3870 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_add_expr.py
--rw-r--r--   0        0        0      326 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_atom_expr.py
--rw-r--r--   0        0        0     9384 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_expr.py
--rw-r--r--   0        0        0     3877 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_mul_expr.py
--rw-r--r--   0        0        0      315 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_paren_expr.py
--rw-r--r--   0        0        0      469 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/number_unary_expr.py
--rw-r--r--   0        0        0       30 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/open.py
--rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/option.py
--rw-r--r--   0        0        0       29 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pad.py
--rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/plugin.py
--rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/popmeta.py
--rw-r--r--   0        0        0       32 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/poptag.py
--rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/posting.py
--rw-r--r--   0        0        0      168 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/posting_flag.py
--rw-r--r--   0        0        0       31 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/price.py
--rw-r--r--   0        0        0      831 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/punctuation.py
--rw-r--r--   0        0        0       34 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pushmeta.py
--rw-r--r--   0        0        0       33 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/pushtag.py
--rw-r--r--   0        0        0       31 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/query.py
--rw-r--r--   0        0        0      420 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/spacing.py
--rw-r--r--   0        0        0      331 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/tag.py
--rw-r--r--   0        0        0      592 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/tolerance.py
--rw-r--r--   0        0        0       37 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/total_price.py
--rw-r--r--   0        0        0     4926 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/transaction.py
--rw-r--r--   0        0        0      409 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/transaction_flag.py
--rw-r--r--   0        0        0       36 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/models/unit_price.py
--rw-r--r--   0        0        0     9046 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/parser.py
--rw-r--r--   0        0        0      256 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/printer.py
--rw-r--r--   0        0        0        0 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/py.typed
--rw-r--r--   0        0        0    13605 2023-07-01 13:45:22.518656 autobean-refactor-0.2.4/autobean_refactor/token_store.py
--rw-r--r--   0        0        0      923 2023-07-01 13:45:22.522656 autobean-refactor-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 autobean-refactor-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/LICENSE
+-rw-r--r--   0        0        0      865 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/__init__.py
+-rw-r--r--   0        0        0     8351 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/beancount.lark
+-rw-r--r--   0        0        0     2381 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/editor.py
+-rw-r--r--   0        0        0     1397 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/account.py
+-rw-r--r--   0        0        0       32 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/amount.py
+-rw-r--r--   0        0        0       33 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/balance.py
+-rw-r--r--   0        0        0     6114 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/base.py
+-rw-r--r--   0        0        0     2923 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/block_comment.py
+-rw-r--r--   0        0        0      438 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/bool.py
+-rw-r--r--   0        0        0       31 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/close.py
+-rw-r--r--   0        0        0       35 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/commodity.py
+-rw-r--r--   0        0        0       41 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/compound_amount.py
+-rw-r--r--   0        0        0     1047 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/cost.py
+-rw-r--r--   0        0        0      336 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/cost_component.py
+-rw-r--r--   0        0        0    11370 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/cost_spec.py
+-rw-r--r--   0        0        0      159 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/currency.py
+-rw-r--r--   0        0        0     4933 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/custom.py
+-rw-r--r--   0        0        0      476 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/date.py
+-rw-r--r--   0        0        0     2000 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/document.py
+-rw-r--r--   0        0        0     1438 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/escaped_string.py
+-rw-r--r--   0        0        0       31 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/event.py
+-rw-r--r--   0        0        0      433 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/file.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/__init__.py
+-rw-r--r--   0        0        0     3407 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/amount.py
+-rw-r--r--   0        0        0    14881 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/balance.py
+-rw-r--r--   0        0        0    11726 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/close.py
+-rw-r--r--   0        0        0    11801 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/commodity.py
+-rw-r--r--   0        0        0     5834 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/compound_amount.py
+-rw-r--r--   0        0        0     2147 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/cost_spec.py
+-rw-r--r--   0        0        0    11712 2024-04-07 17:17:36.767094 autobean-refactor-0.2.5/autobean_refactor/models/generated/custom.py
+-rw-r--r--   0        0        0    12638 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/document.py
+-rw-r--r--   0        0        0    12716 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/event.py
+-rw-r--r--   0        0        0     3763 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/file.py
+-rw-r--r--   0        0        0     5480 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/ignored_line.py
+-rw-r--r--   0        0        0     8227 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/include.py
+-rw-r--r--   0        0        0     9314 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/meta_item.py
+-rw-r--r--   0        0        0    12562 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/note.py
+-rw-r--r--   0        0        0     2414 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/number_expr.py
+-rw-r--r--   0        0        0     3924 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/number_paren_expr.py
+-rw-r--r--   0        0        0     3055 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/number_unary_expr.py
+-rw-r--r--   0        0        0    14245 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/open.py
+-rw-r--r--   0        0        0     8947 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/option.py
+-rw-r--r--   0        0        0    12819 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/pad.py
+-rw-r--r--   0        0        0     9249 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/plugin.py
+-rw-r--r--   0        0        0     8045 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/popmeta.py
+-rw-r--r--   0        0        0     8008 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/poptag.py
+-rw-r--r--   0        0        0    15938 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/posting.py
+-rw-r--r--   0        0        0    12604 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/price.py
+-rw-r--r--   0        0        0     9260 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/pushmeta.py
+-rw-r--r--   0        0        0     8020 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/pushtag.py
+-rw-r--r--   0        0        0    12744 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/query.py
+-rw-r--r--   0        0        0     3203 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/tolerance.py
+-rw-r--r--   0        0        0     4346 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/total_cost.py
+-rw-r--r--   0        0        0     4720 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/total_price.py
+-rw-r--r--   0        0        0    15435 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/transaction.py
+-rw-r--r--   0        0        0     4152 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/unit_cost.py
+-rw-r--r--   0        0        0     4703 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/generated/unit_price.py
+-rw-r--r--   0        0        0      162 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/ignored.py
+-rw-r--r--   0        0        0       38 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/ignored_line.py
+-rw-r--r--   0        0        0       33 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/include.py
+-rw-r--r--   0        0        0      423 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/inline_comment.py
+-rw-r--r--   0        0        0      318 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/__init__.py
+-rw-r--r--   0        0        0      921 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/base_property.py
+-rw-r--r--   0        0        0     2213 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/base_token_models.py
+-rw-r--r--   0        0        0     7991 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/fields.py
+-rw-r--r--   0        0        0      441 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/indexes.py
+-rw-r--r--   0        0        0     8020 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/interleaving_comments.py
+-rw-r--r--   0        0        0      250 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/placeholder.py
+-rw-r--r--   0        0        0    14206 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/properties.py
+-rw-r--r--   0        0        0      435 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/registry.py
+-rw-r--r--   0        0        0     2810 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/repeated.py
+-rw-r--r--   0        0        0     3159 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/spacing_accessors.py
+-rw-r--r--   0        0        0     3180 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/surrounding_comments.py
+-rw-r--r--   0        0        0      825 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/token_models.py
+-rw-r--r--   0        0        0    12620 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/internal/value_properties.py
+-rw-r--r--   0        0        0      334 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/link.py
+-rw-r--r--   0        0        0       35 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/meta_item.py
+-rw-r--r--   0        0        0    10447 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/meta_item_internal.py
+-rw-r--r--   0        0        0      346 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/meta_key.py
+-rw-r--r--   0        0        0      603 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/meta_value.py
+-rw-r--r--   0        0        0     2074 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/meta_value_internal.py
+-rw-r--r--   0        0        0     1958 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/note.py
+-rw-r--r--   0        0        0      170 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/null.py
+-rw-r--r--   0        0        0      425 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number.py
+-rw-r--r--   0        0        0     3870 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_add_expr.py
+-rw-r--r--   0        0        0      326 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_atom_expr.py
+-rw-r--r--   0        0        0     9384 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_expr.py
+-rw-r--r--   0        0        0     3877 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_mul_expr.py
+-rw-r--r--   0        0        0      315 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_paren_expr.py
+-rw-r--r--   0        0        0      469 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/number_unary_expr.py
+-rw-r--r--   0        0        0       30 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/open.py
+-rw-r--r--   0        0        0       32 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/option.py
+-rw-r--r--   0        0        0       29 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/pad.py
+-rw-r--r--   0        0        0       32 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/plugin.py
+-rw-r--r--   0        0        0       33 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/popmeta.py
+-rw-r--r--   0        0        0       32 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/poptag.py
+-rw-r--r--   0        0        0       33 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/posting.py
+-rw-r--r--   0        0        0      168 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/posting_flag.py
+-rw-r--r--   0        0        0       31 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/price.py
+-rw-r--r--   0        0        0      831 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/punctuation.py
+-rw-r--r--   0        0        0       34 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/pushmeta.py
+-rw-r--r--   0        0        0       33 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/pushtag.py
+-rw-r--r--   0        0        0       31 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/query.py
+-rw-r--r--   0        0        0      420 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/spacing.py
+-rw-r--r--   0        0        0      331 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/tag.py
+-rw-r--r--   0        0        0      592 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/tolerance.py
+-rw-r--r--   0        0        0       37 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/total_price.py
+-rw-r--r--   0        0        0     4926 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/transaction.py
+-rw-r--r--   0        0        0      409 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/transaction_flag.py
+-rw-r--r--   0        0        0       36 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/models/unit_price.py
+-rw-r--r--   0        0        0     9046 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/parser.py
+-rw-r--r--   0        0        0      256 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/printer.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:17:36.771093 autobean-refactor-0.2.5/autobean_refactor/py.typed
+-rw-r--r--   0        0        0    13605 2024-04-07 17:17:36.775093 autobean-refactor-0.2.5/autobean_refactor/token_store.py
+-rw-r--r--   0        0        0      923 2024-04-07 17:17:36.779093 autobean-refactor-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 autobean-refactor-0.2.5/PKG-INFO
```

### Comparing `autobean-refactor-0.2.4/LICENSE` & `autobean-refactor-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/README.md` & `autobean-refactor-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/beancount.lark` & `autobean-refactor-0.2.5/autobean_refactor/beancount.lark`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/editor.py` & `autobean-refactor-0.2.5/autobean_refactor/editor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections
 import contextlib
 import glob
 import io
 import os.path
+import pathlib
 from typing import Iterator, Optional
 from autobean_refactor import parser as parser_lib, models, printer
 
 
 def _get_include_paths(path: str, file: models.File) -> Iterator[str]:
     for directive in file.raw_directives:
         if not isinstance(directive, models.Include):
@@ -22,24 +23,23 @@
 class Editor:
 
     def __init__(self, parser: Optional[parser_lib.Parser] = None) -> None:
         self._parser = parser or parser_lib.Parser()
 
     @contextlib.contextmanager
     def edit_file(self, path: os.PathLike) -> Iterator[models.File]:
-        with open(path) as f:
-            text = f.read()
+        p = pathlib.Path(path)
+        text = p.read_text()
         file = self._parser.parse(text, models.File)
 
         yield file
 
         updated_text = printer.print_model(file, io.StringIO()).getvalue()
         if updated_text != text:
-            with open(path, 'w') as f:
-                f.write(updated_text)
+            p.write_text(updated_text)
 
     @contextlib.contextmanager
     def edit_file_recursive(self, path: os.PathLike) -> Iterator[dict[str, models.File]]:
         texts = dict[str, str]()
         files = dict[str, models.File]()
         queue = collections.deque([os.path.normpath(path)])
 
@@ -53,11 +53,12 @@
             queue.extend(_get_include_paths(current_path, files[current_path]))
 
         yield files
 
         for current_path in set(texts) - set(files):
             os.unlink(current_path)
         for current_path, file in files.items():
+            os.makedirs(os.path.dirname(current_path), exist_ok=True)
             updated_text = printer.print_model(file, io.StringIO()).getvalue()
-            if updated_text != texts[current_path]:
+            if updated_text != texts.get(current_path):
                 with open(current_path, 'w') as f:
                     f.write(updated_text)
```

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/__init__.py` & `autobean-refactor-0.2.5/autobean_refactor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/base.py` & `autobean-refactor-0.2.5/autobean_refactor/models/base.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/block_comment.py` & `autobean-refactor-0.2.5/autobean_refactor/models/block_comment.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/cost.py` & `autobean-refactor-0.2.5/autobean_refactor/models/cost.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/cost_spec.py` & `autobean-refactor-0.2.5/autobean_refactor/models/cost_spec.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/custom.py` & `autobean-refactor-0.2.5/autobean_refactor/models/custom.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/document.py` & `autobean-refactor-0.2.5/autobean_refactor/models/document.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/escaped_string.py` & `autobean-refactor-0.2.5/autobean_refactor/models/escaped_string.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/amount.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/amount.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/balance.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/balance.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/close.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/close.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/commodity.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/commodity.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/compound_amount.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/compound_amount.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/cost_spec.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/cost_spec.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/custom.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/custom.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/document.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/document.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/event.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/event.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/file.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/file.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/ignored_line.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/ignored_line.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/include.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/include.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/meta_item.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/meta_item.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/note.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/note.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/number_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_paren_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/number_paren_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/number_unary_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/number_unary_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/open.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/open.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/option.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/option.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/pad.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/pad.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/plugin.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/popmeta.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/popmeta.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/poptag.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/poptag.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/posting.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/posting.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/price.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/price.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/pushmeta.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/pushmeta.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/pushtag.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/pushtag.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/query.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/query.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/tolerance.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/tolerance.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/total_cost.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/total_cost.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/total_price.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/total_price.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/transaction.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/transaction.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_cost.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/unit_cost.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/generated/unit_price.py` & `autobean-refactor-0.2.5/autobean_refactor/models/generated/unit_price.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/base_property.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/base_property.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/base_token_models.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/base_token_models.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/fields.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/fields.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/interleaving_comments.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/interleaving_comments.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/properties.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/properties.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/repeated.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/repeated.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/spacing_accessors.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/spacing_accessors.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/surrounding_comments.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/surrounding_comments.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/token_models.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/token_models.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/internal/value_properties.py` & `autobean-refactor-0.2.5/autobean_refactor/models/internal/value_properties.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/meta_item_internal.py` & `autobean-refactor-0.2.5/autobean_refactor/models/meta_item_internal.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/meta_value.py` & `autobean-refactor-0.2.5/autobean_refactor/models/meta_value.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/meta_value_internal.py` & `autobean-refactor-0.2.5/autobean_refactor/models/meta_value_internal.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/note.py` & `autobean-refactor-0.2.5/autobean_refactor/models/note.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/number_add_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/number_add_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/number_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/number_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/number_mul_expr.py` & `autobean-refactor-0.2.5/autobean_refactor/models/number_mul_expr.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/punctuation.py` & `autobean-refactor-0.2.5/autobean_refactor/models/punctuation.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/tolerance.py` & `autobean-refactor-0.2.5/autobean_refactor/models/tolerance.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/models/transaction.py` & `autobean-refactor-0.2.5/autobean_refactor/models/transaction.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/parser.py` & `autobean-refactor-0.2.5/autobean_refactor/parser.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/autobean_refactor/token_store.py` & `autobean-refactor-0.2.5/autobean_refactor/token_store.py`

 * *Files identical despite different names*

### Comparing `autobean-refactor-0.2.4/pyproject.toml` & `autobean-refactor-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "autobean-refactor"
-version = "0.2.4"
+version = "0.2.5"
 description = "An ergonomic and losess beancount manipulation library"
 authors = [
     { name = "SEIAROTg", email = "seiarotg@gmail.com" },
 ]
 dependencies = [
     "lark>=1.1.5",
     "typing-extensions>=4.4.0",
```

### Comparing `autobean-refactor-0.2.4/PKG-INFO` & `autobean-refactor-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobean-refactor
-Version: 0.2.4
+Version: 0.2.5
 Summary: An ergonomic and losess beancount manipulation library
 License: MIT
 Author-email: SEIAROTg <seiarotg@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # autobean-refactor
```

