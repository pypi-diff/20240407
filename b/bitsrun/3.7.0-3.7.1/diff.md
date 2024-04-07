# Comparing `tmp/bitsrun-3.7.0.tar.gz` & `tmp/bitsrun-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitsrun-3.7.0.tar", last modified: Wed Nov 29 04:01:21 2023, max compression
+gzip compressed data, was "bitsrun-3.7.1.tar", last modified: Sun Apr  7 06:40:13 2024, max compression
```

## Comparing `bitsrun-3.7.0.tar` & `bitsrun-3.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:01:21.968379 bitsrun-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-29 04:01:03.000000 bitsrun-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-11-29 04:01:21.968379 bitsrun-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2023-11-29 04:01:03.000000 bitsrun-3.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-11-29 04:01:03.000000 bitsrun-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 04:01:21.968379 bitsrun-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:01:21.964379 bitsrun-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:01:21.964379 bitsrun-3.7.0/src/bitsrun/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-11-29 04:01:03.000000 bitsrun-3.7.0/src/bitsrun/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 04:01:21.964379 bitsrun-3.7.0/src/bitsrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-29 04:01:21.000000 bitsrun-3.7.0/src/bitsrun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:40:13.795425 bitsrun-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 06:40:02.000000 bitsrun-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-07 06:40:13.795425 bitsrun-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-07 06:40:02.000000 bitsrun-3.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-07 06:40:02.000000 bitsrun-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:40:13.795425 bitsrun-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:40:13.791425 bitsrun-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:40:13.791425 bitsrun-3.7.1/src/bitsrun/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-07 06:40:02.000000 bitsrun-3.7.1/src/bitsrun/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:40:13.791425 bitsrun-3.7.1/src/bitsrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 06:40:13.000000 bitsrun-3.7.1/src/bitsrun.egg-info/top_level.txt
```

### Comparing `bitsrun-3.7.0/PKG-INFO` & `bitsrun-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsrun
-Version: 3.7.0
+Version: 3.7.1
 Summary: A headless login / logout script for 10.0.0.55
 Author-email: spencerwooo <spencer.woo@outlook.com>
 License: WTFPL
 Project-URL: homepage, https://github.com/BITNP/bitsrun
 Keywords: bit,srun,srun-login,srun-client,beijing-institute-of-technology
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: rich>=13.3.5
```

### Comparing `bitsrun-3.7.0/README.md` & `bitsrun-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bitsrun-3.7.0/pyproject.toml` & `bitsrun-3.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bitsrun"
-version = "3.7.0"
+version = "3.7.1"
 description = "A headless login / logout script for 10.0.0.55"
 authors = [{ name = "spencerwooo", email = "spencer.woo@outlook.com" }]
 dependencies = [
     "httpx>=0.24.0",
     "rich>=13.3.5",
     "humanize>=4.5.0",
     "click>=8.1.3",
@@ -23,14 +23,15 @@
     "Intended Audience :: Information Technology",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Education",
     "Topic :: Internet",
 ]
 
 [project.urls]
 homepage = "https://github.com/BITNP/bitsrun"
 
@@ -39,14 +40,16 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.ruff]
 line-length = 88
+
+[tool.ruff.lint]
 select = ["E", "F", "I", "N", "B", "SIM"]
 
 [tool.ruff.format]
 # Use single quotes rather than double quotes.
 quote-style = "single"
 
 [tool.mypy]
```

### Comparing `bitsrun-3.7.0/src/bitsrun/cli.py` & `bitsrun-3.7.1/src/bitsrun/cli.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.7.0/src/bitsrun/config.py` & `bitsrun-3.7.1/src/bitsrun/config.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.7.0/src/bitsrun/models.py` & `bitsrun-3.7.1/src/bitsrun/models.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.7.0/src/bitsrun/user.py` & `bitsrun-3.7.1/src/bitsrun/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,25 @@
     def __init__(self, username: str, password: str):
         self.username = username
         self.password = password
 
         # Initialize reused httpx client
         self.client = httpx.Client(base_url=_API_BASE)
 
-        # Get `ac_id` from the redirected login page
+        # Visit another site using HTTP, and let srun redirect to 10.0.0.55
+        # with url params (ac_id, theme, wlanuserip, etc.)
+        # but better to check since the user may have been authenticated
         resp = self.client.get('/', follow_redirects=True)
-        self.acid = resp.url.params.get('ac_id')
+        resp_valid = httpx.Client(base_url='http://www.bit.edu.cn').get(
+            '/', follow_redirects=True
+        )
+        if resp_valid.url.params.get('ac_id') is None:
+            self.acid = resp.url.params.get('ac_id')
+        else:
+            self.acid = resp_valid.url.params.get('ac_id')
 
         # Check current login status and get device `online_ip`
         login_status = get_login_status(client=self.client)
         self.ip = login_status.get('online_ip')
         self.logged_in_user = login_status.get('user_name')
 
         # Validate if current logged in user matches the provided username
```

### Comparing `bitsrun-3.7.0/src/bitsrun/utils.py` & `bitsrun-3.7.1/src/bitsrun/utils.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.7.0/src/bitsrun.egg-info/PKG-INFO` & `bitsrun-3.7.1/src/bitsrun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsrun
-Version: 3.7.0
+Version: 3.7.1
 Summary: A headless login / logout script for 10.0.0.55
 Author-email: spencerwooo <spencer.woo@outlook.com>
 License: WTFPL
 Project-URL: homepage, https://github.com/BITNP/bitsrun
 Keywords: bit,srun,srun-login,srun-client,beijing-institute-of-technology
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: rich>=13.3.5
```

