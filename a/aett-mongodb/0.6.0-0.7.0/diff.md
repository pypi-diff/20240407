# Comparing `tmp/aett-mongodb-0.6.0.tar.gz` & `tmp/aett-mongodb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-mongodb-0.6.0.tar", last modified: Sun Mar 24 18:28:12 2024, max compression
+gzip compressed data, was "aett-mongodb-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
```

## Comparing `aett-mongodb-0.6.0.tar` & `aett-mongodb-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-24 18:28:05.000000 aett-mongodb-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-24 18:28:05.000000 aett-mongodb-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-24 18:28:05.000000 aett-mongodb-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-24 18:28:05.000000 aett-mongodb-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/src/aett/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-03-24 18:28:05.000000 aett-mongodb-0.6.0/src/aett/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:12.589975 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-24 18:28:12.000000 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-24 18:28:12.000000 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:28:12.000000 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-24 18:28:12.000000 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 18:28:12.000000 aett-mongodb-0.6.0/src/aett_mongodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.951434 aett-mongodb-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:10.000000 aett-mongodb-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:10.000000 aett-mongodb-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-07 15:47:16.951434 aett-mongodb-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 15:47:10.000000 aett-mongodb-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 15:47:10.000000 aett-mongodb-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.951434 aett-mongodb-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.947434 aett-mongodb-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.947434 aett-mongodb-0.7.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.947434 aett-mongodb-0.7.0/src/aett/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-07 15:47:10.000000 aett-mongodb-0.7.0/src/aett/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.947434 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-07 15:47:16.000000 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-07 15:47:16.000000 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-07 15:47:16.000000 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-mongodb-0.7.0/src/aett_mongodb.egg-info/top_level.txt
```

### Comparing `aett-mongodb-0.6.0/LICENSE` & `aett-mongodb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-mongodb-0.6.0/PKG-INFO` & `aett-mongodb-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 0.6.0
+Version: 0.7.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
+Requires-Dist: aett-domain>=0.7.0
 Requires-Dist: pymongo~=4.6.2
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-mongodb)](https://pepy.tech/project/aett-mongodb)
+
 Aett Mongo provides the ability to store and retrieve events from a MongoDB collection.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-mongodb-0.6.0/README.md` & `aett-mongodb-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-mongodb)](https://pepy.tech/project/aett-mongodb)
+
 Aett Mongo provides the ability to store and retrieve events from a MongoDB collection.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-mongodb-0.6.0/pyproject.toml` & `aett-mongodb-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.mongodb"]
 
 [project]
 name = "aett-mongodb"
-version = "0.6.0"
+version = "0.7.0"
 description = "MongoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "mongo", "mongodb"]
 dependencies = [
-    'aett-domain >= 0.6.0',
+    'aett-domain >= 0.7.0',
     'pymongo~=4.6.2'
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
 Homepage = "https://github.com/jjrdk/aett"
```

### Comparing `aett-mongodb-0.6.0/src/aett/mongodb/__init__.py` & `aett-mongodb-0.7.0/src/aett/mongodb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import typing
+from typing import Iterable
 from uuid import UUID
 
 import jsonpickle
 import pymongo
 from pymongo import database, results, errors
 
 from aett.eventstore import ICommitEvents, EventStream, IAccessSnapshots, Snapshot, Commit, MAX_INT, EventMessage, \
@@ -25,23 +26,34 @@
         if min_revision > 0:
             filters['StreamRevision']: {'$gte': min_revision}
         if max_revision < MAX_INT:
             filters['StreamRevision']: {'$lte': max_revision}
 
         query_response: pymongo.cursor.Cursor = self.collection.find({'$and': [filters]})
         for doc in query_response.sort('CheckpointToken', direction=pymongo.ASCENDING):
-            yield Commit(bucket_id=doc['BucketId'],
-                         stream_id=doc['StreamId'],
-                         stream_revision=doc['StreamRevision'],
-                         commit_id=UUID(doc['CommitId']),
-                         commit_sequence=doc['CommitSequence'],
-                         commit_stamp=datetime.datetime.fromtimestamp(int(doc['CommitStamp']), datetime.UTC),
-                         headers=jsonpickle.decode(doc['Headers']),
-                         events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(doc['Events'])],
-                         checkpoint_token=doc['CheckpointToken'])
+            yield self._doc_to_commit(doc)
+
+    def get_to(self, bucket_id: str, stream_id: str, max_time: datetime.datetime = datetime.datetime.max) -> \
+            Iterable[Commit]:
+        filters = {"BucketId": bucket_id, "StreamId": stream_id, "CommitStamp": {'$lte': int(max_time.timestamp())}}
+
+        query_response: pymongo.cursor.Cursor = self.collection.find({'$and': [filters]})
+        for doc in query_response.sort('CheckpointToken', direction=pymongo.ASCENDING):
+            yield self._doc_to_commit(doc)
+
+    def _doc_to_commit(self, doc: dict) -> Commit:
+        return Commit(bucket_id=doc['BucketId'],
+                      stream_id=doc['StreamId'],
+                      stream_revision=doc['StreamRevision'],
+                      commit_id=UUID(doc['CommitId']),
+                      commit_sequence=doc['CommitSequence'],
+                      commit_stamp=datetime.datetime.fromtimestamp(int(doc['CommitStamp']), datetime.UTC),
+                      headers=jsonpickle.decode(doc['Headers']),
+                      events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(doc['Events'])],
+                      checkpoint_token=doc['CheckpointToken'])
 
     def commit(self, event_stream: EventStream, commit_id: UUID):
         try:
             ret = self.counters_collection.find_one_and_update(
                 filter={'_id': 'CheckpointToken'},
                 update={'$inc': {'seq': 1}}).get('seq')
             commit = event_stream.to_commit(commit_id)
