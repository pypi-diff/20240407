# Comparing `tmp/metasequoia-sql-0.0.1.tar.gz` & `tmp/metasequoia-sql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.0.1.tar", last modified: Sun Mar 10 08:57:15 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.1.0.tar", last modified: Sun Apr  7 00:15:14 2024, max compression
```

## Comparing `metasequoia-sql-0.0.1.tar` & `metasequoia-sql-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.073382 metasequoia-sql-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-03-04 23:58:54.000000 metasequoia-sql-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2224 2024-03-10 08:57:15.073382 metasequoia-sql-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2024-03-10 08:56:16.000000 metasequoia-sql-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.065873 metasequoia-sql-0.0.1/metasequoia_sql/
--rw-rw-rw-   0        0        0        0 2024-02-03 23:53:25.000000 metasequoia-sql-0.0.1/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.068873 metasequoia-sql-0.0.1/metasequoia_sql/ast/
--rw-rw-rw-   0        0        0       41 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/ast/__init__.py
--rw-rw-rw-   0        0        0    19557 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/ast/nodes.py
--rw-rw-rw-   0        0        0      601 2024-03-07 14:34:24.000000 metasequoia-sql-0.0.1/metasequoia_sql/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.069873 metasequoia-sql-0.0.1/metasequoia_sql/parser/
--rw-rw-rw-   0        0        0        0 2024-03-06 15:19:23.000000 metasequoia-sql-0.0.1/metasequoia_sql/parser/__init__.py
--rw-rw-rw-   0        0        0      274 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/parser/common_parser.py
--rw-rw-rw-   0        0        0    13368 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/parser/mysql_parser.py
--rw-rw-rw-   0        0        0     3019 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/parser/token_scanner.py
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.070873 metasequoia-sql-0.0.1/metasequoia_sql/statements/
--rw-rw-rw-   0        0        0        0 2024-03-06 15:19:23.000000 metasequoia-sql-0.0.1/metasequoia_sql/statements/__init__.py
--rw-rw-rw-   0        0        0     5893 2024-03-09 10:40:40.000000 metasequoia-sql-0.0.1/metasequoia_sql/statements/common.py
--rw-rw-rw-   0        0        0     2948 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/statements/hive.py
--rw-rw-rw-   0        0        0    10400 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/statements/mysql.py
--rw-rw-rw-   0        0        0     3824 2024-03-09 10:40:40.000000 metasequoia-sql-0.0.1/metasequoia_sql/static.py
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.072378 metasequoia-sql-0.0.1/metasequoia_sql/translate/
--rw-rw-rw-   0        0        0      101 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/translate/__init__.py
--rw-rw-rw-   0        0        0     3402 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/translate/from_mysql.py
--rw-rw-rw-   0        0        0     5266 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/translate/full_statement.py
--rw-rw-rw-   0        0        0     1225 2024-03-10 08:55:03.000000 metasequoia-sql-0.0.1/metasequoia_sql/translate/to_hive.py
-drwxrwxrwx   0        0        0        0 2024-03-10 08:57:15.073382 metasequoia-sql-0.0.1/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     2224 2024-03-10 08:57:15.000000 metasequoia-sql-0.0.1/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2024-03-10 08:57:15.000000 metasequoia-sql-0.0.1/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 08:57:15.000000 metasequoia-sql-0.0.1/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-10 08:57:15.000000 metasequoia-sql-0.0.1/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-10 08:57:15.074383 metasequoia-sql-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-03-10 08:56:16.000000 metasequoia-sql-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.623823 metasequoia-sql-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5756 2024-04-07 00:15:14.622823 metasequoia-sql-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5087 2024-04-07 00:13:47.000000 metasequoia-sql-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.581827 metasequoia-sql-0.1.0/auto_test/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/auto_test/__init__.py
+-rw-rw-rw-   0        0        0    96622 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/auto_test/sql_basic_tutorial.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.582827 metasequoia-sql-0.1.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.585827 metasequoia-sql-0.1.0/metasequoia_sql/ast/
+-rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/__init__.py
+-rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/functions.py
+-rw-rw-rw-   0        0        0    17093 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/nodes.py
+-rw-rw-rw-   0        0        0     8458 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/ast/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.586827 metasequoia-sql-0.1.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0     3089 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/text_scanner.py
+-rw-rw-rw-   0        0        0     8206 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/common/token_scanner.py
+-rw-rw-rw-   0        0        0      665 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.588827 metasequoia-sql-0.1.0/metasequoia_sql/objects/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/__init__.py
+-rw-rw-rw-   0        0        0     8175 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/common.py
+-rw-rw-rw-   0        0        0    53603 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/core.py
+-rw-rw-rw-   0        0        0      114 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/data_source.py
+-rw-rw-rw-   0        0        0     2927 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/hive.py
+-rw-rw-rw-   0        0        0    10343 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/objects/mysql.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.589827 metasequoia-sql-0.1.0/metasequoia_sql/parser/
+-rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/__init__.py
+-rw-rw-rw-   0        0        0    69957 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/common.py
+-rw-rw-rw-   0        0        0    13123 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/parser/mysql_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.590827 metasequoia-sql-0.1.0/metasequoia_sql/statements/
+-rw-rw-rw-   0        0        0        0 2024-04-06 23:27:57.000000 metasequoia-sql-0.1.0/metasequoia_sql/statements/__init__.py
+-rw-rw-rw-   0        0        0       45 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/statements/mysql.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.591827 metasequoia-sql-0.1.0/metasequoia_sql/static/
+-rw-rw-rw-   0        0        0      183 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/common.py
+-rw-rw-rw-   0        0        0     2571 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/mysql.py
+-rw-rw-rw-   0        0        0     3824 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/static/other.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.619826 metasequoia-sql-0.1.0/metasequoia_sql/translate/
+-rw-rw-rw-   0        0        0      101 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/__init__.py
+-rw-rw-rw-   0        0        0     3399 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/from_mysql.py
+-rw-rw-rw-   0        0        0     5343 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/full_statement.py
+-rw-rw-rw-   0        0        0     1222 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/metasequoia_sql/translate/to_hive.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.622823 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     5756 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-07 00:15:14.000000 metasequoia-sql-0.1.0/metasequoia_sql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.620825 metasequoia-sql-0.1.0/scripts/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:15:14.621823 metasequoia-sql-0.1.0/scripts/demo/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/__init__.py
+-rw-rw-rw-   0        0        0    67081 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/sql_basic_tutorial.py
+-rw-rw-rw-   0        0        0     2024 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/demo/with_demo.py
+-rw-rw-rw-   0        0        0      278 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/temp_test.py
+-rw-rw-rw-   0        0        0     4882 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.0/scripts/unittest_maker.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 00:15:14.623823 metasequoia-sql-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      976 2024-04-07 00:14:06.000000 metasequoia-sql-0.1.0/setup.py
```

### Comparing `metasequoia-sql-0.0.1/LICENSE` & `metasequoia-sql-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/errors.py` & `metasequoia-sql-0.1.0/metasequoia_sql/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 
 
 class UnSupportDataSourceError(Exception):
     """数据源不支持的语法异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
+
+
+class ScannerError(Exception):
+    """文本扫描异常"""
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/parser/mysql_parser.py` & `metasequoia-sql-0.1.0/metasequoia_sql/parser/mysql_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 Hive 保留字：https://cwiki.apache.org/confluence/display/Hive/LanguageManual+DDL
 """
 
 import enum
 from typing import List
 
 from metasequoia_sql import ast
