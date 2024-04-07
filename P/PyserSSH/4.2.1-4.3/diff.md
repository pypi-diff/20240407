# Comparing `tmp/PyserSSH-4.2.1.tar.gz` & `tmp/PyserSSH-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyserSSH-4.2.1.tar", last modified: Sun Mar 31 07:03:59 2024, max compression
+gzip compressed data, was "PyserSSH-4.3.tar", last modified: Sun Apr  7 10:07:53 2024, max compression
```

## Comparing `PyserSSH-4.2.1.tar` & `PyserSSH-4.3.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 07:03:59.293384 PyserSSH-4.2.1/
--rw-rw-rw-   0        0        0     2198 2024-03-31 07:03:59.293384 PyserSSH-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1852 2024-03-31 07:02:15.000000 PyserSSH-4.2.1/README.md
--rw-rw-rw-   0        0        0      115 2024-03-31 07:03:59.295378 PyserSSH-4.2.1/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-03-31 07:03:49.000000 PyserSSH-4.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:03:59.258337 PyserSSH-4.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 07:03:59.268839 PyserSSH-4.2.1/src/PyserSSH/
--rw-rw-rw-   0        0        0     2048 2024-03-30 12:01:22.000000 PyserSSH-4.2.1/src/PyserSSH/__init__.py
--rw-rw-rw-   0        0        0     6843 2024-03-29 11:11:09.000000 PyserSSH-4.2.1/src/PyserSSH/account.py
--rw-rw-rw-   0        0        0     6997 2024-03-29 11:45:43.000000 PyserSSH-4.2.1/src/PyserSSH/interactive.py
--rw-rw-rw-   0        0        0    13499 2024-03-30 11:13:08.000000 PyserSSH-4.2.1/src/PyserSSH/server.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:03:59.289860 PyserSSH-4.2.1/src/PyserSSH.egg-info/
--rw-rw-rw-   0        0        0     2198 2024-03-31 07:03:58.000000 PyserSSH-4.2.1/src/PyserSSH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-03-31 07:03:59.000000 PyserSSH-4.2.1/src/PyserSSH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 07:03:59.000000 PyserSSH-4.2.1/src/PyserSSH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-03-31 07:03:59.000000 PyserSSH-4.2.1/src/PyserSSH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 07:03:59.000000 PyserSSH-4.2.1/src/PyserSSH.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.672365 PyserSSH-4.3/
+-rw-rw-rw-   0        0        0     2157 2024-04-07 10:07:53.672365 PyserSSH-4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1852 2024-03-31 07:02:15.000000 PyserSSH-4.3/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-07 10:07:53.679882 PyserSSH-4.3/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-07 10:07:23.000000 PyserSSH-4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.471907 PyserSSH-4.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.508903 PyserSSH-4.3/src/PyserSSH/
+-rw-rw-rw-   0        0        0     2067 2024-04-07 09:53:16.000000 PyserSSH-4.3/src/PyserSSH/__init__.py
+-rw-rw-rw-   0        0        0     8384 2024-04-07 10:00:41.000000 PyserSSH-4.3/src/PyserSSH/account.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.609790 PyserSSH-4.3/src/PyserSSH/extensions/
+-rw-rw-rw-   0        0        0     9258 2024-04-06 10:27:06.000000 PyserSSH-4.3/src/PyserSSH/extensions/XHandler.py
+-rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:52.000000 PyserSSH-4.3/src/PyserSSH/extensions/__init__.py
+-rw-rw-rw-   0        0        0     7072 2024-04-06 10:26:37.000000 PyserSSH-4.3/src/PyserSSH/extensions/dialog.py
+-rw-rw-rw-   0        0        0     3582 2024-04-06 10:26:40.000000 PyserSSH-4.3/src/PyserSSH/extensions/moredisplay.py
+-rw-rw-rw-   0        0        0    13483 2024-04-06 10:26:49.000000 PyserSSH-4.3/src/PyserSSH/extensions/processbar.py
+-rw-rw-rw-   0        0        0     1332 2024-04-06 10:26:53.000000 PyserSSH-4.3/src/PyserSSH/extensions/ptop.py
+-rw-rw-rw-   0        0        0     7095 2024-04-07 08:41:56.000000 PyserSSH-4.3/src/PyserSSH/interactive.py
+-rw-rw-rw-   0        0        0    13692 2024-04-07 09:57:13.000000 PyserSSH-4.3/src/PyserSSH/server.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.669376 PyserSSH-4.3/src/PyserSSH/system/
+-rw-rw-rw-   0        0        0     7265 2024-04-06 10:26:25.000000 PyserSSH-4.3/src/PyserSSH/system/SFTP.py
+-rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:54.000000 PyserSSH-4.3/src/PyserSSH/system/__init__.py
+-rw-rw-rw-   0        0        0     1492 2024-04-06 10:26:13.000000 PyserSSH-4.3/src/PyserSSH/system/info.py
+-rw-rw-rw-   0        0        0     8771 2024-04-07 08:44:26.000000 PyserSSH-4.3/src/PyserSSH/system/inputsystem.py
+-rw-rw-rw-   0        0        0     4277 2024-04-06 10:26:21.000000 PyserSSH-4.3/src/PyserSSH/system/interface.py
+-rw-rw-rw-   0        0        0     1799 2024-04-06 10:26:29.000000 PyserSSH-4.3/src/PyserSSH/system/syscom.py
+-rw-rw-rw-   0        0        0     2282 2024-04-06 10:26:32.000000 PyserSSH-4.3/src/PyserSSH/system/sysfunc.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.670365 PyserSSH-4.3/src/PyserSSH.egg-info/
+-rw-rw-rw-   0        0        0     2157 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/top_level.txt
```

### Comparing `PyserSSH-4.2.1/PKG-INFO` & `PyserSSH-4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: PyserSSH
-Version: 4.2.1
-Summary: A easy ssh server
+Version: 4.3
+Summary: python scriptable ssh server library. based on Paramiko
 Home-page: https://github.com/damp11113/PyserSSH
 Author: damp11113
 Author-email: damp51252@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: paramiko
