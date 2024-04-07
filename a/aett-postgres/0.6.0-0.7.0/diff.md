# Comparing `tmp/aett-postgres-0.6.0.tar.gz` & `tmp/aett-postgres-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-postgres-0.6.0.tar", last modified: Sun Mar 24 18:28:03 2024, max compression
+gzip compressed data, was "aett-postgres-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
```

## Comparing `aett-postgres-0.6.0.tar` & `aett-postgres-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:03.877913 aett-postgres-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-24 18:27:59.000000 aett-postgres-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-24 18:27:59.000000 aett-postgres-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-24 18:28:03.873913 aett-postgres-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-24 18:27:59.000000 aett-postgres-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-24 18:27:59.000000 aett-postgres-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:28:03.877913 aett-postgres-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:03.873913 aett-postgres-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:03.873913 aett-postgres-0.6.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:03.873913 aett-postgres-0.6.0/src/aett/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-03-24 18:27:59.000000 aett-postgres-0.6.0/src/aett/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:03.873913 aett-postgres-0.6.0/src/aett_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-24 18:28:03.000000 aett-postgres-0.6.0/src/aett_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-24 18:28:03.000000 aett-postgres-0.6.0/src/aett_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:28:03.000000 aett-postgres-0.6.0/src/aett_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-24 18:28:03.000000 aett-postgres-0.6.0/src/aett_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 18:28:03.000000 aett-postgres-0.6.0/src/aett_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.082473 aett-postgres-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.082473 aett-postgres-0.7.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/src/aett/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/src/aett/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/src/aett_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/top_level.txt
```

### Comparing `aett-postgres-0.6.0/LICENSE` & `aett-postgres-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-postgres-0.6.0/PKG-INFO` & `aett-postgres-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.6.0
+Version: 0.7.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
+Requires-Dist: aett-domain>=0.7.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-postgres)](https://pepy.tech/project/aett-postgres)
+
 Aett Postgres provides the ability to store and retrieve events from a Postgres.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-postgres-0.6.0/README.md` & `aett-postgres-0.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-postgres)](https://pepy.tech/project/aett-postgres)
+
 Aett Postgres provides the ability to store and retrieve events from a Postgres.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-postgres-0.6.0/pyproject.toml` & `aett-postgres-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.postgres"]
 
 [project]
 name = "aett-postgres"
-version = "0.6.0"
+version = "0.7.0"
 description = "Postgres connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "postgres"]
 dependencies = [
-    'aett-domain >= 0.6.0',
+    'aett-domain >= 0.7.0',
     'psycopg-binary~=3.1.18'
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
 Homepage = "https://github.com/jjrdk/aett"
```

### Comparing `aett-postgres-0.6.0/src/aett/postgres/__init__.py` & `aett-postgres-0.7.0/src/aett/postgres/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import datetime
 import typing
+from typing import Iterable
 from uuid import UUID
 
 import jsonpickle
 import psycopg
 
 from aett.eventstore import ICommitEvents, EventStream, IAccessSnapshots, Snapshot, Commit, MAX_INT, TopicMap, \
     EventMessage
@@ -26,37 +28,54 @@
    AND StreamId = %s
    AND StreamRevision >= %s
    AND (StreamRevision - Items) < %s
    AND CommitSequence > %s
  ORDER BY CommitSequence;""", (bucket_id, stream_id, min_revision, max_revision, 0))
         fetchall = cur.fetchall()
         for doc in fetchall:
-            yield Commit(bucket_id=doc[0],
-                         stream_id=doc[1],
-                         stream_revision=doc[3],
-                         commit_id=doc[4],
-                         commit_sequence=doc[5],
-                         commit_stamp=doc[6],
-                         headers=jsonpickle.decode(doc[8]),
-                         events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(doc[9])],
-                         checkpoint_token=doc[7])
+            yield self._item_to_commit(doc)
+
+    def get_to(self, bucket_id: str, stream_id: str, max_time: datetime.datetime = datetime.datetime.max) -> \
+            Iterable[Commit]:
+        cur = self.connection.cursor()
+        cur.execute(f"""SELECT BucketId, StreamId, StreamIdOriginal, StreamRevision, CommitId, CommitSequence, CommitStamp,  CheckpointNumber, Headers, Payload
+          FROM {self._table_name}
+         WHERE BucketId = %s
+           AND StreamId = %s
+           AND CommitStamp <= %s
+         ORDER BY CommitSequence;""", (bucket_id, stream_id, max_time))
+        fetchall = cur.fetchall()
+        for doc in fetchall:
+            yield self._item_to_commit(doc)
+
+    def _item_to_commit(self, item):
+        return Commit(bucket_id=item[0],
+                      stream_id=item[1],
+                      stream_revision=item[3],
+                      commit_id=item[4],
+                      commit_sequence=item[5],
+                      commit_stamp=item[6],
+                      headers=jsonpickle.decode(item[8]),
+                      events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(item[9])],
+                      checkpoint_token=item[7])
 
     def commit(self, event_stream: EventStream, commit_id: UUID):
         try:
             commit = event_stream.to_commit(commit_id)
             cur = self.connection.cursor()
             cur.execute(f"""INSERT
   INTO {self._table_name}
      ( BucketId, StreamId, StreamIdOriginal, CommitId, CommitSequence, StreamRevision, Items, CommitStamp, Headers, Payload )
 VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
 RETURNING CheckpointNumber;""", (commit.bucket_id, commit.stream_id, commit.stream_id,
                                  commit_id, commit.commit_sequence, commit.stream_revision, len(commit.events),
                                  commit.commit_stamp,
                                  jsonpickle.encode(commit.headers, unpicklable=False).encode('utf-8'),
-                                 jsonpickle.encode([e.to_json() for e in commit.events], unpicklable=False).encode('utf-8')))
+                                 jsonpickle.encode([e.to_json() for e in commit.events], unpicklable=False).encode(
+                                     'utf-8')))
             checkpoint_number = cur.fetchone()
             self.connection.commit()
             return Commit(bucket_id=commit.bucket_id,
                           stream_id=commit.stream_id,
                           stream_revision=commit.stream_revision,
                           commit_id=commit_id,
                           commit_sequence=commit.commit_sequence,
@@ -104,29 +123,33 @@
             item = cur.fetchone()
             if item is None:
                 return None
 
             return Snapshot(bucket_id=item[0],
                             stream_id=item[1],
                             stream_revision=int(item[2]),
-                            payload=jsonpickle.decode(item[3].decode('utf-8')))
+                            payload=jsonpickle.decode(item[3].decode('utf-8')),
+                            headers=dict(jsonpickle.decode(item[4].decode('utf-8'))))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with error {e}")
 
-    def add(self, snapshot: Snapshot):
+    def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
+        if headers is None:
+            headers = {}
         try:
             cur = self.connection.cursor()
             j = jsonpickle.encode(snapshot.payload, unpicklable=False)
             cur.execute(
-                f"""INSERT INTO {self._table_name} ( BucketId, StreamId, StreamRevision, Payload) VALUES (%s, %s, %s, %s);""",
+                f"""INSERT INTO {self._table_name} ( BucketId, StreamId, StreamRevision, Payload, Headers) VALUES (%s, %s, %s, %s, %s);""",
                 (snapshot.bucket_id,
                  snapshot.stream_id,
                  snapshot.stream_revision,
-                 j.encode('utf-8')))
+                 j.encode('utf-8'),
+                 jsonpickle.encode(headers, unpicklable=False).encode('utf-8')))
             self.connection.commit()
         except Exception as e:
             raise Exception(
                 f"Failed to add snapshot for stream {snapshot.stream_id} with error {e}")
 
 
 class PersistenceManagement:
@@ -163,14 +186,15 @@
 
 CREATE TABLE {self.snapshots_table_name}
 (
     BucketId varchar(40) NOT NULL,
     StreamId char(40) NOT NULL,
     StreamRevision int NOT NULL CHECK (StreamRevision > 0),
     Payload bytea NOT NULL,
+    Headers bytea NOT NULL,
     CONSTRAINT PK_Snapshots PRIMARY KEY (BucketId, StreamId, StreamRevision)
 );""")
             c.commit()
         except Exception as e:
             pass
 
     def drop(self):
```

### Comparing `aett-postgres-0.6.0/src/aett_postgres.egg-info/PKG-INFO` & `aett-postgres-0.7.0/src/aett_postgres.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.6.0
+Version: 0.7.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
+Requires-Dist: aett-domain>=0.7.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-postgres)](https://pepy.tech/project/aett-postgres)
+
 Aett Postgres provides the ability to store and retrieve events from a Postgres.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

