# Comparing `tmp/ehdtd_daemon-0.1.4.tar.gz` & `tmp/ehdtd_daemon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.4.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.5.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.4.tar` & `ehdtd_daemon-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.4/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.4/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.4/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.4/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     7213 2024-04-05 09:26:48.307492 ehdtd_daemon-0.1.4/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.4/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-04-06 14:50:59.602298 ehdtd_daemon-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.5/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.5/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.5/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0     8259 2024-04-07 06:46:52.304434 ehdtd_daemon-0.1.5/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.5/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      705 2024-04-07 06:19:19.997299 ehdtd_daemon-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.5/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.4/LICENSE` & `ehdtd_daemon-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.4/README.md` & `ehdtd_daemon-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.4/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.5/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.4/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.5/ehdtd_daemon/aux_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.4/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.5/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             The ehdtd-daemon.yaml configuration file follows a YAML\
             (YAML Ain't Markup Language) format. It consists of several sections and parameters,\
             allowing customization of the daemon's behavior. See README.md for the format details.
 
     Commands:
         start       Start the daemon
         stop        Stop the daemon
+        check   Check exchange connectivity
 
     """
 
     result = 0
     global DAEMON_RUNNING # pylint: disable=global-statement
 
     argv = sys.argv[1:]
@@ -60,14 +61,15 @@
     Options:
         -h, --help                  Display this help message and exit.
         -c, --config=CONFIG_FILE    Specify the config file .
 
     Commands:
         start   Start the daemon
         stop    Stop the daemon
+        check   Check exchange connectivity
 
     """
 
     try:
         optlist, args = getopt.getopt(argv, 'hc:', ['help', 'config='])
     except getopt.GetoptError:
         print(help_msg, flush=True)
@@ -95,15 +97,34 @@
 
     log_dir = config_data['global']['log_dir']
     run_dir = config_data['global']['run_dir']
     run_file = os.path.join(run_dir, "ehdtd-daemon.pid")
     log_file = os.path.join(log_dir, "ehdtd-daemon.log")
     err_file = os.path.join(log_dir, "ehdtd-daemon.err")
 
+    connections_ok = True
+    connections_data = {}
+
+    if config_data is not None\
+        and 'exchanges' in config_data\
+        and config_data['exchanges'] is not None\
+        and isinstance(config_data['exchanges'], dict):
+        for exchange in config_data['exchanges']:
+            if exchange is not None and isinstance(exchange, str):
+                connections_data[exchange] = Ehdtd.get_exchange_connectivity(exchange)
+                if connections_data[exchange] is None or not connections_data[exchange]['result']:
+                    connections_ok = False
+    else:
+        connections_ok = False
+
     if command_input == "start":
+        if not connections_ok:
+            print(f'Connection error: {connections_data}')
+            return 1
+
         def capture_signal(signal_number, frame): # pylint: disable=unused-argument
             global DAEMON_RUNNING # pylint: disable=global-statement
             result = True
             DAEMON_RUNNING = False # pylint: disable=unused-variable
             return result
 
         signal.signal(signal.SIGTERM, capture_signal)
@@ -199,14 +220,18 @@
         print(log_msg, end='', flush=True)
         check_pid = os.getpid()
 
         pid_to_kill = None
 
         if os.path.exists(run_file):
             pid_to_kill = int(acf.file_get_contents(run_file))
+        else:
+            if not connections_ok:
+                print(f'Connection error: {connections_data}')
+                return 1
 
         if pid_to_kill is not None and pid_to_kill != check_pid and acf.is_pid_running(pid_to_kill):
             os.kill(pid_to_kill,signal.SIGTERM)
 
         max_wait_to_stop = 900
         time_stop = 0
 
@@ -216,11 +241,15 @@
             time.sleep(5)
 
         if acf.is_pid_running(pid_to_kill):
             os.kill(pid_to_kill,signal.SIGKILL)
             result = 1
         print(' Ready', flush=True)
 
+    elif command_input == "check":
+        print(f'{connections_data}')
+        return 0
+
     return result
 
 if __name__ == "__main__":
     main()
```

### Comparing `ehdtd_daemon-0.1.4/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.1.5/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.4/pyproject.toml` & `ehdtd_daemon-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.4"
+version = "0.1.5"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
```

### Comparing `ehdtd_daemon-0.1.4/PKG-INFO` & `ehdtd_daemon-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