-Provides-Extra: fullsyscom
-Requires-Dist: damp11113; extra == "fullsyscom"
 
 # What is PyserSSH
 
 PyserSSH is a library for remote control your code with ssh client. The aim is to provide a scriptable SSH server which can be made to behave like any SSH-enabled device.
 
 This project is part from [damp11113-library](https://github.com/damp11113/damp11113-library)
```

### Comparing `PyserSSH-4.2.1/README.md` & `PyserSSH-4.3/README.md`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.2.1/setup.py` & `PyserSSH-4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PyserSSH',
-    version='4.2.1', # update pypi (no update for 4.3)
+    version='4.3',
     license='MIT',
     author='damp11113',
     author_email='damp51252@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/damp11113/PyserSSH',
-    description="A easy ssh server",
+    description="python scriptable ssh server library. based on Paramiko",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         "paramiko"
-    ],
-    extras_require={
-        "fullsyscom": ["damp11113"]
-    }
+    ]
 )
```

### Comparing `PyserSSH-4.2.1/src/PyserSSH/__init__.py` & `PyserSSH-4.3/src/PyserSSH/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-PyserSSH - A SSH server. For more info visit https://github.com/damp11113/PyserSSH
+PyserSSH - A Scriptable SSH server. For more info visit https://github.com/damp11113/PyserSSH
 Copyright (C) 2023-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/PyserSSH
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,13 +56,13 @@
     os.environ["pyserssh_enable_damp11113"] = "YES"
 
 try:
     os.environ["pyserssh_log"]
 except:
     os.environ["pyserssh_log"] = "NO"
 
-if os.environ["pyserssh_log"]:
+if os.environ["pyserssh_log"] == "NO":
     logger = logging.getLogger("PyserSSH")
     logger.disabled = True
 
 if os.environ["pyserssh_systemmessage"] == "YES":
     print(system_banner)
```

### Comparing `PyserSSH-4.2.1/src/PyserSSH/account.py` & `PyserSSH-4.3/src/PyserSSH/account.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-PyserSSH - A SSH server. For more info visit https://github.com/damp11113/PyserSSH
+PyserSSH - A Scriptable SSH server. For more info visit https://github.com/damp11113/PyserSSH
 Copyright (C) 2023-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/PyserSSH
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,24 +22,53 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import pickle
+import time
+import atexit
+import threading
 
 class AccountManager:
-    def __init__(self, anyuser=False, historylimit=10):
+    def __init__(self, anyuser=False, historylimit=10, autosave=False, autosavedelay=60, autoload=False, autoloadfile="autosave_session.ses"):
         self.accounts = {}
         self.anyuser = anyuser
         self.historylimit = historylimit
+        self.autosavedelay = autosavedelay
+
+        self.__autosavework = False
+        self.__autosaveworknexttime = 0
 
         if self.anyuser:
             print("history system can't work if 'anyuser' is enable")
 
+        if autoload:
+            self.load(autoloadfile)
+
+        if autosave:
+            self.__autosavethread = threading.Thread(target=self.__autosave)
+            self.__autosavethread.start()
+            atexit.register(self.__saveexit)
+
+    def __autosave(self):
+        self.save("autosave_session.ses")
+        self.__autosaveworknexttime = time.time() + self.autosavedelay
+        self.__autosavework = True
+        while self.__autosavework:
+            if int(self.__autosaveworknexttime) == int(time.time()):
+                self.save("autosave_session.ses")
+                self.__autosaveworknexttime = time.time() + self.autosavedelay
+
+    def __saveexit(self):
+        self.__autosavework = False
+        self.save("autosave_session.ses")
+        self.__autosavethread.join()
+
     def validate_credentials(self, username, password):
         if username in self.accounts and self.accounts[username]["password"] == password or self.anyuser:
             return True
         return False
 
     def get_permissions(self, username):
         if username in self.accounts:
@@ -62,19 +91,19 @@
         if username in self.accounts:
             self.accounts[username]["password"] = new_password
 
     def set_permissions(self, username, new_permissions):
         if username in self.accounts:
             self.accounts[username]["permissions"] = new_permissions
 
-    def save_to_file(self, filename):
+    def save(self, filename="session.ssh"):
         with open(filename, 'wb') as file:
             pickle.dump(self.accounts, file)
 
-    def load_from_file(self, filename):
+    def load(self, filename):
         try:
             with open(filename, 'rb') as file:
                 self.accounts = pickle.load(file)
         except FileNotFoundError:
             print("File not found. No accounts loaded.")
         except Exception as e:
             print(f"An error occurred: {e}. No accounts loaded.")
@@ -110,20 +139,32 @@
         if username in self.accounts and "sftp_path" in self.accounts[username]:
             return self.accounts[username]["sftp_path"]
         return ""
 
     def get_user_timeout(self, username):
         if username in self.accounts and "timeout" in self.accounts[username]:
             return self.accounts[username]["timeout"]
-        return 0
+        return None
 
-    def set_user_timeout(self, username, timeout=0):
+    def set_user_timeout(self, username, timeout=None):
         if username in self.accounts:
             self.accounts[username]["timeout"] = timeout
 
+    def get_user_last_login(self, username):
+        if username in self.accounts and "lastlogin" in self.accounts[username]:
+            return self.accounts[username]["lastlogin"]
+        return None
+
+    def set_user_last_login(self, username, ip, timelogin=time.time()):
+        if username in self.accounts:
+            self.accounts[username]["lastlogin"] = {
+                "ip": ip,
+                "time": timelogin
+            }
+
     def add_history(self, username, command):
         if not self.anyuser:
             if username in self.accounts:
                 if "history" not in self.accounts[username]:
                     self.accounts[username]["history"] = []  # Initialize history list if it doesn't exist
 
                 history_limit = self.historylimit if self.historylimit is not None else float('inf')
@@ -154,8 +195,8 @@
             return None  # User or history not found
 
     def get_lastcommand(self, username):
         if not self.anyuser:
             if username in self.accounts and "lastcommand" in self.accounts[username]:
                 command = self.accounts[username]["lastcommand"]
                 return command
-            return None  # User or history not found
+            return None  # User or history not found
```

### Comparing `PyserSSH-4.2.1/src/PyserSSH/interactive.py` & `PyserSSH-4.3/src/PyserSSH/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-PyserSSH - A SSH server. For more info visit https://github.com/damp11113/PyserSSH
+PyserSSH - A Scriptable SSH server. For more info visit https://github.com/damp11113/PyserSSH
 Copyright (C) 2023-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/PyserSSH
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -98,25 +98,26 @@
                         channel.sendall(passwordmask)
                     else:
                         channel.sendall(byte)
 
         channel.sendall(b'\r\n')
 
     except socket.timeout:
+        channel.setblocking(False)
+        channel.settimeout(None)
+        channel.sendall(b'\r\n')
         output = ""
     except Exception:
+        channel.setblocking(False)
+        channel.settimeout(None)
+        channel.sendall(b'\r\n')
         raise
     else:
         output = buffer.decode('utf-8')
 
-    if timeout != 0:
-        channel.settimeout(0)
-        channel.setblocking(False)
-        channel.sendall(b'\r\n')
-
     # Return default value if specified and no input given
     if defaultvalue is not None and not output.strip():
         return defaultvalue
     else:
         return output
 
 def wait_inputkey(client, prompt="", raw=False, timeout=0):
@@ -140,22 +141,22 @@
 
             return byte.decode('utf-8') # only regular character
 
         else:
             return byte
 
     except socket.timeout:
-        channel.settimeout(0)
         channel.setblocking(False)
+        channel.settimeout(None)
         channel.send("\r\n")
         return None
     except Exception:
-        if timeout != 0:
-            channel.settimeout(0)
-            channel.setblocking(False)
+        channel.setblocking(False)
+        channel.settimeout(None)
+        channel.send("\r\n")
         raise
 
 def wait_choose(client, choose, prompt="", timeout=0):
     channel = client["channel"]
 
     chooseindex = 0
     chooselen = len(choose) - 1
@@ -189,16 +190,16 @@
                 if chooseindex < 0:
                     chooseindex = 0
             elif keyinput == b'\x1b[C':  # Down arrow key
                 chooseindex += 1
                 if chooseindex > chooselen:
                     chooseindex = chooselen
         except socket.timeout:
-            channel.settimeout(0)
             channel.setblocking(False)
+            channel.settimeout(None)
             channel.send("\r\n")
             return chooseindex
         except Exception:
-            if timeout != 0:
-                channel.settimeout(0)
-                channel.setblocking(False)
+            channel.setblocking(False)
+            channel.settimeout(None)
+            channel.send("\r\n")
             raise
```

### Comparing `PyserSSH-4.2.1/src/PyserSSH/server.py` & `PyserSSH-4.3/src/PyserSSH/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-PyserSSH - A SSH server. For more info visit https://github.com/damp11113/PyserSSH
+PyserSSH - A Scriptable SSH server. For more info visit https://github.com/damp11113/PyserSSH
 Copyright (C) 2023-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/PyserSSH
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -143,14 +143,16 @@
                 }
             client_handler = self.client_handlers[peername]
             client_handler["current_user"] = server.current_user
             client_handler["channel"] = channel  # Update the channel attribute for the client handler
             client_handler["last_activity_time"] = time.time()
             client_handler["last_login_time"] = time.time()
 
