# Comparing `tmp/python-espresso-1.5.tar.gz` & `tmp/python-espresso-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.5.tar", last modified: Sat Apr  6 10:32:21 2024, max compression
+gzip compressed data, was "python-espresso-1.6.tar", last modified: Sun Apr  7 06:05:06 2024, max compression
```

## Comparing `python-espresso-1.5.tar` & `python-espresso-1.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 10:32:21.974613 python-espresso-1.5/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.5/LICENSE
--rw-rw-rw-   0        0        0     2190 2024-04-06 10:32:21.974613 python-espresso-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 10:32:21.958750 python-espresso-1.5/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.5/espresso/Context.py
--rw-rw-rw-   0        0        0     4416 2024-04-04 17:01:38.000000 python-espresso-1.5/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.5/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3303 2024-04-06 08:35:50.000000 python-espresso-1.5/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.5/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.5/espresso/exceptions.py
--rw-rw-rw-   0        0        0      492 2024-04-03 13:48:09.000000 python-espresso-1.5/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:32:21.958750 python-espresso-1.5/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2190 2024-04-06 10:32:21.000000 python-espresso-1.5/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2024-04-06 10:32:21.000000 python-espresso-1.5/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 10:32:21.000000 python-espresso-1.5/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 10:32:21.000000 python-espresso-1.5/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 10:32:21.974613 python-espresso-1.5/setup.cfg
--rw-rw-rw-   0        0        0      531 2024-04-06 10:30:49.000000 python-espresso-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:32:21.974613 python-espresso-1.5/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.5/tests/test_lexer.py
--rw-rw-rw-   0        0        0      980 2024-04-06 09:09:29.000000 python-espresso-1.5/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.055419 python-espresso-1.6/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.6/LICENSE
+-rw-rw-rw-   0        0        0     2190 2024-04-07 06:05:06.055419 python-espresso-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2024-04-06 10:21:01.000000 python-espresso-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.043311 python-espresso-1.6/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.6/espresso/Context.py
+-rw-rw-rw-   0        0        0     4644 2024-04-07 06:02:48.000000 python-espresso-1.6/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3259 2024-04-05 13:34:25.000000 python-espresso-1.6/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3331 2024-04-07 05:04:08.000000 python-espresso-1.6/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.6/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.6/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      492 2024-04-03 13:48:09.000000 python-espresso-1.6/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.049511 python-espresso-1.6/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2190 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-07 06:05:06.000000 python-espresso-1.6/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 06:05:06.056419 python-espresso-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      531 2024-04-07 06:04:12.000000 python-espresso-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:05:06.054414 python-espresso-1.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1102 2024-04-07 05:14:50.000000 python-espresso-1.6/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.6/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 04:53:44.000000 python-espresso-1.6/tests/test_parser.py
```

### Comparing `python-espresso-1.5/LICENSE` & `python-espresso-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.5/PKG-INFO` & `python-espresso-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.5
+Version: 1.6
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.5/README.md` & `python-espresso-1.6/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.5/espresso/Evaluator.py` & `python-espresso-1.6/espresso/Evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,27 @@
         def_space[f.func_name[-1]] = f
 
     def is_variadic(self, func: Func, params: List[Union[str, int]]):
         return len(func.func_argument_types) > 0 and func.func_argument_types[
             0
         ].startswith("*")
 
-    # TODO: Handle overloading
     def get_typed_params(self, func: Func, params: List[Union[str, int]]):
         param_types = func.func_argument_types
         func_name = ".".join(func.func_name)
         parsed_params = []
+        variadic = self.is_variadic(func, params)
 
-        if self.is_variadic(func, params):
+        if variadic:
             param_types = [param_types[0][1:]] * len(param_types)
 
+        # Handling overloading
+        if not variadic and len(param_types) < len(params):
+            raise EspressoTypeError(f"Function '{func_name}' expects {len(param_types)} parameters, but {len(params)} were provided.")
+
         try:
             for i, param_type in enumerate(param_types):
                 param_type = param_type.strip().lower()
                 if param_type.endswith("?"):
                     # if a corresponding param doesn't exist but it is an optional type
                     if len(params) <= i:
                         parsed_params.append(None)
@@ -76,15 +80,15 @@
                     if not isinstance(params[i], int):
                         raise EspressoTypeError(
                             f"Expected type 'int' for parameter {i+1} of function '{func_name}', but received {type(params[i])} instead."
                         )
                 elif param_type == "any":
                     pass
                 else:
-                    raise EspressoTypeError(
+                    raise EspressoNameError(
                         f"Unknown parameter type '{param_type}' for parameter {i+1} of function '{func_name}'."
                     )
 
                 parsed_params.append(params[i])
         except IndexError:
             raise EspressoTypeError(
                 f"Not enough parameters provided for function '{func_name}'."
```

### Comparing `python-espresso-1.5/espresso/Lexer.py` & `python-espresso-1.6/espresso/Lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.5/espresso/Parser.py` & `python-espresso-1.6/espresso/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         return None
 
     def parse_func_params(self, at: int) -> List[Token]:
         assert self.tokens[at].type == TokenType.IDENTIFIER
         offset = 0
 
-        if self.tokens[at + 1].type != TokenType.LPAREN:
+        if at+1 >= len(self.tokens) or self.tokens[at + 1].type != TokenType.LPAREN:
             return [], offset
 
         closing_paren_index = self.get_closing_paren_index(self.tokens, at + 1)
 
         if not closing_paren_index:
             raise EspressoInvalidSyntax(
                 "( Was never closed at {}".format(self.tokens[at + 1].position)
```

### Comparing `python-espresso-1.5/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.6/python_espresso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.5
+Version: 1.6
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.5/setup.py` & `python-espresso-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.5",
+    version="1.6",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.5/tests/test_lexer.py` & `python-espresso-1.6/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.5/tests/test_parser.py` & `python-espresso-1.6/tests/test_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 from espresso.exceptions import EspressoInvalidSyntax
 
 import pytest
 
 parser = Parser()
 lexer = Lexer()
 
+
+def test_should_parse_simple_expression():
+    stack = parser.parse(lexer.lex("foo(bar(baz()))"))
+
+    
+    top = stack.pop()
+    assert isinstance(top, StackFrame)
+    assert top.func_chain == ["foo"]
+
+    top = top.func_params.pop()
+    assert isinstance(top, StackFrame)
+    assert top.func_chain == ["bar"]
+    
+    
 def test_should_resolve_flat_call_stack():
     stack = parser.parse(lexer.lex("32, 33, 34, \"foo\""))
 
     assert stack.pop() == "foo"
 
     assert stack.pop() == 34
     assert stack.pop() == 33
```

