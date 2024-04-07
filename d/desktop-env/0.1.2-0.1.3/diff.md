# Comparing `tmp/desktop_env-0.1.2.tar.gz` & `tmp/desktop_env-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_env-0.1.2.tar", last modified: Sat Feb 24 16:19:03 2024, max compression
+gzip compressed data, was "desktop_env-0.1.3.tar", last modified: Sun Apr  7 09:07:54 2024, max compression
```

## Comparing `desktop_env-0.1.2.tar` & `desktop_env-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.302946 desktop_env-0.1.2/
--rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5185 2024-02-24 16:19:03.302946 desktop_env-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3375 2024-02-20 12:08:59.000000 desktop_env-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.277948 desktop_env-0.1.2/desktop_env/
--rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.2/desktop_env/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.288945 desktop_env-0.1.2/desktop_env/controllers/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.2/desktop_env/controllers/__init__.py
--rw-rw-rw-   0        0        0    15201 2024-02-01 15:36:30.000000 desktop_env-0.1.2/desktop_env/controllers/python.py
--rw-rw-rw-   0        0        0    29690 2024-02-20 09:59:46.000000 desktop_env-0.1.2/desktop_env/controllers/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.289936 desktop_env-0.1.2/desktop_env/envs/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.2/desktop_env/envs/__init__.py
--rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.2/desktop_env/envs/actions.py
--rw-rw-rw-   0        0        0    15594 2024-02-22 15:20:41.000000 desktop_env-0.1.2/desktop_env/envs/desktop_env.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.290945 desktop_env-0.1.2/desktop_env/evaluators/
--rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.2/desktop_env/evaluators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.295946 desktop_env-0.1.2/desktop_env/evaluators/getters/
--rw-rw-rw-   0        0        0     1058 2024-02-23 05:52:56.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/__init__.py
--rw-rw-rw-   0        0        0    31586 2024-02-23 05:56:09.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/chrome.py
--rw-rw-rw-   0        0        0     3253 2024-01-17 17:44:13.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/file.py
--rw-rw-rw-   0        0        0      747 2024-02-06 16:03:40.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/general.py
--rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/gimp.py
--rw-rw-rw-   0        0        0     3322 2024-01-22 08:47:49.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/impress.py
--rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/info.py
--rw-rw-rw-   0        0        0      446 2024-01-13 16:30:16.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/misc.py
--rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/replay.py
--rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/vlc.py
--rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.2/desktop_env/evaluators/getters/vscode.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.301945 desktop_env-0.1.2/desktop_env/evaluators/metrics/
--rw-rw-rw-   0        0        0     3211 2024-02-23 06:01:01.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/__init__.py
--rw-rw-rw-   0        0        0     1434 2024-02-06 16:03:59.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/basic_os.py
--rw-rw-rw-   0        0        0     9516 2024-02-23 06:01:01.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/chrome.py
--rw-rw-rw-   0        0        0    19404 2024-02-23 07:39:51.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/docs.py
--rw-rw-rw-   0        0        0     7018 2024-02-19 09:24:34.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/general.py
--rw-rw-rw-   0        0        0    18353 2024-01-31 19:14:10.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/gimp.py
--rw-rw-rw-   0        0        0     1604 2024-01-13 16:38:52.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/libreoffice.py
--rw-rw-rw-   0        0        0      375 2024-01-28 12:58:23.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/pdf.py
--rw-rw-rw-   0        0        0    23355 2024-02-22 08:39:14.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/slides.py
--rw-rw-rw-   0        0        0    21623 2024-02-21 07:45:46.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/table.py
--rw-rw-rw-   0        0        0    10547 2024-01-31 16:55:47.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/thunderbird.py
--rw-rw-rw-   0        0        0    28945 2024-02-23 07:39:51.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/utils.py
--rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/vlc.py
--rw-rw-rw-   0        0        0     3068 2024-02-23 07:07:59.000000 desktop_env-0.1.2/desktop_env/evaluators/metrics/vscode.py
-drwxrwxrwx   0        0        0        0 2024-02-24 16:19:03.287945 desktop_env-0.1.2/desktop_env.egg-info/
--rw-rw-rw-   0        0        0     5185 2024-02-24 16:19:03.000000 desktop_env-0.1.2/desktop_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-02-24 16:19:03.000000 desktop_env-0.1.2/desktop_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 16:19:03.000000 desktop_env-0.1.2/desktop_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      542 2024-02-24 16:19:03.000000 desktop_env-0.1.2/desktop_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-24 16:19:03.000000 desktop_env-0.1.2/desktop_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-24 16:19:03.302946 desktop_env-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2691 2024-02-24 16:18:57.000000 desktop_env-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/
+-rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7626 2024-04-07 09:07:54.652974 desktop_env-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5745 2024-04-07 09:02:51.000000 desktop_env-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.621513 desktop_env-0.1.3/desktop_env/
+-rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.3/desktop_env/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/controllers/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.3/desktop_env/controllers/__init__.py
+-rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.3/desktop_env/controllers/python.py
+-rw-rw-rw-   0        0        0    29803 2024-03-07 09:50:37.000000 desktop_env-0.1.3/desktop_env/controllers/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/envs/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.3/desktop_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.3/desktop_env/envs/actions.py
+-rw-rw-rw-   0        0        0    15658 2024-03-21 14:27:50.000000 desktop_env-0.1.3/desktop_env/envs/desktop_env.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/evaluators/
+-rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.3/desktop_env/evaluators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.642458 desktop_env-0.1.3/desktop_env/evaluators/getters/
+-rw-rw-rw-   0        0        0     1502 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/__init__.py
+-rw-rw-rw-   0        0        0      539 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/calc.py
+-rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/chrome.py
+-rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/file.py
+-rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/general.py
+-rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/gimp.py
+-rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/impress.py
+-rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/info.py
+-rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/misc.py
+-rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/replay.py
+-rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/vlc.py
+-rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/desktop_env/evaluators/metrics/
+-rw-rw-rw-   0        0        0     4081 2024-03-20 14:11:55.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/basic_os.py
+-rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/chrome.py
+-rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/docs.py
+-rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/general.py
+-rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/gimp.py
+-rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/libreoffice.py
+-rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/others.py
+-rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/pdf.py
+-rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/slides.py
+-rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/table.py
+-rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/thunderbird.py
+-rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/utils.py
+-rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/vlc.py
+-rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/desktop_env.egg-info/
+-rw-rw-rw-   0        0        0     7626 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1552 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      567 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 09:07:54.652974 desktop_env-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2752 2024-04-07 09:04:50.000000 desktop_env-0.1.3/setup.py
```

### Comparing `desktop_env-0.1.2/LICENSE` & `desktop_env-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/controllers/python.py` & `desktop_env-0.1.3/desktop_env/controllers/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 
     def execute_python_command(self, command: str) -> None:
         """
         Executes a python command on the server.
         It can be used to execute the pyautogui commands, or... any other python command. who knows?
         """
         # command_list = ["python", "-c", self.pkgs_prefix.format(command=command)]
-        command_list = ["python3", "-c", self.pkgs_prefix.format(command=command)]
+        command_list = ["python", "-c", self.pkgs_prefix.format(command=command)]
         payload = json.dumps({"command": command_list, "shell": False})
         headers = {
             'Content-Type': 'application/json'
         }
 
         try:
-            response = requests.post(self.http_server + "/execute", headers=headers, data=payload)
+            response = requests.post(self.http_server + "/execute", headers=headers, data=payload, timeout=90)
             if response.status_code == 200:
                 logger.info("Command executed successfully: %s", response.text)
             else:
                 logger.error("Failed to execute command. Status code: %d", response.status_code)
             return response.json()
         except requests.exceptions.RequestException as e:
             logger.error("An error occurred while trying to execute the command: %s", e)
@@ -259,24 +259,27 @@
         else:
             logger.error("Failed to start recording. Status code: %d", response.status_code)
 
     def end_recording(self, dest: str):
         """
         Ends recording the screen.
         """
-        response = requests.post(self.http_server + "/end_recording")
-        if response.status_code == 200:
-            logger.info("Recording stopped successfully")
-            with open(dest, 'wb') as f:
-                for chunk in response.iter_content(chunk_size=8192):
-                    if chunk:
-                        f.write(chunk)
-        else:
-            logger.error("Failed to stop recording. Status code: %d", response.status_code)
-            return None
+        try:
+            response = requests.post(self.http_server + "/end_recording")
+            if response.status_code == 200:
+                logger.info("Recording stopped successfully")
+                with open(dest, 'wb') as f:
+                    for chunk in response.iter_content(chunk_size=8192):
+                        if chunk:
+                            f.write(chunk)
+            else:
+                logger.error("Failed to stop recording. Status code: %d", response.status_code)
+                return None
+        except Exception as e:
+            logger.error("An error occurred while trying to download the recording: %s", e)
 
     # Additional info
     def get_vm_platform(self):
         """
         Gets the size of the vm screen.
         """
         return self.execute_python_command("import platform; print(platform.system())")['output'].strip()
@@ -337,8 +340,8 @@
         }
         response = requests.post(self.http_server + "/list_directory", headers=headers, data=payload)
         if response.status_code == 200:
             logger.info("Directory tree downloaded successfully")
             return response.json()["directory_tree"]
         else:
             logger.error("Failed to get directory tree. Status code: %d", response.status_code)
-            return None
+            return None
```

### Comparing `desktop_env-0.1.2/desktop_env/controllers/setup.py` & `desktop_env-0.1.3/desktop_env/controllers/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,14 +446,16 @@
                 operation(List[str]): each operation is chosen from ['delete', 'upload']
                 args(List[Dict[str, Any]]): parameters for each operation
             different args dict for different operations:
                 for delete:
                     query(str): query pattern string to search files or folder in google drive to delete, please refer to
                         https://developers.google.com/drive/api/guides/search-files?hl=en about how to write query string.
                     trash(bool): whether to delete files permanently or move to trash. By default, trash=false, completely delete it.
+                for mkdirs:
+                    path(List[str]): the path in the google drive to create folder
                 for upload:
                     path(str): remote url to download file
                     dest(List[str]): the path in the google drive to store the downloaded file
         """
         settings_file = config.get('settings_file', 'evaluation_examples/settings/googledrive/settings.yml')
         gauth = GoogleAuth(settings_file=settings_file)
         drive = GoogleDrive(gauth)
```

### Comparing `desktop_env-0.1.2/desktop_env/envs/actions.py` & `desktop_env-0.1.3/desktop_env/envs/actions.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/envs/desktop_env.py` & `desktop_env-0.1.3/desktop_env/envs/desktop_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,59 +49,49 @@
     DesktopEnv with OpenAI Gym interface.
     Fixme: refactor the logic when implementing the multi-process version
     """
 
     def __init__(
             self,
             path_to_vm: str,
+            snapshot_name: str = "init_state",
             action_space: str = "computer_13",
-            task_config: Dict[str, Any] = None,
             tmp_dir: str = "tmp",
             cache_dir: str = "cache",
             screen_size: Tuple[int] = (1920, 1080),
-            headless: bool = False
+            headless: bool = False,
+            require_a11y_tree: bool = True,
     ):
         """
         Args:
             path_to_vm (str): path to .vmx file
             action_space (str): "computer_13" | "pyautogui"
-
-            task_config (Dict[str, Any]): manages task configs integratedly,
-              including
-              * base snapshot
-              * task id (uuid)
-              * instruction
-              * setup config
-              * evaluator config
-
             tmp_dir (str): temporary directory to store trajectory stuffs like
               the extracted screenshots
             cache_dir (str): cache directory to cache task-related stuffs like
               reference file for evaluation
         """
 
         # Initialize environment variables
         self.path_to_vm = os.path.abspath(os.path.expandvars(os.path.expanduser(path_to_vm)))
+        self.snapshot_name = snapshot_name
         self.tmp_dir_base: str = tmp_dir
         self.cache_dir_base: str = cache_dir
-        self.vm_screen_size = screen_size
+        self.vm_screen_size = screen_size  # todo: add the logic to get the screen size from the VM
         self.headless = headless
+        self.require_a11y_tree = require_a11y_tree
 
         os.makedirs(self.tmp_dir_base, exist_ok=True)
 
-        # task-aware stuffs
-        # todo: handling the logic of snapshot directory
-        self._set_task_info(task_config)
-
         # Initialize emulator and controller
         logger.info("Initializing...")
         self._start_emulator()
         self.vm_ip = self._get_vm_ip()
         self.controller = PythonController(vm_ip=self.vm_ip)