+from metasequoia_sql.common.token_scanner import TokenScanner
 from metasequoia_sql.errors import SqlParseError
-from metasequoia_sql.parser.common_parser import SqlParser
-from metasequoia_sql.statements.common import SqlFunction
-from metasequoia_sql.statements.mysql import *
+from metasequoia_sql.objects.mysql import *
+from metasequoia_sql.parser.common import parse_general_expression, parse_sql_column_type
 
 
-class MySQLCreateTableParser(SqlParser):
+class MySQLCreateTableParser:
     """
     当前已知不支持的场景：虚拟列 GENERATED ALWAYS AS（RDS427.prism1.oned_topic_kafka）
     """
 
-    def __init__(self, root: ast.ASTInternal):
+    def __init__(self, root: ast.AST):
         # 过滤 statement 中的空白字符
-        self.tokens: List[ast.AST] = [token for token in root.children if token.is_whitespace is False]
+        self.tokens: List[ast.AST] = [token for token in root.children if token.is_space is False]
         self.n_token = len(self.tokens)
 
         # 初始化自动机状态类
         self.idx = 0  # 当前自动机位置下标
         self.stage = MySQLCreateTableParser.ParseStage.START  # 当前自动机状态
 
         # 初始化匹配结果
@@ -86,20 +86,20 @@
         """解析字段和索引（如果匹配成功返回 True，否则返回 False）"""
         outer_token = self.tokens[self.idx]
         if not isinstance(outer_token, ast.ASTParenthesis):
             raise SqlParseError("cannot find parenthesis after table name")
 
         # 过滤插入语中的空白字符
         inner_tokens: List[ast.AST] = [token for token in outer_token.children if
-                                       token.is_whitespace is False and not isinstance(token, ast.ASTComment)]
+                                       token.is_space is False and token.is_multiline_comment is False]
 
         # 根据逗号拆分插入语中的内容
         column_group_tokens: List[List[ast.AST]] = [[]]
         for token in inner_tokens:
-            if isinstance(token, ast.ASTComma):
+            if token.is_comma:
                 column_group_tokens.append([])
             else:
                 column_group_tokens[-1].append(token)
 
         for column_group in column_group_tokens:
             if column_group[0].equals("PRIMARY"):
                 if self.builder.primary_key is not None:
@@ -110,77 +110,77 @@
                 else:
                     raise SqlParseError("unknown primary key format")
             elif column_group[0].equals("UNIQUE"):
                 if (len(column_group) >= 3 and column_group[1].equals("KEY")
                         and isinstance(column_group[3], ast.ASTParenthesis)):
                     self.builder.add_unique_key(DDLUniqueKeyMySQL(
                         column_group[2].source,
-                        [node.source for node in column_group[3].children if not isinstance(node, ast.ASTComma)]))
+                        [node.source for node in column_group[3].children if not node.is_comma]))
                 else:
                     raise SqlParseError("unknown uniquekey format")
             elif column_group[0].equals("KEY"):
                 if len(column_group) >= 2 and isinstance(column_group[2], ast.ASTParenthesis):
                     self.builder.add_key(DDLKeyMySQL(
                         column_group[1].source,
-                        [node.source for node in column_group[2].children if not isinstance(node, ast.ASTComma)]))
+                        [node.source for node in column_group[2].children if not node.is_comma]))
                 else:
                     raise SqlParseError("unknown key format")
             elif column_group[0].equals("FULLTEXT"):
                 if (len(column_group) >= 3 and column_group[1].equals("KEY")
                         and isinstance(column_group[3], ast.ASTParenthesis)):
                     self.builder.add_fulltext_key(DDLFulltextKeyMysql(
                         column_group[2].source,
-                        [node.source for node in column_group[3].children if not isinstance(node, ast.ASTComma)]))
+                        [node.source for node in column_group[3].children if not node.is_comma]))
                 else:
                     raise SqlParseError("unknown uniquekey format")
             elif column_group[0].equals("CONSTRAINT"):
                 if (len(column_group) >= 8 and
                         isinstance(column_group[4], ast.ASTParenthesis) and
                         isinstance(column_group[7], ast.ASTParenthesis)):
                     self.builder.add_foreign_key(DDLForeignKeyMySQL(
                         column_group[1].source,
-                        [node.source for node in column_group[4].children if not isinstance(node, ast.ASTComma)],
+                        [node.source for node in column_group[4].children if not node.is_comma],
                         column_group[6].source,
-                        [node.source for node in column_group[7].children if not isinstance(node, ast.ASTComma)]
+                        [node.source for node in column_group[7].children if not node.is_comma]
                     ))
             else:
-                position = self.create_token_scanner(column_group)
-                column_name = position.move_as_source()
-                column_type = position.match_function(DDLColumnTypeMySQL)
+                scanner = TokenScanner(column_group)
+                column_name = scanner.pop_as_source()
+                column_type = parse_sql_column_type(scanner)
                 column = DDLColumnMySQL(column_name, column_type)
-                while not position.is_finish():
-                    if position.get().equals("NOT"):
-                        position.match_words(["NOT", "NULL"])
+                while not scanner.is_finish:
+                    if scanner.get().equals("NOT"):
+                        scanner.match("NOT", "NULL")
                         column.is_not_null = True
-                    elif position.get().equals("NULL"):
-                        position.match_words(["NULL"])
+                    elif scanner.get().equals("NULL"):
+                        scanner.match("NULL")
                         column.set_is_allow_null(True)
-                    elif position.get().equals("CHARACTER"):
-                        position.match_words(["CHARACTER", "SET"])
-                        column.set_character_set(position.move_as_source())
-                    elif position.get().equals("COLLATE"):
-                        position.match_words(["COLLATE"])
-                        column.set_collate(position.move_as_source())
-                    elif position.get().equals("DEFAULT"):
-                        position.match_words(["DEFAULT"])
-                        column.default = position.match_function(SqlFunction)
-                    elif position.get().equals("COMMENT"):
-                        position.match_words(["COMMENT"])
-                        column.set_comment(position.move_as_source())
-                    elif position.get().equals("ON"):  # ON UPDATE
-                        position.match_words(["ON", "UPDATE"])
-                        column.on_update = position.match_function(SqlFunction)
-                    elif position.get().equals("AUTO_INCREMENT"):
-                        position.match_words(["AUTO_INCREMENT"])
+                    elif scanner.get().equals("CHARACTER"):
+                        scanner.match("CHARACTER", "SET")
+                        column.set_character_set(scanner.pop_as_source())
+                    elif scanner.get().equals("COLLATE"):
+                        scanner.match("COLLATE")
+                        column.set_collate(scanner.pop_as_source())
+                    elif scanner.get().equals("DEFAULT"):
+                        scanner.match("DEFAULT")
+                        column.default = parse_general_expression(scanner)
+                    elif scanner.get().equals("COMMENT"):
+                        scanner.match("COMMENT")
+                        column.set_comment(scanner.pop_as_source())
+                    elif scanner.get().equals("ON"):  # ON UPDATE
+                        scanner.match("ON", "UPDATE")
+                        column.on_update = parse_general_expression(scanner)
+                    elif scanner.get().equals("AUTO_INCREMENT"):
+                        scanner.match("AUTO_INCREMENT")
                         column.is_auto_increment = True
