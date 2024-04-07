# Comparing `tmp/nodeorc-0.1.0.tar.gz` & `tmp/nodeorc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeorc-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nodeorc-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nodeorc-0.1.0.tar` & `nodeorc-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      187 2024-04-05 15:37:19.397963 nodeorc-0.1.0/.env
--rw-r--r--   0        0        0     1146 2024-04-05 15:37:19.397963 nodeorc-0.1.0/.github/ISSUE_TEMPLATE/issue-report.md
--rw-r--r--   0        0        0     1547 2024-04-05 15:37:19.397963 nodeorc-0.1.0/.github/workflows/publish-release-pypi.yml
--rw-r--r--   0        0        0     2244 2024-04-05 15:37:19.397963 nodeorc-0.1.0/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0     3129 2024-04-05 15:37:19.397963 nodeorc-0.1.0/.gitignore
--rw-r--r--   0        0        0      559 2024-04-05 15:37:19.397963 nodeorc-0.1.0/Dockerfile
--rw-r--r--   0        0        0    34523 2024-04-05 15:37:19.397963 nodeorc-0.1.0/LICENSE
--rw-r--r--   0        0        0    27132 2024-04-05 15:37:19.397963 nodeorc-0.1.0/README.rst
--rw-r--r--   0        0        0     1594 2024-04-05 15:37:19.397963 nodeorc-0.1.0/docker-compose-test.yml
--rw-r--r--   0        0        0  2525884 2024-04-05 15:37:19.409963 nodeorc-0.1.0/docs/static/front.jpg
--rw-r--r--   0        0        0     2718 2024-04-05 15:37:19.409963 nodeorc-0.1.0/mockserver/initializerJson.json
--rw-r--r--   0        0        0       93 2024-04-05 15:37:19.409963 nodeorc-0.1.0/mockserver/mockserver.properties
--rw-r--r--   0        0        0      445 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/callbacks.py
--rw-r--r--   0        0        0     5959 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/config.py
--rw-r--r--   0        0        0      681 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/db/__init__.py
--rw-r--r--   0        0        0      292 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/db/active_config.py
--rw-r--r--   0        0        0      741 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/db/init_basedata.py
--rw-r--r--   0        0        0    10813 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/db/models.py
--rw-r--r--   0        0        0     3761 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/disk_mng.py
--rw-r--r--   0        0        0     2858 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/log.py
--rw-r--r--   0        0        0    10288 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/main.py
--rw-r--r--   0        0        0      959 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/__init__.py
--rw-r--r--   0        0        0     1629 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/callback.py
--rw-r--r--   0        0        0     6378 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/callback_url.py
--rw-r--r--   0        0        0     3966 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/config.py
--rw-r--r--   0        0        0     3301 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/storage.py
--rw-r--r--   0        0        0     4356 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/subtask.py
--rw-r--r--   0        0        0     6261 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/models/task.py
--rw-r--r--   0        0        0      104 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/tasks/__init__.py
--rw-r--r--   0        0        0    24284 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/tasks/local_task.py
--rw-r--r--   0        0        0     8694 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/tasks/task_form.py
--rw-r--r--   0        0        0     2675 2024-04-05 15:37:19.409963 nodeorc-0.1.0/nodeorc/utils.py
--rw-r--r--   0        0        0     1282 2024-04-05 15:37:19.409963 nodeorc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-05 15:37:19.409963 nodeorc-0.1.0/requirements.txt
--rw-r--r--   0        0        0      422 2024-04-05 15:37:19.409963 nodeorc-0.1.0/service/10-toggleusbstick.rules
--rw-r--r--   0        0        0     2467 2024-04-05 15:37:19.409963 nodeorc-0.1.0/service/usb-mount.sh
--rw-r--r--   0        0        0      184 2024-04-05 15:37:19.409963 nodeorc-0.1.0/service/usb-mount@.service
--rw-r--r--   0        0        0        0 2024-04-05 15:37:19.409963 nodeorc-0.1.0/settings/.gitkeep
--rw-r--r--   0        0        0      722 2024-04-05 15:37:19.409963 nodeorc-0.1.0/settings/config_template.json
--rwxr-xr-x   0        0        0    17944 2024-04-05 15:37:19.409963 nodeorc-0.1.0/setup.sh
--rw-r--r--   0        0        0     8907 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    60249 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/examples/ngwerere_transect.nc
--rw-r--r--   0        0        0      496 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_amqp_task.py
--rw-r--r--   0        0        0      802 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_callbacks.py
--rw-r--r--   0        0        0     2493 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_config.py
--rw-r--r--   0        0        0      875 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_disk_management.py
--rw-r--r--   0        0        0      128 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_io.py
--rw-r--r--   0        0        0      726 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_s3.py
--rw-r--r--   0        0        0      184 2024-04-05 15:37:19.409963 nodeorc-0.1.0/tests/test_task.py
--rw-r--r--   0        0        0    28609 1970-01-01 00:00:00.000000 nodeorc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-07 13:03:36.868016 nodeorc-0.1.1/.env
+-rw-r--r--   0        0        0     1146 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/ISSUE_TEMPLATE/issue-report.md
+-rw-r--r--   0        0        0     1547 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/workflows/publish-release-pypi.yml
+-rw-r--r--   0        0        0     2244 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0     3129 2024-04-07 13:03:36.872016 nodeorc-0.1.1/.gitignore
+-rw-r--r--   0        0        0      559 2024-04-07 13:03:36.872016 nodeorc-0.1.1/Dockerfile
+-rw-r--r--   0        0        0    34523 2024-04-07 13:03:36.872016 nodeorc-0.1.1/LICENSE
+-rw-r--r--   0        0        0    27141 2024-04-07 13:03:36.872016 nodeorc-0.1.1/README.rst
+-rw-r--r--   0        0        0     1594 2024-04-07 13:03:36.872016 nodeorc-0.1.1/docker-compose-test.yml
+-rw-r--r--   0        0        0  2525884 2024-04-07 13:03:36.880016 nodeorc-0.1.1/docs/static/front.jpg
+-rw-r--r--   0        0        0     2718 2024-04-07 13:03:36.880016 nodeorc-0.1.1/mockserver/initializerJson.json
+-rw-r--r--   0        0        0       93 2024-04-07 13:03:36.880016 nodeorc-0.1.1/mockserver/mockserver.properties
+-rw-r--r--   0        0        0      445 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/__init__.py
+-rw-r--r--   0        0        0     3705 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/callbacks.py
+-rw-r--r--   0        0        0     5959 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/config.py
+-rw-r--r--   0        0        0      681 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/active_config.py
+-rw-r--r--   0        0        0      741 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/init_basedata.py
+-rw-r--r--   0        0        0    10813 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/db/models.py
+-rw-r--r--   0        0        0     3761 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/disk_mng.py
+-rw-r--r--   0        0        0     2858 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/log.py
+-rw-r--r--   0        0        0    10288 2024-04-07 13:03:36.880016 nodeorc-0.1.1/nodeorc/main.py
+-rw-r--r--   0        0        0      959 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/__init__.py
+-rw-r--r--   0        0        0     1629 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/callback.py
+-rw-r--r--   0        0        0     6378 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/callback_url.py
+-rw-r--r--   0        0        0     3966 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/config.py
+-rw-r--r--   0        0        0     3301 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/storage.py
+-rw-r--r--   0        0        0     4356 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/subtask.py
+-rw-r--r--   0        0        0     6261 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/models/task.py
+-rw-r--r--   0        0        0      104 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/__init__.py
+-rw-r--r--   0        0        0    24586 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/local_task.py
+-rw-r--r--   0        0        0     8694 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/tasks/task_form.py
+-rw-r--r--   0        0        0     2764 2024-04-07 13:03:36.884016 nodeorc-0.1.1/nodeorc/utils.py
+-rw-r--r--   0        0        0     1282 2024-04-07 13:03:36.884016 nodeorc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-07 13:03:36.884016 nodeorc-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      422 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/10-toggleusbstick.rules
+-rw-r--r--   0        0        0     2467 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/usb-mount.sh
+-rw-r--r--   0        0        0      184 2024-04-07 13:03:36.884016 nodeorc-0.1.1/service/usb-mount@.service
+-rw-r--r--   0        0        0        0 2024-04-07 13:03:36.884016 nodeorc-0.1.1/settings/.gitkeep
+-rw-r--r--   0        0        0      722 2024-04-07 13:03:36.884016 nodeorc-0.1.1/settings/config_template.json
+-rwxr-xr-x   0        0        0    18699 2024-04-07 13:03:36.884016 nodeorc-0.1.1/setup.sh
+-rw-r--r--   0        0        0     8907 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    60249 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/examples/ngwerere_transect.nc
+-rw-r--r--   0        0        0      496 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_amqp_task.py
+-rw-r--r--   0        0        0      802 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_callbacks.py
+-rw-r--r--   0        0        0     2493 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_config.py
+-rw-r--r--   0        0        0      875 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_disk_management.py
+-rw-r--r--   0        0        0      128 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_io.py
+-rw-r--r--   0        0        0      726 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_s3.py
+-rw-r--r--   0        0        0      184 2024-04-07 13:03:36.884016 nodeorc-0.1.1/tests/test_task.py
+-rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.1/PKG-INFO
```

### Comparing `nodeorc-0.1.0/.github/ISSUE_TEMPLATE/issue-report.md` & `nodeorc-0.1.1/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/.github/workflows/publish-release-pypi.yml` & `nodeorc-0.1.1/.github/workflows/publish-release-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/.github/workflows/publish-test-pypi.yml` & `nodeorc-0.1.1/.github/workflows/publish-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/.gitignore` & `nodeorc-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/Dockerfile` & `nodeorc-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/LICENSE` & `nodeorc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/README.rst` & `nodeorc-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 installation, please download the setup.sh script from the latest release on the device on which you wish to install it,
 make the script executable and execute the script on a command line interface with the option ``--all``. The steps
 are outlined below:
 
 .. code-block:: shell
 
     # get script from latest release
