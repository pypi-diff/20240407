# Comparing `tmp/ggun-0.0.3-py3-none-any.whl.zip` & `tmp/ggun-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9052 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       23 b- defN 24-Mar-31 13:35 ggun/__init__.py
--rw-rw-r--  2.0 unx     5419 b- defN 24-Mar-31 13:35 ggun/main.py
+Zip file size: 9515 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       23 b- defN 24-Apr-05 13:04 ggun/__init__.py
+-rw-rw-r--  2.0 unx     5578 b- defN 24-Apr-07 15:01 ggun/main.py
 -rw-rw-r--  2.0 unx       20 b- defN 24-Mar-31 13:47 ggun/commands/__init__.py
--rw-rw-r--  2.0 unx    14277 b- defN 24-Mar-31 20:49 ggun/commands/test.py
+-rw-rw-r--  2.0 unx    14337 b- defN 24-Apr-07 15:13 ggun/commands/test.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 13:35 utils/__init__.py
--rw-rw-r--  2.0 unx     1577 b- defN 24-Apr-02 13:45 utils/api_call.py
--rw-rw-r--  2.0 unx     2261 b- defN 24-Mar-31 13:35 utils/list_files.py
--rw-rw-r--  2.0 unx      241 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       35 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      897 b- defN 24-Apr-02 13:46 ggun-0.0.3.dist-info/RECORD
-12 files, 24853 bytes uncompressed, 7558 bytes compressed:  69.6%
+-rw-rw-r--  2.0 unx     1480 b- defN 24-Apr-07 15:01 utils/api_call.py
+-rw-rw-r--  2.0 unx     3315 b- defN 24-Apr-07 15:13 utils/list_files.py
+-rw-rw-r--  2.0 unx      231 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       35 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      897 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/RECORD
+12 files, 26019 bytes uncompressed, 8021 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: utils/api_call.py
 Comment: 
 
 Filename: utils/list_files.py
 Comment: 
 
-Filename: ggun-0.0.3.dist-info/METADATA
+Filename: ggun-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: ggun-0.0.3.dist-info/WHEEL
+Filename: ggun-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ggun-0.0.3.dist-info/entry_points.txt
+Filename: ggun-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ggun-0.0.3.dist-info/top_level.txt
+Filename: ggun-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ggun-0.0.3.dist-info/RECORD
+Filename: ggun-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ggun/main.py

```diff
@@ -16,16 +16,15 @@
         return parts
 
 
 def ggun():
     """Main function for the CLI tool."""
     parser = argparse.ArgumentParser(
         prog="ggun",
-        description="Ggun CLI tool for smart contract management"
-        " and development.",
+        description="Ggun CLI tool for smart contract management" " and development.",
         formatter_class=CustomFormatter,
     )
     parser.add_argument("-V", "--version", action="version", version="%(prog)s 1.0")
     subparsers = parser.add_subparsers(
         dest="command", help="Commands", metavar="COMMAND"
     )
     # Commands
@@ -135,10 +134,13 @@
             "\nhttp://book.getfoundry.sh/reference/forge/forge.html"
         )
         print(info_msg)
         sys.exit(1)
 
     print(f"Executing command: {args.command}")
 
+    # Most commands are currently unimplemented, if we get to this part it is definitely unimplemented
+    print(f"Command not implemented yet: ggun {args.command}")
+
 
 if __name__ == "__main__":
     ggun()
```

## ggun/commands/test.py

```diff
@@ -1,24 +1,24 @@
 import argparse
 from utils.api_call import api_call
-from utils.list_files import list_git_files
+from utils.list_files import list_git_files, list_forge_test_strace_files
 import os
 
 
-def test(current_directory, *args):
+def test(current_directory, *args: argparse.Namespace):
     """
     Executes the test command by preparing and uploading files located in the
     current directory to the API for fuzzing.
 
     Args:
         current_directory (str): The directory from which files will be listed
         and prepared for upload.
         *args: Variable length argument list to capture additional arguments passed to the command.
     """
-    git_tracked_files = list_git_files(
+    git_tracked_files = list_forge_test_strace_files(
         current_directory,
         False,
         [
             ".png",
             ".jpg",
             ".jpeg",
             ".gif",
@@ -44,15 +44,15 @@
                 pass
                 # Upload everything inside of the directory
                 # for root, _dirs, files in os.walk(file_path):
                 #     for file in files:
                 #         files_to_upload[os.path.join(root, file)] = open(
                 #             os.path.join(root, file), "rb"
                 #         )
-    
+
     if not files_to_upload:
         print("Nothing to compile")
         return
 
     # Upload all of the files to the API
     api_key = "YourSecretAPIKey"
```

## utils/api_call.py

