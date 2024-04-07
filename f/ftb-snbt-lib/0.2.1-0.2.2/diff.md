# Comparing `tmp/ftb-snbt-lib-0.2.1.tar.gz` & `tmp/ftb-snbt-lib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb-snbt-lib-0.2.1.tar", last modified: Fri Apr  5 14:19:18 2024, max compression
+gzip compressed data, was "ftb-snbt-lib-0.2.2.tar", last modified: Sun Apr  7 05:23:04 2024, max compression
```

## Comparing `ftb-snbt-lib-0.2.1.tar` & `ftb-snbt-lib-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.716735 ftb-snbt-lib-0.2.2/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 05:23:04.000000 ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 05:23:04.720735 ftb-snbt-lib-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 05:23:00.000000 ftb-snbt-lib-0.2.2/setup.py
```

### Comparing `ftb-snbt-lib-0.2.1/LICENSE` & `ftb-snbt-lib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/PKG-INFO` & `ftb-snbt-lib-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -106,15 +106,16 @@
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
```

### Comparing `ftb-snbt-lib-0.2.1/README.md` & `ftb-snbt-lib-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,16 @@
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
```

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/parse.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 def p_value(p):
     """value : compound
                 | list
                 | array
                 | BOOL
                 | BYTE
                 | SHORT
+                | FLOAT
                 | DOUBLE
                 | LONG
                 | INTEGER
                 | STRING"""
     p[0] = p[1]
 
 def p_list(p):
```

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/parsetab.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/parsetab.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET SEMICOLON SHORT STRINGsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | array\n                | BOOL\n                | BYTE\n                | SHORT\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETarray : LBRACKET NAME SEMICOLON values RBRACKET\n                | LBRACKET NAME SEMICOLON RBRACKETvalues : values value\n              | values COMMA value\n              | value'
+_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE FLOAT INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET SEMICOLON SHORT STRINGsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | array\n                | BOOL\n                | BYTE\n                | SHORT\n                | FLOAT\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETarray : LBRACKET NAME SEMICOLON values RBRACKET\n                | LBRACKET NAME SEMICOLON RBRACKETvalues : values value\n              | values COMMA value\n              | value'
     
