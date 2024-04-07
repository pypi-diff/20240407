# Comparing `tmp/pyeventmanager-0.5.2.tar.gz` & `tmp/pyeventmanager-0.5.3.tar.gz`

## Comparing `pyeventmanager-0.5.2.tar` & `pyeventmanager-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/event_manager.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/fork_types.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/base.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/batch.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/scheduled.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/base.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/memory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/tests/test_dummy.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.gitignore
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/README.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/event_manager.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/fork_types.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/listeners/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/listeners/base.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/listeners/batch.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/listeners/scheduled.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/listeners/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/queues/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/queues/base.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/event_manager/queues/memory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/tests/test_dummy.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/.gitignore
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/README.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 pyeventmanager-0.5.3/PKG-INFO
```

### Comparing `pyeventmanager-0.5.2/CHANGELOG.md` & `pyeventmanager-0.5.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.5.3](https://github.com/JeordyR/PyEventManager/compare/v0.5.2...v0.5.3) (2024-04-06)
+
+
+### Bug Fixes
+
+* remove prints and a few debug logs from batch listener ([37999a3](https://github.com/JeordyR/PyEventManager/commit/37999a3c5d83884d1ecc11157448fb251d9752c2))
+
 ## [0.5.2](https://github.com/JeordyR/PyEventManager/compare/v0.5.1...v0.5.2) (2024-04-06)
 
 
 ### Bug Fixes
 
 * fix batch to handle 0 batch_count, EventManager methods to classmethods, schedule listener to daemon ([c503205](https://github.com/JeordyR/PyEventManager/commit/c5032051d44e561734a4797d43cde1f3a07be3eb))
```

### Comparing `pyeventmanager-0.5.2/.github/workflows/ci.yml` & `pyeventmanager-0.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/.github/workflows/docs.yml` & `pyeventmanager-0.5.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/event_manager.py` & `pyeventmanager-0.5.3/event_manager/event_manager.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/tree.py` & `pyeventmanager-0.5.3/event_manager/tree.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/listeners/base.py` & `pyeventmanager-0.5.3/event_manager/listeners/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/listeners/batch.py` & `pyeventmanager-0.5.3/event_manager/listeners/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,45 +20,39 @@
     Function that will run in a thread to batch up the events, then call the stored function to process them.
 
     Args:
         batch_window (int): How long to batch up event data when invoked before processing events.
         queue (QueueInterface): Queue used to batch up the events.
         callback (Callable): Function to call to process the events.
     """
-    print("starting...")
     logger.debug(f"Starting batch input for {callback.__name__}...")
 
-    sleep_time = 1 if batch_window else batch_idle_window
+    sleep_time = batch_idle_window if batch_idle_window > 0 else 1
     elapsed = 0
 
     while True:
-        print("looping...")
         time.sleep(sleep_time)
         elapsed += 1
 
         logger.debug(f"{callback.__name__}: {queue.last_updated=}")
 
         if batch_count > 0 and len(queue) >= batch_count:
-            print("breaking for batch count...")
             break
         elif batch_idle_window > 0 and queue.last_updated:
             since_last = datetime.now() - queue.last_updated
             since_last = since_last.seconds
             logger.debug(f"{callback.__name__}: {since_last=}")
 
             if since_last > batch_idle_window:
-                print("breaking for idle window...")
                 break
             else:
-                print("waiting for idle window...")
                 logger.info(
                     f"Batch data updated too recently for func {callback.__name__}, waiting {batch_window} seconds."
                 )
         elif batch_window > 0 and batch_window <= elapsed:
-            print("breaking for batch window...")
             break
 
     logger.debug(f"Batching complete for {callback.__name__}, executing...")
 
     if batch_count > 0:
         return callback(queue.get_all())
```

### Comparing `pyeventmanager-0.5.2/event_manager/listeners/scheduled.py` & `pyeventmanager-0.5.3/event_manager/listeners/scheduled.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/listeners/simple.py` & `pyeventmanager-0.5.3/event_manager/listeners/simple.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/queues/base.py` & `pyeventmanager-0.5.3/event_manager/queues/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/event_manager/queues/memory.py` & `pyeventmanager-0.5.3/event_manager/queues/memory.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/.gitignore` & `pyeventmanager-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/README.md` & `pyeventmanager-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.2/pyproject.toml` & `pyeventmanager-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyeventmanager"
-version = "0.5.2"
+version = "0.5.3"
 authors = [{ name = "Jeordy", email = "JeordyR@users.noreply.github.com" }]
 description = "Event management system for Python with support for Threading and Multiprocessing for task running."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `pyeventmanager-0.5.2/PKG-INFO` & `pyeventmanager-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyeventmanager
-Version: 0.5.2
+Version: 0.5.3
 Summary: Event management system for Python with support for Threading and Multiprocessing for task running.
 Project-URL: Documentation, https://event-manager.jeofi.com
 Project-URL: Homepage, https://event-manager.jeofi.com
 Project-URL: Repository, https://github.com/JeordyR/PyEventManager
 Project-URL: Issues, https://github.com/JeordyR/PyEventManager/issues
 Author-email: Jeordy <JeordyR@users.noreply.github.com>
 Classifier: Operating System :: OS Independent
```

