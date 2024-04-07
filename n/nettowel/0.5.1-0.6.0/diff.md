# Comparing `tmp/nettowel-0.5.1.tar.gz` & `tmp/nettowel-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettowel-0.5.1.tar", max compression
+gzip compressed data, was "nettowel-0.6.0.tar", max compression
```

## Comparing `nettowel-0.5.1.tar` & `nettowel-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-05-30 07:46:29.939791 nettowel-0.5.1/LICENSE
--rw-r--r--   0        0        0     4149 2023-05-30 07:46:53.171877 nettowel-0.5.1/README.md
--rw-r--r--   0        0        0       39 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/__init__.py
--rw-r--r--   0        0        0       73 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/__main__.py
--rw-r--r--   0        0        0      441 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/_common.py
--rw-r--r--   0        0        0        0 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/__init__.py
--rw-r--r--   0        0        0     3140 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/_common.py
--rw-r--r--   0        0        0       62 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/_output.py
--rw-r--r--   0        0        0     1084 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/diff.py
--rw-r--r--   0        0        0      507 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/help.py
--rw-r--r--   0        0        0     1448 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/ip.py
--rw-r--r--   0        0        0    10255 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/jinja.py
--rw-r--r--   0        0        0      316 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/logging.py
--rw-r--r--   0        0        0     2801 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/main.py
--rw-r--r--   0        0        0      643 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/napalm.py
--rw-r--r--   0        0        0     6929 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/netmiko.py
--rw-r--r--   0        0        0      642 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/nornir.py
--rw-r--r--   0        0        0     1102 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/pandas.py
--rw-r--r--   0        0        0    12319 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/restconf.py
--rw-r--r--   0        0        0      643 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/scrapli.py
--rw-r--r--   0        0        0      655 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/textfsm.py
--rw-r--r--   0        0        0     3908 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/ttp.py
--rw-r--r--   0        0        0     2627 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/yaml.py
--rw-r--r--   0        0        0      986 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/exceptions.py
--rw-r--r--   0        0        0     3142 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/jinja.py
--rw-r--r--   0        0        0      133 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/logger.py
--rw-r--r--   0        0        0     2659 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/netmiko.py
--rw-r--r--   0        0        0      731 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/pandas.py
--rw-r--r--   0        0        0        0 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/py.typed
--rw-r--r--   0        0        0     2094 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/restconf.py
--rw-r--r--   0        0        0      613 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/trogon_tui.py
--rw-r--r--   0        0        0      621 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/ttp.py
--rw-r--r--   0        0        0      799 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/yaml.py
--rw-r--r--   0        0        0     2966 2023-05-30 07:46:29.951791 nettowel-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 nettowel-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 15:41:07.424669 nettowel-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4708 2024-04-07 15:41:22.464805 nettowel-0.6.0/README.md
+-rw-r--r--   0        0        0       39 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/__main__.py
+-rw-r--r--   0        0        0      441 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/_common.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/__init__.py
+-rw-r--r--   0        0        0     3140 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/_common.py
+-rw-r--r--   0        0        0       62 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/_output.py
+-rw-r--r--   0        0        0     1084 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/diff.py
+-rw-r--r--   0        0        0      507 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/help.py
+-rw-r--r--   0        0        0     1448 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/ip.py
+-rw-r--r--   0        0        0    10255 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/jinja.py
+-rw-r--r--   0        0        0     4825 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/jsonpatch.py
+-rw-r--r--   0        0        0      316 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/logging.py
+-rw-r--r--   0        0        0     2891 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/main.py
+-rw-r--r--   0        0        0      643 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/napalm.py
+-rw-r--r--   0        0        0     6929 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/netmiko.py
+-rw-r--r--   0        0        0      642 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/nornir.py
+-rw-r--r--   0        0        0     1102 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/pandas.py
+-rw-r--r--   0        0        0    12319 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/restconf.py
+-rw-r--r--   0        0        0      643 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/scrapli.py
+-rw-r--r--   0        0        0      655 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/textfsm.py
+-rw-r--r--   0        0        0     3908 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/ttp.py
+-rw-r--r--   0        0        0     2627 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/cli/yaml.py
+-rw-r--r--   0        0        0      966 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/exceptions.py
+-rw-r--r--   0        0        0     3142 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/jinja.py
+-rw-r--r--   0        0        0     1210 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/jsonpatch.py
+-rw-r--r--   0        0        0      133 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/logger.py
+-rw-r--r--   0        0        0     2659 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/netmiko.py
+-rw-r--r--   0        0        0      731 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/pandas.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/py.typed
+-rw-r--r--   0        0        0     2146 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/restconf.py
+-rw-r--r--   0        0        0      613 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/trogon_tui.py
+-rw-r--r--   0        0        0      621 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/ttp.py
+-rw-r--r--   0        0        0      799 2024-04-07 15:41:07.432669 nettowel-0.6.0/nettowel/yaml.py
+-rw-r--r--   0        0        0     3177 2024-04-07 15:41:07.436669 nettowel-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 nettowel-0.6.0/PKG-INFO
```

### Comparing `nettowel-0.5.1/LICENSE` & `nettowel-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/README.md` & `nettowel-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,21 @@
 Collection of useful network automation functions 
 
 
 > ⚠️ `nettowel` is under heavy construction and not production ready. Feedback is highly appreciated.
 
 
 ## Install