-        self.setup_controller = SetupController(vm_ip=self.vm_ip, cache_dir=self.cache_dir)
+        self.setup_controller = SetupController(vm_ip=self.vm_ip, cache_dir=self.cache_dir_base)
 
         # Meta info of the VM, move to the reset() function
         self.vm_platform: str = ""  # self.controller.get_vm_platform()
 
         # mode: human or machine
         assert action_space in ["computer_13", "pyautogui"]
         self.action_space = action_space
@@ -143,35 +133,40 @@
             except Exception as e:
                 print(e)
                 time.sleep(5)
                 logger.info("Retrying...")
         raise Exception("Failed to get VM IP address!")
 
     def _save_state(self):
-        _execute_command(["vmrun", "-T", "ws" "snapshot", self.path_to_vm, self.snapshot_path])
+        _execute_command(["vmrun", "-T", "ws" "snapshot", self.path_to_vm, self.snapshot_name])
 
     def _get_screenshot(self):
         # random_uuid = str(uuid.uuid4())
         # os.makedirs(os.path.join("tmp", random_uuid), exist_ok=True)
         # image_path = os.path.join("tmp", random_uuid, "screenshot.png")
         image_path: str = os.path.join(self.tmp_dir, "screenshots", "{:d}.png".format(self._step_no))
 
         # Get the screenshot and save to the image_path
-        screenshot = self.controller.get_screenshot()
+        max_retries = 20
+        for _ in range(max_retries):
+            screenshot = self.controller.get_screenshot()
+            if screenshot is not None:
+                break
+            time.sleep(1)
+
         with open(image_path, "wb") as f:
             f.write(screenshot)
 
         return image_path
 
     def _get_obs(self):
         screenshot_image_path = self._get_screenshot()
         return screenshot_image_path
 
     def _set_task_info(self, task_config: Dict[str, Any]):
-        self.snapshot_path = task_config["snapshot"]
         self.task_id: str = task_config["id"]
         self.cache_dir: str = os.path.join(self.cache_dir_base, self.task_id)
         os.makedirs(self.cache_dir, exist_ok=True)
         self.instruction = task_config["instruction"]
         self.config = task_config["config"] if "config" in task_config else []
 
         # evaluator dict
@@ -183,25 +178,25 @@
         # if func is a str list, then result, expected (if exists), options (if exists) should also be lists of the same length
         # even if one of the metrics does not need expected or options field, it should be included in the list with None
         self.evaluator = task_config["evaluator"]
         self.metric: Metric = [getattr(metrics, func) for func in self.evaluator["func"]] \
             if isinstance(self.evaluator["func"], list) \
             else getattr(metrics, self.evaluator["func"])
         self.metric_conj: str = self.evaluator.get("conj", "and")  # take conjunction of multiple metrics
-        if "result" in self.evaluator:
+        if "result" in self.evaluator and len(self.evaluator["result"])>0:
             self.result_getter: Getter = [getattr(getters, "get_{:}".format(res["type"])) for res in
                                           self.evaluator["result"]] \
                 if isinstance(self.evaluator["result"], list) \
                 else getattr(getters, "get_{:}".format(self.evaluator["result"]["type"]))
         else:
             self.result_getter = [None] * len(self.metric) \
                 if isinstance(self.metric, list) \
                 else None
 
-        if "expected" in self.evaluator:
+        if "expected" in self.evaluator and len(self.evaluator["expected"])>0:
             self.expected_getter: Getter = [getattr(getters, "get_{:}".format(exp["type"])) if exp else None for exp in
                                             self.evaluator["expected"]] \
                 if isinstance(self.evaluator["expected"], list) \
                 else getattr(getters, "get_{:}".format(self.evaluator["expected"]["type"]))
         else:
             self.expected_getter = [None] * len(self.metric) \
                 if isinstance(self.metric, list) \
@@ -235,16 +230,16 @@
         logger.info("Setup new temp dir...")
         self.tmp_dir = tempfile.mkdtemp(
             prefix="{:d}.{:}.".format(self._traj_no, self.task_id),
             dir=self.tmp_dir_base
         )
         os.makedirs(os.path.join(self.tmp_dir, "screenshots"))
 
-        logger.info("Reverting to snapshot to {}...".format(self.snapshot_path))
-        _execute_command(["vmrun", "-T", "ws", "revertToSnapshot", self.path_to_vm, self.snapshot_path])
+        logger.info("Reverting to snapshot to {}...".format(self.snapshot_name))
+        _execute_command(["vmrun", "-T", "ws", "revertToSnapshot", self.path_to_vm, self.snapshot_name])
         time.sleep(5)
 
         print(self.vm_screen_size)
         logger.info("Starting emulator...")
         self._start_emulator()
         logger.info("Emulator started.")
 
@@ -257,15 +252,15 @@
         self.setup_controller.setup(self.config)
 
         time.sleep(5)
         logger.info("Environment setup complete.")
 
         observation = {
             "screenshot": self._get_obs(),
-            "accessibility_tree": self.controller.get_accessibility_tree(),
+            "accessibility_tree": self.controller.get_accessibility_tree() if self.require_a11y_tree else None,
         }
         return observation
 
     def step(self, action, pause=0.5):
         self._step_no += 1
         self.action_history.append(action)
 
@@ -293,16 +288,16 @@
                 self.controller.execute_action(action)
             else:
                 # the set of all possible python commands insides `pyautogui`
                 self.controller.execute_python_command(action)
 
         observation = {
             "screenshot": self._get_obs(),
-            "accessibility_tree": self.controller.get_accessibility_tree(),
-            "terminal": self.controller.get_terminal_output(),
+            "accessibility_tree": self.controller.get_accessibility_tree() if self.require_a11y_tree else None,
+            # "terminal": self.controller.get_terminal_output(),
             "instruction": self.instruction
         }
 
         return observation, reward, done, info
 
     def evaluate(self):
         """
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/__init__.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,18 +13,27 @@
     get_profile_name,
     get_number_of_search_results,
     get_googledrive_file,
     get_active_tab_info,
     get_enable_do_not_track,
     get_enable_enhanced_safety_browsing,
     get_new_startup_page,
-    get_find_unpacked_extension_path
+    get_find_unpacked_extension_path,
+    get_data_delete_automacally,
+    get_active_tab_html_parse,
+    get_active_tab_url_parse,
+    get_gotoRecreationPage_and_get_html_content,
+    get_url_dashPart,
+    get_active_url_from_accessTree,
+    get_find_installed_extension_name,
+    get_info_from_website
 )
-from .file import get_cloud_file, get_vm_file, get_cache_file
-from .general import get_vm_command_line, get_vm_terminal_output
+from .file import get_cloud_file, get_vm_file, get_cache_file, get_content_from_vm_file
+from .general import get_vm_command_line, get_vm_terminal_output, get_vm_command_error
 from .gimp import get_gimp_config_file
-from .impress import get_audio_in_slide
+from .impress import get_audio_in_slide, get_background_image_in_slide
 from .info import get_vm_screen_size, get_vm_window_size, get_vm_wallpaper, get_list_directory
-from .misc import get_rule, get_accessibility_tree
+from .misc import get_rule, get_accessibility_tree, get_rule_relativeTime, get_time_diff_range
 from .replay import get_replay
 from .vlc import get_vlc_playing_info, get_vlc_config, get_default_video_player
 from .vscode import get_vscode_config
+from .calc import get_conference_city_in_order
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/file.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import os
 from typing import Dict, List, Set
 from typing import Optional, Any, Union
-
+from datetime import datetime
 import requests
+import pandas as pd
+
+
+def get_content_from_vm_file(env, config: Dict[str, Any]) -> Any:
+    """
+    Config:
+        path (str): absolute path on the VM to fetch
+    """
+
+    path = config["path"]
+    file_path = get_vm_file(env, {"path": path, "dest": os.path.basename(path)})
+    file_type, file_content = config['file_type'], config['file_content']
+    if file_type == 'xlsx':
+        if file_content == 'last_row':
+            df = pd.read_excel(file_path)
+            last_row = df.iloc[-1]
+            last_row_as_list = last_row.astype(str).tolist()
+            return last_row_as_list
+    else:
+        raise NotImplementedError(f"File type {file_type} not supported")
 
 
 def get_cloud_file(env, config: Dict[str, Any]) -> Union[str, List[str]]:
     """
     Config:
         path (str|List[str]): the url to download from
         dest (str|List[str])): file name of the downloaded file
@@ -54,42 +74,51 @@
         path (str): absolute path on the VM to fetch
         dest (str): file name of the downloaded file
         multi (bool) : optional. if path and dest are lists providing
           information of multiple files. defaults to False
         gives (List[int]): optional. defaults to [0]. which files are directly
           returned to the metric. if len==1, str is returned; else, list is
           returned.
+        only support for single file now:
+        time_suffix(bool): optional. defaults to False. if True, append the current time in required format.
+        time_format(str): optional. defaults to "%Y_%m_%d". format of the time suffix.
     """
-
+    time_format = "%Y_%m_%d"
     if not config.get("multi", False):
         paths: List[str] = [config["path"]]
         dests: List[str] = [config["dest"]]
+        if "time_suffix" in config.keys() and config["time_suffix"]:
+            if "time_format" in config.keys():
+                time_format = config["time_format"]
+            # Insert time before . in file type suffix
+            paths = [p.split(".")[0] + datetime.now().strftime(time_format) + "." + p.split(".")[1] if "." in p else p for p in paths]
+            dests = [d.split(".")[0] + datetime.now().strftime(time_format) + "." + d.split(".")[1] if "." in d else d for d in dests]
     else:
         paths: List[str] = config["path"]
         dests: List[str] = config["dest"]
+
+
     cache_paths: List[str] = []
 
     gives: Set[int] = set(config.get("gives", [0]))
 
     for i, (p, d) in enumerate(zip(paths, dests)):
         _path = os.path.join(env.cache_dir, d)
-
         file = env.controller.get_file(p)
         if file is None:
             #return None
             # raise FileNotFoundError("File not found on VM: {:}".format(config["path"]))
             if i in gives:
                 cache_paths.append(None)
             continue
 
         if i in gives:
             cache_paths.append(_path)
         with open(_path, "wb") as f:
             f.write(file)
-
     return cache_paths[0] if len(cache_paths)==1 else cache_paths
 
 
 def get_cache_file(env, config: Dict[str, str]) -> str:
     """
     Config:
         path (str): relative path in cache dir
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/general.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/general.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,10 +17,26 @@
 
     if response.status_code == 200:
         return response.json()["output"]
     else:
         logger.error("Failed to get vm command line. Status code: %d", response.status_code)
         return None
 
