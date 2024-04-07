# Comparing `tmp/flapi-0.4.1.tar.gz` & `tmp/flapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flapi-0.4.1.tar", max compression
+gzip compressed data, was "flapi-1.0.0.tar", max compression
```

## Comparing `flapi-0.4.1.tar` & `flapi-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1088 2024-01-20 10:41:54.139710 flapi-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     2298 2024-01-20 10:41:54.139710 flapi-0.4.1/README.md
--rw-r--r--   0        0        0     8288 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__comms.py
--rw-r--r--   0        0        0     1330 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__context.py
--rw-r--r--   0        0        0     2220 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__decorate.py
--rw-r--r--   0        0        0     5624 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__enable.py
--rw-r--r--   0        0        0      692 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__init__.py
--rw-r--r--   0        0        0      500 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__main__.py
--rw-r--r--   0        0        0      951 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/__util.py
--rw-r--r--   0        0        0     4066 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/_consts.py
--rw-r--r--   0        0        0      199 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/__init__.py
--rw-r--r--   0        0        0      333 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/consts.py
--rw-r--r--   0        0        0     1472 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/install.py
--rw-r--r--   0        0        0     6346 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/repl.py
--rw-r--r--   0        0        0      841 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/uninstall.py
--rw-r--r--   0        0        0     1066 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/cli/util.py
--rw-r--r--   0        0        0     3063 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/errors.py
--rw-r--r--   0        0        0        0 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/py.typed
--rw-r--r--   0        0        0     3508 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/script/capout.py
--rw-r--r--   0        0        0     3784 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/script/consts.py
--rw-r--r--   0        0        0     5879 2024-01-20 10:41:54.139710 flapi-0.4.1/flapi/script/device_flapi_server.py
--rw-r--r--   0        0        0     1554 2024-01-20 10:41:54.139710 flapi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 flapi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-07 14:03:21.651530 flapi-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2664 2024-04-07 14:03:21.655530 flapi-1.0.0/README.md
+-rw-r--r--   0        0        0     8369 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__comms.py
+-rw-r--r--   0        0        0     1551 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__context.py
+-rw-r--r--   0        0        0     2220 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__decorate.py
+-rw-r--r--   0        0        0     6259 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__enable.py
+-rw-r--r--   0        0        0      684 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__main__.py
+-rw-r--r--   0        0        0      765 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__util.py
+-rw-r--r--   0        0        0     3780 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/_consts.py
+-rw-r--r--   0        0        0      199 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/consts.py
+-rw-r--r--   0        0        0     1670 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/install.py
+-rw-r--r--   0        0        0     6885 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/repl.py
+-rw-r--r--   0        0        0      841 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/uninstall.py
+-rw-r--r--   0        0        0     1066 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/util.py
+-rw-r--r--   0        0        0     3474 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/errors.py
+-rw-r--r--   0        0        0        0 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/py.typed
+-rw-r--r--   0        0        0     3803 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/capout.py
+-rw-r--r--   0        0        0     3780 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/consts.py
+-rw-r--r--   0        0        0     4556 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/device_flapi_receive.py
+-rw-r--r--   0        0        0     1694 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/device_flapi_respond.py
+-rw-r--r--   0        0        0     5550 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/flapi_response.py
+-rw-r--r--   0        0        0     1545 2024-04-07 14:03:21.655530 flapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 flapi-1.0.0/PKG-INFO
```

### Comparing `flapi-0.4.1/LICENSE.md` & `flapi-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flapi-0.4.1/README.md` & `flapi-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,24 @@
    `pip install flapi`
 
 2. Install the Flapi server to FL Studio by running `flapi install`. If you
    have changed your FL Studio user data folder, you will need to enter it.
 
 3. On Windows, install a virtual MIDI loopback tool such as
    [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) and use it
-   to create a virtual MIDI port named `Flapi`. On MacOS, Flapi is able to
-   create this MIDI port automatically, so this step is not required.
+   to create two virtual MIDI ports, named `Flapi Request` and
+   `Flapi Response`. On MacOS, Flapi is able to create these MIDI ports
+   automatically, so this step is not required.
 
 4. Start or restart FL Studio. The server should be loaded automatically, but