-                    elif position.get().equals("UNSIGNED"):
-                        position.match_words(["UNSIGNED"])
+                    elif scanner.get().equals("UNSIGNED"):
+                        scanner.match("UNSIGNED")
                         column.is_unsigned = True
-                    elif position.get().equals("ZEROFILL"):
-                        position.match_words(["ZEROFILL"])
+                    elif scanner.get().equals("ZEROFILL"):
+                        scanner.match("ZEROFILL")
                         column.is_zerofill = True
                     else:
                         raise SqlParseError(f"Cannot parse ddl column: {column_group}")
                 self.builder.append_column(column)
 
         self.idx += 1
         self.stage = MySQLCreateTableParser.ParseStage.AFTER_COLUMNS_AND_KEY_LIST
@@ -188,21 +188,21 @@
 
     def _parse_table_config(self):
         tokens = self.tokens[self.idx:]
         if len(tokens) >= 1 and isinstance(tokens[-1], ast.ASTSemicolon):
             tokens.pop()
         i = 0
         while i < len(tokens):
-            if isinstance(tokens[i], ast.ASTComment):
+            if tokens[i].is_multiline_comment:
                 i += 1
             elif tokens[i].equals("ENGINE"):
                 if i + 2 < len(tokens) and tokens[i + 1].equals("="):
                     self.builder.set_engine(tokens[i + 2].source)
                 else:
-                    raise SqlParseError("unknown engine")
+                    raise SqlParseError(f"unknown engine: {tokens}")
                 i += 3
             elif tokens[i].equals("AUTO_INCREMENT"):
                 if i + 2 < len(tokens) and tokens[i + 1].equals("="):
                     self.builder.set_table_auto_increment(int(tokens[i + 2].source))
                 else:
                     raise SqlParseError("unknown AUTO_INCREMENT")
                 i += 3
@@ -249,9 +249,9 @@
         AFTER_TABLE_NAME = 300  # 已匹配表名
         AFTER_COLUMNS_AND_KEY_LIST = 400  # 已匹配字段和索引信息
         FINISH = 1000  # 已匹配完成
 
 
 def parse_mysql_create_table_statement(sql: str) -> DDLCreateTableStatementMySQL:
     # 将 sql 解析为多个表达式，并检查是否有且只有 1 个表达式
-    root: ast.ASTStatement = ast.ASTParser(sql).parse()
+    root: ast.AST = ast.parse_as_statements(sql)[0]
     return MySQLCreateTableParser(root).builder
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/statements/common.py` & `metasequoia-sql-0.1.0/metasequoia_sql/objects/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,113 @@
 """
 通用的 SQL 语法对象
 """
 
 import abc
-import enum
 from typing import Optional, List
 
-__all__ = ["DataSource", "SqlBase", "SqlFunction", "DDLColumnType", "DDLColumn", "DDLPrimaryKey", "DDLUniqueKey",
-           "DDLKey", "DDLForeignKey", "DDLFulltextKey", "DDLCreateTableStatement"]
+from metasequoia_sql import ast
 
-
-# ------------------------------ 数据源相关类 ------------------------------
-class DataSource(enum.Enum):
-    """数据源类型"""
-    MYSQL = enum.auto()
-    HIVE = enum.auto()
+__all__ = [
+    # ---------- 抽象基类 ----------
+    "SQLBase",
+
+    # ---------- 单项式级别 ----------
+    # 单项式抽象基类
+    "SQLMonomial",
+
+    # 函数调用（及其子类字段类型）；变量引用
+    "SQLFunction", "SQLColumnType", "SQLVariable",
+
+    # ---------- 其他类型 ----------
+    "SQLSimpleExpression",
+    "DDLColumn",
+    "DDLPrimaryKey",
+    "DDLUniqueKey",
+    "DDLKey", "DDLForeignKey", "DDLFulltextKey", "DDLCreateTableStatement"
+]
 
 
 # ------------------------------ 抽象基类 ------------------------------
 
 
-class SqlBase(abc.ABC):
+class SQLBase(abc.ABC):
+    @property
     @abc.abstractmethod
     def source(self) -> str:
         """返回 SQL 源码"""
 
