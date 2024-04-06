# Comparing `tmp/smolt-0.1.tar.gz` & `tmp/smolt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smolt-0.1.tar", last modified: Wed Mar 27 23:30:00 2024, max compression
+gzip compressed data, was "smolt-0.2.tar", last modified: Sat Apr  6 22:25:56 2024, max compression
```

## Comparing `smolt-0.1.tar` & `smolt-0.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     5054 2024-03-27 22:54:32.405193 smolt-0.1/README.md
--rw-r--r--   0        0        0      583 2024-03-27 23:30:00.895059 smolt-0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 02:15:07.135346 smolt-0.1/smolt/__init__.py
--rw-r--r--   0        0        0     1364 2024-03-27 21:26:32.967010 smolt-0.1/smolt/cli.py
--rw-r--r--   0        0        0     1615 2024-03-27 23:20:10.169331 smolt-0.1/smolt/gdb.py
--rw-r--r--   0        0        0     4880 2024-03-27 22:51:10.587507 smolt-0.1/smolt/include/smolt.h
--rw-r--r--   0        0        0     1029 2024-03-27 23:19:50.332001 smolt-0.1/smolt/itm.py
--rw-r--r--   0        0        0     2097 2024-03-27 23:19:58.540471 smolt-0.1/smolt/meta.py
--rw-r--r--   0        0        0     5417 1970-01-01 00:00:00.000000 smolt-0.1/PKG-INFO
+-rw-r--r--   0        0        0     5444 2024-04-01 00:14:36.962714 smolt-0.2/README.md
+-rw-r--r--   0        0        0      727 2024-04-06 22:25:56.396082 smolt-0.2/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-01 00:07:29.455474 smolt-0.2/smolt/__init__.py
+-rw-r--r--   0        0        0     1349 2024-04-01 00:08:15.633177 smolt-0.2/smolt/cli.py
+-rw-r--r--   0        0        0     1615 2024-04-06 22:25:46.892997 smolt-0.2/smolt/gdb.py
+-rw-r--r--   0        0        0     9772 2024-04-06 21:59:33.787659 smolt-0.2/smolt/include/smolt.h
+-rw-r--r--   0        0        0      989 2024-04-06 22:03:59.737759 smolt-0.2/smolt/itm.py
+-rw-r--r--   0        0        0     4303 2024-04-01 20:37:00.274374 smolt-0.2/smolt/meta.py
+-rw-r--r--   0        0        0     1941 2024-04-06 21:49:20.169338 smolt-0.2/tests/cpp/conftest.py
+-rw-r--r--   0        0        0     1152 2024-04-01 00:16:27.347191 smolt-0.2/tests/cpp/test_format_arguments.py
+-rw-r--r--   0        0        0     3548 2024-04-06 22:02:21.399177 smolt-0.2/tests/cpp/test_serializers.py
+-rw-r--r--   0        0        0      976 2024-03-31 23:57:46.641285 smolt-0.2/tests/cpp/test_transports.py
+-rw-r--r--   0        0        0       85 2024-03-31 23:49:07.706391 smolt-0.2/tests/cpp/util.py
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 smolt-0.2/PKG-INFO
```

### Comparing `smolt-0.1/README.md` & `smolt-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 Smolt is a small header-only C++ library with no dependencies beyond a C++20 compiler with STL. All use of STL is `constexpr`.
 
 When you make a log call, the format string and other metadata is given a tag ID, so the only data that needs to be sent or stored is the tag ID and the format arguments.
 The host side utilities can then use the tag ID to look up all the metadata from the .elf file and handle string formatting.
 
 ## Features
 - Formatting of values on the host with [Python's format string syntax](https://docs.python.org/3/library/string.html#formatstrings).
-  - Currently supports integral and floating point types up to 32 bit.
+  - Currently supports integral and floating point types up to 64 bit.
+  - Basic support for `std::span` and `std::string_view`.
 - Optional metadata attached to messages.
   - Source location.
 - Pluggable transports.
   - `transport::itm`
     - Streaming logging over ARM ITM over SWO or parallel trace.
   - `transport::ringbuffer`
     - Logging to internal ringbuffer for later readout.
@@ -29,26 +30,27 @@
   - Custom transports only have to implement `log_tag(uint32_t)` and `log_value(uint32_t)`.
 - CLI utility
   - Receive and format log messages over ITM from [Orbuculum](https://github.com/orbcode/orbuculum) and other sources that relay ITM messages over TCP.
 - GDB plugin
   - Read out and format log messages from a ringbuffer in target memory.
 
 ## TODO
+- Add a custom formatter for `std::span` that allows setting both an element formatting specifier and an element separator.
 - Support for more argument types:
-  - `uint64_t`, `int64_t`, `double`
-  - `std::string_view`
-  - `std::span`
-    - With a custom formatter that allows e.g. formatting buffers as hex bytes.
+  - Pointers? (I.e. implicit conversion to `uintptr_t` and default formatting as hex.)
 - More transports:
   - `transport::tee`
     - Allows feeding a single logger into multiple transports.
 - More metadata that can be attached to messages:
   - Severity (info, warning, error, etc…).
+- CLI command that checks format string validity (i.e. whether the format specifiers are valid for the types of arguments passed).
+  Can be added to the end of the build process to allow catching typos in format strings at compile time.
+- More checks and error handling.
 - Documentation.
-- Tests.
+- More tests.
 
 ## Usage
 
 ### Example firmware
 [Try it in Compiler Explorer](https://godbolt.org/z/WPP3a81Mn).
 
 ```cpp
```

### Comparing `smolt-0.1/smolt/cli.py` & `smolt-0.2/smolt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import click
 import pathlib
 import shlex
 
+from . import include_path
 from .meta import ELF
-
 from .itm import start_itm
 
 @click.group(context_settings = {'show_default': True})
 @click.version_option()
 def cli():
     pass
 
 @cli.command()
 @click.argument('elf', type=click.Path(exists = True, dir_okay = False, path_type = pathlib.Path))
 # TODO: JSON option?
 def list(elf):
     '''Read ELF file and list available tags.'''
 
     for tag in ELF(elf).tags():
-        print(f'{tag.addr:08x}: {tag.loc} "{tag.fmt}", {", ".join(tag.args)}')
+        print(f'{tag.addr:08x}: {tag.loc} "{tag.fmt}", {", ".join(str(a) for a in tag.args)}')
 
 @cli.command()
 @click.argument('elf', type=click.Path(exists = True, dir_okay = False, path_type = pathlib.Path))
 @click.option('--itm-channel', type = int, default = 24, help = 'First ITM channel to use.')
 @click.option('--hostname', default = 'localhost', help = 'Hostname to connect to.')
 @click.option('--port', type = int, default = 3443, help = 'Port to connect to.')
 # TODO: Include/exclude timestamp
@@ -32,11 +32,9 @@
 
     start_itm(elf, itm_channel, (hostname, port))
 
 @cli.command()
 def cflags():
     '''Get header include path, pkg-config style.'''
 
-    path = pathlib.Path(__file__).parent.absolute() / 'include'
-
     # TODO: This should probably be handled better, I don't expect it'll work on windows.
-    print(shlex.quote(f'-I{path}'))
+    print(shlex.quote(f'-I{include_path}'))
```

### Comparing `smolt-0.1/smolt/gdb.py` & `smolt-0.2/smolt/gdb.py`

 * *Files identical despite different names*

### Comparing `smolt-0.1/smolt/itm.py` & `smolt-0.2/smolt/itm.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,20 +14,21 @@
     args = []
 
     while True:
         packet = orb.rx()
 
         match packet:
             case swMsg() if packet.srcAddr == itm_channel:
-                tag = elf.tag(packet.value)
-                if tag is None:
-                    print(f'Got unknown tag: {packet.value:08x}')
+                tag_id = packet.value
+                if tag_id == 0:
+                    elf.refresh()
 
-                elif len(args) < len(tag.args):
-                    print(f'Insufficient arguments for tag: {tag.fmt:08x}, {args}')
+                tag = elf.tag(tag_id)
+                if tag is None:
+                    print(f'Got unknown tag: {tag_id:08x}')
 
                 else:
                     ts = time.strftime('%H:%M:%S')
                     m = tag.message(iter(args))
                     print(ts, tag.loc, m.format())
 
                 args = []
```

### Comparing `smolt-0.1/PKG-INFO` & `smolt-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: smolt
-Version: 0.1
+Version: 0.2
 Summary: Small minimal-overhead logging toolkit
 Author-Email: Vegard Storheil Eriksen <zyp@jvnv.net>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: click>=8.1.7
 Requires-Dist: pyelftools>=0.31
-Requires-Dist: python-orbuculum>=0.0.1
-Requires-Dist: cpp-symbol-parser>=0.1
+Requires-Dist: python-orbuculum<0.1,>=0.0.1
+Requires-Dist: cpp-symbol-parser<0.2,>=0.1.1
 Description-Content-Type: text/markdown
 
 # smolt
 
 Small minimal-overhead logging toolkit.
 
 ## Introduction
@@ -25,15 +25,16 @@
 Smolt is a small header-only C++ library with no dependencies beyond a C++20 compiler with STL. All use of STL is `constexpr`.
 
 When you make a log call, the format string and other metadata is given a tag ID, so the only data that needs to be sent or stored is the tag ID and the format arguments.
 The host side utilities can then use the tag ID to look up all the metadata from the .elf file and handle string formatting.
 
 ## Features
 - Formatting of values on the host with [Python's format string syntax](https://docs.python.org/3/library/string.html#formatstrings).
-  - Currently supports integral and floating point types up to 32 bit.
+  - Currently supports integral and floating point types up to 64 bit.
+  - Basic support for `std::span` and `std::string_view`.
 - Optional metadata attached to messages.
   - Source location.
 - Pluggable transports.
   - `transport::itm`
     - Streaming logging over ARM ITM over SWO or parallel trace.
   - `transport::ringbuffer`
     - Logging to internal ringbuffer for later readout.
@@ -42,26 +43,27 @@
   - Custom transports only have to implement `log_tag(uint32_t)` and `log_value(uint32_t)`.
 - CLI utility
   - Receive and format log messages over ITM from [Orbuculum](https://github.com/orbcode/orbuculum) and other sources that relay ITM messages over TCP.
 - GDB plugin
   - Read out and format log messages from a ringbuffer in target memory.
 
 ## TODO
+- Add a custom formatter for `std::span` that allows setting both an element formatting specifier and an element separator.
 - Support for more argument types:
-  - `uint64_t`, `int64_t`, `double`
-  - `std::string_view`
-  - `std::span`
-    - With a custom formatter that allows e.g. formatting buffers as hex bytes.
+  - Pointers? (I.e. implicit conversion to `uintptr_t` and default formatting as hex.)
 - More transports:
   - `transport::tee`
     - Allows feeding a single logger into multiple transports.
 - More metadata that can be attached to messages:
   - Severity (info, warning, error, etc…).
+- CLI command that checks format string validity (i.e. whether the format specifiers are valid for the types of arguments passed).
+  Can be added to the end of the build process to allow catching typos in format strings at compile time.
+- More checks and error handling.
 - Documentation.
-- Tests.
+- More tests.
 
 ## Usage
 
 ### Example firmware
 [Try it in Compiler Explorer](https://godbolt.org/z/WPP3a81Mn).
 
 ```cpp
```

