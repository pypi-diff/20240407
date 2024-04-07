# Comparing `tmp/regexriot-0.0.2.tar.gz` & `tmp/regexriot-0.0.3.tar.gz`

## Comparing `regexriot-0.0.2.tar` & `regexriot-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,38 @@
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 regexriot-0.0.2/overrides.json
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 regexriot-0.0.2/.github/workflows/docsite.yml
--rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 regexriot-0.0.2/.github/workflows/test.yml
--rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/make.bat
--rwxr-xr-x   0        0        0     1574 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/source/conf.py
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/source/index.rst
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/source/modules.rst
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/source/regex_riot_rk22000.rst
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 regexriot-0.0.2/docs/source/tests.rst
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 regexriot-0.0.2/env_files/demo.txt
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 regexriot-0.0.2/env_files/documentation.txt
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 regexriot-0.0.2/env_files/requirements.txt
--rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 regexriot-0.0.2/scripts/build_demo.sh
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 regexriot-0.0.2/scripts/build_docs.sh
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 regexriot-0.0.2/scripts/run_tests.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 regexriot-0.0.2/scripts/serve.sh
--rwxr-xr-x   0        0        0     2536 2020-02-02 00:00:00.000000 regexriot-0.0.2/src/try_it_out.ipynb
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 regexriot-0.0.2/src/RegexRiot/__init__.py
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 regexriot-0.0.2/src/RegexRiot/_operations.py
--rwxr-xr-x   0        0        0     3635 2020-02-02 00:00:00.000000 regexriot-0.0.2/src/RegexRiot/riot.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 regexriot-0.0.2/tests/__init__.py
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 regexriot-0.0.2/tests/test_operations.py
--rwxr-xr-x   0        0        0     2561 2020-02-02 00:00:00.000000 regexriot-0.0.2/tests/test_regextutorials.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 regexriot-0.0.2/tests/test_symbols.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 regexriot-0.0.2/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 regexriot-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 regexriot-0.0.2/README.md
--rwxr-xr-x   0        0        0      447 2020-02-02 00:00:00.000000 regexriot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 regexriot-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 regexriot-0.0.3/overrides.json
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 regexriot-0.0.3/.github/workflows/docsite.yml
+-rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 regexriot-0.0.3/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/make.bat
+-rwxr-xr-x   0        0        0     2586 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/conf.py
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/devlog.rst
+-rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/index.rst
+-rwxr-xr-x   0        0        0      208 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/RegexRiot/BasicExpressions.rst
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/RegexRiot/RiotString.rst
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/RegexRiot/index.rst
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/tests/index.rst
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/tests/operations.rst
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/tests/regextutorials.rst
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 regexriot-0.0.3/docs/source/tests/symbols.rst
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 regexriot-0.0.3/env_files/demo.txt
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 regexriot-0.0.3/env_files/documentation.txt
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 regexriot-0.0.3/env_files/requirements.txt
+-rwxr-xr-x   0        0        0      158 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/build_and_publish.sh
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/make_all.sh
+-rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/make_demo.sh
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/make_docs.sh
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/run_tests.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 regexriot-0.0.3/scripts/serve.sh
+-rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 regexriot-0.0.3/src/try_it_out.ipynb
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 regexriot-0.0.3/src/RegexRiot/__init__.py
+-rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 regexriot-0.0.3/src/RegexRiot/_basic_expressions.py
+-rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 regexriot-0.0.3/src/RegexRiot/_operations.py
+-rwxr-xr-x   0        0        0     3084 2020-02-02 00:00:00.000000 regexriot-0.0.3/src/RegexRiot/_riot.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 regexriot-0.0.3/tests/__init__.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 regexriot-0.0.3/tests/test_operations.py
+-rwxr-xr-x   0        0        0     4074 2020-02-02 00:00:00.000000 regexriot-0.0.3/tests/test_regextutorials.py
+-rwxr-xr-x   0        0        0     1227 2020-02-02 00:00:00.000000 regexriot-0.0.3/tests/test_symbols.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 regexriot-0.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 regexriot-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 regexriot-0.0.3/README.md
+-rwxr-xr-x   0        0        0      447 2020-02-02 00:00:00.000000 regexriot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 regexriot-0.0.3/PKG-INFO
```

### Comparing `regexriot-0.0.2/.github/workflows/docsite.yml` & `regexriot-0.0.3/.github/workflows/docsite.yml`

 * *Files identical despite different names*

### Comparing `regexriot-0.0.2/docs/Makefile` & `regexriot-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regexriot-0.0.2/docs/make.bat` & `regexriot-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `regexriot-0.0.2/docs/source/index.rst` & `regexriot-0.0.3/docs/source/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -7,32 +7,45 @@
 =====================================
 
 A simple easy to use and read regex maker.
 
 .. raw:: html
 
    <iframe
-      src="https://rk22000.github.io/regex-riot-python/demo/repl/?toolbar=1&kernel=python&code=from%20regex_riot_rk22000.riot%20import%20*%0Aone_or_more(DIGIT).then(DOT).then(one_or_more(DIGIT))"
+      src="demo/repl/?toolbar=1&kernel=python&code=from%20RegexRiot%20import%20*%0Aone_or_more(DIGIT).then(DOT).then(one_or_more(DIGIT))"
       width="100%"
-      height="500"
+      height="300"
    ></iframe>
 
 
 See its effectiveness against a few `regex exercises <https://rk22000.github.io/regex-riot-python/demo/notebooks/?path=try_it_out.ipynb>`_.
 
