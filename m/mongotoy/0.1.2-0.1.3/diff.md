# Comparing `tmp/mongotoy-0.1.2.tar.gz` & `tmp/mongotoy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotoy-0.1.2.tar", max compression
+gzip compressed data, was "mongotoy-0.1.3.tar", max compression
```

## Comparing `mongotoy-0.1.2.tar` & `mongotoy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.2/LICENSE
--rw-r--r--   0        0        0      115 2024-03-18 19:08:34.118444 mongotoy-0.1.2/mongotoy/__init__.py
--rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.2/mongotoy/cache.py
--rw-r--r--   0        0        0    41118 2024-03-29 16:27:06.381394 mongotoy-0.1.2/mongotoy/db.py
--rw-r--r--   0        0        0    14311 2024-03-29 18:23:37.162418 mongotoy-0.1.2/mongotoy/documents.py
--rw-r--r--   0        0        0     6554 2024-03-27 16:52:26.158717 mongotoy-0.1.2/mongotoy/errors.py
--rw-r--r--   0        0        0     8959 2024-03-27 16:52:36.825834 mongotoy-0.1.2/mongotoy/expressions.py
--rw-r--r--   0        0        0    11421 2024-03-31 18:40:22.322807 mongotoy-0.1.2/mongotoy/fields.py
--rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.2/mongotoy/geodata.py
--rw-r--r--   0        0        0    36748 2024-03-31 18:37:54.300120 mongotoy-0.1.2/mongotoy/mappers.py
--rw-r--r--   0        0        0     7609 2024-03-19 18:16:23.766912 mongotoy-0.1.2/mongotoy/references.py
--rw-r--r--   0        0        0    10678 2024-03-19 18:22:12.403902 mongotoy-0.1.2/mongotoy/types.py
--rw-r--r--   0        0        0      687 2024-03-30 22:39:28.377403 mongotoy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6650 2024-03-27 16:53:01.008116 mongotoy-0.1.2/README.md
--rw-r--r--   0        0        0     7225 1970-01-01 00:00:00.000000 mongotoy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.3/mongotoy/__init__.py
+-rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.3/mongotoy/cache.py
+-rw-r--r--   0        0        0    49516 2024-04-07 21:04:15.682116 mongotoy-0.1.3/mongotoy/db.py
+-rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.3/mongotoy/documents.py
+-rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.3/mongotoy/errors.py
+-rw-r--r--   0        0        0     7719 2024-04-04 15:48:59.159339 mongotoy-0.1.3/mongotoy/expressions.py
+-rw-r--r--   0        0        0    11917 2024-04-04 15:54:56.024009 mongotoy-0.1.3/mongotoy/fields.py
+-rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.3/mongotoy/geodata.py
+-rw-r--r--   0        0        0    37519 2024-04-07 05:47:07.295684 mongotoy-0.1.3/mongotoy/mappers.py
+-rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.3/mongotoy/references.py
+-rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.3/mongotoy/sync.py
+-rw-r--r--   0        0        0    11819 2024-04-07 21:04:15.689215 mongotoy-0.1.3/mongotoy/types.py
+-rw-r--r--   0        0        0      687 2024-04-07 21:21:43.106575 mongotoy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6650 2024-04-07 05:46:30.648934 mongotoy-0.1.3/README.md
+-rw-r--r--   0        0        0     7225 1970-01-01 00:00:00.000000 mongotoy-0.1.3/PKG-INFO
```

### Comparing `mongotoy-0.1.2/LICENSE` & `mongotoy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.2/mongotoy/cache.py` & `mongotoy-0.1.3/mongotoy/cache.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.2/mongotoy/db.py` & `mongotoy-0.1.3/mongotoy/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import datetime
 import functools
 import inspect
+import math
 import mimetypes
+import os
 import typing
 
 import bson
 import gridfs
 import pymongo
 from motor.core import AgnosticClient, AgnosticDatabase, AgnosticCollection, AgnosticClientSession
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorGridFSBucket, AsyncIOMotorGridOut
 from motor.motor_gridfs import AgnosticGridFSBucket
 from pymongo.read_concern import ReadConcern
 
-from mongotoy import documents, expressions, references, fields, types
-from mongotoy.errors import EngineError, NoResultsError, ManyResultsError
+from mongotoy import documents, expressions, references, fields, types, sync
+from mongotoy.errors import EngineError, NoResultsError, ManyResultsError, SessionError
 
 __all__ = (
     'Engine',
     'Session',
 )
 
 from mongotoy.expressions import Query
@@ -79,26 +81,14 @@
         self._codec_options = codec_options
         self._read_preference = read_preference
         self._read_concern = read_concern
         self._write_concern = write_concern
         self._db_client = None
         self._migration_lock = asyncio.Lock()
 
-    async def connect(self, *conn, ping: bool = False):
-        """
-        Connects to the MongoDB server.
-
-        Args:
-            *conn: Connection arguments for AsyncIOMotorClient.
-            ping (bool): Whether to ping the server after connecting.
-        """
-        self._db_client = AsyncIOMotorClient(*conn)
-        if ping:
-            await self._db_client.admin.command({'ping': 1})
-
     @property
     def client(self) -> AgnosticClient:
         """
         Returns the MongoDB client.
 
         Raises:
             EngineError: If the engine is disconnected, the connect method must be called first.
@@ -120,77 +110,14 @@
             name=self._database,
             codec_options=self._codec_options,
             read_preference=self._read_preference,
             read_concern=self._read_concern,
             write_concern=self._write_concern
         )
 
-    def session(self) -> 'Session':
-        """
-        Creates a new MongoDB session.
-
-        Returns:
-            Session: A new MongoDB session associated with the engine.
-        """
-        return Session(engine=self)
-
-    def transaction(self) -> 'Transaction':
-        """
-        Creates a new MongoDB transaction.
-
-        Returns:
-            Transaction: A new MongoDB transaction associated with the engine
-        """
-        return Transaction(provider=self)
-
-    def collection(self, document_cls_or_name: typing.Type[T] | str) -> AgnosticCollection:
-        """
-        Retrieves the MongoDB collection.
-
-        Args:
-            document_cls_or_name (typing.Type[T] | str): The document class or collection name.
-
-        Returns:
-            AgnosticCollection: The MongoDB collection.
-        """
-        if not isinstance(document_cls_or_name, str):
-            return self._get_document_collection(document_cls_or_name)
-
-        # noinspection PyTypeChecker
-        return self.database[document_cls_or_name].with_options(
-            codec_options=self._codec_options,
-            read_preference=self._read_preference,
-            read_concern=self._read_concern,
-            write_concern=self._write_concern
-        )
-
-    # noinspection SpellCheckingInspection
-    def gridfs(
-            self,
-            bucket_name: str = 'fs',
-            chunk_size_bytes: int = gridfs.DEFAULT_CHUNK_SIZE
-    ) -> AgnosticGridFSBucket:
-        """
-        Retrieves the GridFS bucket.
-
-        Args:
-            bucket_name (str): The name of the GridFS bucket.
-            chunk_size_bytes (int): The chunk size in bytes.
-
-        Returns:
-            AgnosticGridFSBucket: The GridFS bucket.
-        """
-        return AsyncIOMotorGridFSBucket(
-            database=self.database,
-            bucket_name=bucket_name,
-            chunk_size_bytes=chunk_size_bytes,
-            write_concern=self.database.write_concern,
-            read_preference=self.database.read_preference
-        )
-
     def _get_document_indexes(
         self,
         document_cls: typing.Type[documents.BaseDocument],
         parent: str = None
     ) -> list[pymongo.IndexModel]:
         """
         Retrieves document indexes.
@@ -333,20 +260,20 @@
         driver_session: AgnosticClientSession = None
     ):
         """
         Executes document migration.
 
         Args:
             document_cls (typing.Type[T]): The document class.
-            skip_exist (bool, optional): Whether to skip if collection exists.
+            skip_exist (bool, optional): Whether to skip if a collection exists.
             driver_session (AgnosticClientSession, optional): The database session.
         """
         do_apply = True
 
-        # Skip if collection already exists
+        # Skip if a collection already exists
         if skip_exist:
             collections = await self.database.list_collection_names(session=driver_session)
             if document_cls.__collection_name__ in collections:
                 do_apply = False
 
         # Create collection and indexes
         if do_apply:
@@ -372,39 +299,53 @@
             raise TypeError('Seeding function must be async')
 
         func_path = f'{func.__module__}.{func.__name__}'
         do_seeding = True
 
         # Skip if seeding already applied
         if skip_exist:
+            # noinspection PyProtectedMember
             if await session.objects(Seeding).filter(
                 Seeding.function == func_path
-            ).count():
+            )._count():
                 do_seeding = False
 
         if do_seeding:
             await func(session)
-            await session.save(Seeding(function=func_path))
+            # noinspection PyProtectedMember
+            await session._save(Seeding(function=func_path))
 
-    async def migrate(
+    async def _connect(self, *conn, ping: bool = False):
+        """
+        Connects to the MongoDB server.
+
+        Args:
+            *conn: Connection arguments for AsyncIOMotorClient.
+            ping (bool): Whether to ping the server after connecting.
+        """
+        self._db_client = AsyncIOMotorClient(*conn)
+        if ping:
+            await self._db_client.admin.command({'ping': 1})
+
+    async def _migrate(
         self,
         document_cls: typing.Type[T],
         session: 'Session' = None
     ):
         """
         Migrates a document.
 
         Args:
             document_cls (typing.Type[T]): The document class.
             session (Session, optional): The session object.
         """
         driver_session = session.driver_session if session else None
         await self._exec_migration(document_cls, driver_session=driver_session)
 
-    async def migrate_all(
+    async def _migrate_all(
         self,
         documents_cls: list[typing.Type[T]],
         session: 'Session' = None
     ):
         """
         Migrates multiple documents.
 
@@ -418,191 +359,285 @@
             self._exec_migration(
                 doc_cls,
                 skip_exist=False,
                 driver_session=driver_session
             ) for doc_cls in documents_cls if doc_cls.__collection_name__ not in collections
         ])
 
-    async def seeding(
+    async def _seeding(
         self,
         func: typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]],
         session: 'Session' = None
     ):
         """
         Executes seeding for a specific function.
 
         Args:
             func (typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]]): The seeding function.
             session (Session, optional): The session object.
         """
         await self._exec_seeding(func, session=session)
 
-    async def seeding_all(
+    async def _seeding_all(
         self,
         funcs: list[typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]]],
         session: 'Session' = None
     ):
         """
         Executes seeding for multiple functions.
 
         Args:
             funcs (list[Callable[['Session'], Coroutine[Any, Any, None]]]): List of seeding functions.
             session (Session, optional): The session object.
         """
-        seeds = await session.objects(Seeding).fetch()
+        # noinspection PyProtectedMember
+        seeds = await session.objects(Seeding)._fetch()
         seeds = [s.function for s in seeds]
         # noinspection PyUnresolvedReferences
         await asyncio.gather(*[
             self._exec_seeding(
                 func,
                 session=session,
                 skip_exist=False
             ) for func in funcs if f'{func.__module__}.{func.__name__}' not in seeds
         ])
 
+    def session(self) -> 'Session':
+        """
+        Creates a new MongoDB session.
 
-class Session(typing.AsyncContextManager):
-    """
-        Represents a MongoDB session for performing database operations within a transaction-like context.
+        Returns:
+            Session: A new MongoDB session associated with the engine.
+        """
+        return Session(engine=self)
+
+    def collection(self, document_cls_or_name: typing.Type[T] | str) -> AgnosticCollection:
+        """
+        Retrieves the MongoDB collection.
+
+        Args:
+            document_cls_or_name (typing.Type[T] | str): The document class or collection name.
+
+        Returns:
+            AgnosticCollection: The MongoDB collection.
+        """
+        if not isinstance(document_cls_or_name, str):
+            return self._get_document_collection(document_cls_or_name)
+
+        # noinspection PyTypeChecker
+        return self.database[document_cls_or_name].with_options(
+            codec_options=self._codec_options,
+            read_preference=self._read_preference,
+            read_concern=self._read_concern,
+            write_concern=self._write_concern
+        )
+
+    # noinspection SpellCheckingInspection
+    def gridfs(
+        self,
+        bucket_name: str = 'fs',
+        chunk_size_bytes: int = gridfs.DEFAULT_CHUNK_SIZE
+    ) -> AgnosticGridFSBucket:
+        """
+        Retrieves the GridFS bucket.
 
         Args:
-            engine (Engine): The MongoDB engine associated with the session.
+            bucket_name (str): The name of the GridFS bucket.
+            chunk_size_bytes (int): The chunk size in bytes.
+
+        Returns:
+            AgnosticGridFSBucket: The GridFS bucket.
+        """
+        return AsyncIOMotorGridFSBucket(
+            database=self.database,
+            bucket_name=bucket_name,
+            chunk_size_bytes=chunk_size_bytes,
+            write_concern=self.database.write_concern,
+            read_preference=self.database.read_preference
+        )
+
+    @sync.proxy
+    def connect(
+        self,
+        *conn,
+        ping: bool = False
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._connect(*conn, ping)
+
+    @sync.proxy
+    async def migrate(
+        self,
+        document_cls: typing.Type[T],
+        session: 'Session' = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._migrate(document_cls, session)
+
+    @sync.proxy
+    def migrate_all(
+        self,
+        documents_cls: list[typing.Type[T]],
+        session: 'Session' = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._migrate_all(documents_cls, session)
+
+    @sync.proxy
+    def seeding(
+        self,
+        func: typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]],
+        session: 'Session' = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._seeding(func, session)
+
+    @sync.proxy
+    def seeding_all(
+        self,
+        funcs: list[typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]]],
+        session: 'Session' = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._seeding_all(funcs, session)
+
+
+class Session(typing.AsyncContextManager, typing.ContextManager):
+    """
+    Represents a MongoDB session for performing database operations within a transaction-like context.
+
+    Args:
+        engine (Engine): The MongoDB engine associated with the session.
     """
+
     def __init__(self, engine: Engine):
+        # MongoDB engine associated with the session
         self._engine = engine
+        # MongoDB driver session
         self._driver_session = None
 
     @property
     def engine(self) -> Engine:
         """
         Returns the MongoDB engine associated with the session.
-
-        Returns:
-            Engine: The MongoDB engine.
         """
         return self._engine
 
     @property
     def started(self) -> bool:
         """
         Returns a boolean indicating whether the session has been started.
-
-        Returns:
-            bool: True if the session has been started, False otherwise.
         """
         return self._driver_session is not None
 
     @property
     def driver_session(self) -> AgnosticClientSession:
         """
         Returns the MongoDB driver session.
 
         Raises:
             EngineError: If the session is not started.
-
-        Returns:
-            AgnosticClientSession: The MongoDB driver session.
         """
         if not self.started:
-            raise EngineError('Session not started')
+            raise SessionError('Session not started')
         return self._driver_session
 
-    async def start(self):
+    async def __aenter__(self) -> 'Session':
+        """
+        Enables the use of the 'async with' statement.
+        """
+        await self._start()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
+        """
+        Enables the use of the 'async with' statement. Ends the session upon exiting the context.
+        """
+        await self._end()
+
+    def __enter__(self) -> 'Session':
+        return sync.run_sync(self.__aenter__)()
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        sync.run_sync(self.__aexit__)(exc_type, exc_value, traceback)
+
+    async def _start(self):
         """
         Starts the MongoDB session.
 
         Raises:
             EngineError: If the session is already started.
         """
-        if self.started:
-            raise EngineError('Session already started')
-        self._driver_session = await self.engine.client.start_session()
+        if not self._driver_session:
+            self._driver_session = await self.engine.client.start_session()
 
-    async def end(self):
+    async def _end(self):
         """
         Ends the MongoDB session.
 
         Raises:
             EngineError: If the session is not started.
         """
-        if not self.started:
-            raise EngineError('Session not started')
-        await self.driver_session.end_session()
-        self._driver_session = None
-
-    async def __aenter__(self) -> 'Session':
-        """
-        Enables the use of the 'async with' statement.
-
-        Returns:
-            Session: The session instance.
-        """
-        await self.start()
-        return self
+        if self.driver_session:
+            await self.driver_session.end_session()
+            self._driver_session = None
 
-    async def __aexit__(self, __exc_type, __exc_value, __traceback) -> None:
+    async def _save_references(self, doc: T):
         """
-        Enables the use of the 'async with' statement. Ends the session upon exiting the context.
+        Saves referenced documents.
 
         Args:
-            __exc_type: The type of the exception.
-            __exc_value: The exception value.
-            __traceback: The exception traceback.
-        """
-        await self.end()
-
-    def transaction(self) -> 'Transaction':
-        """
-        Creates a new MongoDB transaction.
-
-        Returns:
-            Transaction: A new MongoDB transaction associated with the engine
+            doc (T): The document object.
         """
-        return Transaction(provider=self)
-
-    def objects(self, document_cls: typing.Type[T], dereference_deep: int = 0) -> 'Objects[T]':
-        return Objects(document_cls, session=self, dereference_deep=dereference_deep)
-
-    def fs(self, chunk_size_bytes: int = gridfs.DEFAULT_CHUNK_SIZE) -> 'FsBucket':
-        return FsBucket(self, chunk_size_bytes=chunk_size_bytes)
-
-    async def _save_references(self, doc: T):
         operations = []
         for field, reference in doc.__references__.items():
             obj = getattr(doc, field)
             if obj in (expressions.EmptyValue, None):
                 continue
             if not reference.is_many:
                 obj = [obj]
             operations.append(
-                self.save_all(obj, save_references=True)
+                self._save_all(obj, save_references=True)
             )
 
         await asyncio.gather(*operations)
 
-    async def save(self, doc: T, save_references: bool = False):
+    async def _save(self, doc: T, save_references: bool = False):
+        """
+        Saves a document to the database.
+
+        Args:
+            doc (T): The document object to save.
+            save_references (bool): Whether to save referenced documents.
+        """
         operations = []
         if save_references:
             operations.append(self._save_references(doc))
 
         son = doc.dump_bson()
-        operations.append(
-            self.engine.collection(doc.__collection_name__).update_one(
-                filter=Query.Eq('_id', son.pop('_id')),
-                update={'$set': son},
-                upsert=True,
-                session=self.driver_session
-            )
-        )
         await asyncio.gather(*operations)
+        await self.engine.collection(doc.__collection_name__).update_one(
+            filter=Query.Eq('_id', son.pop('_id')),
+            update={'$set': son},
+            upsert=True,
+            session=self.driver_session
+        )
+
+    async def _save_all(self, docs: list[T], save_references: bool = False):
+        """
+        Saves a list of documents to the database.
 
-    async def save_all(self, docs: list[T], save_references: bool = False):
-        await asyncio.gather(*[self.save(i, save_references) for i in docs if i is not None])
+        Args:
+            docs (list[T]): The list of document objects to save.
+            save_references (bool): Whether to save referenced documents.
+        """
+        await asyncio.gather(*[self._save(i, save_references) for i in docs if i is not None])
 
     async def _delete_cascade(self, doc: T):
+        """
+        Deletes documents that reference the given document.
+
+        Args:
+            doc (T): The document object to delete.
+        """
         doc_cls = type(doc)
         rev_references = references.get_reverse_references(document_cls=doc_cls)
         operations = []
 
         # Get reverse references
         for ref_doc_cls, refs in rev_references.items():
             ref_doc_objects = self.objects(ref_doc_cls, dereference_deep=1)
@@ -629,142 +664,208 @@
                             if getattr(i, reference.ref_field.name) != getattr(doc, reference.ref_field.name)
                         ]
                         if not value:
                             do_delete = True
                             break
                         setattr(ref_doc, field_name, value)
                         # Apply update
