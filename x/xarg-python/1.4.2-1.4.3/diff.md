# Comparing `tmp/xarg-python-1.4.2.tar.gz` & `tmp/xarg-python-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.2.tar", last modified: Sat Apr  6 10:43:04 2024, max compression
+gzip compressed data, was "xarg-python-1.4.3.tar", last modified: Sun Apr  7 18:23:28 2024, max compression
```

## Comparing `xarg-python-1.4.2.tar` & `xarg-python-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-06 10:43:04.735508 xarg-python-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-06 10:43:04.735508 xarg-python-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/xarg/
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.2/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22972 2024-04-06 10:36:59.000000 xarg-python-1.4.2/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-06 10:42:08.000000 xarg-python-1.4.2/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-04-05 16:52:06.000000 xarg-python-1.4.2/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.2/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.2/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.2/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.2/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.2/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.192449 xarg-python-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-07 18:23:28.192449 xarg-python-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-07 18:23:28.192449 xarg-python-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.182449 xarg-python-1.4.3/xarg/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.3/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22718 2024-04-07 18:19:56.000000 xarg-python-1.4.3/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-07 18:22:33.000000 xarg-python-1.4.3/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-06 18:33:10.000000 xarg-python-1.4.3/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.3/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2024-04-07 18:03:05.000000 xarg-python-1.4.3/xarg/logger.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.3/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.3/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.3/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.3/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 18:23:28.192449 xarg-python-1.4.3/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 18:23:28.000000 xarg-python-1.4.3/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4.2/LICENSE` & `xarg-python-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/PKG-INFO` & `xarg-python-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

### Comparing `xarg-python-1.4.2/README.md` & `xarg-python-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/setup.cfg` & `xarg-python-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/setup.py` & `xarg-python-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/actuator.py` & `xarg-python-1.4.3/xarg/actuator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # coding:utf-8
 
 from argparse import Namespace
 from errno import EINTR
 from errno import ENOENT
 import logging
-import os
+from logging import Logger
 import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
-from colorlog import ColoredFormatter
-
+from .attribute import __prog_name__
+from .logger import log
+from .logger import once_filter as log_once_filter
 from .parser import argp
 from .util import singleton
 
-DEFAULT_LOG_FORMAT = "%(log_color)s%(message)s"
-DEFAULT_LOG_COLORS = {
-    "DEBUG": "black",
-    "INFO": "white",
-    "WARNING": "yellow",
-    "ERROR": "red",
-    "CRITICAL": "light_red",
-}
-
 
 class add_command:
     '''Define a new command-line node.
 
     For example:
 
     >>> from xarg import add_command\n
@@ -331,23 +324,20 @@
     >>>         argv=argv,\n
     >>>         prog="xarg-example",\n
     >>>         description="Simple command-line tool based on argparse.")\n
     '''
 
     LOGGER_ARGUMENT_GROUP = "logger options"
 
-    def __init__(self, version: Optional[str] = None,
-                 enable_logger: bool = True):
-        assert isinstance(version, str) or version is None
-        assert isinstance(enable_logger, bool)
-        self.__prog: str = "xarg"
+    def __init__(self):
+        self.__prog: str = __prog_name__
         self.__root: Optional[add_command] = None
         self.__args: Namespace = Namespace()
-        self.__version: Optional[str] = version
-        self.__enable_logger: bool = enable_logger
+        self.__version: Optional[str] = None
+        self.__logging: log = log(True)
 
     @property
     def prog(self) -> str:
         return self.__prog
 
     @property
     def root(self) -> Optional[add_command]:
@@ -380,28 +370,44 @@
 
     @version.setter
     def version(self, value: str):
         assert isinstance(value, str)
         _version = value.strip()
         self.__version = _version
 
-    @property
-    def enable_logger(self) -> bool:
-        return self.__enable_logger
+    def initiate_logging(self, level: Optional[str] = None,
+                         handlers: Optional[Iterable[logging.Handler]] = None,
+                         filters: Optional[Iterable[logging.Filter]] = None):
+        assert self.logging.enabled is True
+        logger: logging.Logger = self.logger
+
+        if isinstance(level, str):
+            logger.setLevel(logging._nameToLevel[level.upper()])
+
+        if filters is None:
+            filters = [log_once_filter()]
+
+        for filter in filters:
+            logger.addFilter(filter)
+
+        if handlers is None:
+            handlers = [self.logging.new_stream_handler(stream=sys.stdout)]
 
-    @enable_logger.setter
-    def enable_logger(self, value: bool):
-        assert isinstance(value, bool)
-        self.__enable_logger = value
+        for handler in handlers:
+            logger.addHandler(handler)
 
     @property
-    def logger(self) -> logging.Logger:
+    def logging(self) -> log:
+        return self.__logging
+
+    @property
+    def logger(self) -> Logger:
         '''Logger.
         '''
-        return logging.getLogger(self.prog)
+        return self.logging.get_logger(self.prog)
 
     def stdout(self, context: Any):
         '''Output string to sys.stdout.
         '''
         sys.stdout.write(f"{context}\n")
         sys.stdout.flush()
 