+Installation 
+------------
+
+RegexRiot can be installed using pip.
+
+.. code::
+
+   pip install RegexRiot
 
 
 .. toctree::
-   :maxdepth: 2
-   :caption: API:
    :hidden:
+   :caption: Modules
 
-   modules
+   RegexRiot/index
+   tests/index
+
+.. toctree::
+   :hidden:
+   :caption: Extra Stuff
 
+   devlog
 
 
 Indices and tables
-==================
+------------------
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `regexriot-0.0.2/src/try_it_out.ipynb` & `regexriot-0.0.3/src/try_it_out.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9579166666666666%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from RegexRiot import *\\n')], delete: [0]}}, insert: "*

 * *            "[(4, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', "*

 * *            "['Years before 1990\\n', '-----------------\\n', 'Match titles of all films produced "*

 * *            "before 1990.\\n', '\\n', '- 1 The Shawshank Redemption (1994)\\n', '- 2 The Godfather "*

 * *            "(1972)\\n', '- 3 The Godfather: Part II (1974)\\n', '- 4 Pulp Fiction (1994)\\n', '- "*

 * *             […]*

```diff
@@ -12,15 +12,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from RegexRiot.riot import *\n",
+                "from RegexRiot import *\n",
                 "def showcase(rs:RiotString, lines):\n",
                 "    if rs is None:\n",
                 "        print(\"You forgot to set `rs` to a Riot Expression\")\n",
                 "        print(\"Feel free to use the hint\")\n",
                 "        return\n",
                 "    rs = rs.compile()\n",
                 "    for ln in lines:\n",
@@ -65,14 +65,67 @@
                 "Earth to sun distance 149600000 km\n",
                 "Acceleration of gravity 9.80665 m/s^2\n",
                 "Circumference to diameter ratio 3.141592\n",
                 "Gas constant 8.3144621 J/mol*K\n",
                 "\"\"\".strip().split('\\n')\n",
                 "showcase(rs, lines)\n"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Years before 1990\n",