+    def __str__(self) -> str:
+        return self.__repr__()
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} source={self.source}>"
+
+
+# ------------------------------ 单项式级别类 ------------------------------
+
+class SQLMonomial(SQLBase, abc.ABC):
+    """单项式级别抽象类"""
+
 
-class SqlFunction(SqlBase, abc.ABC):
+class SQLFunction(SQLMonomial):
     """函数调用语句"""
 
-    def __init__(self, name: str, params: Optional[List[str]] = None):
-        if params is None:
-            params = []
+    def __init__(self, name: str, params: List["SQLSimpleExpression"]):
         self._name = name  # 函数名称
         self._params = params  # 函数参数
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name
 
     @property
-    def params(self):
+    def params(self) -> List["SQLSimpleExpression"]:
         return self._params
 
+    @property
     def source(self) -> str:
-        if len(self._params) > 0:
-            type_params = "(" + ", ".join(self._params) + ")"
-            return f"{self._name}{type_params}"
+        if len(self.params) > 0:
+            type_params = "(" + ", ".join([param.source for param in self.params]) + ")"
+            return f"{self.name}{type_params}"
         else:
-            return self._name
+            return self.name
 
 
-# ------------------------------ DDL 相关通用类 ------------------------------
+class SQLColumnType(SQLFunction):
+    """DDL 中的字段类型
+
+    以是类型名称或函数调用（类型的注释）。因为在其他场景下，类型名称均不允许单独使用，所以在这里额外处理。
+    """
+
+    def __init__(self, name: str, params: Optional[List["SQLSimpleExpression"]] = None):
+        super().__init__(name, params if params is not None else [])
+
+
+class SQLVariable(SQLMonomial):
+    """变量引用语句"""
 
+    def __init__(self, name: str):
+        self._name = name.upper()  # 变量名称
 
-class DDLColumnType(SqlFunction):
-    """【DDL】建表语句或修改表结构语句中的字段类型"""
+    @property
+    def name(self) -> str:
+        return self._name
 
+    @property
+    def source(self) -> str:
+        return self.name
+
+
+# ------------------------------ DDL 相关通用类 ------------------------------
 
-class DDLColumn(SqlBase):
+class DDLColumn(SQLBase):
     """【DDL】建表语句中的字段信息"""
 
-    def __init__(self, column_name: str, column_type: "DDLColumnType", comment: Optional[str] = None):
+    def __init__(self, column_name: str, column_type, comment: Optional[str] = None):
         self._column_name = column_name.strip("`")
         self._column_type = column_type
         self._comment = comment
 
     @property
     def column_name(self):
         return self.get_column_name()
@@ -80,66 +122,105 @@
 
     def get_column_name(self, with_quote: bool = True):
         if with_quote:
             return f"`{self._column_name}`"
         else:
             return self._column_name
 
-    def set_comment(self, comment: Optional[str]):
+    def set_column_name(self, column_name: str) -> None:
+        self._column_name = column_name
+
+    def set_column_type(self, column_type: "SQLColumnType") -> None:
+        self._column_type = column_type
+
+    def set_comment(self, comment: Optional[str]) -> None:
         self._comment = comment
 
+    @property
     def source(self) -> str:
-        res = f"{self._column_name} {self.column_type.source()}"
+        res = f"{self._column_name} {self.column_type.source}"
         if self.comment is not None:
             res += f" COMMENT {self.comment}"
         return res
 
 
-class DDLPrimaryKey(SqlBase):
+class DDLPrimaryKey(SQLBase):
     def __init__(self, column: str):
-        self.column: str = column
+        self._column: str = column
+
+    @property
+    def column(self) -> str:
+        return self._column
 
+    @property
     def source(self) -> str:
-        return f"PRIMARY KEY ({self.column})" if self.column is not None else ""
+        return f"PRIMARY KEY ({self._column})" if self._column is not None else ""
 
 
-class DDLUniqueKey(SqlBase):
+class DDLUniqueKey(SQLBase):
     def __init__(self, name: str, columns: List[str]):
-        self.name: str = name
-        self.columns: List[str] = columns
+        self._name = name
+        self._columns = columns
+
+    @property
+    def name(self) -> str:
+        return self._name
 
+    @property
+    def columns(self) -> List[str]:
+        return self._columns
+
+    @property
     def source(self) -> str:
         if len(self.columns) > 0:
             columns_str = ", ".join([f"{column}" for column in self.columns])
             return f"UNIQUE KEY {self.name} ({columns_str})"
 
 
-class DDLKey(SqlBase):
+class DDLKey(SQLBase):
     def __init__(self, name: str, columns: List[str]):
