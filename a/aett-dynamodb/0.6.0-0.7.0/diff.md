# Comparing `tmp/aett-dynamodb-0.6.0.tar.gz` & `tmp/aett-dynamodb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-dynamodb-0.6.0.tar", last modified: Sun Mar 24 18:28:04 2024, max compression
+gzip compressed data, was "aett-dynamodb-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
```

## Comparing `aett-dynamodb-0.6.0.tar` & `aett-dynamodb-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-24 18:27:59.000000 aett-dynamodb-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-24 18:27:59.000000 aett-dynamodb-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-24 18:27:59.000000 aett-dynamodb-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-24 18:27:59.000000 aett-dynamodb-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/src/aett/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-03-24 18:27:59.000000 aett-dynamodb-0.6.0/src/aett/dynamodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:04.306620 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-24 18:28:04.000000 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-24 18:28:04.000000 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:28:04.000000 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 18:28:04.000000 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 18:28:04.000000 aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.562626 aett-dynamodb-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.562626 aett-dynamodb-0.7.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/src/aett/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/src/aett/dynamodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/top_level.txt
```

### Comparing `aett-dynamodb-0.6.0/LICENSE` & `aett-dynamodb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-dynamodb-0.6.0/PKG-INFO` & `aett-dynamodb-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.6.0
+Version: 0.7.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
-Requires-Dist: boto3[crt]~=1.34.64
+Requires-Dist: aett-domain>=0.7.0
+Requires-Dist: boto3[crt]~=1.34.79
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-dynamodb)](https://pepy.tech/project/aett-dynamodb)
+
 Aett DynamoDB provides the ability to store and retrieve events from a DynamoDB table.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-dynamodb-0.6.0/README.md` & `aett-dynamodb-0.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-dynamodb)](https://pepy.tech/project/aett-dynamodb)
+
 Aett DynamoDB provides the ability to store and retrieve events from a DynamoDB table.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

### Comparing `aett-dynamodb-0.6.0/pyproject.toml` & `aett-dynamodb-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.dynamodb"]
 
 [project]
 name = "aett-dynamodb"
-version = "0.6.0"
+version = "0.7.0"
 description = "DynamoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "dynamodb"]
 dependencies = [
-    'aett-domain >= 0.6.0',
-    'boto3[crt]~=1.34.64'
+    'aett-domain >= 0.7.0',
+    'boto3[crt]~=1.34.79'
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
 Homepage = "https://github.com/jjrdk/aett"
```

### Comparing `aett-dynamodb-0.6.0/src/aett/dynamodb/__init__.py` & `aett-dynamodb-0.7.0/src/aett/dynamodb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import typing
+from typing import Iterable
 from uuid import UUID
 
 import boto3
 import jsonpickle
-from boto3.dynamodb.conditions import Key
+from boto3.dynamodb.conditions import Key, Attr
 
 from aett.eventstore import ICommitEvents, EventStream, IAccessSnapshots, Snapshot, Commit, MAX_INT, EventMessage, \
     TopicMap
 
 
 def _get_resource(region: str):
     return boto3.resource('dynamodb',
@@ -34,36 +35,53 @@
             ConsistentRead=True,
             ProjectionExpression='BucketId,StreamId,StreamRevision,CommitId,CommitSequence,CommitStamp,Headers,Events',
             KeyConditionExpression=(Key("BucketAndStream").eq(f'{bucket_id}{stream_id}')
                                     & Key("StreamRevision").between(min_revision, max_revision)),
             ScanIndexForward=True)
         items = query_response['Items']
         for item in items:
-            yield Commit(
-                bucket_id=item['BucketId'],
-                stream_id=item['StreamId'],
-                stream_revision=int(item['StreamRevision']),
-                commit_id=UUID(item['CommitId']),
-                commit_sequence=int(item['CommitSequence']),
-                commit_stamp=datetime.datetime.fromtimestamp(int(item['CommitStamp']), datetime.UTC),
-                headers=jsonpickle.decode(item['Headers']),
-                events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(item['Events'])],
-                checkpoint_token=0)
+            yield self._item_to_commit(item)
+
+    def get_to(self, bucket_id: str, stream_id: str, max_time: datetime.datetime = datetime.datetime.max) -> \
+            Iterable[Commit]:
+        query_response = self.table.scan(IndexName="CommitStampIndex",
+                                         ConsistentRead=True,
+                                         Select='ALL_ATTRIBUTES',
+                                         FilterExpression=(
+                                                 Key("BucketAndStream").eq(f'{bucket_id}{stream_id}')
+                                                 & Attr('CommitStamp').lte(int(max_time.timestamp()))))
+        items = query_response['Items']
+        for item in items:
+            if item['CommitStamp'] > max_time.timestamp():
+                break
+            yield self._item_to_commit(item)
+
+    def _item_to_commit(self, item: dict) -> Commit:
+        return Commit(
+            bucket_id=item['BucketId'],
+            stream_id=item['StreamId'],
+            stream_revision=int(item['StreamRevision']),
+            commit_id=UUID(item['CommitId']),
+            commit_sequence=int(item['CommitSequence']),
+            commit_stamp=datetime.datetime.fromtimestamp(int(item['CommitStamp']), datetime.UTC),
+            headers=jsonpickle.decode(item['Headers']),
+            events=[EventMessage.from_json(e, self.topic_map) for e in jsonpickle.decode(item['Events'])],
+            checkpoint_token=0)
 
     def commit(self, event_stream: EventStream, commit_id: UUID):
         try:
             commit = event_stream.to_commit(commit_id)
             item = {
                 'BucketAndStream': f'{event_stream.bucket_id}{event_stream.stream_id}',
                 'BucketId': event_stream.bucket_id,
                 'StreamId': event_stream.stream_id,
                 'StreamRevision': commit.stream_revision,
                 'CommitId': str(commit_id),
                 'CommitSequence': commit.commit_sequence,
-                'CommitStamp': int(datetime.datetime.now(datetime.UTC).timestamp()),
+                'CommitStamp': int(commit.commit_stamp.timestamp()),
                 'Headers': jsonpickle.encode(commit.headers, unpicklable=False),
                 'Events': jsonpickle.encode([e.to_json() for e in commit.events], unpicklable=False)
             }
             response = self.table.put_item(
                 TableName=self.table_name,
                 Item=item,
                 ReturnValues='NONE',
@@ -116,27 +134,31 @@
             )
             if len(query_response['Items']) == 0:
                 return None
             item = query_response['Items'][0]
             return Snapshot(bucket_id=item['BucketId'],
                             stream_id=item['StreamId'],
                             stream_revision=int(item['StreamRevision']),
-                            payload=item['Payload'])
+                            payload=item['Payload'],
+                            headers=dict(jsonpickle.decode(item['Headers'])))
         except Exception as e:
             raise Exception(
                 f"Failed to get snapshot for stream {stream_id} with status code {e.response['ResponseMetadata']['HTTPStatusCode']}")
 
