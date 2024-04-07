# Comparing `tmp/praetorian-cli-0.5.0.tar.gz` & `tmp/praetorian-cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praetorian-cli-0.5.0.tar", last modified: Fri Mar 22 19:14:04 2024, max compression
+gzip compressed data, was "praetorian-cli-0.7.1.tar", last modified: Sun Apr  7 01:40:20 2024, max compression
```

## Comparing `praetorian-cli-0.5.0.tar` & `praetorian-cli-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.804572 praetorian-cli-0.5.0/
--rw-r--r--   0 privateducky   (501) staff       (20)     1607 2024-03-22 19:14:04.804461 praetorian-cli-0.5.0/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)     1105 2024-03-21 22:30:25.000000 praetorian-cli-0.5.0/README.md
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.795237 praetorian-cli-0.5.0/praetorian_cli/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian-cli-0.5.0/praetorian_cli/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)      506 2024-03-18 11:12:25.000000 praetorian-cli-0.5.0/praetorian_cli/cli.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.798181 praetorian-cli-0.5.0/praetorian_cli/handlers/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian-cli-0.5.0/praetorian_cli/handlers/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     4865 2024-03-22 17:58:03.000000 praetorian-cli-0.5.0/praetorian_cli/handlers/backend.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.799110 praetorian-cli-0.5.0/praetorian_cli/sdk/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3293 2024-03-18 11:12:25.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/account.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2405 2024-03-22 11:17:56.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/chaos.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.803481 praetorian-cli-0.5.0/praetorian_cli/sdk/test/
--rw-r--r--   0 privateducky   (501) staff       (20)      465 2024-03-21 11:35:21.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1292 2024-03-22 11:17:56.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_file_upload.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2720 2024-03-22 10:22:51.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_job_capabilities.py
--rw-r--r--   0 privateducky   (501) staff       (20)      784 2024-03-22 11:11:23.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_manual_risk.py
--rw-r--r--   0 privateducky   (501) staff       (20)      661 2024-03-22 10:22:51.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_nvd.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1847 2024-03-22 10:22:51.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_seed.py
--rw-r--r--   0 privateducky   (501) staff       (20)      903 2024-03-22 11:17:56.000000 praetorian-cli-0.5.0/praetorian_cli/sdk/test/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-03-22 19:14:04.804156 praetorian-cli-0.5.0/praetorian_cli.egg-info/
--rw-r--r--   0 privateducky   (501) staff       (20)     1607 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)      752 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/SOURCES.txt
--rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/dependency_links.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/entry_points.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/requires.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-03-22 19:14:04.000000 praetorian-cli-0.5.0/praetorian_cli.egg-info/top_level.txt
--rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian-cli-0.5.0/pyproject.toml
--rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-03-22 19:14:04.805076 praetorian-cli-0.5.0/setup.cfg
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.572665 praetorian-cli-0.7.1/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-07 01:40:20.572561 praetorian-cli-0.7.1/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian-cli-0.7.1/README.md
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.566842 praetorian-cli-0.7.1/praetorian_cli/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian-cli-0.7.1/praetorian_cli/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      624 2024-04-04 16:57:50.000000 praetorian-cli-0.7.1/praetorian_cli/cli.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.569383 praetorian-cli-0.7.1/praetorian_cli/handlers/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian-cli-0.7.1/praetorian_cli/handlers/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2118 2024-04-07 01:32:46.000000 praetorian-cli-0.7.1/praetorian_cli/handlers/account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     4265 2024-04-07 01:32:42.000000 praetorian-cli-0.7.1/praetorian_cli/handlers/backend.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      436 2024-04-07 01:29:50.000000 praetorian-cli-0.7.1/praetorian_cli/handlers/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.570052 praetorian-cli-0.7.1/praetorian_cli/sdk/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2793 2024-04-07 01:33:46.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/chaos.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/keychain.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.571981 praetorian-cli-0.7.1/praetorian_cli/sdk/test/
+-rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-07 01:31:02.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_file_upload.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2418 2024-04-07 01:32:14.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_job_capabilities.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-07 01:32:19.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_link_account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      748 2024-04-07 01:32:29.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_manual_risk.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-07 01:31:41.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_nvd.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1814 2024-04-07 01:31:28.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_seed.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      879 2024-04-07 01:31:15.000000 praetorian-cli-0.7.1/praetorian_cli/sdk/test/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:40:20.572321 praetorian-cli-0.7.1/praetorian_cli.egg-info/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/entry_points.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/requires.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-07 01:40:20.000000 praetorian-cli-0.7.1/praetorian_cli.egg-info/top_level.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian-cli-0.7.1/pyproject.toml
+-rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-07 01:40:20.573145 praetorian-cli-0.7.1/setup.cfg
```

### Comparing `praetorian-cli-0.5.0/PKG-INFO` & `praetorian-cli-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.5.0
+Version: 0.7.1
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,19 +47,19 @@
 
 ## Developers
 
 Integrate the CLI into your own application:
 
 1. Include the dependency ``praetorian-cli`` in your project
 2. Import the Chaos class ``from praetorian_cli.sdk.chaos import Chaos``