-        self.name: str = name
-        self.columns: List[str] = columns
+        self._name: str = name
+        self._columns: List[str] = columns
 
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def columns(self) -> List[str]:
+        return self._columns
+
+    @property
     def source(self) -> str:
         if len(self.columns) > 0:
             columns_str = ", ".join([f"{column}" for column in self.columns])
             return f"KEY {self.name} ({columns_str})"
 
 
-class DDLFulltextKey(SqlBase):
+class DDLFulltextKey(SQLBase):
     def __init__(self, name: str, columns: List[str]):
-        self.name: str = name
-        self.columns: List[str] = columns
+        self._name: str = name
+        self._columns: List[str] = columns
 
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def columns(self) -> List[str]:
+        return self._columns
+
+    @property
     def source(self) -> str:
         if len(self.columns) > 0:
             columns_str = ", ".join([f"{column}" for column in self.columns])
             return f"FULLTEXT KEY {self.name} ({columns_str})"
 
 
-class DDLForeignKey(SqlBase):
+class DDLForeignKey(SQLBase):
     def __init__(self, constraint_name: str, slave_columns: List[str], master_table_name: str,
                  master_columns: List[str]):
         """
 
         Parameters
         ----------
         constraint_name : str
@@ -152,24 +233,39 @@
             主表的字段名
         """
         self.constraint_name = constraint_name
         self.slave_columns = slave_columns
         self.master_table_name = master_table_name
         self.master_columns = master_columns
 
+    @property
     def source(self) -> str:
         slave_columns_str = ", ".join([f"{column}" for column in self.slave_columns])
         master_columns_str = ", ".join([f"{column}" for column in self.master_columns])
         return f"CONSTRAINT {self.constraint_name} FOREIGN KEY({slave_columns_str}) REFERENCES {self.master_table_name}({master_columns_str})"
 
 
+# ------------------------------ DSL 相关通用类 ------------------------------
+
+
+class SQLSimpleExpression(SQLMonomial):
+    """字段表达式"""
+
+    def __init__(self, tokens: List[ast.AST], alias: Optional[str] = None):
+        super().__init__(tokens)
+        self._alias = alias
+
+    def alias(self) -> Optional[str]:
+        return self._alias
+
+
 # ------------------------------ 表达式层级 ------------------------------
 
 