-   if not, you may need to set it up in FL Studio's MIDI settings.
+   if not, you may need to set it up in FL Studio's MIDI settings. To do this,
+   set each MIDI port to have a unique port number in the outputs section,
+   configure the input ports to match the port numbers of their corresponding
+   output ports, then assign the "Flapi Request" port to the "Flapi Request"
+   script and the "Flapi Response" port to the "Flapi Response" script.
 
 ## Usage
 
 ### As a library
 
 ```py
 import flapi
@@ -60,15 +65,15 @@
 Flapi also supports a bare-bones server-side REPL, where all input is executed
 within FL Studio (as opposed to forwarding function data).
 
 ```py
 $ flapi -s server
 >>> import sys
 >>> sys.version
-'3.9.1 (default, Oct 14 2021, 10:29:32) [MSC v.1929 64 bit (AMD64)]'
+'3.12.1 (tags/v3.12.1:2305ca5, Dec  7 2023, 22:03:25) [MSC v.1937 64 bit (AMD64)]'
 # It's running inside FL Studio!
 >>> print("Hello")
 Hello
 # Stdout is redirected back to the client too!
 ```
 
 ## Credits
```

### Comparing `flapi-0.4.1/flapi/__context.py` & `flapi-1.0.0/flapi/__context.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,35 @@
 from flapi.errors import FlapiContextError
 if TYPE_CHECKING:
     from flapi.__decorate import ApiCopyType
 
 
 @dataclass
 class FlapiContext:
-    port: BaseIOPort
+    req_port: BaseIOPort
     """
-    The Mido port that Flapi uses to communicate with FL Studio
+    The Mido port that Flapi uses to send requests to FL Studio
+    """
+
+    res_port: BaseIOPort
+    """
+    The Mido port that Flapi uses to receive responses from FL Studio
     """
 
     functions_backup: 'ApiCopyType'
     """
     References to all the functions we replaced in the FL Studio API, so that
     we can set them back as required.
     """
 
+    client_id: Optional[int]
+    """
+    Unique client ID for this instance of the Flapi client
+    """
+
 
 context: Optional[FlapiContext] = None
 """
 The current context for Flapi
 """
```

### Comparing `flapi-0.4.1/flapi/__decorate.py` & `flapi-1.0.0/flapi/__decorate.py`

 * *Files identical despite different names*

### Comparing `flapi-0.4.1/flapi/__enable.py` & `flapi-1.0.0/flapi/__enable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """
 # Flapi > Initialize
 
 Code for initializing/closing Flapi
 """
 import logging
+import random
 import mido  # type: ignore
 from typing import Protocol, Generic, TypeVar, Optional
-from mido.ports import BaseOutput, BaseInput, IOPort  # type: ignore
+from mido.ports import BaseOutput, BaseInput  # type: ignore
 from . import _consts as consts
-from .__context import set_context, pop_context, FlapiContext
-from .__comms import fl_exec, heartbeat, version_query, poll_for_message
+from .__context import set_context, get_context, pop_context, FlapiContext
+from .__comms import (
+    fl_exec,
+    hello,
+    version_query,
+    poll_for_message,
+    client_goodbye,
+)
 from .__decorate import restore_original_functions, add_wrappers
 from .errors import FlapiPortError, FlapiConnectionError, FlapiVersionError
 
 
 log = logging.getLogger(__name__)
 
 
 T = TypeVar('T', BaseInput, BaseOutput, covariant=True)
 
 
 class OpenPortFn(Protocol, Generic[T]):
     """Function that opens a Mido port"""