-    wget https://github.com/localdevices/nodeorc/releases/latest/setup.sh
+    wget https://github.com/localdevices/nodeorc/releases/latest/download/setup.sh
     # make the setup script executable
     chmod +x setup.sh
     # execute script
     ./setup.sh --all
 
 The setup procedure will ask several inputs including the url and your username and password for the LiveOpenRiverCam
 server. Note that these credentials will not be stored on the device, but only used to receive a temporary access token
```

### Comparing `nodeorc-0.1.0/docker-compose-test.yml` & `nodeorc-0.1.1/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/docs/static/front.jpg` & `nodeorc-0.1.1/docs/static/front.jpg`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/mockserver/initializerJson.json` & `nodeorc-0.1.1/mockserver/initializerJson.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/callbacks.py` & `nodeorc-0.1.1/nodeorc/callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/config.py` & `nodeorc-0.1.1/nodeorc/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/db/__init__.py` & `nodeorc-0.1.1/nodeorc/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/db/init_basedata.py` & `nodeorc-0.1.1/nodeorc/db/init_basedata.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/db/models.py` & `nodeorc-0.1.1/nodeorc/db/models.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/disk_mng.py` & `nodeorc-0.1.1/nodeorc/disk_mng.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/log.py` & `nodeorc-0.1.1/nodeorc/log.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/main.py` & `nodeorc-0.1.1/nodeorc/main.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/__init__.py` & `nodeorc-0.1.1/nodeorc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/callback.py` & `nodeorc-0.1.1/nodeorc/models/callback.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/callback_url.py` & `nodeorc-0.1.1/nodeorc/models/callback_url.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/config.py` & `nodeorc-0.1.1/nodeorc/models/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/storage.py` & `nodeorc-0.1.1/nodeorc/models/storage.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/subtask.py` & `nodeorc-0.1.1/nodeorc/models/subtask.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/models/task.py` & `nodeorc-0.1.1/nodeorc/models/task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/tasks/local_task.py` & `nodeorc-0.1.1/nodeorc/tasks/local_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
             try:
                 h_a = get_water_level(
                     timestamp,
                     file_fmt=self.water_level_file_template,
                     datetime_fmt=self.settings["water_level_datetimefmt"],
                     allowed_dt=self.settings["allowed_dt"]
                 )
+                self.logger.info(f"Water level found with value {h_a} m.")
             except Exception as e:
                 message = f"Could not obtain a water level for date {timestamp.strftime('%Y%m%d')} at timestamp {timestamp.strftime('%Y%m%dT%H%M%S')}. Reason: {e}"
                 device.message = message
                 db.session.commit()
                 raise ValueError(message)
             # create the task object from all data
             task = create_task(
@@ -269,45 +270,48 @@
                 logger=self.logger
             )
             # set cur_path to tmp location (only used on exception)
             cur_path = os.path.join(task_path, filename)
             # process the task
             task.execute(task_path)
             # if the video was treated successfully, then we may move it to a location of interest if wanted
-            if self.disk_management.success_path:
+            if self.disk_management.results_path:
                 dst_path = os.path.join(
-                    self.disk_management.success_path,
+                    self.disk_management.results_path,
                     timestamp.strftime("%Y%m%d")
                 )
             # video is success, if task form is still CANDIDATE, upgrade to ACCEPTED
             config.patch_active_config_to_accepted()
             # perform the callbacks here only when video was successfully completed
+            # set files and cleanup
+            self._set_results_to_final_path(cur_path, dst_path, filename, task_path)
             callback_success = self._post_callbacks(task.callbacks)
 
         except Exception as e:
             callback_success = False  # video was unsuccessful so callbacks are also not successful
             message = f"Error processing {file_path}: {str(e)}"
             device.message = message
             db.session.commit()
             self.logger.error(message)
             # find back the file and place in the failed location, organised per day
             if timestamp:
                 dst_path = os.path.join(self.disk_management.failed_path, timestamp.strftime("%Y%m%d"))
             else:
                 dst_path = self.disk_management.failed_path
+            # set files and cleanup
+            self._set_results_to_final_path(cur_path, dst_path, filename, task_path)
             # also check if the current form is a CANDIDATE form. If so report to device and roll back to the ACCEPTED FORM
             task_form_template = config.get_active_task_form(db.session, parse=False)
 
-        # set files and cleanup
-        self._set_results_to_final_path(cur_path, dst_path, filename, task_path)
         # once done, the file is removed from list of considered files for processing
         self.processed_files.remove(file_path)
         # if callbacks were successful, try to send off old callbacks that were not successful earlier
-        self.logger.debug("Checking for old callbacks to send")
-        self._post_old_callbacks()
+        if callback_success:
+            self.logger.debug("Checking for old callbacks to send")
+            self._post_old_callbacks()
         # processing done, so set back to False
         self.logger.debug("Processing done, setting processing state to False")
         self.processing = False
         # shutdown if configured to shutdown after task
         self._shutdown_or_not()
         # check if any reboots are needed and reboot
         self.reboot_now_or_not()
@@ -321,15 +325,15 @@
         self.logger.debug(f"Video file moved from {cur_path} to {dst_path}")
 
         if os.path.isdir(task_path):
             # remove any left over temporary files
             shutil.rmtree(task_path)
 
     def _shutdown_or_not(self):
-        if self.shutdown_after_task:
+        if self.settings["shutdown_after_task"]:
             self.logger.info("Task done! Shutting down...")
             os.system("/sbin/shutdown -h now")
 
     def _post_callbacks(self, callbacks):
         """
         Performs callbacks in a list, and returns True when all were successful
 
@@ -582,14 +586,15 @@
     # output file templates are filled in with the timestamp
     output_files = {
         k: models.File(
             remote_name=v["remote_name"].format(timestamp.strftime('%Y%m%dT%H%M%S')),
             tmp_name=v["tmp_name"]
         ) for k, v in task_form["output_files"].items()
     }
+    all_files = dict(**input_files, **output_files)
     # callback jsons are converted to Callback objects
     callbacks = []
     for cb in task_form["callbacks"]:
         # replace/remove time stamp
         if "timestamp" in cb:
             cb.pop("timestamp")
         if "storage" in cb:
@@ -597,15 +602,15 @@
         if "file" in cb:
             file = cb.pop("file")
             if file:
                 cb["file"] = output_files[file]
         if "files_to_send" in cb:
             files_to_send = cb.pop("files_to_send")
             if files_to_send:
-                cb["files_to_send"] = {fn: output_files[fn] for fn in files_to_send}
+                cb["files_to_send"] = {fn: all_files[fn] for fn in files_to_send}
         cb_obj = models.Callback(
             storage=storage,
             timestamp=timestamp,
             **cb
         )
         callbacks.append(cb_obj)
```