+def get_vm_command_error(env, config: Dict[str, str]):
+    vm_ip = env.vm_ip
+    port = 5000
+    command = config["command"]
+    shell = config.get("shell", False)
+
+    response = requests.post(f"http://{vm_ip}:{port}/execute", json={"command": command, "shell": shell})
+
+    print(response.json())
+
+    if response.status_code == 200:
+        return response.json()["error"]
+    else:
+        logger.error("Failed to get vm command line error. Status code: %d", response.status_code)
+        return None
+
 
 def get_vm_terminal_output(env, config: Dict[str, str]):
     return env.controller.get_terminal_output()
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/gimp.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/info.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/info.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/replay.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/replay.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/vlc.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/getters/vscode.py` & `desktop_env-0.1.3/desktop_env/evaluators/getters/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/__init__.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from .basic_os import (
     check_gnome_favorite_apps,
     is_utc_0,
     check_text_enlarged,
-    check_moved_jpgs
+    check_moved_jpgs,
+    is_in_vm_clickboard
 )
 from .chrome import (
     is_expected_tabs,
     is_expected_bookmarks,
     compare_pdfs,
     compare_htmls,
     compare_archive,
     is_cookie_deleted,
     is_shortcut_on_desktop,
     check_font_size,
     check_enabled_experiments,
     check_history_deleted,
     is_expected_search_query,
     is_expected_active_tab,
-    is_added_to_steam_cart
+    is_expected_url_pattern_match,
+    is_added_to_steam_cart,
+    is_expected_installed_extensions,
+    compare_pdf_images
 )
 from .docs import (
     compare_font_names,
     compare_subscript_contains,
     has_page_numbers_in_footers,
     compare_docx_lines,
     evaluate_colored_words_in_tables,
@@ -40,45 +44,63 @@
     compare_docx_tables,
     compare_line_spacing,
     compare_insert_equation,
     compare_highlighted_text,
     is_first_line_centered,
     check_file_exists,
     check_tabstops,
-    compare_contains_image
+    compare_contains_image,
+    compare_docx_files_and_ignore_new_lines,
+    compare_docx_images,
+    compare_image_text,
+    compare_references
 )
 from .general import (
     check_csv,
     check_accessibility_tree,
     run_sqlite3,
     check_json,
     check_list,
     exact_match,
     is_in_list,
     fuzzy_match,
-    check_include_exclude
+    check_include_exclude,
+    check_direct_json_object,
+    compare_time_in_speedtest_results,
+    is_included_all_json_objects,
+    is_gold_text_included_in_pdf,
+    check_line_number,
+    file_contains,
+    compare_terminal_and_txt,
+    fuzzy_place_math,
+    compare_python_pure_text,
+    diff_text_file,
+    literal_match
 )
 from .gimp import (
+    check_structure_sim_resized,
     check_brightness_decrease_and_structure_sim,
     check_contrast_increase_and_structure_sim,
     check_saturation_increase_and_structure_sim,
-    check_image_size_and_structure_sim,
+    check_image_size,
     check_image_mirror,
     check_palette_and_structure_sim,
     check_textbox_on_leftside,
     check_green_background,
     check_file_exists_and_structure_sim,
     check_triangle_position,
     check_structure_sim,
     check_config_status,
     compare_image_list,
     increase_saturation,
     decrease_brightness,
     check_file_exists,
-    compare_triangle_positions
+    compare_triangle_positions,
+    check_sharper,
+    check_image_file_size
 )
 from .libreoffice import check_libre_locale
 from .pdf import check_pdf_pages
 from .slides import (
     check_presenter_console_disable,
     check_image_stretch_and_center,
     check_slide_numbers_color,
@@ -89,15 +111,16 @@
     check_left_panel,
     check_transition,
     check_page_number_colors,
     check_auto_saving_time
 )
 from .table import (
     compare_table,
-    compare_csv
+    compare_csv,
+    compare_conference_city_in_order
 )
 from .thunderbird import (
     check_thunderbird_prefs,
     check_thunderbird_filter,
     check_thunderbird_folder
 )
 from .vlc import (
@@ -114,15 +137,20 @@
     check_qt_slider_colours,
     check_global_key_play_pause
 )
 from .vscode import (
     compare_text_file,
     compare_config,
     compare_answer,
+    compare_result_files,
     is_extension_installed,
     check_json_settings,
-    check_json_keybindings
+    check_json_keybindings,
+    check_python_file_by_test_suite,
+    check_python_file_by_gold_file,
+    check_html_background_image,
+    compare_zip_files
 )
-
+from .others import compare_epub, check_mp3_meta
 
 def infeasible():
     pass
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/basic_os.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/basic_os.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import subprocess
-
-
 def check_gnome_favorite_apps(apps_str: str, rule):
     # parse the string like "['thunderbird.desktop', 'vim.desktop', 'google-chrome.desktop']"
     # to a list of strings
     apps = eval(apps_str)
 
     expected_apps = rule["expected"]
 
@@ -52,7 +49,20 @@
     if len(moved_jpgs) != len(expected_jpgs):
         return 0
 
     if set(moved_jpgs) == set(expected_jpgs):
         return 1
     else:
         return 0
+
+
+def is_in_vm_clickboard(config, terminal_output):
+    print("terminal_output: ")
+    print(terminal_output)
+    print("config: ")
+    print(config)
+    expected_results = config["expected"]
+    # check if terminal_output has expected results
+    if not isinstance(expected_results, list):
+        return 1 if expected_results in terminal_output else 0
+    else:
+        return 1 if all(result in terminal_output for result in expected_results) else 0
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/chrome.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/chrome.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,85 @@
 import logging
 import os
 import re
 import shutil
+from itertools import product
 from typing import Any, Dict, List, Union
 
-import fitz  # PyMuPDF
 import rapidfuzz.fuzz as fuzz
 from bs4 import BeautifulSoup, Tag
 
 from desktop_env.evaluators.metrics.utils import are_lists_equal, compare_urls
 
 logger = logging.getLogger("desktopenv.metrics.chrome")
 
 
 def is_expected_active_tab(active_tab_info: Dict[str, str], rule: Dict[str, Any]) -> float:
     """
     Checks if the expected active tab is open in Chrome.
     """
+    if not active_tab_info:
+        return 0.
+
     match_type = rule['type']
 
     if match_type == "url":
         expected_url = rule['url']
-        actual_url = active_tab_info.get('url', None)
+        if isinstance(active_tab_info, Dict):
+            actual_url = active_tab_info.get('url', None)
+        else:
+            actual_url = active_tab_info
         print("expected_url: {}".format(expected_url))
         print("actual_url: {}".format(actual_url))
         return 1 if compare_urls(expected_url, actual_url) else 0
     else:
         logger.error(f"Unknown type: {match_type}")
         return 0
 
 
+# rules[expected] is a string-formatted regex
+def is_expected_url_pattern_match(result, rules) -> float:
+    """
+    This function is used to search the expected pattern in the url using regex.
+    result is the return value of function "activte_tab_info" or return value of function "get_active_url_from_accessTree"   
+    """
+    if not result:
+        return 0.
+
+    if type(result) == dict:
+        result_url = result["url"]
+        print("result url: {}".format(result_url))
+    else:
+        result_url = result
+    # expect_regex = re.compile(rules["expected"])
+    patterns = rules["expected"]
+    print("expected_regex: {}".format(patterns))
+    for pattern in patterns:
+        match = re.search(pattern, result_url)
+        print(match)
+        if not match:
+            return 0.
+    return 1.
+
+
+def is_expected_installed_extensions(installed_extensions, expected) -> float:
+    print("installed_extensions: ")
+    print(installed_extensions)
+    expected_extensions = expected["expected"]
+
+    # whether the expected extensions are installed
+    set_expected_extensions = set(expected_extensions)
+    set_installed_extensions = set(installed_extensions)
+
+    if set_expected_extensions.issubset(set_installed_extensions):
+        return 1.
+    else:
+        return 0.
+
+
 def is_expected_tabs(open_tabs: List[Dict[str, str]], rule: Dict[str, Any]) -> float:
     """
     Checks if the expected tabs are open in Chrome.
     """
 
     match_type = rule['type']
 
@@ -56,14 +102,37 @@
         bookmark_bar_folders_names = [bookmark['name'] for bookmark in bookmarks['bookmark_bar']['children'] if
                                       bookmark['type'] == 'folder']
         return 1. if set(bookmark_bar_folders_names) == set(rule['names']) else 0.
     elif rule['type'] == "bookmark_bar_websites_urls":
         bookmark_bar_websites_urls = [bookmark['url'] for bookmark in bookmarks['bookmark_bar']['children'] if
                                       bookmark['type'] == 'url']
         return 1. if set(bookmark_bar_websites_urls) == set(rule['urls']) else 0.
+    elif rule['type'] == "liked_authors_websites_urls":
+        # Check if "liked authors" folder exists
+        liked_authors_folder = next((bookmark for bookmark in bookmarks['bookmark_bar']['children'] if
+                                     bookmark['type'] == 'folder' and bookmark['name'] == 'Liked Authors'), None)
+        if liked_authors_folder:
+            # Check if it contains the specified URLs
+            liked_authors_urls = [bookmark['url'] for bookmark in liked_authors_folder['children'] if
+                                  bookmark['type'] == 'url']
+
+            urls = rule['urls']
+
+            for idx, url in enumerate(urls):
+                if isinstance(url, str):
+                    urls[idx] = [url]
+
+            combinations = product(*urls)
+
+            for combination in combinations:
+                if set(combination) == set(liked_authors_urls):
+                    return 1.
+            return 0.
+        else:
+            return 0.
     else:
         raise TypeError(f"{rule['type']} not support yet!")
 
 
 def is_expected_search_query(active_tab_info: Dict[str, str], rules: Dict[str, Any]) -> float:
     expected = rules['expect']
     pattern = expected['pattern']
@@ -95,33 +164,89 @@
             text2 = extract_text_from_pdf(path2)
             score += fuzz.ratio(text1, text2) / 100
         except Exception as e:
             logger.info(f"[ERROR]: unexpected error occurred when comparing PDF files: {e}")
     return score / len(pdf2_path)
 
 
+import fitz
+from PIL import Image
+from borb.pdf import Document
+from borb.pdf import PDF
+
+from pathlib import Path
+import typing
+
+
+def compare_pdf_images(pdf1_path: str, pdf2_path: str, **kwargs) -> float:
+    if not pdf1_path or not pdf2_path:
+        return 0.
+
+    def extract_images_from_pdf(pdf_path):
+        pdf_document = fitz.open(pdf_path)
+        images = []
+
+        for page_number in range(pdf_document.page_count):
+            page = pdf_document[page_number]
+            pixmap = page.get_pixmap()
+
+            img = Image.frombytes("RGB", [pixmap.width, pixmap.height], pixmap.samples)
+
+            images.append(img)
+
+        return images
+
+    def fix_pdf(in_path: Path, out_path: Path) -> None:
+        doc: typing.Optional[Document] = None
+        with open(in_path, "rb") as fh:
+            doc = PDF.loads(fh)
+        with open(out_path, "wb") as fh:
+            PDF.dumps(fh, doc)
+
+    fix_pdf(Path(pdf1_path), Path(pdf1_path))
+    fix_pdf(Path(pdf2_path), Path(pdf2_path))
+
+    images1 = extract_images_from_pdf(pdf1_path)
+    images2 = extract_images_from_pdf(pdf2_path)
+
+    if len(images1) != len(images2):
+        return 0.
+
+    for img1, img2 in zip(images1, images2):
+        if img1.tobytes() != img2.tobytes():
+            return 0.
+
+    return 1.
+
+
 def compare_archive(pred_path: str, gold_path: str, **kwargs) -> float:
     """
     Compare two archives. Note that the files in the archives should be of the same type.
     """
-    if not pred_path: return 0.
+    file_path = kwargs.pop('file_path', '')
+
+    if not pred_path:
+        return 0.
     pred_folder = os.path.splitext(pred_path)[0] + '_pred'
     gold_folder = os.path.splitext(gold_path)[0] + '_gold'
 
     if os.path.exists(pred_folder):  # remove existing folder for new predictions
         shutil.rmtree(pred_folder, ignore_errors=True)
     os.makedirs(pred_folder)
     shutil.unpack_archive(pred_path, pred_folder)
+
     if not os.path.exists(gold_folder):  # use cache if exists
         os.makedirs(gold_folder)
         shutil.unpack_archive(gold_path, gold_folder)
 
-    pred_files = sorted(os.listdir(pred_folder))
-    gold_files = sorted(os.listdir(gold_folder))
-    if pred_files != gold_files: return 0.
+    pred_files = sorted(os.listdir(os.path.join(pred_folder, file_path)))
+    gold_files = sorted(os.listdir(os.path.join(gold_folder, file_path)))
+
+    if pred_files != gold_files:
+        return 0.
 
     def get_compare_function():
         file_type = kwargs.pop('file_type', 'text')
         if file_type == 'text':
             from .vscode import compare_text_file
             return compare_text_file
         elif file_type == 'pdf':
@@ -149,16 +274,16 @@
             return compare_videos
         else:
             raise ValueError('[ERROR]: not support file type: %s' % file_type)
 
     score = 0
     compare_function = get_compare_function()
     for f1, f2 in zip(pred_files, gold_files):
