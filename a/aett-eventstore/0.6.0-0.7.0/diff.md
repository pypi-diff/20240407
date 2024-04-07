# Comparing `tmp/aett-eventstore-0.6.0.tar.gz` & `tmp/aett-eventstore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-eventstore-0.6.0.tar", last modified: Sun Mar 24 18:28:06 2024, max compression
+gzip compressed data, was "aett-eventstore-0.7.0.tar", last modified: Sun Apr  7 15:47:20 2024, max compression
```

## Comparing `aett-eventstore-0.6.0.tar` & `aett-eventstore-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.752905 aett-eventstore-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-24 18:28:06.752905 aett-eventstore-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:28:06.752905 aett-eventstore-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.748905 aett-eventstore-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.748905 aett-eventstore-0.6.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.748905 aett-eventstore-0.6.0/src/aett/eventstore/
--rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/src/aett/eventstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.752905 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-24 18:28:06.000000 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-24 18:28:06.000000 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:28:06.000000 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-24 18:28:06.000000 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 18:28:06.000000 aett-eventstore-0.6.0/src/aett_eventstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:06.752905 aett-eventstore-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/tests/test_EventStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/tests/test_Memento.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-24 18:28:01.000000 aett-eventstore-0.6.0/tests/test_Topics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.833998 aett-eventstore-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:20.833998 aett-eventstore-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett/eventstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/src/aett/eventstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_EventStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Topics.py
```

### Comparing `aett-eventstore-0.6.0/LICENSE` & `aett-eventstore-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.6.0/PKG-INFO` & `aett-eventstore-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.6.0
+Version: 0.7.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,event sourcing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing>=3.7.4.3
 Requires-Dist: jsonpickle>=3.0.3
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-eventstore)](https://pepy.tech/project/aett-eventstore)
+
 Provides a framework for managing event streams.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `EventStream` class.
 
 ```python
```

### Comparing `aett-eventstore-0.6.0/pyproject.toml` & `aett-eventstore-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.eventstore"]
 
 [project]
 name = "aett-eventstore"
-version = "0.6.0"
+version = "0.7.0"
 description = "Event store for Python"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "event sourcing"]
 dependencies = [
     'typing >= 3.7.4.3',
     'jsonpickle>=3.0.3'
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
 Homepage = "https://github.com/jjrdk/aett"
```

### Comparing `aett-eventstore-0.6.0/src/aett/eventstore/__init__.py` & `aett-eventstore-0.7.0/src/aett/eventstore/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 class TopicMap:
     """
     Represents a map of topics to event classes.
     """
 
     def __init__(self):
         self.__topics = {}
+
     #
     # def __new__(cls):
     #     if not hasattr(cls, '__singleton_instance'):
     #         cls.__singleton_instance = super(TopicMap, cls).__new__(cls)
     #     return cls.__singleton_instance
 
     def add(self, topic: str, cls: type):
@@ -240,36 +241,39 @@
     """
 
     payload: str
     """
     Gets the snapshot or materialized view of the stream at the revision indicated.
     """
 
+    headers: Dict[str, str]
+
     @staticmethod
-    def from_memento(bucket_id: str, memento: Memento) -> 'Snapshot':
+    def from_memento(bucket_id: str, memento: Memento, headers: Dict[str, str]) -> 'Snapshot':
         """
         Converts the memento to a snapshot which can be persisted.
         :param bucket_id: The value which uniquely identifies the bucket to which the stream belongs.
         :param memento:  The memento to be converted.
+        :param headers: The headers to assign to the snapshot
         :return:
         """
         return Snapshot(bucket_id=bucket_id, stream_id=memento.id, stream_revision=memento.version,
-                        payload=jsonpickle.encode(memento.payload))
+                        payload=jsonpickle.encode(memento.payload), headers=headers)
 
 
 class ICommitEvents(ABC):
     """
     Indicates the ability to commit events and access events to and from a given stream.
 
     Instances of this class must be designed to be multi-thread safe such that they can be shared between threads.
     """
 
     @abstractmethod
-    def get(self, bucket_id: str, stream_id: str, min_revision: int = 0, max_revision: int = MAX_INT) -> Iterable[
-        Commit]:
+    def get(self, bucket_id: str, stream_id: str, min_revision: int = 0, max_revision: int = MAX_INT) -> \
+            Iterable[Commit]:
         """
         Gets the corresponding commits from the stream indicated starting at the revision specified until the
         end of the stream sorted in ascending order--from oldest to newest.
 
         :param bucket_id: The value which uniquely identifies bucket the stream belongs to.
         :param stream_id: The stream from which the events will be read.
         :param min_revision: The minimum revision of the stream to be read.
@@ -277,14 +281,30 @@
         :return: A series of committed events from the stream specified sorted in ascending order.
         :raises StorageException:
         :raises StorageUnavailableException:
         """
         pass
 
     @abstractmethod
+    def get_to(self, bucket_id: str, stream_id: str, max_time: datetime.datetime = datetime.datetime.max) -> \
+            Iterable[Commit]:
+        """
+        Gets the corresponding commits from the stream indicated starting at the revision specified until the
+        end of the stream sorted in ascending order--from oldest to newest.
+
+        :param bucket_id: The value which uniquely identifies bucket the stream belongs to.
+        :param stream_id: The stream from which the events will be read.
+        :param max_time: The max timestamp to return.
+        :return: A series of committed events from the stream specified sorted in ascending order.
+        :raises StorageException:
+        :raises StorageUnavailableException:
+        """
+        pass
+
+    @abstractmethod
     def commit(self, event_stream: 'EventStream', commit_id: UUID):
         """
         Writes the to-be-committed events stream provided to the underlying persistence mechanism.
 
         :param commit_id: The identifier of the commit.
         :param event_stream: The series of events and associated metadata to be committed.
         :raises ConcurrencyException:
@@ -310,19 +330,21 @@
         :return: If found, returns the snapshot for the stream indicated; otherwise null.
         :raises StorageException:
         :raises StorageUnavailableException:
         """
         pass
 
     @abstractmethod
-    def add(self, snapshot: Snapshot):
+    def add(self, snapshot: Snapshot, headers: Dict[str, str] = None):
         """
-        Adds the snapshot provided to the stream indicated. Using a snapshotId of Guid.Empty will always persist the snapshot.
+        Adds the snapshot provided to the stream indicated. Using a snapshotId of Guid.Empty will always persist the
+        snapshot.
 
         :param snapshot: The snapshot to save.
+        :param headers: The metadata to assign to the snapshot.
         :raises StorageException:
         :raises StorageUnavailableException:
         """
         pass
 
 
 class StreamNotFoundException(Exception):
@@ -436,8 +458,7 @@
         self.stream_id = stream_id
         self.version = stream_revision
         self.commit_sequence: int = 0
         self.committed_headers: dict[str, object] = {}
         self.uncommitted_headers: dict[str, object] = {}
         self.committed: list[EventMessage] = []
         self.uncommitted: list[EventMessage] = []
-
```

### Comparing `aett-eventstore-0.6.0/src/aett_eventstore.egg-info/PKG-INFO` & `aett-eventstore-0.7.0/src/aett_eventstore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.6.0
+Version: 0.7.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,event sourcing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing>=3.7.4.3
 Requires-Dist: jsonpickle>=3.0.3
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-eventstore)](https://pepy.tech/project/aett-eventstore)
+
 Provides a framework for managing event streams.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `EventStream` class.
 
 ```python
```

### Comparing `aett-eventstore-0.6.0/tests/test_EventStream.py` & `aett-eventstore-0.7.0/tests/test_EventStream.py`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.6.0/tests/test_Serialization.py` & `aett-eventstore-0.7.0/tests/test_Serialization.py`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.6.0/tests/test_Topics.py` & `aett-eventstore-0.7.0/tests/test_Topics.py`

 * *Files identical despite different names*

