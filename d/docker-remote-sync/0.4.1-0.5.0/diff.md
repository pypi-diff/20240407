# Comparing `tmp/docker_remote_sync-0.4.1.tar.gz` & `tmp/docker_remote_sync-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_remote_sync-0.4.1.tar", max compression
+gzip compressed data, was "docker_remote_sync-0.5.0.tar", max compression
```

## Comparing `docker_remote_sync-0.4.1.tar` & `docker_remote_sync-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/LICENSE
--rw-r--r--   0        0        0     1272 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/Readme.md
--rw-r--r--   0        0        0        0 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/__init__.py
--rw-r--r--   0        0        0     2233 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/__main__.py
--rw-r--r--   0        0        0       13 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/config.py
--rw-r--r--   0        0        0      462 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/docker_interface.py
--rw-r--r--   0        0        0      230 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/io_util.py
--rw-r--r--   0        0        0      549 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/remote.py
--rw-r--r--   0        0        0      639 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/subprocess_utils.py
--rw-r--r--   0        0        0     2421 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/drsync/sync.py
--rw-r--r--   0        0        0      641 2024-01-20 08:02:21.866360 docker_remote_sync-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 docker_remote_sync-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1272 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-07 14:01:28.161317 docker_remote_sync-0.5.0/drsync/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/__main__.py
+-rw-r--r--   0        0        0       13 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/config.py
+-rw-r--r--   0        0        0      462 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/docker_interface.py
+-rw-r--r--   0        0        0      230 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/io_util.py
+-rw-r--r--   0        0        0      549 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/remote.py
+-rw-r--r--   0        0        0      639 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/subprocess_utils.py
+-rw-r--r--   0        0        0     2615 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/drsync/sync.py
+-rw-r--r--   0        0        0      641 2024-04-07 14:01:28.165317 docker_remote_sync-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 docker_remote_sync-0.5.0/PKG-INFO
```

### Comparing `docker_remote_sync-0.4.1/LICENSE` & `docker_remote_sync-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.4.1/Readme.md` & `docker_remote_sync-0.5.0/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.4.1/drsync/__main__.py` & `docker_remote_sync-0.5.0/drsync/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,43 +19,54 @@
         description="Utility to sync updated docker layers between two docker host machines",
         epilog="""
 ○ Do not delete the cache folder on the remote machine to be able to take advantage of incremental file sync
 ○ Example usage: `docker-remote-sync alpine:latest remotehost "~/my_alpine_cache"`
 """,
         formatter_class=argparse.RawTextHelpFormatter,
     )
-    parser.add_argument(
-        "image_name", help="Docker image on local machine"
-    )
+    parser.add_argument("image_name", help="Docker image on local machine")
     parser.add_argument("remote", help="Address of remote")
     parser.add_argument("--port", help="Alternate ssh port on remote", required=False)
     parser.add_argument("remote_cache_folder", help="Cache folder on remote")
     parser.add_argument(
         "--docker-cmd",
         help="Alternate docker command. Defaults to `docker`. Eg. `colima x - docker` or `podman`",
         default="docker",
         required=False,
     )
+    parser.add_argument(
+        "--additional-ssh-args",
+        help="Additional ssh arguments enclosed in quotes",
+        required=False,
+    )
     return parser.parse_args()
 
 
 def main():
     args = parse_arguments()
     with TemporaryDirectory() as temp_extraction_folder, io.BytesIO() as temp_tar_file:
         remote = args.remote
         port = args.port
         image_name = args.image_name
         remote_cache_folder = args.remote_cache_folder
         docker_cmd = args.docker_cmd
+        additional_ssh_args = args.additional_ssh_args
+
         save_docker_image(docker_cmd, image_name, temp_tar_file)
         temp_tar_file.seek(0)
         extract_tar_file(temp_tar_file, temp_extraction_folder)
         rce = functools.partial(run_cmd_on_remote, conn=get_remote_conn(remote, port))
 
         create_remote_folder(remote_cache_folder, rce)
-        sync_folders(temp_extraction_folder, remote, port, remote_cache_folder)
+        sync_folders(
+            temp_extraction_folder,
+            remote,
+            port,
+            remote_cache_folder,
+            additional_ssh_args,
+        )
         remote_image_file = build_remote_tar(rce, remote_cache_folder)
         load_image_on_remote(rce, remote_image_file, image_name)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `docker_remote_sync-0.4.1/drsync/remote.py` & `docker_remote_sync-0.5.0/drsync/remote.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.4.1/drsync/subprocess_utils.py` & `docker_remote_sync-0.5.0/drsync/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `docker_remote_sync-0.4.1/drsync/sync.py` & `docker_remote_sync-0.5.0/drsync/sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import re
 import sys
 import tarfile
-from typing import Callable
+from typing import Callable, Optional
 
 from drsync.io_util import print_error, print_header
 from drsync.subprocess_utils import check_subprocess_errors, start_subprocess
 
 
-def sync_folders(source_folder: str, remote: str, port: int | None, remote_folder: str):
+def sync_folders(
+    source_folder: str,
+    remote: str,
+    port: int | None,
+    remote_folder: str,
+    additional_ssh_args: Optional[str] = None,
+):
     print_header("Syncing local changes with remote")
     rsync_executable = "rsync"
     ssh_cmd_with_port = ()
     if port is not None:
-        ssh_cmd_with_port = ("-e", f"'ssh -p {port}'")
+        additional_ssh_args = f"{additional_ssh_args} -p {port}"
+    if additional_ssh_args is not None:
+        ssh_cmd_with_port = ("-e", f"'ssh {additional_ssh_args}'")
     try:
         process = start_subprocess(
             rsync_executable,
             "--delete",
             "--archive",
             "--ignore-times",
             "--recursive",
@@ -64,8 +72,8 @@
         output = rce(f"docker tag {image_sha256} {image_name}")
         print(output)
     elif len(matches := re.findall(".*Loaded image: (.*)", output)) > 0:
         output = rce(f"docker tag {matches[0]} {image_name}")
         print(output)
     else:
         print_error(f"Unexpected output from docker load command execution\n{output}")
-        sys.exit(1)
+        sys.exit(1)
```

### Comparing `docker_remote_sync-0.4.1/pyproject.toml` & `docker_remote_sync-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-remote-sync"
-version = "0.4.1"
+version = "0.5.0"
 description = "Utility to sync updated docker layers between 2 docker host machines"
 authors = ["Vamsi Talupula <tanavamsikrishna@outlook.com>"]
 readme = "Readme.md"
 repository = "https://github.com/tanavamsikrishna/docker-remote-sync"
 packages = [{ include = "drsync" }]
 
 [tool.poetry.dependencies]
```

### Comparing `docker_remote_sync-0.4.1/PKG-INFO` & `docker_remote_sync-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-remote-sync
-Version: 0.4.1
+Version: 0.5.0
 Summary: Utility to sync updated docker layers between 2 docker host machines
 Home-page: https://github.com/tanavamsikrishna/docker-remote-sync
 Author: Vamsi Talupula
 Author-email: tanavamsikrishna@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