-    def add(self, snapshot: Snapshot):
+    def add(self, snapshot: Snapshot, headers: typing.Dict[str, str] = None):
+        if headers is None:
+            headers = {}
         try:
             item = {
                 'BucketAndStream': f"{snapshot.bucket_id}{snapshot.stream_id}",
                 'BucketId': snapshot.bucket_id,
                 'StreamId': snapshot.stream_id,
                 'StreamRevision': snapshot.stream_revision,
-                'Payload': snapshot.payload
+                'Payload': snapshot.payload,
+                'Headers': jsonpickle.encode(headers, unpicklable=False)
             }
             _ = self.table.put_item(
                 TableName=self.table_name,
                 Item=item,
                 ReturnValues='NONE',
                 ReturnValuesOnConditionCheckFailure='NONE',
                 ConditionExpression='attribute_not_exists(BucketAndStream) AND attribute_not_exists(StreamRevision)'
@@ -164,24 +186,33 @@
                 KeySchema=[
                     {'AttributeName': 'BucketAndStream', 'KeyType': 'HASH'},
                     {'AttributeName': 'CommitSequence', 'KeyType': 'RANGE'}
                 ],
                 AttributeDefinitions=[
                     {'AttributeName': 'BucketAndStream', 'AttributeType': 'S'},
                     {'AttributeName': 'CommitSequence', 'AttributeType': 'N'},
-                    {'AttributeName': 'StreamRevision', 'AttributeType': 'N'}
+                    {'AttributeName': 'StreamRevision', 'AttributeType': 'N'},
+                    {'AttributeName': 'CommitStamp', 'AttributeType': 'N'}
                 ],
                 LocalSecondaryIndexes=[
                     {
                         'IndexName': "RevisionIndex",
                         'KeySchema': [
                             {'AttributeName': 'BucketAndStream', 'KeyType': 'HASH'},
                             {'AttributeName': 'StreamRevision', 'KeyType': 'RANGE'}
                         ],
                         'Projection': {'ProjectionType': 'ALL'}
+                    },
+                    {
+                        'IndexName': "CommitStampIndex",
+                        'KeySchema': [
+                            {'AttributeName': 'BucketAndStream', 'KeyType': 'HASH'},
+                            {'AttributeName': 'CommitStamp', 'KeyType': 'RANGE'}
+                        ],
+                        'Projection': {'ProjectionType': 'ALL'}
                     }],
                 TableClass='STANDARD',
                 StreamSpecification={'StreamEnabled': True, 'StreamViewType': 'NEW_IMAGE'},
                 ProvisionedThroughput={"ReadCapacityUnits": 10, "WriteCapacityUnits": 10, })
 
         if self.snapshots_table_name not in table_names:
             _ = self.dynamodb.create_table(
```

### Comparing `aett-dynamodb-0.6.0/src/aett_dynamodb.egg-info/PKG-INFO` & `aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.6.0
+Version: 0.7.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,28 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjrdk/aett
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.6.0
-Requires-Dist: boto3[crt]~=1.34.64
+Requires-Dist: aett-domain>=0.7.0
+Requires-Dist: boto3[crt]~=1.34.79
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
 
+[![Downloads](https://static.pepy.tech/badge/aett-dynamodb)](https://pepy.tech/project/aett-dynamodb)
+
 Aett DynamoDB provides the ability to store and retrieve events from a DynamoDB table.
 
 ## Usage
 
 To create an event stream to manage events, you can use the `PersistenceManagement` class.
 
 ```python
```

