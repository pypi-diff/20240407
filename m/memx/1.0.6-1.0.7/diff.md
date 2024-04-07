# Comparing `tmp/memx-1.0.6.tar.gz` & `tmp/memx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memx-1.0.6.tar", last modified: Sun Feb 25 09:13:05 2024, max compression
+gzip compressed data, was "memx-1.0.7.tar", last modified: Sun Apr  7 13:35:04 2024, max compression
```

## Comparing `memx-1.0.6.tar` & `memx-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-02-25 09:13:05.856798 memx-1.0.6/
--rw-r--r--   0 iacobrazvan   (501) staff       (20)      918 2024-02-25 09:13:05.856022 memx-1.0.6/PKG-INFO
--rw-r--r--   0 iacobrazvan   (501) staff       (20)      388 2024-02-25 09:02:16.000000 memx-1.0.6/README.md
-drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-02-25 09:13:05.847808 memx-1.0.6/memx/
--rw-r--r--   0 iacobrazvan   (501) staff       (20)       99 2024-02-25 08:32:07.000000 memx-1.0.6/memx/__init__.py
--rw-r--r--   0 iacobrazvan   (501) staff       (20)     5488 2024-02-25 08:31:06.000000 memx-1.0.6/memx/main.py
-drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-02-25 09:13:05.854512 memx-1.0.6/memx.egg-info/
--rw-r--r--   0 iacobrazvan   (501) staff       (20)      918 2024-02-25 09:13:05.000000 memx-1.0.6/memx.egg-info/PKG-INFO
--rw-r--r--   0 iacobrazvan   (501) staff       (20)      187 2024-02-25 09:13:05.000000 memx-1.0.6/memx.egg-info/SOURCES.txt
--rw-r--r--   0 iacobrazvan   (501) staff       (20)        1 2024-02-25 09:13:05.000000 memx-1.0.6/memx.egg-info/dependency_links.txt
--rw-r--r--   0 iacobrazvan   (501) staff       (20)        7 2024-02-25 09:13:05.000000 memx-1.0.6/memx.egg-info/requires.txt
--rw-r--r--   0 iacobrazvan   (501) staff       (20)        5 2024-02-25 09:13:05.000000 memx-1.0.6/memx.egg-info/top_level.txt
--rw-r--r--   0 iacobrazvan   (501) staff       (20)       38 2024-02-25 09:13:05.856966 memx-1.0.6/setup.cfg
--rw-r--r--   0 iacobrazvan   (501) staff       (20)      745 2024-02-25 09:12:29.000000 memx-1.0.6/setup.py
+drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-04-07 13:35:04.530529 memx-1.0.7/
+-rwx------   0 iacobrazvan   (501) staff       (20)     1063 2024-02-25 09:19:58.000000 memx-1.0.7/LICENSE
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)      959 2024-04-07 13:35:04.522428 memx-1.0.7/PKG-INFO
+-rwx------   0 iacobrazvan   (501) staff       (20)      407 2024-04-07 13:20:00.000000 memx-1.0.7/README.md
+drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-04-07 13:35:04.494932 memx-1.0.7/memx/
+-rwx------   0 iacobrazvan   (501) staff       (20)      230 2024-04-07 12:51:42.000000 memx-1.0.7/memx/__init__.py
+-rwx------   0 iacobrazvan   (501) staff       (20)     5812 2024-04-07 13:31:47.000000 memx-1.0.7/memx/main.py
+drwxr-xr-x   0 iacobrazvan   (501) staff       (20)        0 2024-04-07 13:35:04.512950 memx-1.0.7/memx.egg-info/
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)      959 2024-04-07 13:35:03.000000 memx-1.0.7/memx.egg-info/PKG-INFO
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)      195 2024-04-07 13:35:04.000000 memx-1.0.7/memx.egg-info/SOURCES.txt
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)        1 2024-04-07 13:35:03.000000 memx-1.0.7/memx.egg-info/dependency_links.txt
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)        7 2024-04-07 13:35:03.000000 memx-1.0.7/memx.egg-info/requires.txt
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)        5 2024-04-07 13:35:03.000000 memx-1.0.7/memx.egg-info/top_level.txt
+-rw-r--r--   0 iacobrazvan   (501) staff       (20)       38 2024-04-07 13:35:04.530967 memx-1.0.7/setup.cfg
+-rwx------   0 iacobrazvan   (501) staff       (20)      745 2024-04-07 12:45:46.000000 memx-1.0.7/setup.py
```

### Comparing `memx-1.0.6/PKG-INFO` & `memx-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: memx
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python Library to Manipulate macOS Processes.
 Author: Iacob Razvan Mihai
 Author-email: razvan.iacob@protonmail.com
 License: MIT
 Keywords: memory,macos,hacking
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: psutil
 
 #  MemX
 ## A Python Library to Manipulate macOS Processes.
 ---
 ### Example usage:
 ```
-from MemX import *
+from memx import *
 
 mx = Process("assaultcube")
+mx.fetch_modules()
 base = Module(mx, "assaultcube").BaseAddress
 
 s = mx.read_longlong(base + 0x1D9EF0)
 healthAddr = mx.read_longlong(s) + 0x418
 
 print(f"Health value: {mx.read_int(healthAddr)}")
 ```
