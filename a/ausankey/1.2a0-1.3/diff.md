# Comparing `tmp/ausankey-1.2a0.tar.gz` & `tmp/ausankey-1.3.tar.gz`

## Comparing `ausankey-1.2a0.tar` & `ausankey-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ausankey-1.2a0/ausankey/__init__.py
--rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 ausankey-1.2a0/ausankey/ausankey.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ausankey-1.2a0/tests/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ausankey-1.2a0/tests/fruit.csv
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ausankey-1.2a0/tests/generic_test.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ausankey-1.2a0/tests/test_fruit_defaults.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ausankey-1.2a0/tests/test_fruit_setup.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ausankey-1.2a0/.gitignore
--rw-r--r--   0        0        0    35146 2020-02-02 00:00:00.000000 ausankey-1.2a0/LICENSE
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 ausankey-1.2a0/README.md
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 ausankey-1.2a0/pyproject.toml
--rw-r--r--   0        0        0    43063 2020-02-02 00:00:00.000000 ausankey-1.2a0/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ausankey-1.3/ausankey/__init__.py
+-rw-r--r--   0        0        0    31411 2020-02-02 00:00:00.000000 ausankey-1.3/ausankey/ausankey.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ausankey-1.3/tests/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ausankey-1.3/tests/fruit.csv
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ausankey-1.3/tests/generic_test.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ausankey-1.3/tests/test_fruit_defaults.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ausankey-1.3/tests/test_fruit_setup.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ausankey-1.3/.gitignore
+-rw-r--r--   0        0        0    35146 2020-02-02 00:00:00.000000 ausankey-1.3/LICENSE
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ausankey-1.3/README.md
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 ausankey-1.3/pyproject.toml
+-rw-r--r--   0        0        0    43279 2020-02-02 00:00:00.000000 ausankey-1.3/PKG-INFO
```

### Comparing `ausankey-1.2a0/tests/test_fruit_defaults.py` & `ausankey-1.3/tests/test_fruit_defaults.py`

 * *Files identical despite different names*

### Comparing `ausankey-1.2a0/LICENSE` & `ausankey-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ausankey-1.2a0/README.md` & `ausankey-1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,23 @@
 [![PyPI version](https://badge.fury.io/py/auSankey.svg)](https://badge.fury.io/py/auSankey)
 [![Coverage Status](https://coveralls.io/repos/github/AUMAG/auSankey/badge.svg?branch=main)](https://coveralls.io/github/AUMAG/auSankey?branch=main)
 
 [![Python package](https://github.com/AUMAG/auSankey/actions/workflows/check.yml/badge.svg)](https://github.com/AUMAG/auSankey/actions/workflows/check.yml)
 [![Jekyll Pages](https://github.com/AUMAG/auSankey/actions/workflows/doc.yml/badge.svg)](https://github.com/AUMAG/auSankey/actions/workflows/doc.yml)
 [![Publish release](https://github.com/AUMAG/ausankey/actions/workflows/release.yml/badge.svg)](https://github.com/AUMAG/ausankey/actions/workflows/release.yml)
 
+This package is [available on PyPi](https://pypi.org/project/ausankey/) and can be installed via:
+
+    pip install ausankey
+
 User documentation for the repository is published via GitHub Pages: https://aumag.github.io/ausankey/
 
+Code documentation by Mkdocs is available here:
+https://aumag.github.io/ausankey/reference/
+
 ## Minimal example
 
 ![example](https://aumag.github.io/ausankey/frame3_pretty.png)
 
 ``` python
 import ausankey as sky
 import matplotlib.pyplot as plt
```

#### html2text {}

```diff
@@ -4,18 +4,20 @@
 github/AUMAG/auSankey/badge.svg?branch=main)](https://coveralls.io/github/
 AUMAG/auSankey?branch=main) [![Python package](https://github.com/AUMAG/
 auSankey/actions/workflows/check.yml/badge.svg)](https://github.com/AUMAG/
 auSankey/actions/workflows/check.yml) [![Jekyll Pages](https://github.com/
 AUMAG/auSankey/actions/workflows/doc.yml/badge.svg)](https://github.com/AUMAG/
 auSankey/actions/workflows/doc.yml) [![Publish release](https://github.com/
 AUMAG/ausankey/actions/workflows/release.yml/badge.svg)](https://github.com/
-AUMAG/ausankey/actions/workflows/release.yml) User documentation for the
-repository is published via GitHub Pages: https://aumag.github.io/ausankey/ ##
-Minimal example ![example](https://aumag.github.io/ausankey/frame3_pretty.png)
-``` python import ausankey as sky import matplotlib.pyplot as plt import pandas
-as pd data = pd.DataFrame([ ("a",1.0,"ab",2.0,"a",1.0),
-("a",1.0,"ba",0.8,"ba",0.4), ("c",1.5,"cd",0.5,"d",2.0),
-("b",0.5,"ba",0.8,"ba",0.4), ("b",0.5,"ab",0.8,"a",1.0),
-("d",2.0,"cd",0.4,"d",1.0), ("e",1.0,"e",1.0,"e",3.0), ]) plt.figure()
-sky.sankey( data, sort = âtopâ, titles = ["Stage 1","Stage 2","Stage 3"],
-valign = "center", ) plt.show() ``` ## Requirements * Python 3.x * matplotlib *
-numpy * pandas
+AUMAG/ausankey/actions/workflows/release.yml) This package is [available on
+PyPi](https://pypi.org/project/ausankey/) and can be installed via: pip install
+ausankey User documentation for the repository is published via GitHub Pages:
+https://aumag.github.io/ausankey/ Code documentation by Mkdocs is available
+here: https://aumag.github.io/ausankey/reference/ ## Minimal example ![example]
+(https://aumag.github.io/ausankey/frame3_pretty.png) ``` python import ausankey
+as sky import matplotlib.pyplot as plt import pandas as pd data = pd.DataFrame(
+[ ("a",1.0,"ab",2.0,"a",1.0), ("a",1.0,"ba",0.8,"ba",0.4),
+("c",1.5,"cd",0.5,"d",2.0), ("b",0.5,"ba",0.8,"ba",0.4),
+("b",0.5,"ab",0.8,"a",1.0), ("d",2.0,"cd",0.4,"d",1.0),
+("e",1.0,"e",1.0,"e",3.0), ]) plt.figure() sky.sankey( data, sort = âtopâ,
+titles = ["Stage 1","Stage 2","Stage 3"], valign = "center", ) plt.show() ```
+## Requirements * Python 3.x * matplotlib * numpy * pandas
```

### Comparing `ausankey-1.2a0/pyproject.toml` & `ausankey-1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ausankey"
-version = "1.2a"
+version = "1.3"
 
 description = "Sankey diagrams simply"
 readme = "README.md"
 license = {file = "LICENSE"}
 
 dependencies = [
     "matplotlib",
@@ -70,15 +70,16 @@
 ]
 
 [tool.hatch.envs.doc]
 dependencies = ["mkdocs", "mkdocstrings[python]"]
 
 [tool.hatch.envs.doc.scripts]
 ref = "mkdocs -v build"
-img = "cd docs; python sankey_doc_examples.py; cp -v *.png ../_site/"
+img = "cd docs; python sankey_doc_examples.py"
+icp = "cd docs; cp -v *.png ../_site/"
 
 
 [tool.hatch.envs.test]
 dependencies = [
     "pytest", "coverage", "coveralls",
     "mkdocstrings","mkdocstrings-python",
 ]
```

### Comparing `ausankey-1.2a0/PKG-INFO` & `ausankey-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ausankey
-Version: 1.2a0
+Version: 1.3
 Summary: Sankey diagrams simply
 Project-URL: Homepage, https://github.com/AUMAG/ausankey
 Project-URL: Documentation, https://aumag.github.io/ausankey/
 Project-URL: Repository, https://github.com/AUMAG/ausankey.git
 Project-URL: Issues, https://github.com/AUMAG/ausankey/issues
 Project-URL: Changelog, https://github.com/AUMAG/ausankey/blob/master/CHANGELOG.md
 Author-email: Will Robertson <wspr81@gmail.com>
@@ -703,16 +703,23 @@
 [![PyPI version](https://badge.fury.io/py/auSankey.svg)](https://badge.fury.io/py/auSankey)
 [![Coverage Status](https://coveralls.io/repos/github/AUMAG/auSankey/badge.svg?branch=main)](https://coveralls.io/github/AUMAG/auSankey?branch=main)
 
 [![Python package](https://github.com/AUMAG/auSankey/actions/workflows/check.yml/badge.svg)](https://github.com/AUMAG/auSankey/actions/workflows/check.yml)
 [![Jekyll Pages](https://github.com/AUMAG/auSankey/actions/workflows/doc.yml/badge.svg)](https://github.com/AUMAG/auSankey/actions/workflows/doc.yml)
 [![Publish release](https://github.com/AUMAG/ausankey/actions/workflows/release.yml/badge.svg)](https://github.com/AUMAG/ausankey/actions/workflows/release.yml)
 
+This package is [available on PyPi](https://pypi.org/project/ausankey/) and can be installed via:
+
+    pip install ausankey
+
 User documentation for the repository is published via GitHub Pages: https://aumag.github.io/ausankey/
 
+Code documentation by Mkdocs is available here:
+https://aumag.github.io/ausankey/reference/
+
 ## Minimal example
 
 ![example](https://aumag.github.io/ausankey/frame3_pretty.png)
 
 ``` python
 import ausankey as sky
 import matplotlib.pyplot as plt
```