-3. Import the Account class ``from praetorian_cli.sdk.account import Account``
+3. Import the Keychain class ``from praetorian_cli.sdk.keychain import Keychain``
 4. Call any function (example below)
 
 ### Example
 
 ```python
 from praetorian_cli.sdk.chaos import Chaos
-from praetorian_cli.sdk.account import Account
+from praetorian_cli.sdk.keychain import Keychain
 
-chaos = Chaos(Account(profile='United States'))
+chaos = Chaos(Keychain(profile='United States'))
 chaos.add_seed('example.com')
 ```
```

### Comparing `praetorian-cli-0.5.0/README.md` & `praetorian-cli-0.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 ## Developers
 
 Integrate the CLI into your own application:
 
 1. Include the dependency ``praetorian-cli`` in your project
 2. Import the Chaos class ``from praetorian_cli.sdk.chaos import Chaos``
-3. Import the Account class ``from praetorian_cli.sdk.account import Account``
+3. Import the Keychain class ``from praetorian_cli.sdk.keychain import Keychain``
 4. Call any function (example below)
 
 ### Example
 
 ```python
 from praetorian_cli.sdk.chaos import Chaos
-from praetorian_cli.sdk.account import Account
+from praetorian_cli.sdk.keychain import Keychain
 
-chaos = Chaos(Account(profile='United States'))
+chaos = Chaos(Keychain(profile='United States'))
 chaos.add_seed('example.com')
 ```
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/handlers/backend.py` & `praetorian-cli-0.7.1/praetorian_cli/handlers/backend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,120 @@
 import os
 import click
 
