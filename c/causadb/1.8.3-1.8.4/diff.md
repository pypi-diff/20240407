# Comparing `tmp/causadb-1.8.3.tar.gz` & `tmp/causadb-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.8.3.tar", max compression
+gzip compressed data, was "causadb-1.8.4.tar", max compression
```

## Comparing `causadb-1.8.3.tar` & `causadb-1.8.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      642 2024-04-06 14:31:51.873085 causadb-1.8.3/README.md
--rw-r--r--   0        0        0      115 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-06 14:32:18.441332 causadb-1.8.3/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/examples/heating.py
--rw-r--r--   0        0        0    15743 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/model.py
--rw-r--r--   0        0        0     2555 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/plotting.py
--rw-r--r--   0        0        0      215 2024-04-06 14:31:51.873085 causadb-1.8.3/causadb/utils.py
--rw-r--r--   0        0        0      797 2024-04-06 14:32:17.345322 causadb-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-07 13:47:50.687443 causadb-1.8.4/README.md
+-rw-r--r--   0        0        0      115 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-07 13:48:33.635564 causadb-1.8.4/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/causadb.py
+-rw-r--r--   0        0        0     2109 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/cli/account.py
+-rw-r--r--   0        0        0     3153 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/cli/main.py
+-rw-r--r--   0        0        0     7104 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15743 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-07 13:47:50.687443 causadb-1.8.4/causadb/utils.py
+-rw-r--r--   0        0        0      797 2024-04-07 13:48:32.859562 causadb-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.4/PKG-INFO
```

### Comparing `causadb-1.8.3/README.md` & `causadb-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/causadb.py` & `causadb-1.8.4/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/cli/account.py` & `causadb-1.8.4/causadb/cli/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 
 
 @app.command()
 def setup():
     """
     Set up a CausaDB account on this device
     """
-    token_id = typer.prompt(
-        "Token ID")
     token_secret = typer.prompt(
-        "Token secret")
+        "Enter your token (begins with cdb_)")
 
     headers = {"token": token_secret}
 
     response = requests.get(
         f"{CAUSADB_URL}/account",
         headers=headers
     )
@@ -37,15 +35,14 @@
 
         config = {}
         if os.path.exists(config_filepath):
             with open(config_filepath, "r") as f:
                 config = toml.load(f)
 
         config["default"] = {
-            "token_id": token_id,
             "token_secret": token_secret,
         }
 
         with open(config_filepath, "w") as f:
             toml.dump(config, f)
 
     else:
@@ -74,32 +71,7 @@
         # Delete the token from ~/.causadb/config.toml.
 
         with open(config_filepath, "w") as f:
             toml.dump({}, f)
 
         typer.echo(
             f"Account successfully removed from this device. You can add it again with `causadb account setup`.")
-
-
-@app.command()
-def info():
-    """
-    Show information about the account
-    """
-    # Get config from ~/.causadb/config.toml
-    dir_name = os.path.expanduser("~/.causadb")
-    config_filepath = os.path.join(dir_name, "config.toml")
-
-    if not os.path.exists(config_filepath):
-        typer.echo(
-            "No config found in ~/.causadb/config.toml.")
-        return 1
-
-    # Get the token from ~/.causadb/config.toml.
-    with open(config_filepath, "r") as f:
-        config = toml.load(f)
-
-    org_id = config[list(config.keys())[0]]["org_id"]
-    token = config[list(config.keys())[0]]["token"]
-
-    typer.echo(f"Organization ID: {org_id}")
-    typer.echo(f"Token: {token}")
```

### Comparing `causadb-1.8.3/causadb/cli/data.py` & `causadb-1.8.4/causadb/cli/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,8 @@
         data = response.json()
         if data["status"] == "success":
             typer.echo("Successfully removed datasource.")
         else:
             typer.echo(f"Failed to remove datasource: {data['message']}")
     else:
         typer.echo(
-            f"Failed to remove datasource. Server responded with status code {response.status_code}.")
+            f"Failed to remove datasource. Server responded with status code {response.status_code}. Message: {response.json()['detail']}")
```

### Comparing `causadb-1.8.3/causadb/cli/main.py` & `causadb-1.8.4/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/cli/models.py` & `causadb-1.8.4/causadb/cli/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 ):
     """
     Show info about a model.
     """
 
     if model_name is None:
         model_name = typer.prompt(
-            "Enter the name of the model you wish to attach data to (e.g. my-model)")
+            "Enter the name of the model you wish to retrieve information about (e.g. my-model)")
 
     config = load_config()
     token_secret = config["default"]["token_secret"]
 
     headers = {"token": token_secret}
 
     data = requests.get(
@@ -179,15 +179,15 @@
     typer.echo(f"{data_name} successfully attached to {model_name}.")
 
 
 @app.command()
 def detach(
     model_name: Annotated[str, typer.Option(
         "--model",
-        help="The name of the model you wish to attach data to.")] = None
+        help="The name of the model you wish to detach data from.")] = None
 ):
     """
     Detach a datasource from a model.
     """
 
     if model_name is None:
         model_name = typer.prompt(
@@ -245,15 +245,15 @@
 ):
     """
     Show status of a model.
     """
 
     if model_name is None:
         model_name = typer.prompt(
-            "Enter the name of the model you wish to attach data to (e.g. my-model)")
+            "Enter the name of the model you wish to retrieve status for (e.g. my-model)")
 
     config = load_config()
     token_secret = config["default"]["token_secret"]
 
     headers = {"token": token_secret}
 
     data = requests.get(
```

### Comparing `causadb-1.8.3/causadb/cli/utils.py` & `causadb-1.8.4/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/data.py` & `causadb-1.8.4/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/examples/heating.py` & `causadb-1.8.4/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/model.py` & `causadb-1.8.4/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/causadb/plotting.py` & `causadb-1.8.4/causadb/plotting.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.3/pyproject.toml` & `causadb-1.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.8.3"
+version = "1.8.4"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.8.3/PKG-INFO` & `causadb-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.8.3
+Version: 1.8.4
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