-                        operations.append(self.save(ref_doc))
+                        operations.append(self._save(ref_doc))
 
                 # Apply delete
                 if do_delete:
-                    operations.append(self.delete(ref_doc, delete_cascade=True))
+                    operations.append(self._delete(ref_doc, delete_cascade=True))
 
         await asyncio.gather(*operations)
 
-    async def delete(self, doc: T, delete_cascade: bool = False):
+    async def _delete(self, doc: T, delete_cascade: bool = False):
+        """
+        Deletes a document from the database.
+
+        Args:
+            doc (T): The document object to delete.
+            delete_cascade (bool): Whether to delete referenced documents.
+        """
         operations = []
         if delete_cascade:
             operations.append(self._delete_cascade(doc))
 
         await asyncio.gather(*operations)
         await self.engine.collection(doc.__collection_name__).delete_one(
             filter=Query.Eq('_id', doc.id),
             session=self.driver_session
         )
 
-    async def delete_all(self, docs: list[T], delete_cascade: bool = False):
-        await asyncio.gather(*[self.delete(i, delete_cascade) for i in docs if i is not None])
+    async def _delete_all(self, docs: list[T], delete_cascade: bool = False):
+        """
+        Deletes a list of documents from the database.
+
+        Args:
+            docs (list[T]): The list of document objects to delete.
+            delete_cascade (bool): Whether to delete referenced documents.
+        """
+        await asyncio.gather(*[self._delete(i, delete_cascade) for i in docs if i is not None])
 