```diff
@@ -1,42 +1,37 @@
 import requests
 import os
 
-# API_URL = os.getenv("API_URL")
-# if API_URL is None:
-#     raise ValueError(
-#         "API_URL environment variable not set. Please set the API_URL environment variable."
-#     )
-API_URL = "https://api.ggun.app:8080"
-
-TIMEOUT_TIME = 120
+API_URL = os.getenv("GGUN_API_URL", "https://api.ggun.app:8080")
+TIMEOUT_TIME = 300
+print(f"GGUN: using api url: {API_URL}")
 
 
 def api_call(api_key, endpoint, req_type, data=None, files=None):
     endpoint_fmtd = f"/{endpoint}" if not endpoint.startswith("/") else endpoint
     url = f"{API_URL}/{endpoint_fmtd}"
 
     headers = {
         "X-API-KEY": api_key,
         # "Content-Type": "application/json" # This is set automatically when using files in requests
     }
     if req_type == "POST":
-        if files:
-            # When uploading files, the 'files' parameter is used in requests.post
-            # The 'Content-Type' header is set automatically, so it's omitted here
-            response = requests.post(
-                url, headers=headers, files=files, timeout=TIMEOUT_TIME
-            )
-        else:
-            # For regular POST requests with JSON data
-            response = requests.post(
-                url, headers=headers, json=data, timeout=TIMEOUT_TIME
+        if files and data:
+            raise ValueError(
+                "Sending both files and data in the same request not yet tested"
             )
+        # When uploading files, the 'files' parameter is used in requests.post
+        # The 'Content-Type' header is set automatically by requests, so it's omitted here
+        response = requests.post(
+            url, headers=headers, json=data, files=files, timeout=TIMEOUT_TIME
+        )
     elif req_type == "GET":
         response = requests.get(url, headers=headers, timeout=TIMEOUT_TIME)
+    else:
+        raise ValueError(f"Invalid request type: {req_type}")
 
     if response.status_code == 200:
         print(f"({req_type}) {endpoint} API Call Successful")
         return response.json()
     else:
         error_message = (
             f"API Call failed with status code: {response.status_code}, "
```

## utils/list_files.py

```diff
@@ -1,37 +1,68 @@
 import subprocess
 import os
+import re
+from os.path import expanduser
 
 
-def list_git_files(directory, show_tree, exclude_file_types):
+def list_forge_test_strace_files(directory, show_tree, exclude_file_types=[]):
+    """
+    List all files in a directory that are being used by forge test.
+    """
+    # Define the command to be executed
+    command = "strace -f -e trace=%file -e read=none -e write=none forge test 2>&1 | grep -E 'openat\\(.*\\.sol'"
+
+    # Change the current working directory to ~/Test_Ggun/vanilla
+    cwd = expanduser("~/Test_Ggun/vanilla")
+
+    # Run the command
+    process = subprocess.Popen(
+        command,
+        shell=True,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        cwd=cwd,
+        text=True,
+    )
+
+    # Read the output
+    output, _ = process.communicate()
+
+    # Find all paths in the output
+    paths = re.findall(r"\"(.+\.sol)\"", output)
+
+    return paths
+
+
+
+
+def list_git_files(directory, show_tree, exclude_file_types=[]):
     """
     List all files in a directory that are not ignored by git using `git ls-files` command.
 
     This function uses the `git ls-files` command to list all files that are not ignored
     by .gitignore files. It can also display the directory tree structure if requested.
 
     Args:
         directory (str): The root directory to list files from.
         show_tree (bool, optional): If True, prints the directory tree structure. Defaults to False.
     """
+    # TODO use dulwich for ls-files, so we don't have to shell out, see https://stackoverflow.com/questions/50912696/dulwich-cheat-sheet-how-to-reproduce-git-ls-files
     try:
         file_list = []
         # Change the current working directory to the specified directory
-        original_directory = (
-            subprocess.check_output("pwd", shell=True).decode("utf-8").strip()
-        )
+        original_directory = os.getcwd()
         os.chdir(directory)
 
         # Execute `git ls-files` command to list all tracked files
         result = subprocess.check_output(
             "find . -type f \( -name '*.sol' -o -name '*.toml' \)",
             shell=True,
         ).decode("utf-8")
 
-
         # Change back to the original directory
         os.chdir(original_directory)
 
         files = result.split("\n")
 
         for file in files:
             if not any(file.endswith(ext) for ext in exclude_file_types):
@@ -59,8 +90,12 @@
 
     print("\nTesting list_git_files with show_tree=True")
     file_list = list_git_files(directory, show_tree=True)
     print(file_list)
 
 
 if __name__ == "__main__":
-    test_list_git_files()
+    # test_list_git_files()
+    directory = "~/Test_Ggun/vanilla"
+    files = list_forge_test_strace_files(directory, show_tree=True)
+    print(files)
+
```

