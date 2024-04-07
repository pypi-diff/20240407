# Comparing `tmp/aett-domain-0.6.0.tar.gz` & `tmp/aett-domain-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-domain-0.6.0.tar", last modified: Sun Mar 24 18:28:04 2024, max compression
+gzip compressed data, was "aett-domain-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
```

## Comparing `aett-domain-0.6.0.tar` & `aett-domain-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.966652 aett-domain-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-24 18:27:59.000000 aett-domain-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-24 18:27:59.000000 aett-domain-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-24 18:28:04.966652 aett-domain-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-24 18:27:59.000000 aett-domain-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-24 18:27:59.000000 aett-domain-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:28:04.966652 aett-domain-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.962652 aett-domain-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.962652 aett-domain-0.6.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.962652 aett-domain-0.6.0/src/aett/domain/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-03-24 18:27:59.000000 aett-domain-0.6.0/src/aett/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.966652 aett-domain-0.6.0/src/aett_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-24 18:28:04.000000 aett-domain-0.6.0/src/aett_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-24 18:28:04.000000 aett-domain-0.6.0/src/aett_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:28:04.000000 aett-domain-0.6.0/src/aett_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-24 18:28:04.000000 aett-domain-0.6.0/src/aett_domain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 18:28:04.000000 aett-domain-0.6.0/src/aett_domain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.491793 aett-domain-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:08.000000 aett-domain-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:08.000000 aett-domain-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-07 15:47:16.491793 aett-domain-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 15:47:08.000000 aett-domain-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-07 15:47:08.000000 aett-domain-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.491793 aett-domain-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.487793 aett-domain-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.487793 aett-domain-0.7.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.491793 aett-domain-0.7.0/src/aett/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-07 15:47:08.000000 aett-domain-0.7.0/src/aett/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.491793 aett-domain-0.7.0/src/aett_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-07 15:47:16.000000 aett-domain-0.7.0/src/aett_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-07 15:47:16.000000 aett-domain-0.7.0/src/aett_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-domain-0.7.0/src/aett_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-07 15:47:16.000000 aett-domain-0.7.0/src/aett_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-domain-0.7.0/src/aett_domain.egg-info/top_level.txt
```

### Comparing `aett-domain-0.6.0/LICENSE` & `aett-domain-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-domain-0.6.0/PKG-INFO` & `aett-domain-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 0.6.0
+Version: 0.7.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,ddd,domain
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=0.6.0
+Requires-Dist: aett-eventstore>=0.7.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-domain)](https://pepy.tech/project/aett-domain)
+
 Aett Domain provide base classes for `aggregate` and `saga` as encapsulations of business rules and processes, respectively.
 
 ## Usage
 
 The `Aggregate` class is abstract and a subtype aggregate would implement the external interfaces and internal behavior
 and define which events are raised as a response input.
```

### Comparing `aett-domain-0.6.0/README.md` & `aett-domain-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-domain)](https://pepy.tech/project/aett-domain)
+
 Aett Domain provide base classes for `aggregate` and `saga` as encapsulations of business rules and processes, respectively.
 
 ## Usage
 
 The `Aggregate` class is abstract and a subtype aggregate would implement the external interfaces and internal behavior
 and define which events are raised as a response input.
```

### Comparing `aett-domain-0.6.0/pyproject.toml` & `aett-domain-0.7.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.domain"]
 
 [project]
 name = "aett-domain"
-version = "0.6.0"
+version = "0.7.0"
 description = "Domain modeling types aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "ddd", "domain"]
 dependencies = [
     'multipledispatch >= 1.0.0',
-    'aett-eventstore>=0.6.0'
+    'aett-eventstore>=0.7.0'
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
 Homepage = "https://github.com/jjrdk/aett"
```

### Comparing `aett-domain-0.6.0/src/aett/domain/__init__.py` & `aett-domain-0.7.0/src/aett/domain/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -79,14 +79,18 @@
     def id(self) -> str:
         return self._id
 
     @property
     def version(self) -> int:
         return self._version
 
+    @property
+    def headers(self):
+        return self._headers
+
     def transition(self, event: BaseEvent) -> None:
         """
         Transitions the saga to the next state based on the event
         :param event: The trigger event
         :return: None
         """
         # Use multiple dispatch to call the correct apply method
@@ -105,22 +109,51 @@
 
 
 class AggregateRepository(ABC):
     TAggregate = typing.TypeVar('TAggregate', bound=Aggregate)
 
     @abstractmethod
     def get(self, cls: typing.Type[TAggregate], stream_id: str, max_version: int = 2 ** 32) -> TAggregate:
+        """
+        Gets the aggregate with the specified stream id and type
+
+        :param cls: The type of the aggregate
+        :param stream_id: The id of the stream to load
+        :param max_version: The max aggregate version to load.
+        """
+        pass
+
+    def get_to(self, cls: typing.Type[TAggregate], stream_id: str,
+               max_time: datetime = datetime.datetime.max) -> TAggregate:
+        """
+        Gets the aggregate with the specified stream id and type
+
+        :param cls: The type of the aggregate
+        :param stream_id: The id of the stream to load
+        :param max_time: The max aggregate timestamp to load.
+        """
+        pass
+
+    @abstractmethod
+    def save(self, aggregate: T, headers: Dict[str, str] = None) -> None:
+        """
+        Save the aggregate to the repository.
+
+        :param aggregate: The aggregate to save.
+        :param headers: The headers to assign to the commit.
+        """
         pass
 
     @abstractmethod
-    def save(self, aggregate: T) -> None:
+    def snapshot(self, cls: typing.Type[TAggregate], stream_id: str, version: int, headers: Dict[str, str]) -> None:
         pass
 
     @abstractmethod
-    def snapshot(self, cls: typing.Type[TAggregate], stream_id: str, version: int) -> None:
+    def snapshot_at(self, cls: typing.Type[TAggregate], stream_id: str, cut_off: datetime.datetime,
+                    headers: Dict[str, str]) -> None:
         pass
 
 
 class SagaRepository(ABC):
     TSaga = typing.TypeVar('TSaga', bound=Saga)
 
     @abstractmethod
@@ -151,33 +184,58 @@
             aggregate.apply_memento(memento_type(**jsonpickle.decode(snapshot.payload)))
         for commit in commits:
             for event in commit.events:
                 aggregate.raise_event(event.body)
         aggregate.uncommitted.clear()
         return aggregate
 
-    def save(self, aggregate: TAggregate) -> None:
+    def get_to(self, cls: typing.Type[TAggregate], stream_id: str,
+               max_time: datetime = datetime.datetime.max) -> TAggregate:
+        commits = self._store.get_to(bucket_id=self._bucket_id,
+                                     stream_id=stream_id,
+                                     max_time=max_time)
+        aggregate = cls(stream_id)
+        for commit in commits:
+            for event in commit.events:
+                aggregate.raise_event(event.body)
+        aggregate.uncommitted.clear()
+        return aggregate
+
+    def save(self, aggregate: TAggregate, headers: Dict[str, str] = None) -> None:
+        if headers is None:
+            headers = {}
         if len(aggregate.uncommitted) == 0:
             return
         stream = EventStream.load(bucket_id=self._bucket_id,
                                   stream_id=aggregate.id,
                                   client=self._store,
                                   max_version=2 ** 32)
         for event in aggregate.uncommitted:
             stream.add(event)
+        for key, value in headers.items():
+            stream.set_header(key=key, value=value)
         self._store.commit(stream, uuid.uuid4())
         aggregate.uncommitted.clear()
 
-    def snapshot(self, cls: typing.Type[TAggregate], stream_id: str, version: int = MAX_INT) -> None:
+    def snapshot(self, cls: typing.Type[TAggregate], stream_id: str, version: int = MAX_INT,
+                 headers: Dict[str, str] = None) -> None:
         agg = self.get(cls, stream_id, version)
-        memento = agg.get_memento()
-        snapshot = Snapshot(bucket_id=self._bucket_id, stream_id=stream_id,
+        self._snapshot_aggregate(agg, headers)
+
+    def snapshot_at(self, cls: typing.Type[TAggregate], stream_id: str, cut_off: datetime.datetime,
+                    headers: Dict[str, str] = None) -> None:
+        agg = self.get_to(cls, stream_id, cut_off)
+        self._snapshot_aggregate(agg, headers)
+
+    def _snapshot_aggregate(self, aggregate: Aggregate, headers: Dict[str, str] = None) -> None:
+        memento = aggregate.get_memento()
+        snapshot = Snapshot(bucket_id=self._bucket_id, stream_id=aggregate.id,
                             payload=jsonpickle.encode(memento.payload, unpicklable=False),
-                            stream_revision=memento.version)
-        self._snapshot_store.add(snapshot)
+                            stream_revision=memento.version, headers={})
+        self._snapshot_store.add(snapshot=snapshot, headers=headers)
 
     def __init__(self, bucket_id: str, store: ICommitEvents, snapshot_store: IAccessSnapshots):
         self._bucket_id = bucket_id
         self._store = store
         self._snapshot_store = snapshot_store
```

### Comparing `aett-domain-0.6.0/src/aett_domain.egg-info/PKG-INFO` & `aett-domain-0.7.0/src/aett_domain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 0.6.0
+Version: 0.7.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,ddd,domain
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=0.6.0
+Requires-Dist: aett-eventstore>=0.7.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-domain)](https://pepy.tech/project/aett-domain)
+
 Aett Domain provide base classes for `aggregate` and `saga` as encapsulations of business rules and processes, respectively.
 
 ## Usage
 
 The `Aggregate` class is abstract and a subtype aggregate would implement the external interfaces and internal behavior
 and define which events are raised as a response input.
```

