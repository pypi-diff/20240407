# Comparing `tmp/docker_remote_sync-0.5.0.tar.gz` & `tmp/docker_remote_sync-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_remote_sync-0.5.0.tar", max compression
+gzip compressed data, was "docker_remote_sync-0.5.1.tar", max compression
```

## Comparing `docker_remote_sync-0.5.0.tar` & `docker_remote_sync-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/LICENSE
--rw-r--r--   0        0        0     1272 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/Readme.md
--rw-r--r--   0        0        0        0 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/drsync/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/__main__.py
--rw-r--r--   0        0        0       13 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/config.py
--rw-r--r--   0        0        0      462 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/docker_interface.py
--rw-r--r--   0        0        0      230 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/io_util.py
--rw-r--r--   0        0        0      549 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/remote.py
--rw-r--r--   0        0        0      639 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/subprocess_utils.py
--rw-r--r--   0        0        0     2615 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/sync.py
--rw-r--r--   0        0        0      641 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 docker_remote_sync-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1272 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/__main__.py
+-rw-r--r--   0        0        0       13 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/config.py
+-rw-r--r--   0        0        0      434 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/docker_interface.py
+-rw-r--r--   0        0        0      230 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/io_util.py
+-rw-r--r--   0        0        0      549 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/remote.py
+-rw-r--r--   0        0        0      639 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/subprocess_utils.py
+-rw-r--r--   0        0        0     2766 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/drsync/sync.py
+-rw-r--r--   0        0        0      641 2024-04-07 15:02:24.155171 docker_remote_sync-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 docker_remote_sync-0.5.1/PKG-INFO
```

### Comparing `docker_remote_sync-0.5.0/LICENSE` & `docker_remote_sync-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.0/Readme.md` & `docker_remote_sync-0.5.1/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.0/drsync/__main__.py` & `docker_remote_sync-0.5.1/drsync/__main__.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.0/drsync/remote.py` & `docker_remote_sync-0.5.1/drsync/remote.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.0/drsync/subprocess_utils.py` & `docker_remote_sync-0.5.1/drsync/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.5.0/drsync/sync.py` & `docker_remote_sync-0.5.1/drsync/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,34 @@
 ):
     print_header("Syncing local changes with remote")
     rsync_executable = "rsync"
     ssh_cmd_with_port = ()
     if port is not None:
         additional_ssh_args = f"{additional_ssh_args} -p {port}"
     if additional_ssh_args is not None:
-        ssh_cmd_with_port = ("-e", f"'ssh {additional_ssh_args}'")
+        ssh_cmd_with_port = ("-e", f"ssh {additional_ssh_args}")
+        print(ssh_cmd_with_port)
     try:
         process = start_subprocess(
             rsync_executable,
             "--delete",
             "--archive",
             "--ignore-times",
             "--recursive",
             "--verbose",
             *ssh_cmd_with_port,
             f"{source_folder}/",
             f"{remote}:{remote_folder}",
             output="print",
         )
         process.wait()
-        check_subprocess_errors(process.stderr.readlines())
+        if process.stderr is not None:
+            check_subprocess_errors(process.stderr.readlines())
+        if process.returncode != 0:
+            sys.exit(process.returncode)
     except FileNotFoundError as e:
         if e.filename == rsync_executable:
             print(f"Could not find {rsync_executable} executable", file=sys.stderr)
             sys.exit(1)
         else:
             raise e
```

### Comparing `docker_remote_sync-0.5.0/pyproject.toml` & `docker_remote_sync-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-remote-sync"
-version = "0.5.0"
+version = "0.5.1"
 description = "Utility to sync updated docker layers between 2 docker host machines"
 authors = ["Vamsi Talupula <tanavamsikrishna@outlook.com>"]
 readme = "Readme.md"
 repository = "https://github.com/tanavamsikrishna/docker-remote-sync"
 packages = [{ include = "drsync" }]
 
 [tool.poetry.dependencies]
```

### Comparing `docker_remote_sync-0.5.0/PKG-INFO` & `docker_remote_sync-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-remote-sync
-Version: 0.5.0
+Version: 0.5.1
 Summary: Utility to sync updated docker layers between 2 docker host machines
 Home-page: https://github.com/tanavamsikrishna/docker-remote-sync
 Author: Vamsi Talupula
 Author-email: tanavamsikrishna@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