+                "-----------------\n",
+                "Match titles of all films produced before 1990.\n",
+                "\n",
+                "- 1 The Shawshank Redemption (1994)\n",
+                "- 2 The Godfather (1972)\n",
+                "- 3 The Godfather: Part II (1974)\n",
+                "- 4 Pulp Fiction (1994)\n",
+                "- 5 The Good, the Bad and the Ugly (1966)\n",
+                "- 6 The Dark Knight (2008)\n",
+                "- 7 12 Angry Men (1957)\n",
+                "- 8 Schindler's List (1993)\n",
+                "- 9 The Lord of the Rings: The Return of the King (2003)\n",
+                "- 10 Fight Club (1999)\n",
+                "\n",
+                "<details>\n",
+                "<summary>\n",
+                "Hint: You can create a regex set in the following two ways <code>riot(a,b,c,d)</code>, <code>riot(a, to=b)</code>\n",
+                "</summary>\n",
+                "\n",
+                "```py\n",
+                "BEGINING.then(one_or_more(ANYTHING)).then(OPEN_PARENTHESIS).then(1).then(DIGIT).then(riot(0, to=8)).then(DIGIT).then(CLOSE_PARENTHESIS)\n",
+                "```\n",
+                "\n",
+                "</details>"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "rs = BEGINING.then(one_or_more(ANYTHING)).then(OPEN_PARENTHESIS).then(1).\\\n",
+                "    then(DIGIT).then(riot(0, to=8)).then(DIGIT).then(CLOSE_PARENTHESIS)\n",
+                "lines = \"\"\"1 The Shawshank Redemption (1994)\n",
+                "2 The Godfather (1972)\n",
+                "3 The Godfather: Part II (1974)\n",
+                "4 Pulp Fiction (1994)\n",
+                "5 The Good, the Bad and the Ugly (1966)\n",
+                "6 The Dark Knight (2008)\n",
+                "7 12 Angry Men (1957)\n",
+                "8 Schindler's List (1993)\n",
+                "9 The Lord of the Rings: The Return of the King (2003)\n",
+                "10 Fight Club (1999)\n",
+                "\"\"\".strip().split('\\n')\n",
+                "showcase(rs, lines)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `regexriot-0.0.2/tests/test_operations.py` & `regexriot-0.0.3/tests/test_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.RegexRiot.riot import *
+from src.RegexRiot import *
 import unittest
 
 class RiotOperationsString(unittest.TestCase):
     """
     These tests will check that the RiotStrings are forming correctly.
     Another set of tests will check wheter the RiotString match correctly.
     
@@ -12,7 +12,10 @@
         self.assertEqual(str(DIGIT.then(NON_ALPHANUM)), r'\d\W')
     
     def test_one_or_more(self):
         self.assertEqual(str(DIGIT.one_or_more()), r'\d+')
         self.assertEqual(str(riot('hello').one_or_more()), r'(hello)+')
         self.assertEqual(str(one_or_more(DIGIT)), r'\d+')
         self.assertEqual(str(one_or_more(riot('hello'))), r'(hello)+')
+
+    def test_one_or_more_around_then(self):
+        self.assertEqual(str(one_or_more(DIGIT.then(ALPHANUM))), r'(\d\w)+')
```

### Comparing `regexriot-0.0.2/tests/test_symbols.py` & `regexriot-0.0.3/tests/test_symbols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.RegexRiot.riot import *
+from src.RegexRiot import *
 import unittest
 
 class LiteralsStringValueTests(unittest.TestCase):
     
     def test_digit(self):
         self.assertEqual(str(DIGIT), r'\d')
         self.assertEqual(str(NON_DIGIT), r'\D')
@@ -25,7 +25,16 @@
     def test_dot(self):
         self.assertEqual(str(DOT), r'\.')
     
     def test_custom_string(self):
         words = ['hello','there', ',', ' ', 'general', 'kenobi']
         for w in words:
             self.assertEqual(str(riot(w)), w)
+    
+    def test_begining_and_end(self):
+        self.assertEqual(str(BEGINING), r'^')
+        self.assertEqual(str(END), r'$')
+    
+    def test_round_parentheses(self):
+        self.assertEqual(str(OPEN_PARENTHESIS), r'\(')
+        self.assertEqual(str(CLOSE_PARENTHESIS), r'\)')
+
```

### Comparing `regexriot-0.0.2/LICENSE` & `regexriot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regexriot-0.0.2/README.md` & `regexriot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `regexriot-0.0.2/PKG-INFO` & `regexriot-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: RegexRiot
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple easy to use and read regex maker.
 Author-email: Rahul Kandekar <rahukand@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