-class DDLCreateTableStatement(SqlBase, abc.ABC):
+class DDLCreateTableStatement(SQLBase, abc.ABC):
     """【DDL】CREATE TABLE 语句"""
 
     def __init__(self,
                  schema_name: Optional[str] = None,
                  table_name: Optional[str] = None,
                  comment: Optional[str] = None):
         self._schema_name = schema_name
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/statements/hive.py` & `metasequoia-sql-0.1.0/metasequoia_sql/objects/hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Hive 语句相关元素对象
 """
 
 from typing import Dict, List, Optional
 
-from metasequoia_sql.statements.common import *
+from metasequoia_sql.objects.common import *
 
 
-class DDLColumnTypeHive(DDLColumnType):
+class DDLColumnTypeHive(SQLColumnType):
     """【DDL】Hive 的字段类型对象"""
 
 
 class DDLColumnHive(DDLColumn):
     """【DDL】Hive 建表语句或修改表结构语句中的字段信息"""
 
 
@@ -41,15 +41,15 @@
     def change_type(self, hashmap: Dict[str, str], remove_param: bool = True):
         """更新每个字段的变量类型"""
         for column in self.columns:
             old_column_type = column.column_type.name
             new_column_type = hashmap[old_column_type.upper()]
             column.column_type._name = new_column_type
             if remove_param is True:
-                column.column_type._params = []
+                column.column_type._function_params = []
 
     def append_partition_by_column(self, column: DDLColumnHive):
         """添加分区字段"""
         self.partition_by.append(column)
 
     def source(self, n_indent: int = 4) -> str:
         indentation = " " * n_indent  # 缩进字符串
@@ -58,20 +58,19 @@
             result += " IF NOT EXISTS"
         result += " "
         if self._schema_name is not None:
             result += f"`{self._schema_name}`."
         result += f"`{self._table_name}`(\n"
         columns_and_keys = []
         for column in self.columns:
-            columns_and_keys.append(f"{indentation}{column.source()}")
+            columns_and_keys.append(f"{indentation}{column.source}")
         result += ",\n".join(columns_and_keys)
         result += "\n)"
         if self._comment is not None:
             result += f" COMMENT {self._comment}"
         if len(self.partition_by) > 0:
             partition_columns = []
             for column in self.partition_by:
-                partition_columns.append(column.source())
+                partition_columns.append(column.source)
             partition_str = ", ".join(partition_columns)
             result += f" PARTITIONED BY ({partition_str})"
-        result += ";"
         return result
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/statements/mysql.py` & `metasequoia-sql-0.1.0/metasequoia_sql/objects/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 """
 MySQL 专用的语法对象
 """
 
 from typing import Optional, Dict, List
 
-from metasequoia_sql.statements.common import *
+from metasequoia_sql.objects.common import *
+from metasequoia_sql.objects.core import *
 
 __all__ = ["DDLColumnTypeMySQL", "DDLColumnMySQL", "DDLPrimaryKeyMySQL", "DDLUniqueKeyMySQL", "DDLKeyMySQL",
            "DDLForeignKeyMySQL", "DDLFulltextKeyMysql", "DDLCreateTableStatementMySQL"]
 
 
-class DDLColumnTypeMySQL(DDLColumnType):
+class DDLColumnTypeMySQL(SQLColumnType):
     """【DDL】MySQL 的字段类型对象"""
 
 
 class DDLColumnMySQL(DDLColumn):
     """【DDL】建表语句或修改表结构语句中的字段信息"""
 
     def __init__(self, column_name: str,
-                 column_type: DDLColumnTypeMySQL,
+                 column_type: SQLGeneralExpression,
                  is_unsigned: bool = False,
                  is_zerofill: bool = False,
                  character_set: Optional[str] = None,
                  collate: Optional[str] = None,
                  is_allow_null: bool = False,
                  is_not_null: bool = False,
                  is_auto_increment: bool = False,
-                 default: Optional[SqlFunction] = None,
-                 on_update: Optional[SqlFunction] = None,
+                 default: Optional[SQLGeneralExpression] = None,
+                 on_update: Optional[SQLGeneralExpression] = None,
                  comment: Optional[str] = None
                  ):
         super().__init__(column_name, column_type, comment)
         self.is_unsigned: bool = is_unsigned
         self.is_zerofill: bool = is_zerofill
         self.character_set: Optional[str] = character_set
         self.collate: Optional[str] = collate
         self.is_allow_null: bool = is_allow_null  # 是否显式地允许 NULL 值
         self.is_not_null: bool = is_not_null
         self.is_auto_increment: bool = is_auto_increment
-        self.default: Optional[SqlFunction] = default
-        self.on_update: Optional[SqlFunction] = on_update
+        self.default: Optional[SQLGeneralExpression] = default
+        self.on_update: Optional[SQLGeneralExpression] = on_update
 
     def set_is_unsigned(self, is_unsigned: bool) -> None:
         self.is_unsigned = is_unsigned
 
     def set_is_allow_null(self, is_allow_null: bool) -> None:
         self.is_allow_null = is_allow_null
 
@@ -64,17 +65,14 @@
 
     def set_default(self, default: Optional[str]):
         self.default = default
 
     def set_on_update(self, on_update: Optional[str]):
         self.on_update = on_update
 
-    def change_to_data_source(self, data_source: DataSource, type_hash):
-        """转换为 DataSource 的类型的字段"""
-
     def source(self) -> str:
         res = f"{self._column_name} {self.column_type.source()}"
         if self.is_unsigned is True:
             res += " UNSIGNED"
         if self.is_zerofill is True:
             res += " ZEROFILL"
         if self.character_set is not None:
@@ -84,17 +82,17 @@
         if self.is_allow_null is True:
             res += " NULL"
         if self.is_not_null is True:
             res += " NOT NULL"
         if self.is_auto_increment is True:
             res += " AUTO_INCREMENT"
         if self.default is not None:
-            res += f" DEFAULT {self.default.source()}"
+            res += f" DEFAULT {self.default.source}"
         if self.on_update is not None:
-            res += f" ON UPDATE {self.on_update.source()}"
+            res += f" ON UPDATE {self.on_update.source}"
         if self.comment is not None:
             res += f" COMMENT {self.comment}"
         return res
 
 
 class DDLPrimaryKeyMySQL(DDLPrimaryKey):
     """【DDL】主键索引"""
@@ -220,15 +218,15 @@
     def change_type(self, hashmap: Dict[str, str], remove_param: bool = True):
         """更新每个字段的变量类型"""
         for column in self.columns:
             old_column_type = column.column_type.name
             new_column_type = hashmap[old_column_type.upper()]
             column.column_type._name = new_column_type
             if remove_param is True:
-                column.column_type._params = []
+                column.column_type._function_params = []
 
     def append_column(self, column: DDLColumnMySQL):
         """添加字段"""
         self.columns.append(column)
 
     def source(self, n_indent: int = 4) -> str:
         indentation = " " * n_indent  # 缩进字符串
@@ -239,23 +237,23 @@
         if self._schema_name is not None:
             result += f"`{self._schema_name}`."
         result += f"`{self._table_name}`(\n"
         columns_and_keys = []
         for column in self.columns:
             columns_and_keys.append(f"{indentation}{column.source()}")
         if self.primary_key is not None:
-            columns_and_keys.append(f"{indentation}{self.primary_key.source()}")
+            columns_and_keys.append(f"{indentation}{self.primary_key.source}")
         for unique_key in self.unique_key:
-            columns_and_keys.append(f"{indentation}{unique_key.source()}")
+            columns_and_keys.append(f"{indentation}{unique_key.source}")
         for key in self.key:
-            columns_and_keys.append(f"{indentation}{key.source()}")
+            columns_and_keys.append(f"{indentation}{key.source}")
         for fulltext_key in self.fulltext_key:
-            columns_and_keys.append(f"{indentation}{fulltext_key.source()}")
+            columns_and_keys.append(f"{indentation}{fulltext_key.source}")
         for foreign_key in self.foreign_key:
-            columns_and_keys.append(f"{indentation}{foreign_key.source()}")
+            columns_and_keys.append(f"{indentation}{foreign_key.source}")
         result += ",\n".join(columns_and_keys)
         result += "\n)"
         if self.engine is not None:
             result += f" ENGINE = {self.engine}"
         if self.auto_increment is not None:
             result += f" AUTO_INCREMENT = {self.auto_increment}"
         if self.default_charset is not None:
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/static.py` & `metasequoia-sql-0.1.0/metasequoia_sql/static/other.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/translate/from_mysql.py` & `metasequoia-sql-0.1.0/metasequoia_sql/translate/from_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 类型转换：将 MySQL 特性的 SQL 语句转化为全特性 SQL 语句
 """
 