### Comparing `nodeorc-0.1.0/nodeorc/tasks/task_form.py` & `nodeorc-0.1.1/nodeorc/tasks/task_form.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/nodeorc/utils.py` & `nodeorc-0.1.1/nodeorc/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,7 +97,9 @@
         return True
     else:
         return False
 
 
 def reboot_now():
     os.system("/sbin/shutdown -r now")
+    # in case this fails, do a sudo shutdown
+    os.system("sudo /sbin/shutdown -r now")
```

### Comparing `nodeorc-0.1.0/pyproject.toml` & `nodeorc-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/service/usb-mount.sh` & `nodeorc-0.1.1/service/usb-mount.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/settings/config_template.json` & `nodeorc-0.1.1/settings/config_template.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/setup.sh` & `nodeorc-0.1.1/setup.sh`

 * *Files 2% similar despite different names*

```diff
@@ -59,36 +59,35 @@
     else
         echo "System unknown I can't help you with updating"
         exit 1
     fi
   echo 'Dependencies installed. Now install NodeORC.'
 }
 
-
 install_nodeorc () {
     echo "========================================================================"
     echo 'INSTALLING NODEOPENRIVERCAM'
     echo "========================================================================"
         python3 -m venv $HOME/venv/nodeorc
         # activate the new environment
         source $HOME/venv/nodeorc/bin/activate
         # install the current source code
-        pip install .
+        pip install --upgrade nodeorc
         deactivate
     echo ''
     echo '------------------------------------------------------------------------'
     echo 'NodeORC installed. Now setup the automated service.'
     echo '------------------------------------------------------------------------'
 }
 
 install_service () {
     # export variables for some static files below
     export SCRIPT_FOLDER=$PWD/$(dirname $0)
-    export CONFIG_TEMPLATE="${SCRIPT_FOLDER}/settings/config_template.json"
-    export CONFIG_NEW="${SCRIPT_FOLDER}/settings/config_device.json"
+    export CONFIG_TEMPLATE="${HOME}/.nodeorc/config_template.json"
+    export CONFIG_NEW="${HOME}/.nodeorc/config_device.json"
     export CONFIG_DBASE=${HOME}/.nodeorc/nodeorc_config.db
 
     echo "========================================================================"
     echo 'CONFIGURE AND SETUP NODEORC AS A BACKGROUND SERVICE '
     echo "========================================================================"
     echo ""
     echo "In this installation part, NodeORC will be configured, and converted into an automatically running"
@@ -297,14 +296,44 @@
         echo "I was not able to find a USB device. Did you forget to insert one? I am shutting down..."
         exit 1
     fi
 
 }
 setup_nodeorc_config(){
     source ${HOME}/venv/nodeorc/bin/activate
+	cat > ${CONFIG_TEMPLATE} <<EOF
+{
+    "callback_url": {
+        "url": "http://127.0.0.1:8000",
+        "token_refresh_end_point": "/api/token/refresh/",
+        "token_refresh": "",
+        "token_access": ""
+    },
+    "storage": {
+        "url": "./tmp",
+        "bucket_name": "examplevideo"
+    },
+    "settings": {
+        "parse_dates_from_file": true,
+        "video_file_fmt": "{%Y%m%d_%H%M%S}.mp4",
+        "water_level_fmt": "all_levels.txt",
+        "water_level_datetimefmt": "%Y%m%d_%H%M%S",
+        "allowed_dt": 3600,
+        "shutdown_after_task": false,
+        "reboot_after": 86400
+
+    },
+    "disk_management": {
+        "home_folder": "",
+        "min_free_space": 2,
+        "critical_space": 1,
+        "frequency": 3600
+    }
+}
+EOF
 
     echo "Setting up configuration with LiveORC connection to ${URL}..."
     jq ".callback_url.url=\"${URL}\" | .callback_url.token_refresh=\"${REFRESH}\" | .callback_url.token_access=\"${ACCESS}\" | .disk_management.home_folder=\"${NODEORC_DATA_PATH}\"" ${CONFIG_TEMPLATE} > ${CONFIG_NEW}
 
     # we now have a solid configuration file, now initialize the database, and upload this to the database
     if [[ -f ${CONFIG_DBASE} ]]
     then
```

### Comparing `nodeorc-0.1.0/tests/conftest.py` & `nodeorc-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/tests/examples/ngwerere_transect.nc` & `nodeorc-0.1.1/tests/examples/ngwerere_transect.nc`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/tests/test_callbacks.py` & `nodeorc-0.1.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/tests/test_config.py` & `nodeorc-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/tests/test_disk_management.py` & `nodeorc-0.1.1/tests/test_disk_management.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/tests/test_s3.py` & `nodeorc-0.1.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.0/PKG-INFO` & `nodeorc-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeorc
-Version: 0.1.0
+Version: 0.1.1
 Summary: NodeORC: Automated edge and cloud image-based discharge estimation with OpenRiverCam
 Author-email: Hessel Winsemius <winsemius@rainbowsensing.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -123,15 +123,15 @@
 installation, please download the setup.sh script from the latest release on the device on which you wish to install it,
 make the script executable and execute the script on a command line interface with the option ``--all``. The steps
 are outlined below:
 
 .. code-block:: shell
 
     # get script from latest release
-    wget https://github.com/localdevices/nodeorc/releases/latest/setup.sh
+    wget https://github.com/localdevices/nodeorc/releases/latest/download/setup.sh
     # make the setup script executable
     chmod +x setup.sh
     # execute script
     ./setup.sh --all
 
 The setup procedure will ask several inputs including the url and your username and password for the LiveOpenRiverCam
 server. Note that these credentials will not be stored on the device, but only used to receive a temporary access token
```