-        fp1 = os.path.join(pred_folder, f1)
-        fp2 = os.path.join(gold_folder, f2)
+        fp1 = os.path.join(pred_folder, file_path, f1)
+        fp2 = os.path.join(gold_folder, file_path, f2)
         score += compare_function(fp1, fp2, **kwargs)
     return score / len(pred_files)
 
 
 def compare_htmls(html_path1: str, html_path2: str) -> float:
     """
     Compare two HTML files.
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/general.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/thunderbird.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,219 +1,176 @@
-import csv
-import functools
 import json
-import operator
+import logging
 import re
-import sqlite3
-from numbers import Number
-from typing import Callable, Any, Union
-from typing import Dict, List, Pattern
+from typing import List, Pattern, Dict, Match
+from typing import Union, Any, TypeVar, Callable
 
-import lxml.etree
-from lxml.cssselect import CSSSelector
-from lxml.etree import _Element
-from rapidfuzz import fuzz
+from .utils import _match_record
+from .utils import _match_value_to_rule as _match_pref
 
-from .utils import _match_record, _match_value_to_rule
+logger = logging.getLogger("desktopenv.metric.thunderbird")
 
+V = TypeVar("Value")
 
-def check_include_exclude(result: str, rules: Dict[str, List[str]]) -> float:
-    if result is None:
-        return 0.
-
-    print(result, rules)
-    include = rules.get("include", [])
-    exclude = rules.get("exclude", [])
-    if all(r in result for r in include) and all(r not in result for r in exclude):
-        return 1.
-    else:
-        return 0.
-
-
-def exact_match(result, rules) -> float:
-    expect = rules["expected"]
-    print(result, expect)
-
-    if result == expect:
-        return 1.
-    else:
-        return 0.
-
-def is_in_list(result, rules) -> float:
-    expect = rules["expected"]
-    if expect in result:
-        return 1.
-    else:
-        return 0.
-    
-def fuzzy_match(result, rules) -> float:
-    expect = rules["expected"]
-
-    return fuzz.ratio(result, expect) / 100.
+_pref_pattern: Pattern[str] = re.compile(r'^user_pref\("(?P<key>(?:[^"]|\\")+)\", (?P<val>.+)\);$');
 
 
-def check_csv(result: str, rules: Dict[str, List[Dict[str, str]]]) -> float:
+def check_thunderbird_prefs(result: str, rule: Dict[str, Dict[str, Dict[str, Any]]]):
     """
     Args:
-        result (str): path to csv file
-        rules (Dict[str, List[Dict[str, str]]]): dict like
+        result (str): path to result file
+        rule (Dict[str, Dict[str, Dict[str, Any]]]): dict like
           {
-            "expect": [{key: value}]
-            "unexpect": [{key: value}]
+            "expect": {
+                str: {
+                    "method": str
+                    "ref": something
+                }
+            }
+            "unexpect": {
+                str: {
+                    "method": str
+                    "ref": something
+                }
+            }
           }
 
     Returns:
         float
     """
 
     if result is None:
         return 0.
 
-    expect_metrics = [False] * len(rules.get("expect", []))
+    expect_rules = rule.get("expect", {})
+    unexpect_rules = rule.get("unexpect", {})
+
+    expect_metrics = {k: False for k in expect_rules}
     unexpect_metric = True
     with open(result) as f:
-        reader = csv.DictReader(f)
-
-        for rcd in reader:
-            for i, r in enumerate(rules.get("expect", [])):
-                expect_metrics[i] = expect_metrics[i] or _match_record(r, rcd)
-            unexpect_metric = unexpect_metric and not any(_match_record(r, rcd) for r in rules.get("unexpect", []))
-    return float(all(expect_metrics) and unexpect_metric)
+        for l in f:
+            match_: Match[str] = _pref_pattern.match(l.strip())
+            if match_ is None:
+                continue
+
+            key: str = match_.group("key")
+            # value: str = match_.group("val")
+            # if value in {"true", "false"}:
+            # value = value.title()
+            # value: V = eval(value)
+            value = json.loads(match_.group("val"))
+            if key in expect_rules:
+                logger.debug("K: %s, V: %s", key, repr(value))
+                expect_metrics[key] = _match_pref(value, expect_rules[key])
+            elif key in unexpect_rules:
+                unexpect_metric = unexpect_metric and not _match_pref(value, unexpect_rules[key])
+
+    return float(all(expect_metrics.values()) and unexpect_metric)
+
+
+_value_processor: Callable[[str], str] = lambda val: val.replace("\\\"", "\"").replace("\\\\", "\\")
+# _condition_pattern: Pattern[str] = re.compile(r'(?P<type>AND|OR) \((?P<key>[\w ]+),(?P<rel>[\w ' + '\'' + r']+),(?:"(?P<val2>(?:[^"]|\")+)"|(?P<val1>[^)]+))\)')
+_condition_pattern: Pattern[str] = re.compile(
+    r'\b(?:AND|OR) \((?:[\w ]+),(?:[\w ' + '\'' + r']+),(?:"(?:(?:[^"]|\")+)"|(?:[^)]+))\)|\bALL\b')
 
 
-def check_list(result: str, rules: Dict[str, List[str]]) -> float:
+def check_thunderbird_filter(result: str, rules: Dict[str, List[Dict[str, str]]]) -> float:
     """
     Args:
-        result (str): path to list file
-        rules (Dict[str, List[str]]): dict like
+        result (str): path to filter def file
+        rules (Dict[str, List[Dict[str, str]]]): dict like
           {
-            "expect": list of str as regexes
-            "unexpect": list of str as regexes
+            "expect": [{key: value}]
+            "unexpect": [{key: value}]
           }
 
     Returns:
         float
     """
 
     if result is None:
         return 0.
 
-    expect_patterns: List[Pattern[str]] = [re.compile(ptt) for ptt in rules.get("expect", [])]
-    unexpect_patterns: List[Pattern[str]] = [re.compile(ptt) for ptt in rules.get("unexpect", [])]
-
-    expect_metrics = [False] * len(expect_patterns)
-    unexpect_metric = True
+    # read filter def file
+    # a filter:
+    # {
+    #   "name": "Name",
+    #   "enabled": "yes" | "no",
+    #   "type": "17",
+    #   "action": "Move to folder" | ...,
+    #   "actionValue": ...,
+    #   "condition": [...]
+    # }
+    filters: List[Dict[str, Union[str, List[str]]]] = []
     with open(result) as f:
         for l in f:
-            for i, r in enumerate(expect_patterns):
-                expect_metrics[i] = expect_metrics[i] or (r.search(l) is not None)
-            unexpect_metric = unexpect_metric and all(r.search(l) is None for r in unexpect_patterns)
-    return float(all(expect_metrics) and unexpect_metric)
-
-
-_accessibility_ns_map = {"st": "uri:deskat:state.at-spi.gnome.org"
-    , "attr": "uri:deskat:attributes.at-spi.gnome.org"
-    , "cp": "uri:deskat:component.at-spi.gnome.org"
-    , "doc": "uri:deskat:document.at-spi.gnome.org"
-    , "docattr": "uri:deskat:attributes.document.at-spi.gnome.org"
-    , "txt": "uri:deskat:text.at-spi.gnome.org"
-    , "val": "uri:deskat:value.at-spi.gnome.org"
-    , "act": "uri:deskat:action.at-spi.gnome.org"
-                         }
-
-
-def check_accessibility_tree(result: str, rules: Dict[str, Any]) -> float:
-    """
-    Args:
-        result (str): XML of GNOME Accessibility Tree
-        rules (Dict[str, Any]): dict like
-          {
-            "selectors": list of str as CSS selectors, will be connected by ", "
-              to form a composite selector. Only one from `selectors` and
-              `xpath` is needed. If both are present, `xpath` takes the
-              priority.
-            "xpath": str as xpath. Only one from `selectors` and `xpath` is
-              needed. If both are present, `xpath` takes the priority.
-            "text": str as the expected text content of the selected element.
-            "exact": bool specifying whether exact match or fuzzy match should
-              be performed. defaults to True
-          }
-
-    Returns:
-        float
-    """
-
-    at: _Element = lxml.etree.fromstring(result)
-    if "xpath" in rules:
-        elements: List[_Element] = at.xpath(rules["xpath"], namespaces=_accessibility_ns_map)
-    elif "selectors" in rules:
-        selector = CSSSelector(", ".join(rules["selectors"]), namespaces=_accessibility_ns_map)
-        elements: List[_Element] = selector(at)
-    else:
-        raise ValueError("At least one of xpath and selectors is required")
-
-    if len(elements) == 0:
-        return 0.
-
-    if "text" in rules:
-        match_func: Callable[[str], Number] = functools.partial(operator.eq if rules["exact"] \
-                                                                    else (lambda a, b: fuzz.ratio(a, b) / 100.)
-                                                                , rules["text"]
-                                                                )
-        match_score: Number = 0
-        for elm in elements:
-            match_score = max(match_score, match_func(elm.text or None))
-    else:
-        match_score = 1.
-
-    return float(match_score)
-
-
-# def check_existence(result: str, *args) -> float:
-# return 1. - (result is None)
-
-def run_sqlite3(result: str, rules: Dict[str, Any]) -> float:
-    connection: sqlite3.Connection = sqlite3.connect(result)
-    cursor: sqlite3.Cursor = connection.execute(rules["sql"])
-    return float(cursor.fetchone()[0] or 0)
+            if l.startswith("name="):
+                filter_: Dict[str, Union[str, List[str]]] = {}
+                filter_["name"] = _value_processor(l[6:-2])
+            elif l.startswith("enabled="):
+                filter_["enabled"] = _value_processor(l[9:-2])
+            elif l.startswith("type="):
+                filter_["type"] = _value_processor(l[6:-2])
+            elif l.startswith("action="):
+                filter_["action"] = _value_processor(l[8:-2])
+            elif l.startswith("actionValue="):
+                filter_["actionValue"] = _value_processor(l[13:-2])
+            elif l.startswith("condition="):
+                condition_str: str = _value_processor(l[11:-2])
+                logger.debug("FILTER CONDITION: %s", condition_str)
+
+                conditions: List[str] = \
+                    _condition_pattern.findall(condition_str)
+                logger.debug("FILTER CONDITIONS: %s", repr(conditions))
+
+                filter_["condition"] = conditions
+                logger.debug("FILTER %s", repr(filter_))
+                filters.append(filter_)
 
+    expect_metrics = [False] * len(rules.get("expect", []))
+    unexpect_metric = True
+    for flt in filters:
+        for i, r in enumerate(rules.get("expect", [])):
+            expect_metrics[i] = expect_metrics[i] or _match_record(r, flt)
+        unexpect_metric = unexpect_metric and not any(_match_record(r, flt) for r in rules.get("unexpect", []))
+    return float(all(expect_metrics) and unexpect_metric)
 
-def check_json(result: str, rules: Dict[str, List[Dict[str, Union[List[str], str]]]]) -> float:
-    """
-    Args:
-        result (str): path to json file
-        rules (Dict[str, List[Dict[str, Union[List[str], str]]]]): dict like
-          {
-            "expect": [
-                {
-                    "key": list of str
-                    "method": str
-                    "ref": something
-                }
-            ],
-            "unexpect": <the same as `expect`
-          }
 
-    Returns:
-        float
+def check_thunderbird_folder(result: Union[str, List[str]], reference: Union[str, List[str]], **kwargs) -> float:
     """
-
-    if result is None:
-        return 0.
-    with open(result) as f:
-        result: Dict[str, Any] = json.load(f)
-
-    expect_rules = rules.get("expect", {})
-    unexpect_rules = rules.get("unexpect", {})
-
-    metric = True
-    for r in expect_rules:
-        value = result
-        for k in r["key"]:
-            value = value[k]
-        metric = metric and _match_value_to_rule(value, r)
-    for r in unexpect_rules:
-        value = result
-        for k in r["key"]:
-            value = value[k]
-        metric = metric and not _match_value_to_rule(value, r)
-    return metric
+    Check the file or file_list that each text file contains all messages in a folder in Thunderbird. Each message is started with `FROM - `.
+    **kwargs:
+        ignore_status (bool): for comparison, ignore the status (X-Mozilla-Status: 0000) of each message. default: False
+        ignore_keys (bool): for comparison, ignore the keys (X-Mozilla-Keys: label) of each message. default: False
+        remove_deleted (bool): ignore deleted messages which has status code 0008 or 0009. default: True
+        remove_duplicate (bool): remove duplicate messages. default: True
+    """
+
+    def normalize_msg(msg, options):
+        ignore_status = options.get('ignore_status', False)
+        ignore_keys = options.get('ignore_keys', False)
+        if ignore_status:
+            msg = re.sub(r'X-Mozilla-Status\d?:[\s\d]+', '', msg)
+        if ignore_keys:
+            msg = re.sub(r'(X-Mozilla-Keys:[^\n]*?)\n(MIME-Version)', r'\2', msg)
+        return msg.strip()
+
+    def read_thunderbird_folder_file(path: str) -> str:
+        with open(path, 'r') as inf:
+            data = inf.read().strip()
+            messages = []
+            for mail in data.split('FROM - '):
+                if mail.strip(): continue
+                if kwargs.get('remove_deleted', True) and re.search(r'X-Mozilla-Status: 000[89]', mail): continue
+                messages.append('FROM - ' + normalize_msg(mail, kwargs))
+            if kwargs.get('remove_duplicate', True):
+                messages = set(messages)
+        return '\n'.join(sorted(messages))
+
+    if type(reference) != list:
+        result, reference = [result], [reference]
+    for pred, gold in zip(result, reference):
+        if pred is None: return .0
+        mail1 = read_thunderbird_folder_file(pred)
+        mail2 = read_thunderbird_folder_file(gold)
+        if mail1 != mail2: return .0
+    return 1.0
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/gimp.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/gimp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from typing import List, Union
 from skimage.metrics import structural_similarity as ssim
 from PIL import Image, ImageChops, ImageStat
 
 
 def compare_image_list(pred_img_path_list: Union[str, List[str]],
-                   gold_img_path_list: Union[str, List[str]]) -> float:
+                       gold_img_path_list: Union[str, List[str]]) -> float:
     """ Compare two image lists, only if all images are the same, return 1.0, otherwise return 0.0
     """
     if type(pred_img_path_list) != list:
         pred_img_path_list = [pred_img_path_list]
         gold_img_path_list = [gold_img_path_list]
     for pred_img_path, gold_img_path in zip(pred_img_path_list, gold_img_path_list):
         if not pred_img_path or not gold_img_path:
@@ -173,27 +173,37 @@
 def calculate_contrast(image):
     """Calculate the contrast of an image as the standard deviation of the pixel
     values."""
     pixels = np.asarray(image, dtype=np.float32)
     return np.std(pixels)
 
 
+def calculate_image_sharpness(image_path):
+    # Load the image in grayscale
+    image = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
+    # Apply the Laplacian operator
+    laplacian = cv2.Laplacian(image, cv2.CV_64F)
+    # Calculate the variance
+    variance = np.var(laplacian)
+    return variance
+
+
 def structure_check_by_mse(img1, img2, threshold=0.03):
     """Check if two images are approximately the same by MSE"""
     mse = np.mean(
         (np.array(img1, dtype=np.float32) / 255
          - np.array(img2, dtype=np.float32) / 255) ** 2)
     structure_same = True if mse < threshold else False
     print("MSE: ", mse)
     return structure_same
 
 
 def structure_check_by_ssim(img1, img2, threshold=0.9):
     """Check if two images are approximately the same by SSIM"""
-    similarity = ssim(np.array(img1), np.array(img2), multichannel=True)
+    similarity = ssim(np.array(img1), np.array(img2), multichannel=True, channel_axis=-1)
     print("SSIM: ", similarity)
     return similarity >= threshold
 
 
 def check_brightness_decrease_and_structure_sim(src_path, tgt_path):
     """
     Check the brightness of src is lower than tgt and the structures are similar
@@ -291,15 +301,16 @@
 
     # Load the image
     img = Image.open(tgt_path)
     img_array = np.array(img)
 
     # We assume the triangle is a different color from the background
     # Find the unique colors
-    unique_colors, counts = np.unique(img_array.reshape(-1, img_array.shape[2]), axis=0, return_counts=True)
+    unique_colors, counts = np.unique(img_array.reshape(-1, img_array.shape[2]), axis=0,
+                                      return_counts=True)
     unique_colors_sorted = unique_colors[np.argsort(counts)]
 
     # Assuming the background is the most common color and the triangle is a different color
     triangle_color = unique_colors_sorted[1]
 
     # Create a mask where the triangle pixels are True
     triangle_mask = np.all(img_array == triangle_color, axis=2)
@@ -333,14 +344,33 @@
 
     img_src = Image.open(src_path)
     img_tgt = Image.open(tgt_path)
     structure_same = structure_check_by_ssim(img_src, img_tgt)
     return structure_same
 
 
+def check_structure_sim_resized(src_path, tgt_path):
+    """
+    Check if the structure of the two images are similar after resizing.
+    gimp:d16c99dc-2a1e-46f2-b350-d97c86c85c15
+    """
+    if src_path is None or tgt_path is None:
+        return 0.
+
+    img_src = Image.open(src_path)
+    img_tgt = Image.open(tgt_path)
+
+    # Resize the images to the same size
+    img_src = img_src.resize(img_tgt.size)
+
+    # Check if the structure is similar
+    structure_same = structure_check_by_ssim(img_src, img_tgt)
+    return structure_same
+
+
 def check_contrast_increase_and_structure_sim(src_path, tgt_path):
     """
     Check if the src image has higher contrast than the tgt image and the structures are similar
     gimp:f723c744-e62c-4ae6-98d1-750d3cd7d79d
     """
     if src_path is None or tgt_path is None:
         return 0.
@@ -384,42 +414,36 @@
             if items[0] == rule["key"][0] \
                     and items[1] == rule["key"][1] \
                     and items[-1] == rule["value"]:
                 return 1.
     return 0.
 
 
-def check_image_size_and_structure_sim(src_path, tgt_path, height=512, width=None):
+def check_image_size(src_path, rule):
     """
-    Check if the size of the src image is correct and the structure of the two images are similar.
-    gimp:d16c99dc-2a1e-46f2-b350-d97c86c85c15
+    Check if the size of the src image is correct
+    multi-apps:42f4d1c7-4521-4161-b646-0a8934e36081
     """
-
-    if src_path is None or tgt_path is None:
+    if src_path is None:
         return 0.
 
-    # Load images
-    source_image = Image.open(src_path)
-    target_image = Image.open(tgt_path)
+    # Load the image
+    img = Image.open(src_path)
 
-    # Check size
-    if width is not None:
-        width_same = source_image.size[0] == width
-    else:
-        width_same = True
-    if height is not None:
-        height_same = source_image.size[1] == height
+    # Check the size
+    if rule.get("height", None) is not None:
+        height_same = img.size[1] == rule["height"]
     else:
         height_same = True
+    if rule.get("width", None) is not None:
+        width_same = img.size[0] == rule["width"]
+    else:
+        width_same = True
 
-    # Check structure
-    resized_target_image = target_image.resize(source_image.size)
-    structure_same = structure_check_by_ssim(source_image, resized_target_image)
-
-    if width_same and height_same and structure_same:
+    if height_same and width_same:
         return 1.
     else:
         return 0.
 
 
 def check_palette_and_structure_sim(src_path, tgt_path):
     """
@@ -517,14 +541,39 @@
                 r, g, b = source_pixels[x, y][:3]
                 if not (g > r and g > b):
                     return 0.
 
     return 1.
 
 
+def check_sharper(src_path, tgt_path):
+    """
+    Check if the source image is sharper than the target image.
+    multi-app:bb7db4c2-30b5-4be7-8dd7-b8c4ec7d3108
+    """
+    sharpness_src = calculate_image_sharpness(src_path)
+    sharpness_tgt = calculate_image_sharpness(tgt_path)
+    return 1.0 if sharpness_src > sharpness_tgt else 0.0
+
+
+def check_image_file_size(src_path, rule):
+    """
+    Check if the size of the src image within 500KB
+    """
+    if src_path is None:
+        return 0.0
+
+    # Check the size
+    file_size = os.path.getsize(src_path)
+    if file_size < rule["max_size"]:
+        return 1.0
+    else:
+        return 0.0
+
+
 if __name__ == "__main__":
     actual_config_path = "../../../cache/sessionrc_test"
     rule = {
         "key": "hide-docks",
         "value": "no"
     }
     print(check_config_status(actual_config_path, rule))
@@ -546,7 +595,24 @@
     src_path = "../../../cache/734d6579-c07d-47a8-9ae2-13339795476b/green_background_with_object.png"
     tgt_path = "../../../cache/734d6579-c07d-47a8-9ae2-13339795476b/white_background_with_object.png"
     print(check_green_background(src_path, tgt_path))
 
     tgt_path = "../../../cache/f4aec372-4fb0-4df5-a52b-79e0e2a5d6ce/Triangle_In_The_Middle.png"
     print(check_triangle_position(tgt_path))
 
+    src_path = "../../../cache/bb7db4c2-30b5-4be7-8dd7-b8c4ec7d3108/anmi_sharper.png"
+    tgt_path = "../../../cache/bb7db4c2-30b5-4be7-8dd7-b8c4ec7d3108/anmi.png"
+    print(check_sharper(src_path, tgt_path))
+
+    src_path = "../../../cache/3c8f201a-009d-4bbe-8b65-a6f8b35bb57f/compressed.jpeg"
+    rule = {
+        "max_size": 500000
+    }
+    print(check_image_file_size(src_path, rule))
+
+    src_path = "../../../cache/d16c99dc-2a1e-46f2-b350-d97c86c85c15/resized.png"
+    tgt_path = "../../../cache/d16c99dc-2a1e-46f2-b350-d97c86c85c15/dog_with_background.png"
+    rule = {
+        "height": 512
+    }
+    print(check_image_size(src_path, rule))
+    print(check_structure_sim_resized(src_path, tgt_path))
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/libreoffice.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/libreoffice.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,7 @@
         if len(setup_locale_setting) > 0 \
         else locale_setting[0].text
 
     return float(any(fnmatch.fnmatchcase(setup_locale_setting, ptn) \
                      for ptn in rules["locale_set"]
                      )
                  )
-
-
-if __name__ == "__main__":
-    path1 = "../../任务数据/LibreOffice Calc/registrymodifications.ru.xcu"
-    print(check_libre_locale(path1, {"locale_set": ["ru-*", "de-*", "fr-*"
-        , "pt-*", "es-*", "it-*"
-                                                    ]
-                                     }
-                             )
-          )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/slides.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/slides.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     the_image = original_slide_images[0]
 
     # Get the images that modified in width and height
     for modified_image in modified_slide_images:
         if the_image.image.blob == modified_image.image.blob:
             the_modified_image = modified_image
 
-    if (abs(the_modified_image.width - original_pres.slide_width) > Inches(0.1) or
-            abs(the_modified_image.height - original_pres.slide_height) > Inches(0.1) or
-            abs(the_modified_image.left - (original_pres.slide_width - the_modified_image.width) / 2) > Inches(0.1) or
-            abs(the_modified_image.top - (original_pres.slide_height - the_modified_image.height) / 2) > Inches(0.1)):
+    if (abs(the_modified_image.width - original_pres.slide_width) > Inches(0.5) or
+            abs(the_modified_image.height - original_pres.slide_height) > Inches(0.5) or
+            abs(the_modified_image.left - (original_pres.slide_width - the_modified_image.width) / 2) > Inches(0.5) or
+            abs(the_modified_image.top - (original_pres.slide_height - the_modified_image.height) / 2) > Inches(0.5)):
         return 0.
 
     return 1.
 
 
 def is_red_color(color):
     # judge if the color is red
@@ -161,103 +161,107 @@
     if len(prs1.slides) != len(prs2.slides) and examine_number_of_slides:
         return 0
 
     slide_idx = 0
     # compare the content of each slide
     for slide1, slide2 in zip(prs1.slides, prs2.slides):
         slide_idx += 1
+
         def get_slide_background_color(slide):
             background = slide.background
             if background.fill.background():
                 return background.fill.fore_color.rgb
             else:
                 return None
-            
+
         if get_slide_background_color(slide1) != get_slide_background_color(slide2) and examine_background_color:
             return 0
-        
+
         def get_slide_notes(slide):
             notes_slide = slide.notes_slide
             if notes_slide:
                 return notes_slide.notes_text_frame.text
             else:
                 return None
-        
-        if get_slide_notes(slide1) != get_slide_notes(slide2) and examine_note:
+
+        if get_slide_notes(slide1).strip() != get_slide_notes(slide2).strip() and examine_note:
             return 0
         # check if the shapes are the same
         for shape1, shape2 in zip(slide1.shapes, slide2.shapes):
             if examine_title_bottom_position:
                 if hasattr(shape1, "text") and hasattr(shape2, "text") and shape1.text == shape2.text:
                     if shape1.text == "Product Comparison" and (shape1.top <= shape2.top or shape1.top < 3600000):
                         return 0
                 elif shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
                     return 0