-_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,3,3,-20,-25,-19,-23,3,3,-24,3,-22,-21,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,27,29,32,38,39,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-8,-20,-19,-22,-21,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,24,25,26,27,29,32,38,39,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,30,-8,-20,-19,-22,-21,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,31,32,33,34,35,36,37,38,39,],[8,8,-3,-6,-2,-4,8,25,25,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,25,-8,25,-20,-25,-19,-23,25,25,-24,25,-22,-21,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,27,28,29,31,32,33,36,37,38,39,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-8,34,-20,-25,-19,-23,-24,34,-22,-21,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,35,36,37,38,39,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,29,32,-20,-25,-19,-23,38,-24,39,-22,-21,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,19,19,-20,-25,-19,-23,19,19,-24,19,-22,-21,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,20,20,-20,-25,-19,-23,20,20,-24,20,-22,-21,]),'SHORT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,21,21,-20,-25,-19,-23,21,21,-24,21,-22,-21,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,22,22,-20,-25,-19,-23,22,22,-24,22,-22,-21,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,23,23,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,23,23,-20,-25,-19,-23,23,23,-24,23,-22,-21,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,24,24,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,24,24,-20,-25,-19,-23,24,24,-24,24,-22,-21,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,28,29,31,32,33,34,35,36,37,38,39,],[-3,-2,26,26,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,26,26,-20,-25,-19,-23,26,26,-24,26,-22,-21,]),'COLON':([7,8,],[12,13,]),'SEMICOLON':([30,],[35,]),}
+_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,3,3,-21,-26,-20,-24,3,3,-25,3,-23,-22,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,30,33,39,40,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,-21,-20,-23,-22,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,30,33,39,40,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,31,-8,-21,-20,-23,-22,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,32,33,34,35,36,37,38,39,40,],[8,8,-3,-6,-2,-4,8,26,26,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,26,-8,26,-21,-26,-20,-24,26,26,-25,26,-23,-22,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,29,30,32,33,34,37,38,39,40,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,35,-21,-26,-20,-24,-25,35,-23,-22,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,36,37,38,39,40,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,30,33,-21,-26,-20,-24,39,-25,40,-23,-22,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,19,19,-21,-26,-20,-24,19,19,-25,19,-23,-22,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,20,20,-21,-26,-20,-24,20,20,-25,20,-23,-22,]),'SHORT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,21,21,-21,-26,-20,-24,21,21,-25,21,-23,-22,]),'FLOAT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,22,22,-21,-26,-20,-24,22,22,-25,22,-23,-22,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,23,23,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,23,23,-21,-26,-20,-24,23,23,-25,23,-23,-22,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,24,24,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,24,24,-21,-26,-20,-24,24,24,-25,24,-23,-22,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,25,25,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,25,25,-21,-26,-20,-24,25,25,-25,25,-23,-22,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,27,27,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,27,27,-21,-26,-20,-24,27,27,-25,27,-23,-22,]),'COLON':([7,8,],[12,13,]),'SEMICOLON':([31,],[36,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'snbt':([0,],[1,]),'compound':([0,12,13,26,28,34,35,37,],[2,16,16,16,16,16,16,16,]),'key_value_pairs':([3,],[4,]),'key_value_pair':([3,4,11,],[6,10,14,]),'value':([12,13,26,28,34,35,37,],[15,27,31,33,36,31,33,]),'list':([12,13,26,28,34,35,37,],[17,17,17,17,17,17,17,]),'array':([12,13,26,28,34,35,37,],[18,18,18,18,18,18,18,]),'values':([26,35,],[28,37,]),}
+_lr_goto_items = {'snbt':([0,],[1,]),'compound':([0,12,13,27,29,35,36,38,],[2,16,16,16,16,16,16,16,]),'key_value_pairs':([3,],[4,]),'key_value_pair':([3,4,11,],[6,10,14,]),'value':([12,13,27,29,35,36,38,],[15,28,32,34,37,32,34,]),'list':([12,13,27,29,35,36,38,],[17,17,17,17,17,17,17,]),'array':([12,13,27,29,35,36,38,],[18,18,18,18,18,18,18,]),'values':([27,36,],[29,38,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
@@ -37,19 +37,20 @@
   ('key_value_pair -> STRING COLON value','key_value_pair',3,'p_key_value_pair','parse.py',32),
   ('value -> compound','value',1,'p_value','parse.py',36),
   ('value -> list','value',1,'p_value','parse.py',37),
   ('value -> array','value',1,'p_value','parse.py',38),
   ('value -> BOOL','value',1,'p_value','parse.py',39),
   ('value -> BYTE','value',1,'p_value','parse.py',40),
   ('value -> SHORT','value',1,'p_value','parse.py',41),
-  ('value -> DOUBLE','value',1,'p_value','parse.py',42),
-  ('value -> LONG','value',1,'p_value','parse.py',43),
-  ('value -> INTEGER','value',1,'p_value','parse.py',44),
-  ('value -> STRING','value',1,'p_value','parse.py',45),
-  ('list -> LBRACKET values RBRACKET','list',3,'p_list','parse.py',49),
-  ('list -> LBRACKET RBRACKET','list',2,'p_list','parse.py',50),
-  ('array -> LBRACKET NAME SEMICOLON values RBRACKET','array',5,'p_array','parse.py',57),
-  ('array -> LBRACKET NAME SEMICOLON RBRACKET','array',4,'p_array','parse.py',58),
-  ('values -> values value','values',2,'p_values','parse.py',65),
-  ('values -> values COMMA value','values',3,'p_values','parse.py',66),
-  ('values -> value','values',1,'p_values','parse.py',67),
+  ('value -> FLOAT','value',1,'p_value','parse.py',42),
+  ('value -> DOUBLE','value',1,'p_value','parse.py',43),
+  ('value -> LONG','value',1,'p_value','parse.py',44),
+  ('value -> INTEGER','value',1,'p_value','parse.py',45),
+  ('value -> STRING','value',1,'p_value','parse.py',46),
+  ('list -> LBRACKET values RBRACKET','list',3,'p_list','parse.py',50),
+  ('list -> LBRACKET RBRACKET','list',2,'p_list','parse.py',51),
+  ('array -> LBRACKET NAME SEMICOLON values RBRACKET','array',5,'p_array','parse.py',58),
+  ('array -> LBRACKET NAME SEMICOLON RBRACKET','array',4,'p_array','parse.py',59),
+  ('values -> values value','values',2,'p_values','parse.py',66),
+  ('values -> values COMMA value','values',3,'p_values','parse.py',67),
+  ('values -> value','values',1,'p_values','parse.py',68),
 ]
```

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/cpp.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ctokens.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/lex.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/yacc.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ygen.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/tag.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Short", "Integer", "Long", "Double", "Bool", "String", "List", "Array", "Compound"]
+__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Short", "Integer", "Float", "Long", "Double", "Bool", "String", "List", "Array", "Compound"]
 
 class InvalidTypeError(ValueError):
     def __init__(self, item, cls):
         self.item = item
         self.cls = cls
         super().__init__(f"{self.item!r} is not a valid type for the items of {cls.__name__}.\nThis error is likely caused by a type mismatch in a list.")
 
@@ -54,14 +54,18 @@
     size = 4
 
 class Long(NumericInteger):
     __slots__ = ()
     size = 8
     suffix = "L"
 
+class Float(Numeric, float):
+    __slots__ = ()
+    suffix = "f"
+
 class Double(Numeric, float):
     __slots__ = ()
     suffix = "d"
 
 class Bool(Base, int):
     __slots__ = ()
     write_func = "bool"
```

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/token.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     "LBRACE",
     "RBRACE",
     "LBRACKET",
     "RBRACKET",
     "BOOL",
     "BYTE",
     "SHORT",
+    "FLOAT",
     "DOUBLE",
     "LONG",
     "INTEGER",
     "STRING",
     "NAME",
     "COLON",
     "SEMICOLON",
@@ -56,14 +57,19 @@
     return t
 
 def t_SHORT(t):
     r'\-?[0-9]+s'
     t.value = Short(t.value[:-1])
     return t
 
+def t_FLOAT(t):
+    r'\-?[0-9]+\.[0-9]+f'
+    t.value = Float(t.value[:-1])
+    return t
+
 def t_DOUBLE(t):
     r'\-?[0-9]+\.[0-9]+d'
     t.value = Double(t.value[:-1])
     return t
 
 def t_LONG(t):
     r'\-?[0-9]+L'
```

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib/write.py` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib/write.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb-snbt-lib-0.2.2/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -106,15 +106,16 @@
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
-| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
+| Float | A 32-bit, single-precision floating-point number.<br>Range: ``-3.4E+38`` ~ ``+3.4E+38`` | ``<number>f`` | ``12.345f`` |
+| Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
```

### Comparing `ftb-snbt-lib-0.2.1/pyproject.toml` & `ftb-snbt-lib-0.2.2/pyproject.toml`

 * *Files identical despite different names*