+It is recommended to install `nettowel` with [pipx](https://pipx.pypa.io/). Therefore you have the dependencies isolated and you can use the `nettowel` or `nt` command.
 
-You can install it directly from pypi
+```bash
+pipx install nettowel[full]
+```
+
+You can also install it directly from pypi
 
 ```bash
 pip install nettowel
 ```
 
 To reduce the dependencies the extra dependencies are grouped
 
@@ -27,14 +32,15 @@
 - ttp
 - textfsm
 - napalm
 - netmiko
 - scrapli
 - nornir
 - pandas
+- jsonpatch
 - tui
 
 ```bash
 pip install nettowel[jinja]
 pip install nettowel[full]
 ```
 
@@ -130,14 +136,26 @@
 
 ![yaml load](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-load.png)
 
 #### dump
 
 ![yaml dump](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-dump.png)
 
+
+### JSON Patch ([RFC 6902](http://tools.ietf.org/html/rfc6902))
+
+#### create
+
+![JSON Patch create](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/jsonpatch-create.png)
+
+#### apply
+
+![JSON Patch apply](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/jsonpatch-apply.png)
+
+
 ### Help
 
 ![Help QRcode](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/nettowel-help.png)
 
 
 ### Settings
```

### Comparing `nettowel-0.5.1/nettowel/cli/_common.py` & `nettowel-0.6.0/nettowel/cli/_common.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/diff.py` & `nettowel-0.6.0/nettowel/cli/diff.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/ip.py` & `nettowel-0.6.0/nettowel/cli/ip.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/jinja.py` & `nettowel-0.6.0/nettowel/cli/jinja.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/main.py` & `nettowel-0.6.0/nettowel/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from nettowel.cli.yaml import app as yaml_app
 from nettowel.cli.nornir import app as nornir_app
 from nettowel.cli.napalm import app as napalm_app
 from nettowel.cli.netmiko import app as netmiko_app
 from nettowel.cli.scrapli import app as scrapli_app
 from nettowel.cli.restconf import app as restconf_app
 from nettowel.cli.pandas import app as pandas_app
+from nettowel.cli.jsonpatch import app as jsonpatch_app
 from nettowel.cli.help import get_qrcode, HELP_MARKDOWN
 
 from nettowel.exceptions import NettowelDependencyMissing
 
 app = get_typer_app(help="Awesome collection of network automation functions")
 
 for subapp, name in [
@@ -36,14 +37,15 @@
     (yaml_app, "yaml"),
     (nornir_app, "nornir"),
     (napalm_app, "napalm"),
     (netmiko_app, "netmiko"),
     (scrapli_app, "scrapli"),
     (restconf_app, "restconf"),
     (pandas_app, "pandas"),
+    (jsonpatch_app, "jsonpatch"),
 ]:
     app.add_typer(subapp, name=name)
 
 
 @app.command()
 def help(
     ctx: typer.Context,
```

### Comparing `nettowel-0.5.1/nettowel/cli/napalm.py` & `nettowel-0.6.0/nettowel/cli/napalm.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/netmiko.py` & `nettowel-0.6.0/nettowel/cli/netmiko.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/nornir.py` & `nettowel-0.6.0/nettowel/cli/nornir.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/pandas.py` & `nettowel-0.6.0/nettowel/cli/pandas.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/restconf.py` & `nettowel-0.6.0/nettowel/cli/restconf.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/scrapli.py` & `nettowel-0.6.0/nettowel/cli/scrapli.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/textfsm.py` & `nettowel-0.6.0/nettowel/cli/textfsm.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/ttp.py` & `nettowel-0.6.0/nettowel/cli/ttp.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/cli/yaml.py` & `nettowel-0.6.0/nettowel/cli/yaml.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/jinja.py` & `nettowel-0.6.0/nettowel/jinja.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/netmiko.py` & `nettowel-0.6.0/nettowel/netmiko.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/pandas.py` & `nettowel-0.6.0/nettowel/pandas.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/restconf.py` & `nettowel-0.6.0/nettowel/restconf.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,21 +48,20 @@
             return "201 Created"
         if response.text == "":
             return "Empty Response"
         return response.json() if not return_xml else response.text
     except requests.exceptions.ConnectionError as exc:
         raise NettowelRestconfError(str(exc), None)
     except requests.exceptions.RequestException as exc:
-        if exc.request:
+        exc_response: Any = None
+        if exc.request is not None and exc.response is not None:
             if not exc.response.text:
-                response = None
+                exc_response = None
             else:
                 if return_xml:
                     return exc.response.text
                 try:
-                    response = exc.response.json()
+                    exc_response = exc.response.json()
                 except json.decoder.JSONDecodeError:
-                    response = exc.response.text
-        else:
-            response = None
-        log.debug(response)
-        raise NettowelRestconfError(str(exc), response)
+                    exc_response = exc.response.text
+        log.debug(exc_response)
+        raise NettowelRestconfError(str(exc), exc_response)
```

### Comparing `nettowel-0.5.1/nettowel/trogon_tui.py` & `nettowel-0.6.0/nettowel/trogon_tui.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/ttp.py` & `nettowel-0.6.0/nettowel/ttp.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/nettowel/yaml.py` & `nettowel-0.6.0/nettowel/yaml.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.1/pyproject.toml` & `nettowel-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 [tool.poetry]
 name = "nettowel"
-version = "0.5.1"
+version = "0.6.0"
 description = "Network Automation Collection"
 authors = ["ubaumann <github@m.ubaumann.ch>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/InfrastructureAsCode-ch/nettowel"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = "^0.9"
+typer = "^0.9|^0.10|^0.11|^0.12"
 rich = "^12|^13"
-Jinja2 = {version = "^3.0.3", optional = true}
+Jinja2 = {version = "^3", optional = true}
 ttp = {version = "^0.9", optional = true}
 textfsm = {version = "^1.1", optional = true}
 napalm = {version = "^4", optional = true}
 netmiko = {version = "^4", optional = true}
 scrapli = {version = "^2023.1.30", optional = true}
 nornir = {version = "^3.2", optional = true}
-"ruamel.yaml" = "^0.17.21"
+"ruamel.yaml" = "^0.18"
 jinja2schema = {version = "^0.1.4", optional = true}
 qrcode = "^7.3.1"
 python-dotenv = "^1"
 requests = "^2.27.1"
 nornir-napalm = {version = "^0.4", optional = true}
 nornir-scrapli = {version = "^2023.1.30", optional = true}
 nornir-utils = {version = "^0.2.0", optional = true}
 nornir-jinja2 = {version = "^0.2.0", optional = true}
 nornir-pyxl = {version = "^1.0.1", optional = true}
 nornir-http = {version = "^0.1", optional = true}
 nornir-netmiko = {version = "^1.0.0", optional = true}
 nornir-rich = {version = "^0.1", optional = true}
 pandas = {version = "^2", optional = true}
-trogon = {version = "^0.4.0", optional = true}
+trogon = {version = "^0.5.0", optional = true}
+jsonpatch = {version = "^1.33", optional = true}
+
 
 [tool.poetry.dev-dependencies]
-black = "^22|^23"
-pytest = "^7"
+black = "^22|^23|^24"
+pytest = "^7|^8"
 mypy = "^0.942|^1"
 types-requests = "^2.27.20"
 
 [tool.poetry.extras]
 jinja = ["Jinja2", "jinja2schema"]
 ttp = ["ttp"]
 textfsm = ["textfsm"]
 napalm = ["napalm"]
 netmiko = ["netmiko"]
 scrapli = ["scrapli"]
 nornir = ["nornir", "nornir-napalm", "nornir-scrapli", "nornir-utils", "nornir-jinja2", "nornir-pyxl", "nornir-http", "nornir-netmiko", "nornir-rich"]
 pandas = ["pandas"]
 tui = ["trogon"]
+jsonpatch = ["jsonpatch"]
 full = [
     "Jinja2", 
     "jinja2schema", 
     "ttp", 
     "textfsm", 
     "napalm", 
     "netmiko", 
@@ -70,15 +75,16 @@
     "nornir-utils", 
     "nornir-jinja2", 
     "nornir-pyxl", 
     "nornir-http", 
     "nornir-netmiko", 
     "nornir-rich", 
     "pandas",
-    "trogon"
+    "trogon",
+    "jsonpatch"
 ]
 
 [tool.poetry.scripts]
 nettowel = 'nettowel.cli.main:run'
 nt = 'nettowel.cli.main:run'
 
 [build-system]
```

### Comparing `nettowel-0.5.1/PKG-INFO` & `nettowel-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: nettowel
-Version: 0.5.1
+Version: 0.6.0
 Summary: Network Automation Collection
 Home-page: https://github.com/InfrastructureAsCode-ch/nettowel
 License: Apache 2.0
 Author: ubaumann
 Author-email: github@m.ubaumann.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: full
 Provides-Extra: jinja
+Provides-Extra: jsonpatch
 Provides-Extra: napalm
 Provides-Extra: netmiko
 Provides-Extra: nornir
 Provides-Extra: pandas
 Provides-Extra: scrapli
 Provides-Extra: textfsm
 Provides-Extra: ttp
 Provides-Extra: tui
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0) ; extra == "jinja" or extra == "full"
+Requires-Dist: Jinja2 (>=3,<4) ; extra == "jinja" or extra == "full"
 Requires-Dist: jinja2schema (>=0.1.4,<0.2.0) ; extra == "jinja" or extra == "full"
+Requires-Dist: jsonpatch (>=1.33,<2.0) ; extra == "jsonpatch" or extra == "full"
 Requires-Dist: napalm (>=4,<5) ; extra == "napalm" or extra == "full"
 Requires-Dist: netmiko (>=4,<5) ; extra == "netmiko" or extra == "full"
 Requires-Dist: nornir (>=3.2,<4.0) ; extra == "nornir" or extra == "full"
 Requires-Dist: nornir-http (>=0.1,<0.2) ; extra == "nornir" or extra == "full"
 Requires-Dist: nornir-jinja2 (>=0.2.0,<0.3.0) ; extra == "nornir" or extra == "full"
 Requires-Dist: nornir-napalm (>=0.4,<0.5) ; extra == "nornir" or extra == "full"
 Requires-Dist: nornir-netmiko (>=1.0.0,<2.0.0) ; extra == "nornir" or extra == "full"
@@ -38,20 +41,20 @@
 Requires-Dist: nornir-scrapli (>=2023.1.30,<2024.0.0) ; extra == "nornir" or extra == "full"
 Requires-Dist: nornir-utils (>=0.2.0,<0.3.0) ; extra == "nornir" or extra == "full"
 Requires-Dist: pandas (>=2,<3) ; extra == "pandas" or extra == "full"
 Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12,<14)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: ruamel.yaml (>=0.18,<0.19)
 Requires-Dist: scrapli (>=2023.1.30,<2024.0.0) ; extra == "scrapli" or extra == "full"
 Requires-Dist: textfsm (>=1.1,<2.0) ; extra == "textfsm" or extra == "full"
-Requires-Dist: trogon (>=0.4.0,<0.5.0) ; extra == "tui" or extra == "full"
+Requires-Dist: trogon (>=0.5.0,<0.6.0) ; extra == "tui" or extra == "full"
 Requires-Dist: ttp (>=0.9,<0.10) ; extra == "ttp" or extra == "full"
-Requires-Dist: typer (>=0.9,<0.10)
+Requires-Dist: typer (>=0.9,<0.13)
 Project-URL: Repository, https://github.com/InfrastructureAsCode-ch/nettowel
 Description-Content-Type: text/markdown
 
 [![PyPI versions](https://img.shields.io/pypi/pyversions/nettowel.svg)](https://pypi.python.org/pypi/nettowel/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![Downloads](https://pepy.tech/badge/nettowel)](https://pepy.tech/project/nettowel)
@@ -60,16 +63,21 @@
 Collection of useful network automation functions 
 
 
 > ⚠️ `nettowel` is under heavy construction and not production ready. Feedback is highly appreciated.
 
 
 ## Install
+It is recommended to install `nettowel` with [pipx](https://pipx.pypa.io/). Therefore you have the dependencies isolated and you can use the `nettowel` or `nt` command.
 
-You can install it directly from pypi
+```bash
+pipx install nettowel[full]
+```
+
+You can also install it directly from pypi
 
 ```bash
 pip install nettowel
 ```
 
 To reduce the dependencies the extra dependencies are grouped
 
@@ -80,14 +88,15 @@
 - ttp
 - textfsm
 - napalm
 - netmiko
 - scrapli
 - nornir
 - pandas
+- jsonpatch
 - tui
 
 ```bash
 pip install nettowel[jinja]
 pip install nettowel[full]
 ```
 
@@ -183,14 +192,26 @@
 
 ![yaml load](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-load.png)
 
 #### dump
 
 ![yaml dump](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-dump.png)
 
+
+### JSON Patch ([RFC 6902](http://tools.ietf.org/html/rfc6902))
+
+#### create
+
+![JSON Patch create](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/jsonpatch-create.png)
+
+#### apply
+
+![JSON Patch apply](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/jsonpatch-apply.png)
+
+
 ### Help
 
 ![Help QRcode](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/nettowel-help.png)
 
 
 ### Settings
```

