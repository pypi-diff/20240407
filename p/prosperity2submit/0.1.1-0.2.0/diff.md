# Comparing `tmp/prosperity2submit-0.1.1.tar.gz` & `tmp/prosperity2submit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.1.1.tar", last modified: Sun Apr  7 01:01:25 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.0.tar", last modified: Sun Apr  7 15:36:19 2024, max compression
```

## Comparing `prosperity2submit-0.1.1.tar` & `prosperity2submit-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 01:01:23.000000 prosperity2submit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 15:36:16.000000 prosperity2submit-0.2.0/prosperity2submit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 15:36:19.000000 prosperity2submit-0.2.0/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 15:36:17.000000 prosperity2submit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:36:19.891889 prosperity2submit-0.2.0/setup.cfg
```

### Comparing `prosperity2submit-0.1.1/LICENSE` & `prosperity2submit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.1/PKG-INFO` & `prosperity2submit-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.1.1
+Version: 0.2.0
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.1.1/README.md` & `prosperity2submit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.1/prosperity2submit/core.py` & `prosperity2submit-0.2.0/prosperity2submit/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import keyring
 import requests
 import time
 import webbrowser
 from collections import defaultdict
-from datetime import datetime, timezone
 from functools import partial
-from getpass import getpass
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 from pathlib import Path
 from requests_toolbelt import MultipartEncoder
 from typing import Any, Optional
 
 KEYRING_SERVICE = "prosperity2submit"
 KEYRING_USERNAME = "prosperity-id-token"
@@ -21,91 +19,83 @@
 prosperity2submit needs your Prosperity ID token to make authenticated requests to Prosperity's internal API.
 Your token is stored in the local storage item with the `CognitoIdentityServiceProvider.<some id>.<email>.idToken` key on the Prosperity website.
 You can inspect the local storage items of a website by having the website open in the active tab, pressing F12 to open the browser's developer tools, and going to the Application (Chrome) or Storage (Firefox) tab.
 From there, click on Local Storage in the sidebar and select the website that appears underneath the sidebar entry.
 Your token is stored in your system's credentials store for convenience.
     """.strip())
 
-    token = getpass("Prosperity ID token: ")
+    token = input("Prosperity ID token: ")
     keyring.set_password(KEYRING_SERVICE, KEYRING_USERNAME, token)
 
-def request_with_token(*args, **kwargs) -> requests.Response:
+def request_with_token(method: str, url: str, form_data: Optional[dict[str, Any]] = None) -> requests.Response:
     token = keyring.get_password(KEYRING_SERVICE, KEYRING_USERNAME)
     if token is None:
         refresh_token()
-        return request_with_token(*args, **kwargs)
+        return request_with_token(method, url, form_data)
 
-    headers = kwargs.get("headers", {})
-    headers["Authorization"] = f"Bearer {token}"
-    kwargs["headers"] = headers
+    data = None
+    headers = {"Authorization": f"Bearer {token}"}
 
-    response = requests.request(*args, **kwargs)
+    if form_data is not None:
+        encoder = MultipartEncoder(form_data)
+        data = encoder
+        headers["content-type"] = encoder.content_type
+
+    response = requests.request(method, url, data=data, headers=headers)
 
     if response.status_code == 403:
         refresh_token()
-        return request_with_token(*args, **kwargs)
+        return request_with_token(method, url, form_data)
+
+    if response.status_code in [500, 504]:
+        print(f"Received unexpected HTTP {response.status_code} response from the Prosperity API, retrying request")
+        return request_with_token(method, url, form_data)
 
     response.raise_for_status()
     return response
 
 def format_path(path: Path) -> str:
     cwd = Path.cwd()
     if path.is_relative_to(cwd):
         return str(path.relative_to(cwd))
     else:
         return str(path)
 
-def submit_algorithm(algorithm_file: Path) -> None:
-    print(f"Submitting {format_path(algorithm_file)}")
-
-    with algorithm_file.open("rb") as file:
-        form = MultipartEncoder({"file": (algorithm_file.name, file, "text/x-python")})
+def get_current_round() -> str:
+    print("Retrieving current round")
+    rounds = request_with_token("GET", f"{API_BASE_URL}/game/rounds").json()
 
-        request_with_token(
-            "POST",
-            f"{API_BASE_URL}/submission/algo",
-            data=form,
-            headers={"content-type": form.content_type},
-        )
+    open_round = next((r for r in rounds if r["isOpen"]), None)
+    if open_round is None:
+        raise ValueError("No round is currently accepting submissions")
 
-def get_current_round() -> str:
-    round_open_timestamps = [
-        "2024-02-12T09:00:00.000",
-        "2024-04-08T09:00:00.000",
-        "2024-04-11T09:00:00.000",
-        "2024-04-14T09:00:00.000",
-        "2024-04-17T09:00:00.000",
-        "2024-04-20T09:00:00.000",
-    ]
-
-    now = datetime.now(timezone.utc)
-
-    for i, timestamp in enumerate(round_open_timestamps):
-        parsed = datetime.fromisoformat(timestamp).replace(tzinfo=timezone.utc)
-        if now >= parsed:
-            return f"ROUND{i}"
+    return open_round["id"]
 
-    raise ValueError("Could not determine current round")
+def submit_algorithm(algorithm_file: Path) -> None:
+    print(f"Submitting {format_path(algorithm_file)}")
+    request_with_token(
+        "POST",
+        f"{API_BASE_URL}/submission/algo",
+        {"file": (algorithm_file.name, algorithm_file.read_bytes(), "text/x-python")},
+    )
 
 def list_algorithms(round: str) -> list[dict[str, Any]]:
     return request_with_token("GET", f"{API_BASE_URL}/submission/algo/{round}").json()
 
 def get_submission_status(data: dict[str, Any]) -> str:
     status = data["status"]
 
     if data["selectedForRound"]:
         status += " (active)"
 
     return status
 
-def monitor_status(algorithm_file: Path) -> dict[str, Any]:
+def monitor_status(round: str, algorithm_file: Path) -> dict[str, Any]:
     print("Monitoring submission status")
 
-    round = get_current_round()
-
     algorithms = list_algorithms(round)
     data = next(a for a in algorithms if a["fileName"] == algorithm_file.name)
 
     status = get_submission_status(data)
     print(f"Submission status: {status}")
 
     while data["status"] != "FINISHED" and data["status"] != "ERROR":
@@ -165,16 +155,18 @@
     http_server = HTTPServer(("localhost", 0), http_handler)
 
     webbrowser.open(f"https://jmerle.github.io/imc-prosperity-2-visualizer/?open=http://localhost:{http_server.server_port}/{output_file.name}")
     http_server.handle_request()
     http_server.handle_request()
 
 def submit(algorithm_file: Path, output_file: Optional[Path], open_visualizer: bool) -> None:
+    round = get_current_round()
+
     submit_algorithm(algorithm_file)
-    data = monitor_status(algorithm_file)
+    data = monitor_status(round, algorithm_file)
 
     if output_file is not None:
         download_logs(data, output_file)
 
         if data["status"] == "FINISHED":
             log_profit_loss(output_file)
```

### Comparing `prosperity2submit-0.1.1/prosperity2submit/main.py` & `prosperity2submit-0.2.0/prosperity2submit/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.1/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.0/prosperity2submit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.1.1
+Version: 0.2.0
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.1.1/pyproject.toml` & `prosperity2submit-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