-            
+
             if examine_table_bottom_position:
                 if slide_idx == 3 and shape1.shape_type == 19 and shape2.shape_type == 19:
                     if shape1.top <= shape2.top or shape1.top < 3600000:
                         return 0
                 elif shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
                     return 0
-                    
+
             if examine_right_position:
                 if slide_idx == 2 and not hasattr(shape1, "text") and not hasattr(shape2, "text"):
                     if shape1.left <= shape2.left or shape1.left < 4320000:
                         return 0
 
             if examine_top_position:
                 if slide_idx == 2 and shape1.shape_type == 13 and shape2.shape_type == 13:
-                        if shape1.top >= shape2.top or shape1.top > 1980000:
-                            return 0
+                    if shape1.top >= shape2.top or shape1.top > 1980000:
+                        return 0
                 elif shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
                     return 0
-            
+
             if examine_shape_for_shift_size:
                 if shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
-                    if not (hasattr(shape1, "text") and hasattr(shape2, "text") and shape1.text == shape2.text and shape1.text == "Elaborate on what you want to discuss."):
+                    if not (hasattr(shape1, "text") and hasattr(shape2,
+                                                                "text") and shape1.text == shape2.text and shape1.text == "Elaborate on what you want to discuss."):
                         return 0
-                                
-            if (shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height) and examine_shape:
+
+            if (
+                    shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height) and examine_shape:
                 return 0
-            
+
             if examine_image_size:
                 if shape1.shape_type == 13 and shape2.shape_type == 13:
                     if shape1.width != shape2.width or shape1.height != shape2.height:
                         return 0
                 elif shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
                     return 0
-            
+
             if examine_modify_height:
-                if not hasattr(shape1, "text") and not hasattr(shape2, "text") or shape1.shape_type == 5 and shape2.shape_type == 5:
+                if not hasattr(shape1, "text") and not hasattr(shape2,
+                                                               "text") or shape1.shape_type == 5 and shape2.shape_type == 5:
                     if shape1.height != shape2.height:
                         return 0
                 elif shape1.left != shape2.left or shape1.top != shape2.top or shape1.width != shape2.width or shape1.height != shape2.height:
                     return 0
 
             if hasattr(shape1, "text") and hasattr(shape2, "text"):
-                if shape1.text != shape2.text and examine_text:
-                    return 0    
-                
-                # check if the paragraphs are the same
+                if shape1.text.strip() != shape2.text.strip() and examine_text:
+                    return 0
+
+                    # check if the paragraphs are the same
                 for para1, para2 in zip(shape1.text_frame.paragraphs, shape2.text_frame.paragraphs):
                     if para1.alignment != para2.alignment and examine_alignment:
                         return 0
-                        
+
                     # check if the runs are the same
                     if para1.text != para2.text and examine_text:
                         return 0
 
                     if para1.level != para2.level and examine_indent:
                         return 0
 
                     for run1, run2 in zip(para1.runs, para2.runs):
 
                         # check if the font properties are the same                        
-                        if run1.font.name != run2.font.name and examine_font_name:                            
+                        if run1.font.name != run2.font.name and examine_font_name:
                             return 0
 
                         if run1.font.size != run2.font.size and examine_font_size:
                             return 0
 
                         if run1.font.bold != run2.font.bold and examine_font_bold:
                             return 0
@@ -301,18 +305,17 @@
 
                                 text = "".join(t.text for t in paragraph.findall('.//a:t', namespaces))
 
                                 bullets.append((lvl, char, text, color))
 
                             return bullets
 
-                        if examine_bullets and _extract_bullets(run1.part.blob.decode('utf-8')) != _extract_bullets(run2.part.blob.decode('utf-8')):
+                        if examine_bullets and _extract_bullets(run1.part.blob.decode('utf-8')) != _extract_bullets(
+                                run2.part.blob.decode('utf-8')):
                             return 0
-                        
-
 
                     # fixme: Actually there are more properties to be compared, we can add them later via parsing the xml data
 
     return 1
 
 
 def check_strikethrough(pptx_path, rules):
@@ -520,19 +523,7 @@
             else:
                 return 0
 
     except ET.ParseError as e:
         logger.error(f"Error parsing XML: {e}")
     except FileNotFoundError:
         logger.error(f"File not found: {pptx_file}")
-
-
-if __name__ == '__main__':
-    # print(compare_pptx_files(
-    #     r"C:\Users\tianbaox\Desktop\DesktopEnv\cache\550ce7e7-747b-495f-b122-acdc4d0b8e54\New_Club_Spring_2018_Training_Gold.pptx",
-    #     r"C:\Users\tianbaox\Desktop\DesktopEnv\cache\550ce7e7-747b-495f-b122-acdc4d0b8e54\New_Club_Spring_2018_Training_Gold.pptx"))
-    # print(evaluate_presentation_fill_to_rgb_distance(r"C:\Users\tianbaox\Desktop\DesktopEnv\cache\3b27600c-3668-4abd-8f84-7bcdebbccbdb\lec17-gui-events.pptx", {"rgb": (0, 0, 255)}))
-    # print(check_auto_saving_time(r"C:\Users\tianbaox\Desktop\DesktopEnv\cache\2cd43775-7085-45d8-89fa-9e35c0a915cf\registrymodifications.xcu", {"minutes": 3}))
-    print(compare_pptx_files(
-        r"D:\NJU\HKUNLP\Desktop-Env\DesktopEnv\cache\08aced46-45a2-48d7-993b-ed3fb5b32302\22_6_Gold.pptx",
-        r"D:\NJU\HKUNLP\Desktop-Env\DesktopEnv\cache\08aced46-45a2-48d7-993b-ed3fb5b32302\22_6.pptx",
-        examine_shape=False))
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/table.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import functools
 import itertools
 import logging
 import os.path
 # import operator
 from numbers import Number
 from typing import Any, Union, cast, Callable, Iterable
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Set
 
 import openpyxl
 import pandas as pd
 from openpyxl import Workbook
 from openpyxl.cell.cell import Cell
-# from openpyxl.worksheet.cell_range import MultiCellRange
+from openpyxl.utils import get_column_letter
+from openpyxl.worksheet.cell_range import MultiCellRange
 from openpyxl.worksheet.datavalidation import DataValidation
 from openpyxl.worksheet.worksheet import Worksheet
+from rapidfuzz import fuzz
 
-from .utils import _match_value_to_rule, _read_cell_style, read_cell_value
-from .utils import load_charts, load_sparklines, load_rows_or_cols, load_xlsx_styles\
-                 , load_filters, load_pivot_tables
+from desktop_env.evaluators.metrics.utils import _match_value_to_rule, _read_cell_style, read_cell_value
+from desktop_env.evaluators.metrics.utils import load_charts, load_sparklines, load_rows_or_cols, load_xlsx_styles \
+    , load_filters, load_pivot_tables
 
 # from openpyxl.utils import coordinate_to_tuple
 
 logger = logging.getLogger("desktopenv.metric.table")
 
 BOOK = Union[pd.ExcelFile, Workbook, str]
 
@@ -29,24 +31,33 @@
 def _parse_sheet_idx(sheet_idx: Union[int, str]
                      , result: BOOK, expected: BOOK
                      , result_sheet_names: List[str]
                      , expected_sheet_names: List[str]
                      ) -> Tuple[BOOK, str]:
     #  function _parse_sheet_idx {{{ # 
     if isinstance(sheet_idx, int):
-        index: str = result_sheet_names[sheet_idx]
+        try:
+            index: str = result_sheet_names[sheet_idx]
+        except:
+            index = ""
         book: BOOK = result
     elif sheet_idx.startswith("RI"):
-        index: str = result_sheet_names[int(sheet_idx[2:])]
+        try:
+            index: str = result_sheet_names[int(sheet_idx[2:])]
+        except:
+            index = ""
         book: BOOK = result
     elif sheet_idx.startswith("RN"):
         index: str = sheet_idx[2:]
         book: BOOK = result
     elif sheet_idx.startswith("EI"):
-        index: str = expected_sheet_names[int(sheet_idx[2:])]
+        try:
+            index: str = expected_sheet_names[int(sheet_idx[2:])]
+        except:
+            index = ""
         book: BOOK = expected
     elif sheet_idx.startswith("EN"):
         index: str = sheet_idx[2:]
         book: BOOK = expected
     else:
         logger.error("Unrecognized sheet index")
         raise ValueError("Unrecognized sheet index")
@@ -55,32 +66,37 @@
 
 
 SHEET = Union[pd.DataFrame, Worksheet, List[str]]
 
 
 def _load_sheet(book: BOOK, index: str) -> SHEET:
     #  function _load_sheet {{{ # 