+    def transaction(self) -> 'Transaction':
+        """
+        Creates a new MongoDB transaction.
 
-class Transaction(typing.AsyncContextManager):
-    # noinspection GrazieInspection
+        Returns:
+            Transaction: A new MongoDB transaction associated with the engine
+        """
+        return Transaction(session=self)
+
+    def objects(self, document_cls: typing.Type[T], dereference_deep: int = 0) -> 'Objects[T]':
+        """
+        Returns an object manager for the specified document class.
+
+        Args:
+            document_cls (typing.Type[T]): The document class.
+            dereference_deep (int): Depth of dereferencing.
+
+        Returns:
+            Objects[T]: An object manager.
+        """
+        return Objects(document_cls, session=self, dereference_deep=dereference_deep)
+
+    def fs(self, chunk_size_bytes: int = gridfs.DEFAULT_CHUNK_SIZE) -> 'FsBucket':
+        """
+        Returns a GridFS bucket manager.
+
+        Args:
+            chunk_size_bytes (int): The chunk size in bytes.
+
+        Returns:
+            FsBucket: A GridFS bucket manager.
+        """
+        return FsBucket(self, chunk_size_bytes=chunk_size_bytes)
+
+    @sync.proxy
+    def start(self) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._start()
+
+    @sync.proxy
+    def end(self) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._end()
+
+    @sync.proxy
+    def save(
+        self,
+        doc: T,
+        save_references: bool = False
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._save(doc, save_references)
+
+    @sync.proxy
+    def save_all(
+        self,
+        docs: list[T],
+        save_references: bool = False
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._save_all(docs, save_references)
+
+    @sync.proxy
+    def delete(
+        self,
+        doc: T,
+        delete_cascade: bool = False
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._delete(doc, delete_cascade)
+
+    @sync.proxy
+    def delete_all(
+        self,
+        docs: list[T],
+        delete_cascade: bool = False
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._delete_all(docs, delete_cascade)
+
+
+class Transaction(typing.AsyncContextManager, typing.ContextManager):
     """
         Represents a MongoDB transaction for performing atomic operations within a session or engine context.
 
         Args:
-            provider (Session or Engine): The provider of the transaction, either a Session or an Engine.
+            session (Session): The session related with transaction.
     """
 
-    def __init__(self, provider: Session | Engine):
-        self._is_session_provided = isinstance(provider, Session)
-        self._tx_started = False
-        self._tx_context = None
-
-        # Get session instance according provider type
-        if self._is_session_provided:
-            if not provider.started:
-                raise EngineError('Session not started')
-            self._session = provider
-        else:
-            self._session = provider.session()
+    # noinspection PyProtectedMember
+    def __init__(self, session: Session):
+        self._session = session
+
+        # Start transaction
+        self._session.driver_session.start_transaction(
+            read_concern=self._session.engine._read_concern,
+            read_preference=self._session.engine._read_preference,
+            write_concern=self._session.engine._write_concern
+        )
 
     @property
     def session(self) -> 'Session':
         """
         Returns the associated MongoDB session for the transaction.
 
         Returns:
             Session: The associated MongoDB session.
         """
         return self._session
 
-    @property
-    def started(self) -> bool:
+    async def __aenter__(self) -> 'Transaction':
         """
-        Returns a boolean indicating whether the transaction has been started.
+        Enables the use of the 'async with' statement.
 
         Returns:
-            bool: True if the transaction has been started, False otherwise.
+            Transaction: The transaction instance.
         """
-        return self._tx_started
+        return self
 
-    async def start(self):
+    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         """
-        Starts the MongoDB transaction.
+        Enables the use of the 'async with' statement. Ends the transaction upon exiting the context.
 
-        Raises:
-            EngineError: If the transaction is already started.
+        Args:
+            exc_type: The type of the exception.
+            exc_value: The exception value.
+            traceback: The exception traceback.
         """
-        if self._tx_started:
-            raise EngineError('Transaction already started')
-        if not self._is_session_provided:
-            await self._session.start()
-        self._tx_context = await self._session.driver_session.start_transaction().__aenter__()
-        self._tx_started = True
+        if exc_value:
+            await self._abort()
+        else:
+            await self._commit()
+
+    def __enter__(self) -> 'Transaction':
+        return self
 
-    async def commit(self):
+    def __exit__(self, exc_type, exc_value, traceback):
+        sync.run_sync(self.__aexit__)(exc_type, exc_value, traceback)
+
+    async def _commit(self):
         """
         Commits changes and closes the MongoDB transaction.
 
         Raises:
             EngineError: If the transaction is not started.
         """
-        if not self._tx_started:
-            raise EngineError('Transaction not started')
         await self._session.driver_session.commit_transaction()
-        if not self._is_session_provided:
-            await self._session.end()
-        self._tx_started = False
 
-    async def abort(self):
+    async def _abort(self):
         """
         Discards changes and closes the MongoDB transaction.
 
         Raises:
             EngineError: If the transaction is not started.
         """
-        if not self._tx_started:
-            raise EngineError('Transaction not started')
         await self._session.driver_session.abort_transaction()
-        if not self._is_session_provided:
-            await self._session.end()
-        self._tx_started = False
-
-    async def __aenter__(self) -> 'Transaction':
-        """
-        Enables the use of the 'async with' statement.
-
-        Returns:
-            Transaction: The transaction instance.
-        """
-        await self.start()
-        return self
-
-    async def __aexit__(self, __exc_type, __exc_value, __traceback) -> None:
-        """
-        Enables the use of the 'async with' statement. Ends the transaction upon exiting the context.
 
-        Args:
-            __exc_type: The type of the exception.
-            __exc_value: The exception value.
-            __traceback: The exception traceback.
-        """
-        await self._tx_context.__aexit__(__exc_type, __exc_value, __traceback)
-        self._tx_started = False
+    @sync.proxy
+    def commit(self) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._commit()
+
+    @sync.proxy
+    def abort(self) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._abort()
 
 
 class Objects(typing.Generic[T]):
     # noinspection SpellCheckingInspection
     """
         Represents a query set for retrieving documents from the database.
         This class provides methods for filtering, sorting, limiting, and executing queries asynchronously.
@@ -781,15 +882,15 @@
         self._dereference_deep = dereference_deep
         self._collection = session.engine.collection(document_cls)
         self._filter = expressions.Query()
         self._sort = expressions.Sort()
         self._skip = 0
         self._limit = 0
 
-    def __copy_with__(self, **options) -> 'Objects[T]':
+    def __copy__(self, **options) -> 'Objects[T]':
         """
         Creates a shallow copy of the query set with specified options.
 
         Args:
             **options: Additional options to be applied to the copy.
 
         Returns:
@@ -804,85 +905,14 @@
         setattr(objs, '_filter', options.get('_filter', self._filter))
         setattr(objs, '_sort', options.get('_sort', self._sort))
         setattr(objs, '_skip', options.get('_skip', self._skip))
         setattr(objs, '_limit', options.get('_limit', self._limit))
 
         return objs
 
-    async def create(self, **data) -> T:
-        """
-        Creates a new document in the database.
-
-        Args:
-            **data: Keyword arguments representing the document data.
-
-        Returns:
-            T: The newly created document instance.
-        """
-        doc = self._document_cls(**data)
-        await self._session.save(doc, save_references=True)
-        return doc
-
-    def filter(self, *queries: expressions.Query | bool, **filters) -> 'Objects[T]':
-        """
-        Adds filter conditions to the query set.
-
-        Args:
-            *queries (expressions.Query | bool): Variable number of filter expressions.
-            **filters: Keyword arguments representing additional filter conditions.
-
-        Returns:
-            Objects[T]: The updated query set with added filter conditions.
-        """
-        _filter = self._filter
-        for q in queries:
-            _filter = _filter & q
-        if filters:
-            _filter = _filter & expressions.Q(**filters)
-        return self.__copy_with__(_filter=_filter)
-
-    def sort(self, *sorts: expressions.Sort) -> 'Objects[T]':
-        """
-        Adds sort conditions to the query set.
-
-        Args:
-            *sorts (expressions.Sort): Variable number of sort expressions.
-
-        Returns:
-            Objects[T]: The updated query set with added sort conditions.
-        """
-        _sort = self._sort
-        for sort in sorts:
-            _sort = _sort | expressions.Sort(sort)
-        return self.__copy_with__(_sort=_sort)
-
-    def skip(self, skip: int) -> 'Objects[T]':
-        """
-        Sets the number of documents to skip in the result set.
-
-        Args:
-            skip (int): The number of documents to skip.
-
-        Returns:
-            Objects[T]: The updated query set with the skip value set.
-        """
-        return self.__copy_with__(_skip=skip)
-
-    def limit(self, limit: int) -> 'Objects[T]':
-        """
-        Sets the maximum number of documents to return.
-
-        Args:
-            limit (int): The maximum number of documents to return.
-
-        Returns:
-            Objects[T]: The updated query set with the limit value set.
-        """
-        return self.__copy_with__(_limit=limit)
-
     async def __aiter__(self) -> typing.AsyncGenerator[T, None]:
         """
         Asynchronously iterates over the result set, executing the query.
 
         Yields:
             T: The parsed document instances.
 
@@ -905,77 +935,165 @@
         if self._limit > 0:
             pipeline.append({'$limit': self._limit})
 
         cursor = self._collection.aggregate(pipeline, session=self._session.driver_session)
         async for data in cursor:
             yield self._document_cls(**data)
 
-    async def fetch(self, dereference_deep: int = 0) -> list[T]:
+    def __iter__(self) -> typing.Generator[T, None, None]:
+        for doc in sync.as_sync_gen(self.__aiter__()):
+            yield doc
+
+    async def _create(self, **data) -> T:
         """
-        Retrieves all documents in the result set.
+        Creates a new document in the database.
 
         Args:
-            dereference_deep (int): The depth of dereference documents.
+            **data: Keyword arguments representing the document data.
+
+        Returns:
+            T: The newly created document instance.
+        """
+        doc = self._document_cls(**data)
+        # noinspection PyProtectedMember
+        await self._session._save(doc, save_references=True)
+        return doc
+
+    async def _fetch(self) -> list[T]:
+        """
+        Retrieves all documents in the result set.
 
         Returns:
             list[T]: The list of parsed document instances.
         """
-        self._dereference_deep = dereference_deep
         return [doc async for doc in self]
 
-    async def fetch_one(self, dereference_deep: int = 0) -> T:
+    async def _fetch_one(self) -> T:
         """
         Retrieves a specific document in the result set.
 
-        Args:
-            dereference_deep (int): The depth of dereference documents.
-
         Returns:
             T: The parsed document instance.
 
         Raises:
             NoResultsError: If no results are found.
             ManyResultsError: If more than one result is found.
         """
-        docs = await self.limit(2).fetch(dereference_deep)
+        docs = await self.limit(2)._fetch()
         if not docs:
             raise NoResultsError()
         if len(docs) > 1:
             raise ManyResultsError()
         return docs[0]
 
     # noinspection PyShadowingBuiltins
-    async def fetch_by_id(self, value: typing.Any, dereference_deep: int = 0) -> T:
+    async def _fetch_by_id(self, value: typing.Any) -> T:
         """
         Retrieves a document by its identifier.
 
         Args:
             value (typing.Any): The identifier value.
-            dereference_deep (int): The depth of dereference documents.
 
         Returns:
             T: The parsed document instance.
         """
-        id_mapper = self._document_cls.__fields__['id'].mapper
+        # noinspection PyProtectedMember
         return await self.filter(
-            Query.Eq('_id', id_mapper.validate(value))
-        ).fetch_one(dereference_deep)
+            self._document_cls.id == self._document_cls.id._field.mapper.validate(value)
+        )._fetch_one()
 
-    async def count(self) -> int:
+    async def _count(self) -> int:
         """
         Counts the number of documents in the result set.
 
         Returns:
             int: The count of documents.
         """
         return await self._collection.count_documents(
             filter=self._filter,
             session=self._session.driver_session
         )
 
+    def filter(self, *queries: expressions.Query | bool, **filters) -> 'Objects[T]':
+        """
+        Adds filter conditions to the query set.
+
+        Args:
+            *queries (expressions.Query | bool): Variable number of filter expressions.
+            **filters: Keyword arguments representing additional filter conditions.
+
+        Returns:
+            Objects[T]: The updated query set with added filter conditions.
+        """
+        _filter = self._filter
+        for q in queries:
+            _filter = _filter & q
+        if filters:
+            _filter = _filter & expressions.Q(**filters)
+        return self.__copy__(_filter=_filter)
+
+    def sort(self, *sorts: expressions.Sort) -> 'Objects[T]':
+        """
+        Adds sort conditions to the query set.
+
+        Args:
+            *sorts (expressions.Sort): Variable number of sort expressions.
+
+        Returns:
+            Objects[T]: The updated query set with added sort conditions.
+        """
+        _sort = self._sort
+        for sort in sorts:
+            _sort = _sort | expressions.Sort(sort)
+        return self.__copy__(_sort=_sort)
+
+    def skip(self, skip: int) -> 'Objects[T]':
+        """
+        Sets the number of documents to skip in the result set.
+
+        Args:
+            skip (int): The number of documents to skip.
+
+        Returns:
+            Objects[T]: The updated query set with the skip value set.
+        """
+        return self.__copy__(_skip=skip)
+
+    def limit(self, limit: int) -> 'Objects[T]':
+        """
+        Sets the maximum number of documents to return.
+
+        Args:
+            limit (int): The maximum number of documents to return.
+
+        Returns:
+            Objects[T]: The updated query set with the limit value set.
+        """
+        return self.__copy__(_limit=limit)
+
+    @sync.proxy
+    def create(self, **data) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
+        return self._create(**data)
+
+    @sync.proxy
+    def fetch(self) -> typing.Coroutine[typing.Any, typing.Any, list[T]] | list[T]:
+        return self._fetch()
+
+    @sync.proxy
+    def fetch_one(self) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
+        return self._fetch_one()
+
+    @sync.proxy
+    def fetch_by_id(self, value: typing.Any) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
+        return self._fetch_by_id(value)
+
+    @sync.proxy
+    def count(self) -> typing.Coroutine[typing.Any, typing.Any, int] | int:
+        return self._count()
+
 
 # noinspection PyProtectedMember
 class FsBucket(Objects['FsObject']):
     # noinspection SpellCheckingInspection
     """
         Represents a file system bucket for storing and managing file objects.
         This class inherits from Objects and provides methods for file upload,
@@ -995,15 +1113,15 @@
             document_cls=FsObject,
             session=session
         )
         self._bucket = session.engine.gridfs('fs', chunk_size_bytes)
         self._chunk_size_bytes = chunk_size_bytes
 
     # noinspection PyMethodMayBeStatic
-    async def create(
+    async def _create(
         self,
         filename: str,
         src: typing.IO | bytes,
         metadata: dict = None,
         chunk_size_bytes: int = None
     ) -> 'FsObject':
         """
@@ -1035,42 +1153,66 @@
             filename=filename,
             source=src,
             metadata=metadata,
             chunk_size_bytes=chunk_size_bytes or self._chunk_size_bytes,
             session=self._session.driver_session
         )
         # Update obj info
-        obj = await self.fetch_by_id(obj.id)
+        obj = await self._fetch_by_id(obj.id)
 
         return obj
 
-    async def exist(self, filename: str) -> bool:
+    async def _exist(self, filename: str) -> bool:
         """
         Checks if a file exists in the file system bucket.
 
         Args:
             filename (str): The name of the file.
 
         Returns:
             bool: True if the file exists, False otherwise.
         """
-        count = await self.filter(Query.Eq('filename', filename)).count()
+        count = await self.filter(Query.Eq('filename', filename))._count()
         return count > 0
 
-    async def revisions(self, filename: str) -> list['FsObject']:
+    async def _revisions(self, filename: str) -> list['FsObject']:
         """
         Retrieves all revisions of a file from the file system bucket.
 
         Args:
             filename (str): The name of the file.
 
         Returns:
             list[FsObject]: A list of file objects representing revisions.
         """
-        return await self.filter(Query.Eq('filename', filename)).fetch()
+        return await self.filter(Query.Eq('filename', filename))._fetch()
+
+    @sync.proxy
+    def create(
+        self,
+        filename: str,
+        src: typing.IO | bytes,
+        metadata: dict = None,
+        chunk_size_bytes: int = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, 'FsObject'] | 'FsObject':
+        return self._create(filename, src, metadata, chunk_size_bytes)
+
+    @sync.proxy
+    def exist(
+        self,
+        filename: str
+    ) -> typing.Coroutine[typing.Any, typing.Any, bool] | bool:
+        return self._exist(filename)
+
+    @sync.proxy
+    def revisions(
+        self,
+        filename: str
+    ) -> typing.Coroutine[typing.Any, typing.Any, list['FsObject']] | list['FsObject']:
+        return self._revisions(filename)
 
 
 # noinspection PyProtectedMember
 class FsObject(documents.Document):
     """
     Represents a file object stored in the file system.
     This class inherits from Document and provides methods for creating revisions, downloading, and streaming files.
@@ -1088,40 +1230,54 @@
     metadata: types.Json
     chunk_size: int = fields.field(alias='chunkSize')
     length: int
     upload_date: datetime.datetime = fields.field(alias='uploadDate')
 
     __collection_name__ = 'fs.files'
 
-    async def create_revision(self, fs: FsBucket, src: typing.IO | bytes, metadata: dict = None):
+    @property
+    def content_type(self) -> str:
+        return self.metadata.get('contentType')
+
+    @property
+    def chunks(self) -> int:
+        import math
+        return math.ceil(self.length / self.chunk_size)
+
+    async def _create_revision(
+        self,
+        fs: FsBucket,
+        src: typing.IO | bytes,
+        metadata: dict = None
+    ) -> 'FsObject':
         """
         Creates a revision of the file.
 
         Args:
             fs (FsBucket): The file system bucket where the revision will be created.
             src (typing.IO | bytes): The source file object or bytes for the new revision.
             metadata (dict, optional): Additional metadata for the new revision.
 
         """
-        await fs.create(
+        return await fs._create(
             self.filename,
             src=src,
             metadata=metadata,
             chunk_size_bytes=self.chunk_size
         )
 
     # noinspection SpellCheckingInspection
-    async def download(self, fs: FsBucket, dest: typing.IO, revision: int = None):
+    async def _download(self, fs: FsBucket, dest: typing.IO, revision: int = None):
         """
         Downloads the file from the file system.
 
         Args:
             fs (FsBucket): The file system bucket from where the file will be downloaded.
             dest (typing.IO): The destination file object to write the downloaded file contents.
-            revision (int): The revision number of the file to download. If None, downloads the latest revision.
+            revision (int): The revision number of the file to download. If None, download the latest revision.
 
         """
         if revision is None:
             await fs._bucket.download_to_stream(
                 file_id=self.id,
                 destination=dest,
                 session=fs._session.driver_session
@@ -1130,39 +1286,177 @@
             await fs._bucket.download_to_stream_by_name(
                 filename=self.filename,
                 destination=dest,
                 revision=revision,
                 session=fs._session.driver_session
             )
 
-    async def stream(self, fs: FsBucket, revision: int = None) -> AsyncIOMotorGridOut:
+    async def _stream(self, fs: FsBucket, revision: int = None) -> 'FsOutput':
         """
         Streams the file from the file system.
 
         Args:
             fs (FsBucket): The file system bucket from where the file will be streamed.
             revision (int, optional): The revision number of the file to stream. If None, streams the latest revision.
 
         Returns:
             AsyncIOMotorGridOut: An asynchronous grid file stream.
 
         """
         if revision is None:
-            return await fs._bucket.open_download_stream(
+            grid_out = await fs._bucket.open_download_stream(
                 file_id=self.id,
                 session=fs._session.driver_session
             )
-        return await fs._bucket.open_download_stream_by_name(
-            filename=self.filename,
-            revision=revision,
+        else:
+            grid_out = await fs._bucket.open_download_stream_by_name(
+                filename=self.filename,
+                revision=revision,
+                session=fs._session.driver_session
+            )
+        return FsOutput(grid_out)
+
+    async def _delete(self, fs: FsBucket):
+        await fs._bucket.delete(
+            file_id=self.id,
             session=fs._session.driver_session
         )
 
+    @sync.proxy
+    def create_revision(
+        self,
+        fs: FsBucket,
+        src: typing.IO | bytes,
+        metadata: dict = None
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FsObject'], 'FsObject']:
+        return self._create_revision(fs, src, metadata)
+
+    @sync.proxy
+    def download(
+        self,
+        fs: FsBucket,
+        dest: typing.IO,
+        revision: int = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._download(fs, dest, revision)
+
+    @sync.proxy
+    def stream(
+        self,
+        fs: FsBucket,
+        revision: int = None
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'FsOutput'], 'FsOutput']:
+        return self._stream(fs, revision)
+
+    @sync.proxy
+    def delete(self, fs: FsBucket) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        return self._delete(fs)
+
+
+class FsOutput:
+    """
+    Represents a file stored in MongoDB GridFS.
+
+    Args:
+        grid_out (AsyncIOMotorGridOut): The underlying GridFS file object.
+
+    """
+
+    def __init__(self, grid_out: AsyncIOMotorGridOut):
+        self._driver_grid_out = grid_out
+
+    async def _read(self, size: int = -1) -> bytes:
+        """
+        Reads data from the file asynchronously.
+
+        Args:
+            size (int, optional): The number of bytes to read. If not specified or negative, reads until EOF.
+
+        Returns:
+            bytes: The data read from the file.
+        """
+        return await self._driver_grid_out.read(size)
+
+    # noinspection SpellCheckingInspection
+    async def _readchunk(self) -> bytes:
+        """
+        Reads a chunk of data from the file asynchronously.
+
+        Returns:
+            bytes: The data chunk read from the file.
+        """
+        return await self._driver_grid_out.readchunk()
+
+    async def _readline(self, size: int = -1) -> bytes:
+        """
+        Reads a line from the file asynchronously.
+
+        Args:
+            size (int, optional): The maximum number of bytes to read. If not specified or negative, reads until EOF.
+
+        Returns:
+            bytes: The line read from the file.
+        """
+        return await self._driver_grid_out.readline(size)
+
+    def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
+        """
+        Moves the file pointer to a specified position.
+
+        Args:
+            pos (int): The position to seek to.
+            whence (int, optional): The reference point for the seek operation.
+
+        Returns:
+            int: The new position of the file pointer.
+        """
+        return self._driver_grid_out.seek(pos, whence)
+
+    def seekable(self) -> bool:
+        """
+        Checks if the file is seekable.
+
+        Returns:
+            bool: True if the file is seekable, False otherwise.
+        """
+        return self._driver_grid_out.seekable()
+
+    def tell(self) -> int:
+        """
+        Returns the current position of the file pointer.
+
+        Returns:
+            int: The current position of the file pointer.
+        """
+        return self._driver_grid_out.tell()
+
+    def close(self):
+        """Closes the file."""
+        self._driver_grid_out.close()
+
+    @sync.proxy
+    def read(
+        self,
+        size: int = -1
+    ) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
+        return self._read(size)
+
+    # noinspection SpellCheckingInspection
+    @sync.proxy
+    def readchunk(self) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
+        return self._readchunk()
+
+    @sync.proxy
+    def readline(
+        self,
+        size: int = -1
+    ) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
+        return self._readline(size)
+
 
-# noinspection SpellCheckingInspection
 class Seeding(documents.Document):
     """
     Represents a seeding operation in the database.
     This class inherits from Document and tracks seeding functions applied to the database.
 
     Attributes:
         function (str): The name or identifier of the seeding function.
```

### Comparing `mongotoy-0.1.2/mongotoy/documents.py` & `mongotoy-0.1.3/mongotoy/documents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import dataclasses
+import typing
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Any, Literal
 
 import bson
 import pymongo
 from pymongo.read_concern import ReadConcern
 
@@ -238,14 +239,54 @@
     Class representing an embedded document.
 
     This class serves as a base for defining embedded documents within other documents. It inherits functionality
     from the BaseDocument class.
     """
 
 
+@dataclasses.dataclass
+class DocumentConfig:
+    """
+    Represents configuration options for a document in MongoDB.
+
+    This data class defines various settings such as indexes, capped collection options, timeseries collection options,
+    codec options, read preference, read concern, write concern, and extra options for a MongoDB document.
+
+    Attributes:
+        indexes (list[pymongo.IndexModel]): List of index models for the document.
+        capped (bool): Indicates if the collection is capped (default is False).
+        capped_size (int): The maximum size of the capped collection in bytes (default is 16 MB).
+        capped_max (int): The maximum number of documents allowed in a capped collection (default is None).
+        timeseries_field (str): The field name to use as the time field for timeseries collections (default is None).
+        timeseries_meta_field (str): The field name for metadata in timeseries collections (default is None).
+        timeseries_granularity (Literal['seconds', 'minutes', 'hours']): The granularity of time intervals.
+        timeseries_expire_after_seconds (int): The expiration time for documents in a timeseries collection, in seconds.
+        codec_options (bson.CodecOptions): The BSON codec options (default is None).
+        read_preference (pymongo.ReadPreference): The read preference for the document (default is None).
+        read_concern (ReadConcern): The read concern for the document (default is None).
+        write_concern (pymongo.WriteConcern): The written concern for the document (default is None).
+        extra_options (dict): Extra options for the document configuration (default is an empty dictionary).
+
+    """
+
+    indexes: list[pymongo.IndexModel] = dataclasses.field(default_factory=lambda: list())
+    capped: bool = dataclasses.field(default=False)
+    capped_size: int = dataclasses.field(default=16 * (2 ** 20))  # 16 Mb
+    capped_max: int = dataclasses.field(default=None)
+    timeseries_field: str = dataclasses.field(default=None)
+    timeseries_meta_field: str = dataclasses.field(default=None)
+    timeseries_granularity: Literal['seconds', 'minutes', 'hours'] = dataclasses.field(default='seconds')
+    timeseries_expire_after_seconds: int = dataclasses.field(default=None)
+    codec_options: bson.CodecOptions = dataclasses.field(default=None)
+    read_preference: pymongo.ReadPreference = dataclasses.field(default=None)
+    read_concern: ReadConcern = dataclasses.field(default=None)
+    write_concern: pymongo.WriteConcern = dataclasses.field(default=None)
+    extra_options: dict = dataclasses.field(default_factory=lambda: dict())
+
+
 class DocumentMeta(BaseDocumentMeta):
     """
     Metaclass for document class.
     """
 
     # noinspection PyUnresolvedReferences
     def __new__(mcls, name, bases, namespace, **kwargs):
@@ -271,15 +312,15 @@
         _references = OrderedDict()
         for field in _cls.__fields__.values():
             # Check id field
             # noinspection PyProtectedMember
             if field._options.id_field:
                 _id_field = field
 
-            # Unwrap ManyMapper
+            # Unwrap SequenceMapper
             _mapper = field.mapper
             _is_many = False
             if isinstance(_mapper, mappers.SequenceMapper):
                 _mapper = _mapper.unwrap()
                 _is_many = True
 
             # Add references
@@ -310,54 +351,14 @@
         _cls.__collection_name__ = namespace.get('__collection_name__', f'{name.lower()}s')
         _cls.id = _id_field
         _cls.document_config = namespace.get('document_config', DocumentConfig())
 
         return _cls
 
 
-@dataclasses.dataclass
-class DocumentConfig:
-    """
-    Represents configuration options for a document in MongoDB.
-
-    This data class defines various settings such as indexes, capped collection options, timeseries collection options,
-    codec options, read preference, read concern, write concern, and extra options for a MongoDB document.
-
-    Attributes:
-        indexes (list[pymongo.IndexModel]): List of index models for the document.
-        capped (bool): Indicates if the collection is capped (default is False).
-        capped_size (int): The maximum size of the capped collection in bytes (default is 16 MB).
-        capped_max (int): The maximum number of documents allowed in a capped collection (default is None).
-        timeseries_field (str): The field name to use as the time field for timeseries collections (default is None).
-        timeseries_meta_field (str): The field name for metadata in timeseries collections (default is None).
-        timeseries_granularity (Literal['seconds', 'minutes', 'hours']): The granularity of time intervals.
-        timeseries_expire_after_seconds (int): The expiration time for documents in a timeseries collection, in seconds.
-        codec_options (bson.CodecOptions): The BSON codec options (default is None).
-        read_preference (pymongo.ReadPreference): The read preference for the document (default is None).
-        read_concern (ReadConcern): The read concern for the document (default is None).
-        write_concern (pymongo.WriteConcern): The write concern for the document (default is None).
-        extra_options (dict): Extra options for the document configuration (default is an empty dictionary).
-
-    """
-
-    indexes: list[pymongo.IndexModel] = dataclasses.field(default_factory=lambda: list())
-    capped: bool = dataclasses.field(default=False)
-    capped_size: int = dataclasses.field(default=16 * (2 ** 20))  # 16 Mb
-    capped_max: int = dataclasses.field(default=None)
-    timeseries_field: str = dataclasses.field(default=None)
-    timeseries_meta_field: str = dataclasses.field(default=None)
-    timeseries_granularity: Literal['seconds', 'minutes', 'hours'] = dataclasses.field(default='seconds')
-    timeseries_expire_after_seconds: int = dataclasses.field(default=None)
-    codec_options: bson.CodecOptions = dataclasses.field(default=None)
-    read_preference: pymongo.ReadPreference = dataclasses.field(default=None)
-    read_concern: ReadConcern = dataclasses.field(default=None)
-    write_concern: pymongo.WriteConcern = dataclasses.field(default=None)
-    extra_options: dict = dataclasses.field(default_factory=lambda: dict())
-
-
 class Document(BaseDocument, metaclass=DocumentMeta):
     """
     Represents a document in MongoDB.
 
     This class inherits from BaseDocument and implements the DocumentMeta metaclass. It provides functionality
     for dumping BSON data.
 
@@ -400,7 +401,70 @@
             key = field.alias if by_alias else field.name
             value = son.pop(key, expressions.EmptyValue)
             if value is expressions.EmptyValue:
                 continue
             son[reference.key_name] = value
 
         return son
+
+
+# noinspection SpellCheckingInspection
+def get_embedded_document_cls(doc_type: typing.Type | str) -> typing.Type[EmbeddedDocument]:
+    """
+    Get the embedded document class based on its type or name.
+
+    Args:
+        doc_type (Type | str): The type or name of the embedded document.
+
+    Returns:
+        Type['documents.EmbeddedDocument']: The embedded document class.
+
+    Raises:
+        TypeError: If the provided type is not a subclass of mongotoy.EmbeddedDocument.
+    """
+    doc_cls = cache.documents.get_type(doc_type, do_raise=True)
+    if not issubclass(doc_cls, EmbeddedDocument):
+        raise TypeError(f'Type {doc_cls} is not a mongotoy.EmbeddedDocument subclass')
+
+    return doc_cls
+
+
+# noinspection SpellCheckingInspection
+def get_document_cls(doc_type: typing.Type | str) -> typing.Type[Document]:
+    """
+    Get the document class based on its type or name.
+
+    Args:
+        doc_type (Type | str): The type or name of the document.
+
+    Returns:
+        Type['documents.Document']: The document class.
+
+    Raises:
+        TypeError: If the provided type is not a subclass of mongotoy.Document.
+    """
+    doc_cls = cache.documents.get_type(doc_type, do_raise=True)
+    if not issubclass(doc_cls, Document):
+        raise TypeError(f'Type {doc_cls} is not a mongotoy.Document subclass')
+
+    return doc_cls
+
+
+def get_document_field(document_cls: typing.Type[BaseDocument], field_name: str) -> fields.Field:
+    """
+    Get the field from a document class based on the field's name.
+
+    Args:
+        document_cls (Type['documents.BaseDocument']): The document class containing the field.
+        field_name (str): The name of the field.
+
+    Returns:
+        'fields.Field': The field object.
+
+    Raises:
+        TypeError: If the field does not exist in the document class.
+    """
+    field = document_cls.__fields__.get(field_name)
+    if not field:
+        raise TypeError(f'Field `{document_cls.__name__}.{field}` does not exist')
+
+    return field
```

### Comparing `mongotoy-0.1.2/mongotoy/errors.py` & `mongotoy-0.1.3/mongotoy/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,24 @@
         super().__init__(f'[{".".join(loc)}]. {msg}')
 
 
 class EngineError(Exception):
     """
     Error raised for engine-related issues.
 
-    This exception is raised when there are errors related to engine operations, such as database connections
-    or queries.
+    This exception is raised when there are errors related to engine operations
+
+    """
+
+
+class SessionError(Exception):
+    """
+    Error raised for session-related issues.
+
+    This exception is raised when there are errors related to session operations
 
     """
 
 
 class NoResultsError(Exception):
     """
     Error raised when no results are found.
```

### Comparing `mongotoy-0.1.2/mongotoy/expressions.py` & `mongotoy-0.1.3/mongotoy/expressions.py`

 * *Files 14% similar despite different names*

```diff
@@ -256,57 +256,14 @@
         Returns:
             Query: The regex query expression.
         """
         return cls({str(field): {'$regex': value}})
 
 
 # noinspection PyPep8Naming
-class Join(dict[str, list[str]]):
-    """
-    Class representing a join condition for database queries.
-
-    This class provides methods to construct join conditions commonly used in database queries.
-
-    Args:
-        dict[str, list[str]]: A dictionary representing the join condition.
-
-    """
-
-    @classmethod
-    def Eq(cls, left: str, right: str) -> 'Join':
-        """
-        Constructs a join condition for equality.
-
-        Args:
-            left (str): The left side of the join condition.
-            right (str): The right side of the join condition.
-
-        Returns:
-            Join: An instance of the Join class representing the equality join condition.
-
-        """
-        return cls({'$eq': [left, right]})
-
-    @classmethod
-    def In(cls, left: str, right: str) -> 'Join':
-        """
-        Constructs a join condition for membership.
-
-        Args:
-            left (str): The left side of the join condition.
-            right (str): The right side of the join condition.
-
-        Returns:
-            Join: An instance of the Join class representing the membership join condition.
-
-        """
-        return cls({'$in': [left, right]})
-
-
-# noinspection PyPep8Naming
 def Q(**kwargs) -> Query:
     """
     Constructor function to create Query expression.
 
     Args:
         **kwargs: Keyword arguments specifying field names and operator specifications.
     """
```

### Comparing `mongotoy-0.1.2/mongotoy/fields.py` & `mongotoy-0.1.3/mongotoy/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         """
         Get the alias of the field, considering the parent's alias if present.
 
         Returns:
             str: The alias of the field.
         """
         if self._parent:
-            return f'{self._parent._alias}.{self.field.alias}'
+            return f'{self._parent._alias}.{self._field.alias}'
         return self._field.alias
 
     def __str__(self):
         """
         Returns the string representation of the field's alias.
 
         Returns:
@@ -344,14 +344,32 @@
             other: The value or field to compare.
 
         Returns:
             Query: Query object representing less-than-or-equal-to comparison.
         """
         return expressions.Query.Lte(self._alias, other)
 
+    def __pos__(self):
+        """
+        Represents ascending sort expression of the field.
+
+        Returns:
+            Sort: Sort object representing ascending sort expression.
+        """
+        return expressions.Sort.Asc(self)
+
+    def __neg__(self):
+        """
+        Represents descending sort expression of the field.
+
+        Returns:
+            Sort: Sort object representing descending sort expression.
+        """
+        return expressions.Sort.Desc(self)
+
     def __getattr__(self, item):
         """
         Allows accessing nested fields using dot notation.
 
         Args:
             item (str): The name of the nested field.
```

### Comparing `mongotoy-0.1.2/mongotoy/geodata.py` & `mongotoy-0.1.3/mongotoy/geodata.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.2/mongotoy/mappers.py` & `mongotoy-0.1.3/mongotoy/mappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import typing
 import uuid
 from types import UnionType, NoneType
 
 import bson
 
-from mongotoy import cache, expressions, references, types, geodata
+from mongotoy import cache, expressions, types, geodata
 from mongotoy.errors import ValidationError, ErrorWrapper
 
 if typing.TYPE_CHECKING:
     from mongotoy import documents, fields
 
 
 __all__ = (
@@ -359,14 +359,27 @@
         Raises:
             ValidationError: If validation fails.
 
         """
         if not isinstance(value, self.__bind__):
             raise TypeError(f'Invalid data type {type(value)}, required is {self.__bind__}')
 
+        # Validate extra options
+        if self._options.extra:
+            if 'min_items' in self._options.extra:
+                if len(value) < self._options.extra['min_items']:
+                    raise ValueError(
+                        f'Invalid value len {len(value)}, required min_items={self._options.extra["min_items"]}'
+                    )
+            if 'max_items' in self._options.extra:
+                if len(value) > self._options.extra['max_items']:
+                    raise ValueError(
+                        f'Invalid value len {len(value)}, required max_items={self._options.extra["max_items"]}'
+                    )
+
         new_value = []
         errors = []
         for i, val in enumerate(value):
             try:
                 new_value.append(self.mapper(val))
             except ValidationError as e:
                 errors.extend([ErrorWrapper(loc=(str(i),), error=j) for j in e.errors])
@@ -442,15 +455,16 @@
         """
         Get the class of the embedded document.
 
         Returns:
             Type['documents.BaseDocument']: The class of the embedded document.
 
         """
-        return references.get_embedded_document_cls(self._document_cls)
+        from mongotoy import documents
+        return documents.get_embedded_document_cls(self._document_cls)
 
     def validate(self, value) -> typing.Any:
         """
         Validate the embedded document value.
 
         Args:
             value: The value to be validated.
@@ -555,26 +569,28 @@
         """
         Get the class of the referenced document.
 
         Returns:
             Type['documents.BaseDocument']: The class of the referenced document.
 
         """
-        return references.get_document_cls(self._document_cls)
+        from mongotoy import documents
+        return documents.get_document_cls(self._document_cls)
 
     @property
     def ref_field(self) -> 'fields.Field':
         """
         Get the reference field.
 
         Returns:
             Field: The reference field.
 
         """
-        return references.get_field(self._options.ref_field, document_cls=self.document_cls)
+        from mongotoy import documents
+        return documents.get_document_field(self.document_cls, field_name=self._options.ref_field)
 
     def dump_bson(self, value, **options) -> typing.Any:
         """
         Dump the value to BSON.
 
         Args:
             value: The value to be dumped.
```

### Comparing `mongotoy-0.1.2/mongotoy/references.py` & `mongotoy-0.1.3/mongotoy/references.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,15 @@
 import typing
+
 from mongotoy import cache
-from mongotoy.expressions import Join
 
 if typing.TYPE_CHECKING:
     from mongotoy import documents, fields
 
 
-# noinspection SpellCheckingInspection
-def get_embedded_document_cls(doc_type: typing.Type | str) -> typing.Type['documents.EmbeddedDocument']:
-    """
-    Get the embedded document class based on its type or name.
-
-    Args:
-        doc_type (Type | str): The type or name of the embedded document.
-
-    Returns:
-        Type['documents.EmbeddedDocument']: The embedded document class.
-
-    Raises:
-        TypeError: If the provided type is not a subclass of mongotoy.EmbeddedDocument.
-    """
-    from mongotoy import documents
-
-    doc_cls = cache.documents.get_type(doc_type, do_raise=True)
-
-    if not issubclass(doc_cls, documents.EmbeddedDocument):
-        raise TypeError(f'Type {doc_cls} is not a mongotoy.EmbeddedDocument subclass')
-
-    return doc_cls
-
-
-# noinspection SpellCheckingInspection
-def get_document_cls(doc_type: typing.Type | str) -> typing.Type['documents.Document']:
-    """
-    Get the document class based on its type or name.
-
-    Args:
-        doc_type (Type | str): The type or name of the document.
-
-    Returns:
-        Type['documents.Document']: The document class.
-
-    Raises:
-        TypeError: If the provided type is not a subclass of mongotoy.Document.
-    """
-    from mongotoy import documents
-
-    doc_cls = cache.documents.get_type(doc_type, do_raise=True)
-
-    if not issubclass(doc_cls, documents.Document):
-        raise TypeError(f'Type {doc_cls} is not a mongotoy.Document subclass')
-
-    return doc_cls
-
-
-def get_field(field_name: str, document_cls: typing.Type['documents.BaseDocument']) -> 'fields.Field':
-    """
-    Get the field from a document class based on the field's name.
-
-    Args:
-        field_name (str): The name of the field.
-        document_cls (Type['documents.BaseDocument']): The document class containing the field.
-
-    Returns:
-        'fields.Field': The field object.
-
-    Raises:
-        TypeError: If the field does not exist in the document class.
-    """
-    field = document_cls.__fields__.get(field_name)
-
-    if not field:
-        raise TypeError(f'Field `{document_cls.__name__}.{field}` does not exist')
-
-    return field
-
-
 class Reference:
     """
     Represents a reference to another document.
 
     Args:
         document_cls (typing.Type['documents.BaseDocument'] | str): The referenced document class or its name.
         ref_field (str): The name of the field in the referenced document.
@@ -110,28 +40,30 @@
 
         Returns:
             typing.Type['documents.Document']: The referenced document class.
 
         Raises:
             TypeError: If the referenced document is not a subclass of mongotoy.Document.
         """
-        return get_document_cls(self._document_cls)
+        from mongotoy import documents
+        return documents.get_document_cls(self._document_cls)
 
     @property
     def ref_field(self) -> 'fields.Field':
         """
         Get the referenced field.
 
         Returns:
             'fields.Field': The referenced field.
 
         Raises:
             TypeError: If the referenced field does not exist.
         """
-        return get_field(self._ref_field, self.document_cls)
+        from mongotoy import documents
+        return documents.get_document_field(self.document_cls, field_name=self._ref_field)
 
     @property
     def key_name(self) -> str:
         """
         Get the key name.
 
         Returns:
@@ -162,45 +94,43 @@
     Returns:
         list[dict]: The pipeline for dereferencing.
     """
     pipeline = []
     if deep == 0:
         return pipeline
 
-    for reference in references:
-        match_exp = Join.Eq(f"${reference.ref_field.alias}", '$$fk')
-        if reference.is_many:
-            match_exp = Join.In(f"${reference.ref_field.alias}", '$$fk')
-
+    for ref in references:
         pipeline.append(
             {
                 "$lookup": {
-                    'from': reference.document_cls.__collection_name__,
-                    'let': {"fk": f"${reference.key_name}"},
+                    'from': ref.document_cls.__collection_name__,
+                    'let': {"fk": f"${ref.key_name}"},
                     'pipeline': [
                         {
                             "$match": {
-                                "$expr": match_exp
+                                "$expr": {
+                                    '$in' if ref.is_many else '$eq': [f"${ref.ref_field.alias}", '$$fk']
+                                }
                             }
                         },
                         *build_dereference_pipeline(
-                            reference.document_cls.__references__.values(),
+                            ref.document_cls.__references__.values(),
                             deep=deep - 1
                         ),
-                        *([{'$limit': 1}] if not reference.is_many else [])
+                        *([] if ref.is_many else [{'$limit': 1}])
                     ],
-                    'as': reference._name
+                    'as': ref._name
                 }
             }
         )
-        if not reference.is_many:
+        if not ref.is_many:
             pipeline.append(
                 {
                     "$unwind": {
-                        "path": f"${reference._name}",
+                        "path": f"${ref._name}",
                         "preserveNullAndEmptyArrays": True
                     }
                 }
             )
 
     return pipeline
```

### Comparing `mongotoy-0.1.2/mongotoy/types.py` & `mongotoy-0.1.3/mongotoy/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 import collections
 import datetime
+import os
 import re
 import typing
 
 import bson
-from motor.motor_asyncio import AsyncIOMotorGridOut
 
 from mongotoy import geodata
 
 if typing.TYPE_CHECKING:
     from mongotoy import db
 
 
@@ -352,17 +351,66 @@
     """
     id: bson.ObjectId
     filename: str
     metadata: Json
     chunk_size: int
     length: int
     upload_date: datetime.datetime
+    content_type: str
+    chunks: int
+
+    def create_revision(
+        self,
+        fs: 'db.FsBucket',
+        src: typing.IO | bytes,
+        metadata: dict = None
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, 'File'], 'File']:
+        pass
+
+    # noinspection SpellCheckingInspection
+    def download(
+        self,
+        fs: 'db.FsBucket',
+        dest: typing.IO,
+        revision: int = None
+    ) -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        pass
+
+    def stream(
+        self,
+        fs: 'db.FsBucket',
+        revision: int = None
+    ) -> typing.Union[typing.Coroutine[typing.Any, typing.Any, '_FileOut'], '_FileOut']:
+        pass
+
+    def delete(self, fs: 'db.FsBucket') -> typing.Coroutine[typing.Any, typing.Any, None] | None:
+        pass
+
+
+class _FileOut(typing.Protocol):
+    # noinspection SpellCheckingInspection
+    """
+    This is a facade for type mogotoy.db.FsOutput
+    """
+
+    def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
+        pass
+
+    def seekable(self) -> bool:
+        pass
+
+    def tell(self) -> int:
+        pass
 
-    async def create_revision(self, fs: 'db.FsBucket', src: typing.IO | bytes, metadata: dict = None):
+    def close(self):
+        pass
+
+    def read(self, size: int = -1) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
         pass
 
     # noinspection SpellCheckingInspection
-    async def download(self, fs: 'db.FsBucket', dest: typing.IO, revision: int = None):
+    def readchunk(self) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
         pass
 
-    async def stream(self, fs: 'db.FsBucket', revision: int = None) -> AsyncIOMotorGridOut:
+    def readline(self, size: int = -1) -> typing.Coroutine[typing.Any, typing.Any, bytes] | bytes:
         pass
+
```

### Comparing `mongotoy-0.1.2/pyproject.toml` & `mongotoy-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongotoy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Async ODM for MongoDB"
 license = "Apache-2.0"
 authors = ["gurcuff91 <gf.meneses91@gmail.com>"]
 readme = "README.md"
 homepage = "https://gurcuff91.github.io/mongotoy"
 repository = "https://github.com/gurcuff91/mongotoy"
 keywords = ["mapping", "asyncio", "odm", "mongodb"]
```

### Comparing `mongotoy-0.1.2/README.md` & `mongotoy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.2/PKG-INFO` & `mongotoy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongotoy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async ODM for MongoDB
 Home-page: https://gurcuff91.github.io/mongotoy
 License: Apache-2.0
 Keywords: mapping,asyncio,odm,mongodb
 Author: gurcuff91
 Author-email: gf.meneses91@gmail.com
 Requires-Python: >=3.11,<4.0
```

