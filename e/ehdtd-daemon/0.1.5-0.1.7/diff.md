# Comparing `tmp/ehdtd_daemon-0.1.5.tar.gz` & `tmp/ehdtd_daemon-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.5.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.7.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.5.tar` & `ehdtd_daemon-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.5/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.5/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.5/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.5/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     8259 2024-04-07 06:46:52.304434 ehdtd_daemon-0.1.5/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.5/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-04-07 06:19:19.997299 ehdtd_daemon-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.7/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.7/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.7/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0     8482 2024-04-07 11:22:47.531243 ehdtd_daemon-0.1.7/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.7/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      705 2024-04-07 11:19:35.530063 ehdtd_daemon-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.7/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.5/LICENSE` & `ehdtd_daemon-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.5/README.md` & `ehdtd_daemon-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.5/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.7/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.5/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.7/ehdtd_daemon/aux_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.5/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.7/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,15 +114,17 @@
                 if connections_data[exchange] is None or not connections_data[exchange]['result']:
                     connections_ok = False
     else:
         connections_ok = False
 
     if command_input == "start":
         if not connections_ok:
-            print(f'Connection error: {connections_data}')
+            err_msg = pprint.pformat(connections_data, sort_dicts=False)
+            print('Connection error:')
+            print(err_msg)
             return 1
 
         def capture_signal(signal_number, frame): # pylint: disable=unused-argument
             global DAEMON_RUNNING # pylint: disable=global-statement
             result = True
             DAEMON_RUNNING = False # pylint: disable=unused-variable
             return result
@@ -222,15 +224,17 @@
 
         pid_to_kill = None
 
         if os.path.exists(run_file):
             pid_to_kill = int(acf.file_get_contents(run_file))
         else:
             if not connections_ok:
-                print(f'Connection error: {connections_data}')
+                err_msg = pprint.pformat(connections_data, sort_dicts=False)
+                print('Connection error:')
+                print(err_msg)
                 return 1
 
         if pid_to_kill is not None and pid_to_kill != check_pid and acf.is_pid_running(pid_to_kill):
             os.kill(pid_to_kill,signal.SIGTERM)
 
         max_wait_to_stop = 900
         time_stop = 0
@@ -242,14 +246,15 @@
 
         if acf.is_pid_running(pid_to_kill):
             os.kill(pid_to_kill,signal.SIGKILL)
             result = 1
         print(' Ready', flush=True)
 
     elif command_input == "check":
-        print(f'{connections_data}')
+        out_msg = pprint.pformat(connections_data, sort_dicts=False)
+        print(out_msg)
         return 0
 
     return result
 
 if __name__ == "__main__":
     main()
```

### Comparing `ehdtd_daemon-0.1.5/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.1.7/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.5/pyproject.toml` & `ehdtd_daemon-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.5"
+version = "0.1.7"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
```

### Comparing `ehdtd_daemon-0.1.5/PKG-INFO` & `ehdtd_daemon-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.5
+Version: 0.1.7
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