-    if isinstance(book, str):
-        book: str = cast(str, book)
-        csv_name: str = "{:}-{:}.csv".format(os.path.splitext(book)[0], index)
-
-        with open(csv_name) as f:
-            csv_lines: List[str] = list(itertools.dropwhile(lambda l: len(l) == 0
-                                                            , map(lambda l: l.strip()
-                                                                  , reversed(f.read().splitlines())
-                                                                  )
-                                                            )
-                                        )
-        return csv_lines
-    if isinstance(book, pd.ExcelFile):
-        return pd.read_excel(book, index)
-    if isinstance(book, Workbook):
-        return book[index]
-    logger.error("Not supported workbook format")
-    raise NotImplementedError("Not supported workbook format")
+    try:
+        if isinstance(book, str):
+            book: str = cast(str, book)
+            csv_name: str = "{:}-{:}.csv".format(os.path.splitext(book)[0], index)
+
+            with open(csv_name) as f:
+                csv_lines: List[str] = list(itertools.dropwhile(lambda l: len(l) == 0
+                                                                , map(lambda l: l.strip()
+                                                                      , reversed(f.read().splitlines())
+                                                                      )
+                                                                )
+                                            )
+            return csv_lines
+        if isinstance(book, pd.ExcelFile):
+            return pd.read_excel(book, index)
+        if isinstance(book, Workbook):
+            return book[index]
+        logger.error("Not supported workbook format")
+        raise NotImplementedError("Not supported workbook format")
+    except NotImplementedError as e:
+        raise e
+    except:
+        return None
     #  }}} function _load_sheet # 
 
 
 def compare_table(result: str, expected: str = None, **options) -> float:
     #  function compare_table {{{ # 
     """
     Args:
@@ -104,15 +120,14 @@
         xlworkbookr: Workbook = openpyxl.load_workbook(filename=result)
         pdworkbookr = pd.ExcelFile(result)
     except:
         return 0.
     worksheetr_names: List[str] = pdworkbookr.sheet_names
 
     if expected is not None:
-
         xlworkbooke: Workbook = openpyxl.load_workbook(filename=expected)
         pdworkbooke = pd.ExcelFile(expected)
         worksheete_names: List[str] = pdworkbooke.sheet_names
     else:
         xlworkbooke: Workbook = None
         pdworkbooke = None
         worksheete_names: List[str] = None
@@ -135,41 +150,105 @@
         elif r["type"] == "sheet_data":
             #  Compare Sheet Data by Internal Value {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
             # precision: int as number of decimal digits, default to 4
 
             error_limit: int = r.get("precision", 4)
-            sheet1: pd.DataFrame = _load_sheet(*parse_idx(r["sheet_idx0"], pdworkbookr, pdworkbooke)).round(error_limit)
-            sheet2: pd.DataFrame = _load_sheet(*parse_idx(r["sheet_idx1"], pdworkbookr, pdworkbooke)).round(error_limit)
+            sheet1: pd.DataFrame = _load_sheet(*parse_idx(r["sheet_idx0"], pdworkbookr, pdworkbooke))
+            if sheet1 is None:
+                return 0.
+            sheet2: pd.DataFrame = _load_sheet(*parse_idx(r["sheet_idx1"], pdworkbookr, pdworkbooke))
+
+            sheet1 = sheet1.round(error_limit)
+            sheet2 = sheet2.round(error_limit)
             metric: bool = sheet1.equals(sheet2)
             logger.debug("Sheet1: \n%s", str(sheet1))
             logger.debug("Sheet2: \n%s", str(sheet2))
             try:
-                logger.debug("Sheet1 =v= Sheet2: \n%s", str(sheet1==sheet2))
+                logger.debug("Sheet1 =v= Sheet2: \n%s", str(sheet1 == sheet2))
             except:
                 logger.debug("Sheet1 =/v= Sheet2")
             logger.debug("Assertion: %s =v= %s - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
             #  }}} Compare Sheet Data by Internal Value # 
 
         elif r["type"] == "sheet_print":
             #  Compare Sheet Data by Printed Value {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
             # ignore_case: optional, defaults to False
 
             sheet1: List[str] = _load_sheet(*parse_idx(r["sheet_idx0"], result, expected))
+            if sheet1 is None:
+                return 0.
             sheet2: List[str] = _load_sheet(*parse_idx(r["sheet_idx1"], result, expected))
             if r.get("ignore_case", False):
                 sheet1 = [l.lower() for l in sheet1]
                 sheet2 = [l.lower() for l in sheet2]
             metric: bool = sheet1 == sheet2
             logger.debug("Assertion: %s =p= %s - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
             #  }}} Compare Sheet Data by Printed Value # 
 
+        elif r["type"] == "sheet_fuzzy":
+            #  Fuzzy Match for Ranges {{{ # 
+            # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
+            # sheet_idx1: as sheet_idx0
+            # rules: list of dict, each dict is like
+            #   { "range": ["A1:B6", "C2:E5"],
+            #     "type": "includes" | "included_by" | "fuzzy_match" | "exact_match", # 0 includes 1, 0 includes_by 1
+            #     "threshold": 85, // for fuzzy match
+            #     "ignore_case": true | false,
+            #     "ignore_chars": " ()", # filtered out
+            #     "trim_leadings": "+ ", # filtered by lstrip
+            #     "trim_trailings": "", # filtered by rstrip
+            #     "normalization": [["Rd", "Road"]], # filtered by replace
+            #   }
+
+            sheet1: Tuple[BOOK, str] = parse_idx(r["sheet_idx0"], result, expected)
+            sheet2: Tuple[BOOK, str] = parse_idx(r["sheet_idx1"], result, expected)
+            total_metric = True
+            for rl in r["rules"]:
+                for rng in MultiCellRange(rl["range"]):
+                    for cdn in rng.cells:
+                        coordinate: str = "{:}{:d}".format(get_column_letter(cdn[1]), cdn[0])
+                        value1: str = str(read_cell_value(*sheet1, coordinate))
+                        value2: str = str(read_cell_value(*sheet2, coordinate))
+                        logger.debug("%s: %s vs %s", cdn, value1, value2)
+
+                        for rplc in rl.get("normalization", []):
+                            value1 = value1.replace(rplc[0], rplc[1])
+                            value2 = value2.replace(rplc[0], rplc[1])
+                        if "trim_leadings" in rl:
+                            value1 = value1.lstrip(rl["trim_leadings"])
+                            value2 = value2.lstrip(rl["trim_leadings"])
+                        if "trim_trailings" in rl:
+                            value1 = value1.rstrip(rl["trim_trailings"])
+                            value2 = value2.rstrip(rl["trim_trailings"])
+                        if "ignore_chars" in rl:
+                            ignore_chars: Set[str] = set(rl["ignore_chars"])
+                            value1 = "".join(filter(lambda ch: ch not in ignore_chars, value1))
+                            value2 = "".join(filter(lambda ch: ch not in ignore_chars, value2))
+                        if rl.get("ignore_case", False):
+                            value1 = value1.lower()
+                            value2 = value2.lower()
+
+                        if rl["type"] == "includes":
+                            metric: bool = value2 in value1
+                        elif rl["type"] == "included_by":
+                            metric: bool = value1 in value2
+                        elif rl["type"] == "fuzzy_match":
+                            metric: bool = fuzz.ratio(value1, value2) >= rl.get("threshold", 85.)
+                        elif rl["type"] == "exact_match":
+                            metric: bool = value1 == value2
+                        total_metric = total_metric and metric
+
+            metric: bool = total_metric
+            logger.debug("Assertion: %s =~= %s - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
+            #  }}} Fuzzy Match for Ranges # 
+
         elif r["type"] == "sparkline":
             #  Compare Sparklines {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
 
             sparkline1: Dict[str, str] = load_sparklines(*parse_idx(r["sheet_idx0"], result, expected))
             sparkline2: Dict[str, str] = load_sparklines(*parse_idx(r["sheet_idx1"], result, expected))
@@ -191,33 +270,35 @@
 
         elif r["type"] == "style":
             #  Compare Style (Also Conditional Formatiing) {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
             # props: list of str indicating concerned styles, see utils._read_cell_style
 
-            sheet_idx1: Tuple[Book, str] = parse_idx(r["sheet_idx0"], xlworkbookr, xlworkbooke)
+            sheet_idx1: Tuple[BOOK, str] = parse_idx(r["sheet_idx0"], xlworkbookr, xlworkbooke)
             book_name1: str = parse_idx(r["sheet_idx0"], result, expected)[0]
             styles1: Dict[str, List[Any]] = load_xlsx_styles(*sheet_idx1, book_name1, **r)
 
-            sheet_idx2: Tuple[Book, str] = parse_idx(r["sheet_idx1"], xlworkbookr, xlworkbooke)
+            sheet_idx2: Tuple[BOOK, str] = parse_idx(r["sheet_idx1"], xlworkbookr, xlworkbooke)
             book_name2: str = parse_idx(r["sheet_idx1"], result, expected)[0]
             styles2: Dict[str, List[Any]] = load_xlsx_styles(*sheet_idx2, book_name2, **r)
             # number_formats1: List[str] = [c.number_format.lower() for col in sheet1.iter_cols() for c in col if c.value is not None and c.data_type=="n"]
             # number_formats2: List[str] = [c.number_format.lower() for col in sheet2.iter_cols() for c in col if c.value is not None and c.data_type=="n"]
             metric: bool = styles1 == styles2
             logger.debug("Assertion: %s.style == %s.style - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
             #  }}} Compare Style (Also Conditional Formatiing) # 
 
         elif r["type"] == "freeze":
             #  Compare Freezing {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
 
             sheet1: Worksheet = _load_sheet(*parse_idx(r["sheet_idx0"], xlworkbookr, xlworkbooke))
+            if sheet1 is None:
+                return 0.
             sheet2: Worksheet = _load_sheet(*parse_idx(r["sheet_idx1"], xlworkbookr, xlworkbooke))
             metric: bool = sheet1.freeze_panes == sheet2.freeze_panes
             logger.debug("Assertion: %s.freeze(%s) == %s.freeze(%s) - %s"
                          , r["sheet_idx0"], sheet1.freeze_panes
                          , r["sheet_idx1"], sheet2.freeze_panes
                          , metric
                          )
@@ -226,14 +307,16 @@
         elif r["type"] == "zoom":
             #  Check Zooming {{{ # 
             # sheet_idx: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # method: str
             # ref: value
 
             sheet: Worksheet = _load_sheet(*parse_idx(r["sheet_idx"], xlworkbookr, xlworkbooke))
+            if sheet is None:
+                return 0.
             zoom_scale: Number = sheet.sheet_view.zoomScale or 100.
             metric: bool = _match_value_to_rule(zoom_scale, r)
             logger.debug("Assertion: %s.zoom(%.1f) %s %.1f - %s", r["sheet_idx"], zoom_scale, r["method"], r["ref"],
                          metric)
             #  }}} Check Zooming # 
 
         elif r["type"] == "data_validation":
@@ -254,14 +337,16 @@
             #     * errorTitle
             #     * errorStyle
             #     * prompt
             #     * promptTitle
             #     * imeMode
 
             sheet: Worksheet = _load_sheet(*parse_idx(r["sheet_idx"], xlworkbookr, xlworkbooke))
+            if sheet is None:
+                return 0.
             data_validators: List[DataValidation] = sheet.data_validations.dataValidation
 
             total_metric = len(data_validators) >= len(r["dv_props"])
             for dat_vldt in data_validators:
                 metric = False
                 for prpt in r["dv_props"]:
                     metric = metric or all(_match_value_to_rule(getattr(dat_vldt, attrbt)
@@ -320,38 +405,40 @@
         elif r["type"] == "filter":
             #  Compare Filters {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
 
             filters1: Dict[str, Any] = load_filters(*parse_idx(r["sheet_idx0"], xlworkbookr, xlworkbooke), **r)
             filters2: Dict[str, Any] = load_filters(*parse_idx(r["sheet_idx1"], xlworkbookr, xlworkbooke), **r)
-            metric: bool = filters1==filters2
+            metric: bool = filters1 == filters2
             logger.debug("Assertion: %s[filter] == %s[filter] - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
             #  }}} Compare Filters # 
 
         elif r["type"] == "pivot_table":
             #  Compare Pivot Tables {{{ # 
             # sheet_idx0: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # sheet_idx1: as sheet_idx0
             # pivot_props: list of str, see utils.load_pivot_tables
 
             pivots1: Dict[str, Any] = load_pivot_tables(*parse_idx(r["sheet_idx0"], xlworkbookr, xlworkbooke), **r)
             pivots2: Dict[str, Any] = load_pivot_tables(*parse_idx(r["sheet_idx1"], xlworkbookr, xlworkbooke), **r)
-            metric: bool = pivots1==pivots2
+            metric: bool = pivots1 == pivots2
             logger.debug("Assertion: %s[pivot]==%s[pivot] - %s", r["sheet_idx0"], r["sheet_idx1"], metric)
             #  }}} Compare Pivot Tables # 
 
         elif r["type"] == "check_cell":
             #  Check Cell Properties {{{ # 
             # sheet_idx: 0 == "RI0" == "RNSheet1" | "EI0" == "ENSheet1"
             # coordinate: str, "E3"
             # props: dict like {attribute: {"method": str, "ref": anything}}
             #   supported attributes: value & those supported by utils._read_cell_style
 
             sheet: Worksheet = _load_sheet(*parse_idx(r["sheet_idx"], xlworkbookr, xlworkbooke))
+            if sheet is None:
+                return 0.
             # data_frame: pd.DataFrame = _load_sheet(*parse_idx(r["sheet_idx"], pdworkbookr, pdworkbooke))
             cell: Cell = sheet[r["coordinate"]]
             metric: bool = True
             for prpt, rule in r["props"].items():
                 if prpt == "value":
                     val = read_cell_value(*parse_idx(r["sheet_idx"], result, expected), r["coordinate"])
                 else:
@@ -391,85 +478,40 @@
         result_lines = map(str.lower, result_lines)
         expected_lines = map(str.lower, expected_lines)
 
     metric: bool = list(result_lines) == list(expected_lines)
     return float(metric)
 
 
-if __name__ == '__main__':
-    import datetime
-    import sys
-
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
-
-    datetime_str: str = datetime.datetime.now().strftime("%Y%m%d@%H%M%S")
-
-    file_handler = logging.FileHandler(os.path.join("logs", "normal-{:}.log".format(datetime_str)))
-    debug_handler = logging.FileHandler(os.path.join("logs", "debug-{:}.log".format(datetime_str)))
-    stdout_handler = logging.StreamHandler(sys.stdout)
-    sdebug_handler = logging.FileHandler(os.path.join("logs", "sdebug-{:}.log".format(datetime_str)))
-
-    file_handler.setLevel(logging.INFO)
-    debug_handler.setLevel(logging.DEBUG)
-    stdout_handler.setLevel(logging.INFO)
-    sdebug_handler.setLevel(logging.DEBUG)
-
-    formatter = logging.Formatter(
-        fmt="\x1b[1;33m[%(asctime)s \x1b[31m%(levelname)s \x1b[32m%(module)s/%(lineno)d-%(processName)s\x1b[1;33m] \x1b[0m%(message)s")
-    file_handler.setFormatter(formatter)
-    debug_handler.setFormatter(formatter)
-    stdout_handler.setFormatter(formatter)
-    sdebug_handler.setFormatter(formatter)
-
-    stdout_handler.addFilter(logging.Filter("desktopenv"))
-    sdebug_handler.addFilter(logging.Filter("desktopenv"))
-
-    logger.addHandler(file_handler)
-    logger.addHandler(debug_handler)
-    logger.addHandler(stdout_handler)
-    logger.addHandler(sdebug_handler)
-
-    path1 = "snapshots/test/cache/4e6fcf72-daf3-439f-a232-c434ce416af6/Employee_Age_By_Birthday.xlsx"
-    path2 = "snapshots/test/cache/4e6fcf72-daf3-439f-a232-c434ce416af6/Employee_Age_By_Birthday_gold.xlsx"
-    rules = [ { "type": "sheet_data"
-              , "sheet_idx0": 0
-              , "sheet_idx1": "EI0"
-              }
-            ]
-    print(compare_table(path1, path2
-                        , rules=rules
-                        )
-          )
-    print(compare_table(path2, path2
-                        , rules=rules
-                        )
-          )
-
-    # Row Properties
-    # path1 = "../../任务数据/LibreOffice Calc/Date_Budget_Variance_HideNA.xlsx"
-    # path2 = "../../任务数据/LibreOffice Calc/Date_Budget_Variance_HideNA_gold.xlsx"
-    # workbook: Workbook = openpyxl.load_workbook(filename=path1)
-    # worksheet: Worksheet = workbook.active
-    # for r_no, dms in worksheet.column_dimensions.items():
-    # print(r_no, type(r_no), type(dms), dms.hidden)
-
-    # Conditional Formats
-    # import formulas
-    # path1 = "../../任务数据/LibreOffice Calc/Calendar_Highlight_Weekend_Days.xlsx"
-    # path2 = "../../任务数据/LibreOffice Calc/Calendar_Highlight_Weekend_Days_gold.xlsx"
-    # path3 = "../../任务数据/LibreOffice Calc/Calendar_Highlight_Weekend_Days_gold_test.xlsx"
-    # workbook: Workbook = openpyxl.load_workbook(filename=path2)
-    # worksheet: Worksheet = workbook.active
-    # print(worksheet.conditional_formatting)
-    # for itm in worksheet.conditional_formatting:
-    # print(itm.cells)
-    # for r in itm.rules:
-    # print( r.type, r.formula, r.dxf.font.color.rgb
-    # , r.dxf.fill.fgColor.rgb, r.dxf.fill.bgColor.rgb
-    # )
-    # condition = formulas.Parser().ast("=" + r.formula[0])[1].compile()
-    ##print(r.type, r.operator, r.dxfId, r.dxf)
-    # for r in itm.cells:
-    # for c in r.cells:
-    # value = worksheet.cell(row=c[0], column=c[1]).value
-    # print(value, condition(str(value)))
+def compare_conference_city_in_order(actual_city_list_path, expected_city):
+    expected_city_list = expected_city["expected"]
+    wb = openpyxl.load_workbook(actual_city_list_path)
+    sheet = wb.active
+    actual_city_list = []
+    for row in sheet["C2:C22"]:
+        for cell in row:
+            actual_city_list.append(cell.value)
+    # expected_city is the city that we want to compare with the actual city list
+    # must in order index
+    # debug
+    try:
+        for i in range(len(actual_city_list)):
+            if isinstance(expected_city_list[i], str):
+                if expected_city_list[i] not in actual_city_list[i]:
+                    logger.debug(f"Expected city {expected_city_list[i]}; Actual city {actual_city_list[i]}")
+                    print(f"Expected city {expected_city_list[i]}; Actual city {actual_city_list[i]}")
+                    return 0.
+
+
+            elif isinstance(expected_city_list[i], List):
+                if not any(possible_str in actual_city_list[i] for possible_str in expected_city_list[i]):
+                    logger.debug(f"Expected city {expected_city_list[i]}; Actual city {actual_city_list[i]}")
+                    print(f"Expected city {expected_city_list[i]}; Actual city {actual_city_list[i]}")
+                    return 0.
+
+            else:
+                raise TypeError("Expected city should be a string or a list of strings")
+
+    except:
+        return 0.
+
+    return 1.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/utils.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import builtins
+import datetime
 import functools
 import itertools
 import logging
 import operator
 import re
 import zipfile
+import pandas as pd
 from typing import Any, TypeVar, Union, Iterable, Optional, Callable
 from typing import Dict, List, Set, Match, Tuple, Pattern
 from urllib.parse import urlparse, urlunparse
 
 import formulas
 import lxml.cssselect
 import lxml.etree
@@ -120,18 +122,22 @@
     for ch in charts:
         series: List[str] = []
         for ser in ch.series:
             if hasattr(ser.val, "numRef") and hasattr(ser.val.numRef, "f"):
                 value_str: str = ser.val.numRef.f
             elif hasattr(ser.val, "strRef") and hasattr(ser.val.strRef, "f"):
                 value_str: str = ser.val.strRef.f
+            else:
+                value_str: str = ""
             if hasattr(ser.cat, "numRef") and hasattr(ser.cat.numRef, "f"):
                 categ_str: str = ser.cat.numRef.f
             elif hasattr(ser.cat, "strRef") and hasattr(ser.cat.strRef, "f"):
                 categ_str: str = ser.cat.strRef.f
+            else:
+                categ_str: str = ""
             series.append("{:},{:}".format(value_str, categ_str))
         series: str = ";".join(series)
 
         # TODO: maybe more aspects, like chart type
         info: Dict[str, Any] = {}
 
         if "title" in chart_props:
@@ -266,26 +272,29 @@
 
         pivot_set[source] = info
     logger.debug(".[%s].pivots: %s", sheet_name, repr(pivot_set))
     return pivot_set
     #  }}} function load_pivot_tables # 
 
 
-_shared_str_selector = lxml.cssselect.CSSSelector("oo|sst>oo|si>oo|t", namespaces=_xlsx_ns_mapping)
+_shared_str_selector = lxml.cssselect.CSSSelector("oo|sst>oo|si", namespaces=_xlsx_ns_mapping)
+_shared_str_value_selector = lxml.cssselect.CSSSelector("oo|t", namespaces=_xlsx_ns_mapping)
 
 
 def read_cell_value(xlsx_file: str, sheet_name: str, coordinate: str) -> Any:
     #  read_cell_value {{{ # 
     try:
         with zipfile.ZipFile(xlsx_file, "r") as z_f:
             try:
                 with z_f.open("xl/sharedStrings.xml") as f:
                     shared_str_xml: _Element = lxml.etree.fromstring(f.read())
                     str_elements: List[_Element] = _shared_str_selector(shared_str_xml)
-                    shared_strs: List[str] = [elm.text for elm in str_elements]
+                    shared_strs: List[str] = [ "".join(t.text for t in _shared_str_value_selector(elm))\
+                                           for elm in str_elements
+                                             ]
             except:
                 logger.debug("Read shared strings error: %s", xlsx_file)
 
             with z_f.open("xl/workbook.xml") as f:
                 workbook_database: _Element = lxml.etree.fromstring(f.read())
                 sheets: List[_Element] = _sheet_name_selector(workbook_database)
                 sheet_names: Dict[str, str] = {sh.get("name"): sh.get("sheetId") for sh in sheets}
@@ -303,22 +312,23 @@
         return None
 
     cell: Dict[str, str] = xmltodict.parse(lxml.etree.tostring(cell, encoding="unicode")
                                            , process_namespaces=True
                                            , namespaces=_xlsx_ns_imapping
                                            )
     logger.debug("%s.%s[%s]: %s", xlsx_file, sheet_name, coordinate, repr(cell))
-    if "@t" not in cell["c"]:
+    try:
+        if "@t" not in cell["c"] or cell["c"]["@t"] == "n":
+            return float(cell["c"]["v"])
+        if cell["c"]["@t"] == "s":
+            return shared_strs[int(cell["c"]["v"])]
+        if cell["c"]["@t"] == "str":
+            return cell["c"]["v"]
+    except (KeyError, ValueError):
         return None
-    if cell["c"]["@t"] == "s":
-        return shared_strs[int(cell["c"]["v"])]
-    if cell["c"]["@t"] == "n":
-        return float(cell["c"]["v"])
-    if cell["c"]["@t"] == "str":
-        return cell["c"]["v"]
     #  }}} read_cell_value # 
 
 
 # Supported Styles:
 # number_format
 # font_name - str
 # font_family - float
@@ -583,28 +593,28 @@
             "ref": V as ref value
           }
 
     Returns:
         bool
     """
 