-from functools import wraps
-
-from praetorian_cli.sdk.chaos import Chaos
-
-
-def handle_api_error(func):
-    @wraps(func)
-    def handler(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except Exception as e:
-            click.secho(e.args[0], fg='red')
-    return handler
-
-
-@click.group()
-@click.pass_context
-def chaos(ctx):
-    """ Chaos API access """
-    ctx.obj = Chaos(account=ctx.obj)
+from utils import chaos
+from utils import handle_api_error
 
 
 @chaos.command('seeds')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_seeds(controller, seed):
     """ Fetch seed domains """
-    result = controller.my(dict(composite=f'#seed#{seed}'))
+    result = controller.my(dict(key=f'#seed#{seed}'))
     for hit in result.get('seeds', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('assets')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_assets(controller, seed):
     """ Fetch existing assets """
-    result = controller.my(dict(composite=f'#asset#{seed}'))
+    result = controller.my(dict(key=f'#asset#{seed}'))
     for hit in result.get('assets', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('risks')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_risks(controller, seed):
     """ Fetch current risks """
-    result = controller.my(dict(composite=f'#risk#{seed}'))
+    result = controller.my(dict(key=f'#risk#{seed}'))
     for hit in result.get('risks', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('jobs')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_jobs(controller, seed):
     """ Fetch past, present and future jobs """
-    result = controller.my(dict(composite=f'#job#{seed}'))
+    result = controller.my(dict(key=f'#job#{seed}'))
     for hit in result.get('jobs', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('services')
 @click.pass_obj
 @handle_api_error
 @click.option('-port', '--port', default="", help="Filter by port")
 def my_services(controller, port):
     """ Fetch recently seen services """
-    result = controller.my(dict(composite=f'#service#{port}'))
+    result = controller.my(dict(key=f'#service#{port}'))
     for hit in result.get('services', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('files')
 @click.pass_obj
 @handle_api_error
 @click.option('-key', '--key', default="", help="Filter by relative path")
 def my_files(controller, key):
     """ Fetch all file names """
-    result = controller.my(dict(composite=f'#file#{key}'))
+    result = controller.my(dict(key=f'#file#{key}'))
     for hit in result.get('files', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('threats')
 @click.pass_obj
 @handle_api_error
-@click.option('-source', '--source', type=click.Choice(['kev']), default="kev", help="Filter by threat source")
+@click.option('-source', '--source', type=click.Choice(['KEV']), default="KEV", help="Filter by threat source")
 def my_threats(controller, source):
     """ Fetch threat intelligence """
-    result = controller.my(dict(composite=f'#threat#{source}'))
+    result = controller.my(dict(key=f'#threat#{source}'))
     for hit in result.get('threats', []):
-        print(f"{hit['composite']}")
+        print(f"{hit['key']}")
 
 
 @chaos.command('add-seed')
 @click.pass_obj
 @handle_api_error
 @click.argument('seed')
-def add_seed(controller, seed):
+@click.option('-comment', '--comment', default="", help="Add a description")
+def add_seed(controller, seed, comment):
     """ Add a new seed domain """
-    controller.upsert_seed(seed, 0)
+    controller.upsert_seed(seed, status=0, comment=comment)
 
 
 @chaos.command('freeze-seed')
 @click.pass_obj
 @handle_api_error
 @click.argument('seed')
 def freeze_seed(controller, seed):
     """ Freeze a seed domain  """
     controller.upsert_seed(seed, 1)
 
 
 @chaos.command('add-risk')
 @click.pass_obj
 @handle_api_error
-@click.argument('composite')
+@click.argument('key')
 @click.option('-finding', '--finding', required=True, help="Generic risk identifier")
-@click.option('-status', '--status', type=click.IntRange(0, 3), required=False, help="Open (0) Closed (1) Rejected (2) Triaging (3)")
-@click.option('-severity', '--severity', type=click.IntRange(0, 4), required=False, help="Info (0) Low (1) Med (2) High (3) Material (4)")
+@click.option('-status', '--status', type=click.IntRange(0, 3), required=False, help="Open (0) Closed (1) Rejected (2) Triage (3)")
+@click.option('-severity', '--severity', type=click.IntRange(0, 4), required=False, help="Info (0) Med (1) High (2) Critical (3)")
 def add_risk(controller, composite, finding, status=0, severity=0):
-    """ Apply a risk to an asset composite """
-    print(controller.add_risk(composite, finding, status, severity))
+    """ Apply a risk to an asset key """
+    print(controller.add_risk(key, finding, status, severity))
 
 
 @chaos.command('upload')
 @click.pass_obj
 @handle_api_error
 @click.argument('name')
 def upload(controller, name):
@@ -145,23 +128,16 @@
 @click.argument('key')
 @click.argument('path')
 def download(controller, key, path):
     """ Download any previous uploaded file """
     controller.download(key, path)
 
 
-@chaos.command('trigger')
-@click.pass_obj
-@handle_api_error
-@click.argument('capability', type=click.Choice(['nmap', 'screenshot', 'nuclei', 'masscan', 'whois', 'subfinder']))
-@click.argument('composite')
-def trigger(controller, composite, capability):
-    """ Invoke a capability against an asset composite """
-    controller.trigger(capability, composite)
-
-
 @chaos.command('test')
 @click.pass_obj
 def trigger_all_tests(controller):
-    import pytest
+    try:
+        import pytest
+    except ModuleNotFoundError:
+        print("Install pytest using 'pip install pytest' to run this command")
     test_directory = os.path.relpath("praetorian_cli/sdk/test", os.getcwd())
     pytest.main([test_directory])
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/account.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/keychain.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,69 +7,73 @@
 from pathlib import Path
 
 
 def verify_credentials(func):
     @wraps(verify_credentials)
     def handler(*args, **kwargs):
         try:
-            account = args[0].account
-            keychain = account.keychain()
+            keychain = args[0].keychain
+            secrets = keychain.get()
 
-            account.api = keychain.get(account.profile, 'api')
-            account.client_id = keychain.get(account.profile, 'client_id')
-            account.username = keychain.get(account.profile, 'username', fallback=None)
-            account.password = keychain.get(account.profile, 'password', fallback=None)
-            if not (account.username and account.password):
-                new_credentials = account.write_credentials()
-                account.username = new_credentials['username']
-                account.password = new_credentials['password']
+            keychain.api = secrets.get(keychain.profile, 'api')
+            keychain.client_id = secrets.get(keychain.profile, 'client_id')
+            keychain.username = secrets.get(keychain.profile, 'username', fallback=None)
+            keychain.password = secrets.get(keychain.profile, 'password', fallback=None)
+            if not (keychain.username and keychain.password):
+                new_credentials = keychain.write_credentials()
+                keychain.username = new_credentials['username']
+                keychain.password = new_credentials['password']
 
-            account.headers = {
-                'Authorization': f'Bearer {account.token()}',
+            keychain.headers = {
+                'Authorization': f'Bearer {keychain.token()}',
                 'Content-Type': 'application/json'
             }
+            if keychain.account:
+                keychain.headers['Account'] = keychain.account
+
             return func(*args, **kwargs)
 
         except KeyError as e:
             raise Exception('Keychain missing: %s' % e)
         except StopIteration:
-            raise Exception('Could not find "%s" profile in %s' % (args[0].account.profile, args[0].account.keychain_location))
+            raise Exception('Could not find "%s" profile in %s' % (args[0].keychain.profile, args[0].keychain.location))
     handler.__wrapped__ = func
     return handler
 
 
-class Account:
+class Keychain:
 
-    def __init__(self, profile='United States', keychain_location=os.path.join(Path.home(), '.praetorian', 'keychain.ini')):
+    def __init__(self, profile='United States', account=None, location=os.path.join(Path.home(), '.praetorian', 'keychain.ini')):
         self.profile = profile
-        self.keychain_location = keychain_location
+        self.account = account
+        self.location = location
 
-    def keychain(self):
+    def get(self):
         cfg = configparser.ConfigParser()
-        cfg.read(self.keychain_location)
+        cfg.read(self.location)
         if not cfg.sections():
-            exit('[!] No keychain. Please visit research.praetorian.com.')
+            exit('[!] Visit chaos.praetorian.com to obtain a keychain')
         return cfg
 
     def write_credentials(self):
         username = input("Enter username: ")
         password = input("Enter password: ")
 
-        if not exists(self.keychain_location):
-            head, _ = os.path.split(Path(self.keychain_location))
+        if not exists(self.location):
+            head, _ = os.path.split(Path(self.location))
             Path(head).mkdir(parents=True, exist_ok=True)
-            open(self.keychain_location, 'x').close()
+            open(self.location, 'x').close()
 
         cfg = configparser.ConfigParser()
         cfg[self.profile] = {
             'username': username,
             'password': password
         }
         combo = self._merge_configs(cfg, self.keychain())
-        with open(self.keychain_location, 'w') as f:
+        with open(self.location, 'w') as f:
             combo.write(f)
         return {
             'username': username,
             'password': password
         }
 
     def token(self):
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/chaos.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/chaos.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 import os
 import boto3
 import requests
 
-from praetorian_cli.sdk.account import verify_credentials, Account
+from praetorian_cli.sdk.keychain import verify_credentials, Keychain
 
 
 class Chaos:
 
-    def __init__(self, account: Account):
-        self.account = account
+    def __init__(self, keychain: Keychain):
+        self.keychain = keychain
 
     @verify_credentials
     def my(self, params: dict) -> {}:
-        resp = requests.get(f"{self.account.api}/my", params=params, headers=self.account.headers)
+        resp = requests.get(f"{self.keychain.api}/my", params=params, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def trigger(self, capability: str, composite: str):
-        resp = requests.post(f"{self.account.api}/job/{capability}", json=dict(composite=composite), headers=self.account.headers)
+    def add_risk(self, key: str, finding: str, status: int = 0, severity: int = 0):
+        data = dict(key=key, finding=finding, status=status, severity=severity)
+
+        resp = requests.post(f"{self.keychain.api}/risk", json=data, headers=self.keychain.headers)
+        if not resp.ok:
+            raise Exception(f'[{resp.status_code}] Request failed')
+        return resp.json()
+
+    @verify_credentials
+    def upsert_seed(self, dns: str, status: int, comment: str = "") -> {}:
+        data = {"seed": dns, "status": status, "description": comment}
+
+        resp = requests.post(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def add_risk(self, composite: str, finding: str, status: int = 0, severity: int = 0):
-        data = dict(composite=composite, finding=finding, status=status, severity=severity)
-        resp = requests.post(f"{self.account.api}/risk", json=data, headers=self.account.headers)
+    def link_account(self, username: str, config: str):
+        resp = requests.post(f"{self.keychain.api}/account/{username}", json={'config':config}, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def upsert_seed(self, dns: str, status: int) -> {}:
-        resp = requests.post(f"{self.account.api}/seed", json={"seed": dns, "status": status}, headers=self.account.headers)
+    def unlink_account(self, username: str):
+        resp = requests.delete(f"{self.keychain.api}/account/{username}", headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
     def upload(self, name: str):
         with open(name, 'rb') as file:
-            resp = requests.put(f"{self.account.api}/file/{name}", data=file, allow_redirects=True, headers=self.account.headers)
+            resp = requests.put(f"{self.keychain.api}/file", params={"name": name}, data=file, allow_redirects=True, headers=self.keychain.headers)
             if not resp.ok:
                 raise Exception(f'[{resp.status_code}] Request failed')
 
     @verify_credentials
-    def download(self, key: str, download_path: str) -> bool:
+    def download(self, name: str, download_path: str) -> bool:
         directory = os.path.dirname(download_path)
         if directory and not os.path.exists(directory):
             os.makedirs(directory)
 
-        resp = requests.get(f"{self.account.api}/file/{key}", allow_redirects=True, headers=self.account.headers)
+        resp = requests.get(f"{self.keychain.api}/file", params={"name": name}, allow_redirects=True, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         with open(download_path, 'wb') as file:
             file.write(resp.content)
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_file_upload.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_file_upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,21 @@
         with open(self.file, 'w') as file:
             file.write(self.seed)
 
     def test_upload_file(self):
         self.chaos.upload(self.file)
 
     def test_my_file(self):
-        response = self.chaos.my(dict(composite=f'#file#{self.file}'))
+        response = self.chaos.my(dict(key=f'#file#{self.file}'))
         files = response['files']
 
         assert len(files) == 1
         assert files[0]['username'] == self.username
         assert files[0]['name'] == self.file
-        assert files[0]['composite'] == f"#file#{self.file}"
+        assert files[0]['key'] == f"#file#{self.file}"
 
     def test_download_file(self):
         self.chaos.download(self.file, self.downloaded_file)
         assert os.path.exists(self.file) is True
         utils.assert_files_equal(self.file, self.downloaded_file)
 
     def teardown_class(self):
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_job_capabilities.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_job_capabilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,53 +4,48 @@
 
 
 class TestJob(BaseTest):
 
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
         self.seed = "contoso.com"
-        self.capabilities = ['subfinder', 'whois', 'nmap', 'masscan', 'nuclei', 'screenshot']
+        self.capabilities = ['vulnerability', 'whois', 'subfinder', 'cidr', 'portscan', 'code', 'secrets']
         self.utils = Utils(self.chaos)
 
-    def test_trigger_job(self):
-        for capability in self.capabilities:
-            response = self.chaos.trigger(capability, composite=f'#seed#{self.seed}')
-            assert response is not None
-
     def test_my_jobs(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#job#{self.seed}'), 300, 60)
+        response = self.utils.key(dict(key=f'#job#{self.seed}'), 300, 60)
         assert response.get('jobs'), "Received empty response for my jobs"
 
         for my_job in response.get('jobs', []):
             print(my_job)
             assert my_job['username'] == self.username, "Job did not have username"
-            assert self.seed in my_job['composite'], "Job composite did not have required seed"
-            assert my_job['composite'].split('#')[
+            assert self.seed in my_job['key'], "Job key did not have required seed"
+            assert my_job['key'].split('#')[
                        -2] in self.capabilities, "Job capability is not in defined capabilities"
 
     def test_my_assets(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#asset#{self.seed}'), 40, 5)
+        response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'), 40, 5)
         assert response.get('assets'), "Received empty response for my assets"
 
         for my_asset in response.get('assets', []):
             assert my_asset['username'] == self.username, f"Job did not have username = {self.username}"
-            assert self.seed in my_asset['composite'], f"Asset composite did not have required seed = {self.seed}"
+            assert self.seed in my_asset['key'], f"Asset key did not have required seed = {self.seed}"
 
     def test_my_services(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#service#{self.seed}'), 180, 10)
+        response = self.utils.wait_for_key(dict(key=f'#service#{self.seed}'), 180, 10)
         assert response.get('services'), "Received empty response for my services"
 
         for my_service in response.get('services', []):
             assert my_service['username'] == self.username, f"Job did not have username = {self.username}"
-            assert self.seed in my_service['composite'], "Service composite does not have seed"
+            assert self.seed in my_service['key'], "Service key does not have seed"
 
     def test_my_risks(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#risk#{self.seed}'), 300, 30)
+        response = self.utils.wait_for_key(dict(key=f'#risk#{self.seed}'), 300, 30)
         assert response.get('risks'), "Received empty response for my risks"
 
         for my_risk in response.get('risks', []):
             assert my_risk['username'] == self.username, f"Job did not have username = {self.username}"
-            assert self.seed in my_risk['composite'], "Service composite does not have seed"
+            assert self.seed in my_risk['key'], "Service key does not have seed"
 
     def test_delete_seed(self):
         response = self.utils.freeze_seed(self.seed)
         assert response['seed'] == self.seed
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_nvd.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_nvd.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
 class TestNVD(BaseTest):
 
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
 
     def test_my_threats(self):
-        response = self.chaos.my(dict(composite=f'#threat'))
+        response = self.chaos.my(dict(key=f'#threat'))
         assert response is not None, "Received empty response for my Threats"
         assert len(response['threats']) > 1000, "Less than 1000 CVEs received"
 
         for my_threat in response.get('threats', []):
-            assert 'KEV' in my_threat['composite'], "Threat did not have required composite KEV"
-            assert 'CVE' in my_threat['composite'], "Threat did not have required composite CVE"
+            assert 'KEV' in my_threat['key'], "Threat did not have required KEV"
+            assert 'CVE' in my_threat['key'], "Threat did not have required CVE"
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/test/test_seed.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/test/test_seed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from praetorian_cli.sdk.test import BaseTest
 from praetorian_cli.sdk.test.utils import Utils
 
 
-@pytest.fixture(scope="class", params=["contoso.com", "1.1.1.1"])
+@pytest.fixture(scope="class", params=["contoso.com", "1.1.1.1/32"])
 def seed(request):
     request.cls.seed = request.param
 
 
 @pytest.mark.usefixtures("seed")
 class TestSeed(BaseTest):
 
@@ -18,28 +18,28 @@
 
     def test_add_seed(self):
         response = self.utils.add_seed(self.seed)
         assert response['seed'] == self.seed, "Response does not have correct seed"
         assert response['status'] is 0
 
     def test_my_seed(self):
-        response = self.chaos.my(dict(composite=f'#seed#{self.seed}'))
+        response = self.chaos.my(dict(key=f'#seed#{self.seed}'))
         for my_seed in response['seeds']:
             assert my_seed['username'] == self.username, f"Seed did not have username = {self.username}"
             assert my_seed['seed'] in self.seed
 
     def test_my_job(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#job#{self.seed}'))
+        response = self.utils.wait_for_key(dict(key=f'#job#{self.seed}'))
         assert response is not None, "Received empty response for my Jobs"
         for job in response['jobs']:
-            assert job['capability'] is not '', "Job Capability is empty"
+            assert job['name'] is not '', "Job Capability is empty"
             assert job['status'] is not None, "Job Status is empty"
 
     def test_my_asset(self):
-        response = self.utils.wait_for_composite(dict(composite=f'#asset#{self.seed}'))
+        response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'))
         assert response is not None, "Received empty response for my Assets"
         for asset in response['assets']:
             assert asset['seed'] == self.seed, "Seed is empty"
             assert asset['ip'] or asset['dns'], "Asset fields IP and DNS are both empty"
 
     def test_delete_seed(self):
         response = self.utils.freeze_seed(self.seed)
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli/sdk/test/utils.py` & `praetorian-cli-0.7.1/praetorian_cli/sdk/test/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
     assert content1 == content2, f"Contents of the files {file1_path} and {file2_path} file are not equal"
 
 class Utils:
     def __init__(self, chaos):
         self.chaos = chaos
 
-    def wait_for_composite(self, composite, timeout=60, interval=5):
+    def wait_for_key(self, key, timeout=60, interval=5):
         start_time = time.time()
         while time.time() - start_time < timeout:
-            print(f"Trying to get response for my {composite}")
-            response = self.chaos.my(composite)
+            print(f"Trying to get response for my {key}")
+            response = self.chaos.my(key)
             if response:
                 return response
             time.sleep(interval)
 
     def add_seed(self, seed):
         return self.chaos.upsert_seed(seed, 0)
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli.egg-info/PKG-INFO` & `praetorian-cli-0.7.1/praetorian_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.5.0
+Version: 0.7.1
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,19 +47,19 @@
 
 ## Developers
 
 Integrate the CLI into your own application:
 
 1. Include the dependency ``praetorian-cli`` in your project
 2. Import the Chaos class ``from praetorian_cli.sdk.chaos import Chaos``
-3. Import the Account class ``from praetorian_cli.sdk.account import Account``
+3. Import the Keychain class ``from praetorian_cli.sdk.keychain import Keychain``
 4. Call any function (example below)
 
 ### Example
 
 ```python
 from praetorian_cli.sdk.chaos import Chaos
-from praetorian_cli.sdk.account import Account
+from praetorian_cli.sdk.keychain import Keychain
 
-chaos = Chaos(Account(profile='United States'))
+chaos = Chaos(Keychain(profile='United States'))
 chaos.add_seed('example.com')
 ```
```

### Comparing `praetorian-cli-0.5.0/praetorian_cli.egg-info/SOURCES.txt` & `praetorian-cli-0.7.1/praetorian_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 praetorian_cli.egg-info/PKG-INFO
 praetorian_cli.egg-info/SOURCES.txt
 praetorian_cli.egg-info/dependency_links.txt
 praetorian_cli.egg-info/entry_points.txt
 praetorian_cli.egg-info/requires.txt
 praetorian_cli.egg-info/top_level.txt
 praetorian_cli/handlers/__init__.py
+praetorian_cli/handlers/account.py
 praetorian_cli/handlers/backend.py
+praetorian_cli/handlers/utils.py
 praetorian_cli/sdk/__init__.py
-praetorian_cli/sdk/account.py
 praetorian_cli/sdk/chaos.py
+praetorian_cli/sdk/keychain.py
 praetorian_cli/sdk/test/__init__.py
 praetorian_cli/sdk/test/test_file_upload.py
 praetorian_cli/sdk/test/test_job_capabilities.py
+praetorian_cli/sdk/test/test_link_account.py
 praetorian_cli/sdk/test/test_manual_risk.py
 praetorian_cli/sdk/test/test_nvd.py
 praetorian_cli/sdk/test/test_seed.py
 praetorian_cli/sdk/test/utils.py
```

### Comparing `praetorian-cli-0.5.0/setup.cfg` & `praetorian-cli-0.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = praetorian-cli
-version = 0.5.0
+version = 0.7.1
 author = Praetorian Labs
 author_email = research@praetorian.com
 description = For interacting with the Chaos API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/praetorian-inc/praetorian-cli
 classifiers =
```