+
     def __call__(self, *, name: str, virtual: bool = False) -> T:
         ...
 
 
 def open_port(
     port_name: str,
     port_names: list[str],
@@ -50,91 +58,99 @@
         # Connect to it
         return open(name=curr_port_name)  # type: ignore
 
     # If we reach this point, no match was found
     return None
 
 
-def enable(port_name: str = consts.DEFAULT_PORT_NAME) -> bool:
+def enable(
+    req_port: str = consts.DEFAULT_REQ_PORT,
+    res_port: str = consts.DEFAULT_RES_PORT,
+) -> bool:
     """
     Enable Flapi, connecting it to the given MIDI ports
 
     1. Attempt to connect to the port names provided
     2. Decorate the API functions
     3. Attempt to initialize the connection by running setup commands in FL
        Studio.
 
     ## Returns:
 
     * `bool`: whether the initialization was a success. If this is `False`, you
       will need to call `init()` once FL Studio is running and configured
       correctly.
     """
-    log.info(f"Enable Flapi client on port '{port_name}'")
+    log.info(f"Enable Flapi client on ports '{req_port}', '{res_port}'")
     # First, connect to all the MIDI ports
-    inputs = mido.get_input_names()  # type: ignore
-    outputs = mido.get_output_names()  # type: ignore
+    res_ports = mido.get_input_names()  # type: ignore
+    req_ports = mido.get_output_names()  # type: ignore
 
-    log.info(f"Available inputs are: {inputs}")
-    log.info(f"Available outputs are: {outputs}")
+    log.info(f"Available request ports are: {req_ports}")
+    log.info(f"Available response ports are: {res_ports}")
 
     try:
-        res = open_port(port_name, inputs, mido.open_input)  # type: ignore
+        res = open_port(res_port, res_ports, mido.open_input)  # type: ignore
     except Exception:
         log.exception("Error when connecting to input")
         raise
     try:
-        req = open_port(port_name, outputs, mido.open_output)  # type: ignore
+        req = open_port(req_port, req_ports, mido.open_output)  # type: ignore
     except Exception:
         log.exception("Error when connecting to output")
         raise
 
     if res is None or req is None:
         try:
-            port = mido.open_ioport(  # type: ignore
-                name=port_name,
+            req = mido.open_output(  # type: ignore
+                name=req_port,
+                virtual=True,
+            )
+            res = mido.open_input(  # type: ignore
+                name=res_port,
                 virtual=True,
             )
         except NotImplementedError as e:
             # Port could not be opened
             log.exception("Could not open create new port")
-            raise FlapiPortError(port_name) from e
-    else:
-        port = IOPort(res, req)
+            raise FlapiPortError((req_port, res_port)) from e
 
     # Now decorate all of the API functions
     functions_backup = add_wrappers()
 
     # Register the context
-    set_context(FlapiContext(port, functions_backup))
+    set_context(FlapiContext(req, res, functions_backup, None))
 
-    return try_init()
+    return try_init(random.randrange(1, 0x7F))
 
 
-def init():
+def init(client_id: int):
     """
     Initialize Flapi, so that it can send commands to FL Studio.
     """
-    if not try_init():
+    if not try_init(client_id):
         raise FlapiConnectionError(
             "FL Studio did not connect to Flapi - is it running?")
 
 
-def try_init() -> bool:
+def try_init(client_id: int) -> bool:
     """
     Attempt to initialize Flapi, returning whether the operation was a success.
     """
+    assert get_context().client_id is None
+    get_context().client_id = client_id
     # Poll for any new messages from FL Studio and handle them as required
     poll_for_message()
     # Attempt to send a heartbeat message - if we get a response, we're already
     # connected
-    if heartbeat():
+    if hello():
         setup_server()
         return True
     else:
+        get_context().client_id = None
         return False
 
 
 def setup_server():
     """
     Perform the required setup on the server side, importing modules, and the
     like.
@@ -169,19 +185,28 @@
             f"{client_version}. Please update the client using your Python "
             f"package manager. If you are using pip, run "
             f"`pip install --upgrade flapi`."
         )
     # If we reach this point, the versions match
 
 
-def disable():
+def disable(code: int = 0):
     """
-    Disable Flapi, closing its MIDI ports and its connection to FL Studio
+    Disable Flapi, closing its MIDI ports and its connection to FL Studio.
 
     This restores the original functions for the FL Studio API.
+
+    ## Args
+
+    * `code` (`int`, optional): the exit code to relay to the server. Defaults
+      to `0`.
     """
+    # Send a client goodbye
+    client_goodbye(code)
+
     # Close all the ports
     ctx = pop_context()
-    ctx.port.close()
+    ctx.req_port.close()
+    ctx.res_port.close()
 
     # Then restore the functions
     restore_original_functions(ctx.functions_backup)
```

### Comparing `flapi-0.4.1/flapi/__init__.py` & `flapi-1.0.0/flapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 >>> flapi.enable()  # Connect to a MIDI port
 >>> flapi.init()  # Establish the connection with FL Studio
 >>> import transport
 >>> transport.start()  # FL Studio starts playing
 ```
 """
 from .__enable import enable, init, try_init, disable
-from .__comms import heartbeat, fl_exec, fl_eval, fl_print
+from .__comms import hello, fl_exec, fl_eval, fl_print
 from . import errors
 from ._consts import VERSION
 
 
 # Set up the version string
 __version__ = ".".join(str(n) for n in VERSION)
 del VERSION
 
 
 __all__ = [
     "enable",
     "init",
     "try_init",
     "disable",
-    "heartbeat",
+    "hello",
     "fl_exec",
     "fl_eval",
     "fl_print",
     "errors",
 ]
```

### Comparing `flapi-0.4.1/flapi/cli/install.py` & `flapi-1.0.0/flapi/cli/install.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Simple script for installing the Flapi server into FL Studio
 """
 import click
 from shutil import copytree, rmtree
 from pathlib import Path
 from . import consts
-from .util import yn_prompt, output_dir, script_dir
+from .util import yn_prompt, output_dir, server_dir
 
 
 @click.command()
 @click.option(
     "-d",
     "--data-dir",
     default=consts.DEFAULT_IL_DATA_DIR,
@@ -21,15 +21,20 @@
 )
 @click.option(
     "-y",
     "--yes",
     is_flag=True,
     help="Always overwrite the server installation"
 )
-def install(data_dir: Path, yes: bool = False):
+@click.option(
+    "--dev",
+    is_flag=True,
+    help="Install a live (development) server"
+)
+def install(data_dir: Path, yes: bool = False, dev: bool = False):
     """
     Install the Flapi server to FL Studio
     """
     if data_dir == Path("-"):
         data_dir = consts.DEFAULT_IL_DATA_DIR
     # Determine scripts folder location
     output_location = output_dir(data_dir)
@@ -41,15 +46,18 @@
         else:
             if not yn_prompt("Overwrite? [y/N]: ", default=False):
                 print("Operation cancelled")
                 exit(1)
         rmtree(output_location)
 
     # Determine where we are, so we can locate the script folder
-    script_location = script_dir()
+    script_location = server_dir()
 
     # Now copy the script folder to the output folder
-    copytree(script_location, output_location)
+    if dev:
+        output_location.symlink_to(script_location, True)
+    else:
+        copytree(script_location, output_location)
 
     print(
         "Success! Make sure you restart FL Studio so the server is registered"
     )
```

### Comparing `flapi-0.4.1/flapi/cli/repl.py` & `flapi-1.0.0/flapi/cli/repl.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 Starts a simple REPL to interact with FL Studio, using IPython (if available)
 or Python's integrated shell.
 """
 import code
 import click
 import sys
+import os
 import time
+import random
 from typing import Optional
 from traceback import print_exc
 import flapi
 from flapi import (
     enable,
     init,
     try_init,
     disable,
-    heartbeat,
     fl_exec,
     fl_eval,
     fl_print,
 )
 from flapi import _consts as consts
+from flapi.errors import FlapiServerExit
 from flapi.cli import consts as cli_consts
 from .util import handle_verbose
 try:
     import IPython
     from IPython import start_ipython
     from traitlets.config.loader import Config as IPythonConfig
 except ImportError:
@@ -34,15 +36,14 @@
     IPythonConfig = None  # type: ignore
 
 
 SHELL_SCOPE = {
     "enable": enable,
     "init": init,
     "disable": disable,
-    "heartbeat": heartbeat,
     "fl_exec": fl_exec,
     "fl_eval": fl_eval,
     "fl_print": fl_print,
 }
 
 
 def wait_for_connection(max_wait: float) -> bool:
@@ -63,27 +64,29 @@
             return " .."
         elif pos == 4:
             return "  ."
         else:  # pos == 5
             return "   "
 
     start_time = time.time()
-    while not try_init():
+    while not try_init(random.randrange(1, 0x7F)):
         delta = time.time() - start_time
         if delta > max_wait:
             return False
 
         # Print progress
         print(
             f" {ellipsis(delta)} Connecting to FL Studio ({int(delta)}"
             f"/{int(max_wait)}s)",
             end='\r',
         )
 
-    print("Connected to FL Studio")
+    # Yucky thing to ensure that we write all the way to the end of the line
+    msg = "Connected to FL Studio"
+    print(msg + ' ' * (os.get_terminal_size().columns - len(msg)))
     return True
 
 
 def exec_lines(lines: list[str]) -> bool:
     """
     Attempt to execute the given lines on the server.
 
@@ -115,14 +118,20 @@
         exit()
     try:
         if is_statement:
             fl_exec(source)
         else:
             res = fl_eval(source)
             print(repr(res))
+    except FlapiServerExit:
+        print(
+            "Error: the Flapi server exited, likely because FL Studio was "
+            "closed."
+        )
+        exit(1)
     except Exception:
         print_exc()
 
     return True
 
 
 def start_server_shell():
@@ -134,14 +143,15 @@
     last_was_interrupted = False
 
     while True:
         try:
             line = input(">>> " if not len(lines) else "... ")
         except KeyboardInterrupt:
             if last_was_interrupted:
+                disable()
                 exit()
             else:
                 print("\nKeyboard interrupt. Press again to quit")
                 last_was_interrupted = True
                 continue
 
         last_was_interrupted = False
@@ -180,42 +190,48 @@
     "-s",
     "--shell",
     type=click.Choice(["ipython", "python", "server"], case_sensitive=False),
     help="The shell to use with Flapi.",
     default=None,
 )
 @click.option(
-    "-p",
-    "--port",
+    "--req",
+    type=str,
+    help="The name of the MIDI port to send requests on",
+    default=consts.DEFAULT_REQ_PORT,
+)
+@click.option(
+    "--res",
     type=str,
-    help="The name of the MIDI port to connect to",
-    default=consts.DEFAULT_PORT_NAME,
+    help="The name of the MIDI port to receive responses on",
+    default=consts.DEFAULT_RES_PORT,
 )
 @click.option(
     "-t",
     "--timeout",
     type=float,
     help="Maximum time to wait to establish a connection with FL Studio",
     default=cli_consts.CONNECTION_TIMEOUT,
 )
 @click.option('-v', '--verbose', count=True)
 def repl(
     shell: Optional[str] = None,
-    port: str = consts.DEFAULT_PORT_NAME,
+    req: str = consts.DEFAULT_REQ_PORT,
+    res: str = consts.DEFAULT_RES_PORT,
     timeout: float = cli_consts.CONNECTION_TIMEOUT,
     verbose: int = 0,
 ):
     """Main function to set up the Python shell"""
     handle_verbose(verbose)
     print("Flapi interactive shell")
     print(f"Client version: {flapi.__version__}")
     print(f"Python version: {sys.version}")
 
     # Set up the connection
-    status = enable(port)
+    status = enable(req, res)
 
     if not status:
         status = wait_for_connection(timeout)
 
     if shell == "server":
         if status:
             start_server_shell()
@@ -233,15 +249,15 @@
         print(
             "Please verify that FL Studio is running and the server is "
             "installed"
         )
         print("Then, run `init()` to create the connection.")
 
     print("Imported functions:")
-    print("enable, init, disable, heartbeat, fl_exec, fl_eval")
+    print(", ".join(SHELL_SCOPE.keys()))
 
     if shell == "python":
         return start_python_shell()
     elif shell == "ipython":
         if IPython is None:
             print("Error: IPython is not installed!")
             exit(1)
```

### Comparing `flapi-0.4.1/flapi/cli/uninstall.py` & `flapi-1.0.0/flapi/cli/uninstall.py`

 * *Files identical despite different names*

### Comparing `flapi-0.4.1/flapi/cli/util.py` & `flapi-1.0.0/flapi/cli/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,12 +37,12 @@
     """
     Return the path to the directory where the script should be installed
     """
     return data_dir.joinpath(
         "FL Studio", "Settings", "Hardware", "Flapi Server")
 
 
-def script_dir() -> Path:
+def server_dir() -> Path:
     """
     Return the current location of the Flapi server script
     """
-    return Path(__file__).parent.parent.joinpath("script")
+    return Path(__file__).parent.parent.joinpath("server")
```

### Comparing `flapi-0.4.1/flapi/errors.py` & `flapi-1.0.0/flapi/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     """
     Unable to open a MIDI port
 
     On Windows, this happens when trying to create a virtual MIDI port, since
     it is currently impossible to do so without a kernel-mode driver for some
     reason.
     """
-    def __init__(self, port_name: str) -> None:
+
+    def __init__(self, port_names: tuple[str, str]) -> None:
         super().__init__(
-            f"Could not create port '{port_name}'. On Windows, you need to "
+            f"Could not create ports {port_names}. On Windows, you need to "
             f"use software such as Loop MIDI "
             f"(https://www.tobias-erichsen.de/software/loopmidi.html) to "
             f"create the required ports yourself, as doing so requires a "
             f"kernel-mode driver, which cannot be bundled in a Python library."
         )
 
 
@@ -31,14 +32,15 @@
     """
 
 
 class FlapiContextError(Exception):
     """
     Flapi wasn't initialised, so its context could not be loaded
     """
+
     def __init__(self) -> None:
         super().__init__(
             "Could not find Flapi context. Perhaps you haven't initialised "
             "Flapi by calling `flapi.enable()`."
         )
 
 
@@ -48,44 +50,67 @@
     """
 
 
 class FlapiInvalidMsgError(ValueError):
     """
     Flapi unexpectedly received a MIDI message that it could not process
     """
+
     def __init__(self, msg: bytes) -> None:
         super().__init__(
             f"Flapi received a message that it didn't understand. Perhaps "
             f"another device is communicating on Flapi's MIDI port. Message "
             f"received: {bytes_to_str(msg)}"
         )
 
 
 class FlapiServerError(Exception):
     """
     An unexpected error occurred on the server side.
 
     Ensure that the Flapi server and client have matching versions.
     """
+
     def __init__(self, msg: str) -> None:
         super().__init__(
             f"An unexpected server error occurred due to a miscommunication. "
             f"Please ensure the Flapi server version matches that of the "
             f"Flapi client by running the `flapi install` command. "
             f"If they do match, please open a bug report. "
             f"Failure message: {msg}"
         )
 
 
+class FlapiServerExit(Exception):
+    """
+    The Flapi server exited.
+    """
+
+    def __init__(self) -> None:
+        super().__init__(
+            "The Flapi server exited, likely because FL Studio was closed."
+        )
+
+
+class FlapiClientExit(SystemExit):
+    """
+    The flapi client requested to exit
+    """
+
+    def __init__(self, code: int) -> None:
+        super().__init__(code)
+
+
 class FlapiClientError(Exception):
     """
     An unexpected error occurred on the client side.
 
     Ensure that the Flapi server and client have matching versions.
     """
+
     def __init__(self, msg: str) -> None:
         super().__init__(
             f"An unexpected client error occurred due to a miscommunication. "
             f"Please ensure the Flapi server version matches that of the "
             f"Flapi client by running the `flapi install` command. "
             f"If they do match, please open a bug report. "
             f"Failure message: {msg}"
```

### Comparing `flapi-0.4.1/flapi/script/capout.py` & `flapi-1.0.0/flapi/server/capout.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 try:
     # This is the module in most Python installs, used for type safety
     from io import StringIO, TextIOBase
 except ImportError:
     # This is the module in FL Studio for some reason
     from _io import StringIO, _TextIOBase as TextIOBase  # type: ignore
 try:
-    from typing import Optional, Callable
+    from typing import Optional, Callable, Self
 except ImportError:
     pass
 
 
-class CapoutBuffer(TextIOBase):  # type: ignore
+class CapoutBuffer(TextIOBase):
     """
     Custom buffer wrapping a StringIO, so that we can implement a callback
     whenever buffer is flushed, and flush it to the client.
 
     This is probably awful design, but it seems to work so I'm keeping it until
     I feel like writing something nicer.
     """
+
     def __init__(self, callback: 'Callable[[str], None]') -> None:
         self.__callback = callback
         self.__buf = StringIO()
 
     def close(self):
         return self.__buf.close()
 
@@ -103,18 +104,32 @@
         return self.__buf.write(s)
 
 
 class Capout:
     """
     Capture stdout in FL Studio
     """
+
     def __init__(self, callback: 'Callable[[str], None]') -> None:
         self.enabled = False
         self.real_stdout = sys.stdout
         self.fake_stdout = CapoutBuffer(callback)
+        self.target = 0
+
+    def __call__(self, target: int) -> Self:
+        self.target = target
+        return self
+
+    def __enter__(self) -> None:
+        self.enable()
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        self.flush()
+        self.disable()
+        self.target = 0
 
     def flush(self) -> None:
         if self.enabled:
             self.fake_stdout.flush()
 
     def enable(self):
         self.enabled = True
```

### Comparing `flapi-0.4.1/pyproject.toml` & `flapi-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flapi"
-version = "0.4.1"
+version = "1.0.0"
 description = "Remotely control FL Studio using the MIDI Controller Scripting API"
 authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MiguelGuthridge/Flapi"
 
 keywords = [
@@ -28,36 +28,32 @@
     "Environment :: Other Environment",
     "Typing :: Typed",
 ]
 
 include = ["py.typed"]
 
 
-packages = [
-    { include = "flapi" }
-]
+packages = [{ include = "flapi" }]
 
 [tool.poetry.urls]
 "Online Documentation" = "https://miguelguthridge.github.io/Flapi"
 "Bug Tracker" = "https://github.com/MiguelGuthridge/Flapi/issues"
 
 [tool.poetry.scripts]
 flapi = "flapi.__main__:cli"
 
 [tool.mypy]
-exclude = [
-    'flapi/script/*',
-]
+exclude = ['flapi/server/*']
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fl-studio-api-stubs = ">=28.2.2"
-mido = {extras = ["ports-rtmidi"], version = "^1.3.2"}
+mido = { extras = ["ports-rtmidi"], version = "^1.3.2" }
 typing-extensions = "^4.9.0"
-ipython = {version = "^8.18.1", optional = true}
+ipython = { version = "^8.18.1", optional = true }
 click = "^8.1.7"
 click-default-group = "^1.2.4"
 
 [tool.poetry.extras]
 ipython = ["ipython"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `flapi-0.4.1/PKG-INFO` & `flapi-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flapi
-Version: 0.4.1
+Version: 1.0.0
 Summary: Remotely control FL Studio using the MIDI Controller Scripting API
 Home-page: https://github.com/MiguelGuthridge/Flapi
 License: MIT
 Keywords: fl,studio,fl studio,midi,script,midi controller scripting,remote,remote control
 Author: Miguel Guthridge
 Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.9,<4.0
@@ -54,19 +54,24 @@
    `pip install flapi`
 
 2. Install the Flapi server to FL Studio by running `flapi install`. If you
    have changed your FL Studio user data folder, you will need to enter it.
 
 3. On Windows, install a virtual MIDI loopback tool such as
    [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) and use it
-   to create a virtual MIDI port named `Flapi`. On MacOS, Flapi is able to
-   create this MIDI port automatically, so this step is not required.
+   to create two virtual MIDI ports, named `Flapi Request` and
+   `Flapi Response`. On MacOS, Flapi is able to create these MIDI ports
+   automatically, so this step is not required.
 
 4. Start or restart FL Studio. The server should be loaded automatically, but
-   if not, you may need to set it up in FL Studio's MIDI settings.
+   if not, you may need to set it up in FL Studio's MIDI settings. To do this,
+   set each MIDI port to have a unique port number in the outputs section,
+   configure the input ports to match the port numbers of their corresponding
+   output ports, then assign the "Flapi Request" port to the "Flapi Request"
+   script and the "Flapi Response" port to the "Flapi Response" script.
 
 ## Usage
 
 ### As a library
 
 ```py
 import flapi
@@ -94,15 +99,15 @@
 Flapi also supports a bare-bones server-side REPL, where all input is executed
 within FL Studio (as opposed to forwarding function data).
 
 ```py
 $ flapi -s server
 >>> import sys
 >>> sys.version
-'3.9.1 (default, Oct 14 2021, 10:29:32) [MSC v.1929 64 bit (AMD64)]'
+'3.12.1 (tags/v3.12.1:2305ca5, Dec  7 2023, 22:03:25) [MSC v.1937 64 bit (AMD64)]'
 # It's running inside FL Studio!
 >>> print("Hello")
 Hello
 # Stdout is redirected back to the client too!
 ```
 
 ## Credits
```