+            self.accounts.set_user_last_login(self.client_handlers[channel.getpeername()]["current_user"], peername[0])
+
             #if not any(bh_session.remote_version.split("-")[2].startswith(prefix) for prefix in sftpclient):
             if not channel.out_window_size == bh_session.default_window_size:
                 while self.client_handlers[channel.getpeername()]["windowsize"] == {}:
                     pass
 
                 channel.send(f"\033]0;{self.title}\007".encode())
 
@@ -162,15 +164,16 @@
                     self._handle_event("connect", self.client_handlers[channel.getpeername()])
                 except Exception as e:
                     self._handle_event("error", self.client_handlers[channel.getpeername()], e)
 
                 client_handler["connecttype"] = "ssh"
                 if self.enainputsystem:
                     try:
-                        if self.accounts.get_user_timeout(self.client_handlers[channel.getpeername()]["current_user"]) != 0:
+                        if self.accounts.get_user_timeout(self.client_handlers[channel.getpeername()]["current_user"]) != None:
+                            channel.setblocking(False)
                             channel.settimeout(self.accounts.get_user_timeout(self.client_handlers[channel.getpeername()]["current_user"]))
 
                         channel.send(replace_enter_with_crlf(self.accounts.get_prompt(self.client_handlers[channel.getpeername()]["current_user"]) + " ").encode('utf-8'))
                         while True:
                             expect(self, channel, peername)
                     except KeyboardInterrupt:
                         self._handle_event("disconnected", self.client_handlers[peername]["current_user"])
```

### Comparing `PyserSSH-4.2.1/src/PyserSSH.egg-info/PKG-INFO` & `PyserSSH-4.3/src/PyserSSH.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: PyserSSH
-Version: 4.2.1
-Summary: A easy ssh server
+Version: 4.3
+Summary: python scriptable ssh server library. based on Paramiko
 Home-page: https://github.com/damp11113/PyserSSH
 Author: damp11113
 Author-email: damp51252@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: paramiko
-Provides-Extra: fullsyscom
-Requires-Dist: damp11113; extra == "fullsyscom"
 
 # What is PyserSSH
 
 PyserSSH is a library for remote control your code with ssh client. The aim is to provide a scriptable SSH server which can be made to behave like any SSH-enabled device.
 
 This project is part from [damp11113-library](https://github.com/damp11113/damp11113-library)
```