@@ -86,26 +98,30 @@
                 {'BucketId': bucket_id, 'StreamId': stream_id, 'StreamRevision': max_revision})
             if item is None:
                 return None
 
             return Snapshot(bucket_id=item.get('BucketId'),
                             stream_id=item.get('StreamId'),
                             stream_revision=int(item.get('StreamRevision')),
-                            payload=jsonpickle.decode(item.get('Payload')))
+                            payload=jsonpickle.decode(item.get('Payload')),
+                            headers=jsonpickle.decode(item.get('Headers')))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
-    def add(self, snapshot: Snapshot):
+    def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
+        if headers is None:
+            headers = {}
         try:
             doc = {
                 'BucketId': snapshot.bucket_id,
                 'StreamId': snapshot.stream_id,
                 'StreamRevision': snapshot.stream_revision,
-                'Payload': jsonpickle.encode(snapshot.payload)
+                'Payload': jsonpickle.encode(snapshot.payload, unpicklable=False),
+                'Headers': jsonpickle.encode(headers, unpicklable=False)
             }
             _ = self.collection.insert_one(doc)
         except Exception as e:
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
 
@@ -124,19 +140,18 @@
             if counters_collection.count_documents({'_id': 'CheckpointToken'}) == 0:
                 counters_collection.insert_one({'_id': 'CheckpointToken', 'seq': 0})
         except pymongo.errors.CollectionInvalid as e:
             pass
         try:
             commits_collection: database.Collection = self.db.create_collection(self.commits_table_name,
                                                                                 check_exists=True)
-            commits_collection.create_index([("BucketId", pymongo.ASCENDING), ("CheckpointNumber", pymongo.ASCENDING)],
+            commits_collection.create_index([("BucketId", pymongo.ASCENDING), ("CheckpointToken", pymongo.ASCENDING)],
                                             comment="GetFromCheckpoint", unique=True)
             commits_collection.create_index([("BucketId", pymongo.ASCENDING), ("StreamId", pymongo.ASCENDING),
-                                             ("StreamRevisionFrom", pymongo.ASCENDING),
-                                             ("StreamRevisionTo", pymongo.ASCENDING)], comment="GetFrom", unique=True)
+                                             ("StreamRevision", pymongo.ASCENDING)], comment="GetFrom", unique=True)
             commits_collection.create_index([("BucketId", pymongo.ASCENDING), ("StreamId", pymongo.ASCENDING),
                                              ("CommitSequence", pymongo.ASCENDING)], comment="LogicalKey", unique=True)
             commits_collection.create_index([("CommitStamp", pymongo.ASCENDING)], comment="CommitStamp", unique=False)
             commits_collection.create_index([("BucketId", pymongo.ASCENDING), ("StreamId", pymongo.ASCENDING),
                                              ("CommitId", pymongo.ASCENDING)], comment="CommitId", unique=True)
         except pymongo.errors.CollectionInvalid as e:
             pass
```

### Comparing `aett-mongodb-0.6.0/src/aett_mongodb.egg-info/PKG-INFO` & `aett-mongodb-0.7.0/src/aett_mongodb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-mongodb
-Version: 0.6.0
+Version: 0.7.0
 Summary: MongoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,mongo,mongodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
+Requires-Dist: aett-domain>=0.7.0
 Requires-Dist: pymongo~=4.6.2
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-mongodb)](https://pepy.tech/project/aett-mongodb)
+
 Aett Mongo provides the ability to store and retrieve events from a MongoDB collection.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

