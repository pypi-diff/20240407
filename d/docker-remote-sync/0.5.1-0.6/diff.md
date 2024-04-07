# Comparing `tmp/docker_remote_sync-0.5.1.tar.gz` & `tmp/docker_remote_sync-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_remote_sync-0.5.1.tar", max compression
+gzip compressed data, was "docker_remote_sync-0.6.tar", max compression
```

## Comparing `docker_remote_sync-0.5.1.tar` & `docker_remote_sync-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/LICENSE
--rw-r--r--   0        0        0     1272 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/Readme.md
--rw-r--r--   0        0        0        0 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/__main__.py
--rw-r--r--   0        0        0       13 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/config.py
--rw-r--r--   0        0        0      434 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/docker_interface.py
--rw-r--r--   0        0        0      230 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/io_util.py
--rw-r--r--   0        0        0      549 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/remote.py
--rw-r--r--   0        0        0      639 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/subprocess_utils.py
--rw-r--r--   0        0        0     2766 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/sync.py
--rw-r--r--   0        0        0      641 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 docker_remote_sync-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/LICENSE
+-rw-r--r--   0        0        0     1272 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/__main__.py
+-rw-r--r--   0        0        0       13 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/config.py
+-rw-r--r--   0        0        0      434 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/docker_interface.py
+-rw-r--r--   0        0        0      230 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/io_util.py
+-rw-r--r--   0        0        0      548 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/remote.py
+-rw-r--r--   0        0        0      639 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/subprocess_utils.py
+-rw-r--r--   0        0        0     2733 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/drsync/sync.py
+-rw-r--r--   0        0        0      592 2024-04-07 15:15:16.332057 docker_remote_sync-0.6/pyproject.toml
+-rw-r--r--   0        0        0     1989 1970-01-01 00:00:00.000000 docker_remote_sync-0.6/PKG-INFO
```

### Comparing `docker_remote_sync-0.5.1/LICENSE` & `docker_remote_sync-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.1/Readme.md` & `docker_remote_sync-0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.1/drsync/__main__.py` & `docker_remote_sync-0.6/drsync/__main__.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.1/drsync/remote.py` & `docker_remote_sync-0.6/drsync/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     try:
         output: Result = conn.run(cmd)
         return output.stdout
     except invoke.exceptions.UnexpectedExit:
         sys.exit(1)
 
 
-def create_remote_folder(folder: str, rce: Callable[[str], None]):
+def create_remote_folder(folder: str, rce: Callable[[str], str]):
     return rce(f"mkdir -p {folder}")
```

### Comparing `docker_remote_sync-0.5.1/drsync/subprocess_utils.py` & `docker_remote_sync-0.6/drsync/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.1/drsync/sync.py` & `docker_remote_sync-0.6/drsync/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     print_header("Syncing local changes with remote")
     rsync_executable = "rsync"
     ssh_cmd_with_port = ()
     if port is not None:
         additional_ssh_args = f"{additional_ssh_args} -p {port}"
     if additional_ssh_args is not None:
         ssh_cmd_with_port = ("-e", f"ssh {additional_ssh_args}")
-        print(ssh_cmd_with_port)
     try:
         process = start_subprocess(
             rsync_executable,
             "--delete",
             "--archive",
             "--ignore-times",
             "--recursive",
```

### Comparing `docker_remote_sync-0.5.1/pyproject.toml` & `docker_remote_sync-0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "docker-remote-sync"
-version = "0.5.1"
+version = "0.6"
 description = "Utility to sync updated docker layers between 2 docker host machines"
 authors = ["Vamsi Talupula <tanavamsikrishna@outlook.com>"]
 readme = "Readme.md"
 repository = "https://github.com/tanavamsikrishna/docker-remote-sync"
 packages = [{ include = "drsync" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-colorama = "^0.4.6"
-fabric = "^3.2.2"
+colorama = "*"
+fabric = "*"
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^3.0.2"
-black = "^23.10.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 docker-remote-sync = "drsync.__main__:main"
```

### Comparing `docker_remote_sync-0.5.1/PKG-INFO` & `docker_remote_sync-0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: docker-remote-sync
-Version: 0.5.1
+Version: 0.6
 Summary: Utility to sync updated docker layers between 2 docker host machines
 Home-page: https://github.com/tanavamsikrishna/docker-remote-sync
 Author: Vamsi Talupula
 Author-email: tanavamsikrishna@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: fabric (>=3.2.2,<4.0.0)
+Requires-Dist: colorama
+Requires-Dist: fabric
 Project-URL: Repository, https://github.com/tanavamsikrishna/docker-remote-sync
 Description-Content-Type: text/markdown
 
 A utility to sync docker images between two machines while transferring only the changed layers
 
 # Setup
 ### Requirements
```