```

### Comparing `memx-1.0.6/memx/main.py` & `memx-1.0.7/memx/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             i += 1
         return procs[int(input("[MemX] Enter your choice: ")) - 1].pid
     return None        
 
 class Process:
     def __init__(self, ProcessName: str): 
         self.pid = pid_for_pname(ProcessName)
+        self.TEXT = []
         assert (self.pid is not None), "Couldn't find a running instance of %s" % ProcessName
         self.task = ctypes.c_uint32()
         self.mytask=libc.mach_task_self()
         ret=libc.task_for_pid(self.mytask, ctypes.c_int(self.pid), ctypes.pointer(self.task))
         if ret == 5: raise Exception("Please run this app with SUDO.")
         elif ret != 0 : raise Exception("Could not get task for pid %d" % self.pid)
 
@@ -122,22 +123,31 @@
         data_buffer = ctypes.create_string_buffer(data)
         data_len = ctypes.c_ulonglong(len(data))
         libc.mach_vm_protect(self.task, ctypes.c_ulonglong(address), data_len,ctypes.c_bool(False), ctypes.c_int(VM_PROT_ALL))
         res = libc.mach_vm_write(self.task, ctypes.c_ulonglong(address), data_buffer, data_len)
         if res != 0:
             raise Exception("mach_vm_write returned : %s" % res)
 
+    # This was added to speed up the module getting
+    def fetch_modules(self):
+        regs = popen(f"vmmap {self.pid} | grep __TEXT").read().split("\n")
+        self.TEXT = []
+        for reg in regs:
+            if "__TEXT" in reg:
+                self.TEXT.append(reg)
+
 class Module:
     # TODO: Find a normal & faster way
     def __init__(self, Process: Process, ModuleName: str):
         self.proc = Process
-        regs = popen(f"vmmap {self.proc.pid} | grep __TEXT").read().split("\n")
+        if not self.proc.TEXT:
+            raise Exception("Please use fetch_modules() first.")
         self.BaseAddress = None
         self.Size = None
-        for reg in regs:
+        for reg in self.proc.TEXT:
             if ModuleName in reg:
                 ax = reg.split("__TEXT")[1].split("-")
                 self.BaseAddress = int(ax[0], 16)
                 self.Size = int(ax[1].split(" ")[0], 16) - self.BaseAddress
                 break
 
     def search_IDA_pattern(self, ida_pattern: str):
```

### Comparing `memx-1.0.6/memx.egg-info/PKG-INFO` & `memx-1.0.7/memx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: memx
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python Library to Manipulate macOS Processes.
 Author: Iacob Razvan Mihai
 Author-email: razvan.iacob@protonmail.com
 License: MIT
 Keywords: memory,macos,hacking
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: psutil
 
 #  MemX
 ## A Python Library to Manipulate macOS Processes.
 ---
 ### Example usage:
 ```
-from MemX import *
+from memx import *
 
 mx = Process("assaultcube")
+mx.fetch_modules()
 base = Module(mx, "assaultcube").BaseAddress
 
 s = mx.read_longlong(base + 0x1D9EF0)
 healthAddr = mx.read_longlong(s) + 0x418
 
 print(f"Health value: {mx.read_int(healthAddr)}")
 ```
```

### Comparing `memx-1.0.6/setup.py` & `memx-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='memx',
-    version='1.0.6',
+    version='1.0.7',
     author="Iacob Razvan Mihai",
     author_email="razvan.iacob@protonmail.com",
     description='A Python Library to Manipulate macOS Processes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