-    if rule["method"].startswith("re"):
+    if rule["method"].startswith("re"): # re.FLAGs
         flags: List[str] = rule["method"].split(".")[1:]
         flags: Iterable[re.RegexFlag] = (getattr(re, fl) for fl in flags)
         flag: re.RegexFlag = functools.reduce(operator.or_, flags, re.RegexFlag(0))
         logger.debug("REFLAG: %s", repr(flag))
 
         match_: Optional[Match[str]] = re.search(rule["ref"], value, flag)
         return match_ is not None
     if rule["method"] in {"eq", "ne"
         , "le", "lt"
         , "ge", "gt"
                           }:
         return getattr(operator, rule["method"])(value, rule["ref"])
-    if rule["method"].startswith("approx"):
+    if rule["method"].startswith("approx"): # approx:THRESHOLD
         threshold: float = float(rule["method"].split(":")[1])
         logger.debug("Approx: TH%f, REF%f, VAL%s", threshold, rule["ref"], repr(value))
         try:
             value = float(value)
         except (ValueError, TypeError):
             return False
         else:
```

### Comparing `desktop_env-0.1.2/desktop_env/evaluators/metrics/vlc.py` & `desktop_env-0.1.3/desktop_env/evaluators/metrics/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.2/desktop_env.egg-info/SOURCES.txt` & `desktop_env-0.1.3/desktop_env.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 desktop_env/controllers/python.py
 desktop_env/controllers/setup.py
 desktop_env/envs/__init__.py
 desktop_env/envs/actions.py
 desktop_env/envs/desktop_env.py
 desktop_env/evaluators/__init__.py
 desktop_env/evaluators/getters/__init__.py
+desktop_env/evaluators/getters/calc.py
 desktop_env/evaluators/getters/chrome.py
 desktop_env/evaluators/getters/file.py
 desktop_env/evaluators/getters/general.py
 desktop_env/evaluators/getters/gimp.py
 desktop_env/evaluators/getters/impress.py
 desktop_env/evaluators/getters/info.py
 desktop_env/evaluators/getters/misc.py
@@ -28,14 +29,15 @@
 desktop_env/evaluators/metrics/__init__.py
 desktop_env/evaluators/metrics/basic_os.py
 desktop_env/evaluators/metrics/chrome.py
 desktop_env/evaluators/metrics/docs.py
 desktop_env/evaluators/metrics/general.py
 desktop_env/evaluators/metrics/gimp.py
 desktop_env/evaluators/metrics/libreoffice.py
+desktop_env/evaluators/metrics/others.py
 desktop_env/evaluators/metrics/pdf.py
 desktop_env/evaluators/metrics/slides.py
 desktop_env/evaluators/metrics/table.py
 desktop_env/evaluators/metrics/thunderbird.py
 desktop_env/evaluators/metrics/utils.py
 desktop_env/evaluators/metrics/vlc.py
 desktop_env/evaluators/metrics/vscode.py
```

### Comparing `desktop_env-0.1.2/desktop_env.egg-info/requires.txt` & `desktop_env-0.1.3/desktop_env.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -28,17 +28,20 @@
 opencv-python
 ImageHash
 scikit-image
 librosa
 pymupdf
 chardet
 playwright
-backoff
 formulas
 pydrive
 fastdtw
 odfpy
-openai
 func-timeout
 beautifulsoup4
-dashscope
-google-generativeai
+PyYaml
+mutagen
+easyocr
+borb
+pypdf2
+pdfplumber
+wrapt_timeout_decorator
```

### Comparing `desktop_env-0.1.2/setup.py` & `desktop_env-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         except subprocess.CalledProcessError as e:
             print("Failed to run 'playwright install'. Please run 'playwright install' manually.")
             print(e)
 
 
 setup(
     name="desktop_env",
-    version="0.1.2",
+    version="0.1.3",
     author="Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.",
     author_email="tianbaoxiexxx@gmail.com",
     description="The package provides a desktop environment for setting and evaluating desktop automation tasks.",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/xlang-ai/desktop_env",
     packages=find_packages(),
@@ -68,22 +68,25 @@
         "opencv-python",
         "ImageHash",
         "scikit-image",
         "librosa",
         "pymupdf",
         "chardet",
         "playwright",
-        "backoff",
         "formulas",
         "pydrive",
         "fastdtw",
         "odfpy",
-        "openai",
         "func-timeout",
         "beautifulsoup4",
-        "dashscope",
-        "google-generativeai"
+        "PyYaml",
+        "mutagen",
+        "easyocr",
+        "borb",
+        "pypdf2",
+        "pdfplumber",
+        "wrapt_timeout_decorator"
     ],
     cmdclass={
         'install': InstallPlaywrightCommand,  # Use the custom install command
     },
 )
```