@@ -428,34 +434,30 @@
             if len(options) > 0:
                 for i in name:
                     if i in options:
                         return i
             return None
 
         def add_optional_level():
-
-            def get_all_level_name() -> List[str]:
-                return ["fatal", "error", "warn", "info", "debug"]
-
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_level = group.add_mutually_exclusive_group()
 
             option_level = filter_optional_name("--level", "--log-level")
             if isinstance(option_level, str):
                 group_level.add_argument(
                     option_level,
                     type=str,
                     nargs="?",
                     const="info",
                     default="info",
-                    choices=get_all_level_name(),
+                    choices=self.logging.ALLOWED_LOG_LEVELS,
                     dest="_log_level_str_",
                     help="Logger output level, default info.")
 
-            for level in get_all_level_name():
+            for level in self.logging.ALLOWED_LOG_LEVELS:
                 options = []
                 if isinstance(filter_optional_name(f"-{level[0]}"), str):
                     options.append(f"-{level[0]}")
                 if isinstance(filter_optional_name(f"--{level}"), str):
                     options.append(f"--{level}")
                 elif isinstance(filter_optional_name(f"--{level}-level"), str):
                     options.append(f"--{level}-level")
@@ -494,15 +496,15 @@
                 " %(message)s"
 
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group.add_argument(option,
                                type=str,
                                nargs="?",
                                const=DEFAULT_LOG_FMT,
-                               default=DEFAULT_LOG_FORMAT,
+                               default=self.logging.DEFAULT_LOG_FORMAT,
                                metavar="STRING",
                                dest="_log_format_",
                                help="Logger output format.")
 
         def add_optional_console():
             group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_std = group.add_mutually_exclusive_group()
@@ -519,51 +521,41 @@
             if isinstance(option, str):
                 group_std.add_argument(option,
                                        const=sys.stderr,
                                        action="store_const",
                                        dest="_log_console_",
                                        help="Logger output to stderr.")
 
-        if self.enable_logger:
+        if self.logging.enabled:
             add_optional_level()
             add_optional_stream()
             add_optional_format()
             add_optional_console()
 
     def __parse_logger(self, args: Namespace):
-        if not self.enable_logger:
+        if not self.logging.enabled:
             return
 
-        # save debug level to local variable
-        if hasattr(args, "_log_level_str_") and\
-           isinstance(args._log_level_str_, str):
-            level_name = args._log_level_str_.upper()
-            self.logger.setLevel(logging._nameToLevel[level_name])
-
-        def addHandler(handler: logging.Handler):
-            formatter: logging.Formatter = ColoredFormatter(
-                fmt=args._log_format_ if hasattr(args, "_log_format_")
-                and isinstance(args._log_format_, str) else None,
-                datefmt=None,
-                log_colors=DEFAULT_LOG_COLORS,
-                no_color=isinstance(handler, logging.FileHandler))
-            handler.setFormatter(formatter)
-            self.logger.addHandler(handler)
+        level_name: Optional[str] = args._log_level_str_.upper() if hasattr(
+            args, "_log_level_str_") and isinstance(
+            args._log_level_str_, str) else None
+        fmt: Optional[str] = args._log_format_ if hasattr(
+            args, "_log_format_") and isinstance(
+            args._log_format_, str) else None
 
+        handlers: List[logging.Handler] = []
         if hasattr(args, "_log_console_") and args._log_console_ is not None:
-            addHandler(logging.StreamHandler(stream=args._log_console_))
-
+            handlers.append(
+                log.new_stream_handler(stream=args._log_console_, fmt=fmt))
         if hasattr(args, "_log_files_"):
             for filename in args._log_files_:
-                assert isinstance(filename, str), \
-                    f"Unexpected type: {type(filename)}"
-                dirname: str = os.path.dirname(filename)
-                if not os.path.exists(dirname):
-                    os.makedirs(dirname)
-                addHandler(logging.FileHandler(filename))
+                handlers.append(
+                    log.new_file_handler(filename=filename, fmt=fmt))
+
+        self.initiate_logging(level=level_name, handlers=handlers)
 
     def __add_parser(self, _map: Dict[add_command, argp],
                      arg_root: argp, cmd_root: add_command, **kwargs):
         assert isinstance(cmd_root, add_command)
         assert cmd_root not in _map
         _map[cmd_root] = arg_root
```

### Comparing `xarg-python-1.4.2/xarg/colorful.py` & `xarg-python-1.4.3/xarg/colorful.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/complete.py` & `xarg-python-1.4.3/xarg/complete.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/parser.py` & `xarg-python-1.4.3/xarg/parser.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/safefile.py` & `xarg-python-1.4.3/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/scanner.py` & `xarg-python-1.4.3/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg/util.py` & `xarg-python-1.4.3/xarg/util.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.2/xarg_python.egg-info/PKG-INFO` & `xarg-python-1.4.3/xarg_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

