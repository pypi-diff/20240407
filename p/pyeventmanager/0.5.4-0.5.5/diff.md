# Comparing `tmp/pyeventmanager-0.5.4.tar.gz` & `tmp/pyeventmanager-0.5.5.tar.gz`

## Comparing `pyeventmanager-0.5.4.tar` & `pyeventmanager-0.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/event_manager.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/fork_types.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/listeners/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/listeners/base.py
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/listeners/batch.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/listeners/scheduled.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/listeners/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/queues/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/queues/base.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/event_manager/queues/memory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/tests/test_dummy.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/.gitignore
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/README.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 pyeventmanager-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/event_manager.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/fork_types.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/listeners/__init__.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/listeners/base.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/listeners/batch.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/listeners/scheduled.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/listeners/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/queues/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/queues/base.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/event_manager/queues/memory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/tests/test_dummy.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/.gitignore
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/README.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 pyeventmanager-0.5.5/PKG-INFO
```

### Comparing `pyeventmanager-0.5.4/CHANGELOG.md` & `pyeventmanager-0.5.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.5.5](https://github.com/JeordyR/PyEventManager/compare/v0.5.4...v0.5.5) (2024-04-07)
+
+
+### Bug Fixes
+
+* add log when listener raises exception ([88ca42e](https://github.com/JeordyR/PyEventManager/commit/88ca42e218b30fcdb7b2882c6b5712ce156b896e))
+
 ## [0.5.4](https://github.com/JeordyR/PyEventManager/compare/v0.5.3...v0.5.4) (2024-04-07)
 
 
 ### Bug Fixes
 
 * remove broken condition on batch call/return of callback ([55717f9](https://github.com/JeordyR/PyEventManager/commit/55717f99c41fce26b52b51cd50ff633445a113c0))
```

### Comparing `pyeventmanager-0.5.4/.github/workflows/ci.yml` & `pyeventmanager-0.5.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/.github/workflows/docs.yml` & `pyeventmanager-0.5.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/event_manager.py` & `pyeventmanager-0.5.5/event_manager/event_manager.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/tree.py` & `pyeventmanager-0.5.5/event_manager/tree.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/listeners/base.py` & `pyeventmanager-0.5.5/event_manager/listeners/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import inspect
+import logging
 from collections.abc import Callable
 from concurrent.futures import Future
 from typing import Protocol
 
 from event_manager.fork_types import ForkType
 
+logger = logging.getLogger("event_manager")
+
 
 class BaseListener(Protocol):
     """
     An abstract class that represents a listener. It should not be used directly, but through its concrete subclasses.
     """
 
     event: str
@@ -30,8 +33,9 @@
     if _future.set_running_or_notify_cancel():
         try:
             if inspect.getfullargspec(_func).args or inspect.getfullargspec(_func).kwonlyargs:
                 _future.set_result(_func(*args, **kwargs))
             else:
                 _future.set_result(_func())
         except Exception as e:
+            logger.error(f"Listener {_func.__name__} raised exception: {e}")
             _future.set_exception(e)
```

### Comparing `pyeventmanager-0.5.4/event_manager/listeners/batch.py` & `pyeventmanager-0.5.5/event_manager/listeners/batch.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/listeners/scheduled.py` & `pyeventmanager-0.5.5/event_manager/listeners/scheduled.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/listeners/simple.py` & `pyeventmanager-0.5.5/event_manager/listeners/simple.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/queues/base.py` & `pyeventmanager-0.5.5/event_manager/queues/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/event_manager/queues/memory.py` & `pyeventmanager-0.5.5/event_manager/queues/memory.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/.gitignore` & `pyeventmanager-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/README.md` & `pyeventmanager-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.4/pyproject.toml` & `pyeventmanager-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyeventmanager"
-version = "0.5.4"
+version = "0.5.5"
 authors = [{ name = "Jeordy", email = "JeordyR@users.noreply.github.com" }]
 description = "Event management system for Python with support for Threading and Multiprocessing for task running."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `pyeventmanager-0.5.4/PKG-INFO` & `pyeventmanager-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyeventmanager
-Version: 0.5.4
+Version: 0.5.5
 Summary: Event management system for Python with support for Threading and Multiprocessing for task running.
 Project-URL: Documentation, https://event-manager.jeofi.com
 Project-URL: Homepage, https://event-manager.jeofi.com
 Project-URL: Repository, https://github.com/JeordyR/PyEventManager
 Project-URL: Issues, https://github.com/JeordyR/PyEventManager/issues
 Author-email: Jeordy <JeordyR@users.noreply.github.com>
 Classifier: Operating System :: OS Independent
```