-from metasequoia_sql.statements.mysql import *
+from metasequoia_sql.objects.mysql import *
 from metasequoia_sql.translate.full_statement import *
 
 
 def ddl_column_type_from_mysql(column_type: DDLColumnTypeMySQL) -> DDLColumnTypeFull:
     return DDLColumnTypeFull(
         name=column_type.name,
         params=column_type.params
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/translate/full_statement.py` & `metasequoia-sql-0.1.0/metasequoia_sql/translate/full_statement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 包含所有数据库特性的 FullStatement，仅用于数类型转换，不支持其他使用方式
 """
 
 from typing import Optional, List
 
 from metasequoia_sql.errors import FullStatementCalledSource
-from metasequoia_sql.statements.common import *
+from metasequoia_sql.objects.common import *
+from metasequoia_sql.objects.core import SQLGeneralExpression
 
 __all__ = ["DDLColumnTypeFull", "DDLColumnFull", "DDLPrimaryKeyFull", "DDLUniqueKeyFull", "DDLKeyFull",
            "DDLForeignKeyFull", "DDLFulltextKeyFull", "DDLCreateTableStatementFull"]
 
 
 class FullBase:
     """FullStatement 各元素的抽象基类，在调用 source 方法时抛出异常"""
@@ -17,15 +18,15 @@
     def source(self):
         raise FullStatementCalledSource()
 
 
 class DDLColumnTypeFull(FullBase):
     """【DDL】MySQL 的字段类型对象"""
 
-    def __init__(self, name: str, params: Optional[List[str]] = None):
+    def __init__(self, name: str, params: Optional[List[SQLGeneralExpression]] = None):
         self.name = name
         self.params = params
 
 
 class DDLColumnFull(FullBase):
     """【DDL】建表语句或修改表结构语句中的字段信息"""
 
@@ -36,16 +37,16 @@
                  is_unsigned: bool = False,
                  is_zerofill: bool = False,
                  character_set: Optional[str] = None,
                  collate: Optional[str] = None,
                  is_allow_null: bool = False,
                  is_not_null: bool = False,
                  is_auto_increment: bool = False,
-                 default: Optional[SqlFunction] = None,
-                 on_update: Optional[SqlFunction] = None
+                 default: Optional[SQLFunction] = None,
+                 on_update: Optional[SQLFunction] = None
                  ):
         self.column_name = column_name
         self.column_type = column_type
         self.is_unsigned = is_unsigned
         self.is_zerofill = is_zerofill
         self.character_set = character_set
         self.collate = collate
```

### Comparing `metasequoia-sql-0.0.1/metasequoia_sql/translate/to_hive.py` & `metasequoia-sql-0.1.0/metasequoia_sql/translate/to_hive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 类型转换：将全属性 SQL 语句转化为 Hive 特性 SQL 语句
 """
 
-from metasequoia_sql.statements.hive import *
+from metasequoia_sql.objects.hive import *
 from metasequoia_sql.translate.full_statement import *
 
 
 def ddl_column_type_to_hive(column_type: DDLColumnTypeFull) -> DDLColumnTypeHive:
     return DDLColumnTypeHive(
         name=column_type.name,
         params=column_type.params
```

### Comparing `metasequoia-sql-0.0.1/setup.py` & `metasequoia-sql-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.0.1",
+    version="0.1.0",
     description="SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
```

