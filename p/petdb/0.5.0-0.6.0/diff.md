# Comparing `tmp/petdb-0.5.0.tar.gz` & `tmp/petdb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petdb-0.5.0.tar", last modified: Sat Mar  9 13:14:41 2024, max compression
+gzip compressed data, was "petdb-0.6.0.tar", last modified: Sun Apr  7 14:52:44 2024, max compression
```

## Comparing `petdb-0.5.0.tar` & `petdb-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-09 13:14:41.783148 petdb-0.5.0/
--rw-r--r--   0 maks       (501) staff       (20)     1063 2024-02-02 15:52:27.000000 petdb-0.5.0/LICENSE
--rw-r--r--   0 maks       (501) staff       (20)     3375 2024-03-09 13:14:41.782947 petdb-0.5.0/PKG-INFO
--rw-r--r--   0 maks       (501) staff       (20)     2925 2024-03-07 17:28:56.000000 petdb-0.5.0/README.md
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-09 13:14:41.781814 petdb-0.5.0/petdb/
--rw-r--r--   0 maks       (501) staff       (20)      284 2024-02-03 08:22:10.000000 petdb-0.5.0/petdb/__init__.py
--rw-r--r--   0 maks       (501) staff       (20)    16759 2024-03-09 13:03:47.000000 petdb-0.5.0/petdb/pcollection.py
--rw-r--r--   0 maks       (501) staff       (20)     2968 2024-01-30 18:36:49.000000 petdb-0.5.0/petdb/pdb.py
--rw-r--r--   0 maks       (501) staff       (20)       78 2024-02-03 17:34:13.000000 petdb-0.5.0/petdb/pexceptions.py
--rw-r--r--   0 maks       (501) staff       (20)    10246 2024-02-11 15:12:23.000000 petdb-0.5.0/petdb/putils.py
-drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-03-09 13:14:41.782738 petdb-0.5.0/petdb.egg-info/
--rw-r--r--   0 maks       (501) staff       (20)     3375 2024-03-09 13:14:41.000000 petdb-0.5.0/petdb.egg-info/PKG-INFO
--rw-r--r--   0 maks       (501) staff       (20)      237 2024-03-09 13:14:41.000000 petdb-0.5.0/petdb.egg-info/SOURCES.txt
--rw-r--r--   0 maks       (501) staff       (20)        1 2024-03-09 13:14:41.000000 petdb-0.5.0/petdb.egg-info/dependency_links.txt
--rw-r--r--   0 maks       (501) staff       (20)        6 2024-03-09 13:14:41.000000 petdb-0.5.0/petdb.egg-info/top_level.txt
--rw-r--r--   0 maks       (501) staff       (20)      570 2024-03-09 13:14:31.000000 petdb-0.5.0/pyproject.toml
--rw-r--r--   0 maks       (501) staff       (20)       38 2024-03-09 13:14:41.783189 petdb-0.5.0/setup.cfg
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-07 14:52:44.831863 petdb-0.6.0/
+-rw-r--r--   0 maks       (501) staff       (20)     1063 2024-02-02 15:52:27.000000 petdb-0.6.0/LICENSE
+-rw-r--r--   0 maks       (501) staff       (20)     3380 2024-04-07 14:52:44.831668 petdb-0.6.0/PKG-INFO
+-rw-r--r--   0 maks       (501) staff       (20)     2930 2024-04-07 14:51:18.000000 petdb-0.6.0/README.md
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-07 14:52:44.830658 petdb-0.6.0/petdb/
+-rw-r--r--   0 maks       (501) staff       (20)      284 2024-02-03 08:22:10.000000 petdb-0.6.0/petdb/__init__.py
+-rw-r--r--   0 maks       (501) staff       (20)    17227 2024-04-07 13:50:26.000000 petdb-0.6.0/petdb/pcollection.py
+-rw-r--r--   0 maks       (501) staff       (20)     3343 2024-04-07 13:50:26.000000 petdb-0.6.0/petdb/pdb.py
+-rw-r--r--   0 maks       (501) staff       (20)       78 2024-02-03 17:34:13.000000 petdb-0.6.0/petdb/pexceptions.py
+-rw-r--r--   0 maks       (501) staff       (20)    10246 2024-02-11 15:12:23.000000 petdb-0.6.0/petdb/putils.py
+drwxr-xr-x   0 maks       (501) staff       (20)        0 2024-04-07 14:52:44.831500 petdb-0.6.0/petdb.egg-info/
+-rw-r--r--   0 maks       (501) staff       (20)     3380 2024-04-07 14:52:44.000000 petdb-0.6.0/petdb.egg-info/PKG-INFO
+-rw-r--r--   0 maks       (501) staff       (20)      237 2024-04-07 14:52:44.000000 petdb-0.6.0/petdb.egg-info/SOURCES.txt
+-rw-r--r--   0 maks       (501) staff       (20)        1 2024-04-07 14:52:44.000000 petdb-0.6.0/petdb.egg-info/dependency_links.txt
+-rw-r--r--   0 maks       (501) staff       (20)        6 2024-04-07 14:52:44.000000 petdb-0.6.0/petdb.egg-info/top_level.txt
+-rw-r--r--   0 maks       (501) staff       (20)      570 2024-04-07 14:51:39.000000 petdb-0.6.0/pyproject.toml
+-rw-r--r--   0 maks       (501) staff       (20)       38 2024-04-07 14:52:44.831898 petdb-0.6.0/setup.cfg
```

### Comparing `petdb-0.5.0/LICENSE` & `petdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `petdb-0.5.0/PKG-INFO` & `petdb-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: Light weight local document-oriented database
 Author-email: Maks Vinnytskyi <ownerofforest@gmail.com>
 Project-URL: Homepage, https://gitlab.com/Tullp/petdb
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
@@ -40,22 +40,22 @@
 
 ## Dependencies
 
 PetDB was created as a lightweight package, so there are no dependencies.
 
 ## Usage
 
-To use this database you should only import PetDB and create an instance.
+To use this database you should only import PetDB and get an instance.
 By default, it will create folder for storing collections in the current directory,
 but you can provide any path:
 
 ```python
 from petdb import PetDB
 
-db = PetDB(os.path.join(os.getcwd(), "persistent", "storage"))
+db = PetDB.get(os.path.join(os.getcwd(), "persistent", "storage"))
 ```
 
 Next you should select the collection, if it doesn't exist, it will created automatically.
 You can do it just by attribute access, by index key or use a method (it will create a new one if it doesn't exist):
 
 ```python
 users = db.users
@@ -63,15 +63,15 @@
 payments = db.collection("payments")
 ```
 
 ## Examples
 
 ```pycon
 >>> from petdb import PetDB
->>> db = PetDB()
+>>> db = PetDB.get()
 >>> users = db["users"]
 >>> users.insert_many([
 ...     {"name": "John", "age": 28, "subscriptions": ["tv", "cloud"]},
 ...     {"name": "Michael", "age": 32, "subscriptions": ["tv"]},
 ...     {"name": "Sam", "age": 18, "subscriptions": ["music", "cloud"]},
 ...     {"name": "Alex", "age": 24, "subscriptions": ["tv", "music"]},
 ...     {"name": "Bob", "age": 18, "subscriptions": ["music"]},
```

### Comparing `petdb-0.5.0/README.md` & `petdb-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 ## Dependencies
 
 PetDB was created as a lightweight package, so there are no dependencies.
 
 ## Usage
 
-To use this database you should only import PetDB and create an instance.
+To use this database you should only import PetDB and get an instance.
 By default, it will create folder for storing collections in the current directory,
 but you can provide any path:
 
 ```python
 from petdb import PetDB
 
-db = PetDB(os.path.join(os.getcwd(), "persistent", "storage"))
+db = PetDB.get(os.path.join(os.getcwd(), "persistent", "storage"))
 ```
 
 Next you should select the collection, if it doesn't exist, it will created automatically.
 You can do it just by attribute access, by index key or use a method (it will create a new one if it doesn't exist):
 
 ```python
 users = db.users
@@ -50,15 +50,15 @@
 payments = db.collection("payments")
 ```
 
 ## Examples
 
 ```pycon
 >>> from petdb import PetDB
->>> db = PetDB()
+>>> db = PetDB.get()
 >>> users = db["users"]
 >>> users.insert_many([
 ...     {"name": "John", "age": 28, "subscriptions": ["tv", "cloud"]},
 ...     {"name": "Michael", "age": 32, "subscriptions": ["tv"]},
 ...     {"name": "Sam", "age": 18, "subscriptions": ["music", "cloud"]},
 ...     {"name": "Alex", "age": 24, "subscriptions": ["tv", "music"]},
 ...     {"name": "Bob", "age": 18, "subscriptions": ["music"]},
```

### Comparing `petdb-0.5.0/petdb/pcollection.py` & `petdb-0.6.0/petdb/pcollection.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,15 +305,30 @@
 	Represents a single PetDB collection.
 	It provides methods for accessing, managing and manipulating documents.
 
 	:param path: Path to the json file where collection's documents are stored.
 				It also used to specify the name of the collection.
 	"""
 
+	__instances = {}
+
+	@classmethod
+	def get_instance(cls, path: str) -> PetCollection:
+		if path not in cls.__instances:
+			cls.__instances[path] = PetCollection(path)
+		return cls.__instances[path]
+
+	@classmethod
+	def instances(cls) -> dict[str, PetCollection]:
+		return cls.__instances
+
 	def __init__(self, path: str):
+		if path in self.__class__.__instances:
+			raise Exception("This class is a singleton. Please use PetCollection.get_instance() instead.")
+		self.__class__.__instances[path] = self
 		self.__path = path
 		self.name = os.path.basename(path).rsplit(".", 1)[0]
 		if os.path.exists(self.__path):
 			with open(self.__path, "r", encoding="utf-8") as f:
 				super().__init__(json.load(f))
 		else: super().__init__([])
```

### Comparing `petdb-0.5.0/petdb/pdb.py` & `petdb-0.6.0/petdb/pdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,64 +12,78 @@
 	Collections access is provided by forwarding all unknown method calls
 	and property access operations to the :py:meth:`PetDB.collection` method
 	by implementing :py:meth:`PetDB.__getattr__` and :py:meth:`PetDB.__getitem__`.
 
 	:param root: The root path where the folder for storing will be created
 	"""
 
+	__instance = None
+
+	@classmethod
+	def get(cls, root: str = None):
+		if cls.__instance is None:
+			cls.__instance = PetDB(root)
+		return cls.__instance
+
 	def __init__(self, root: str = None):
+		if self.__class__.__instance is not None:
+			raise Exception("This class is a singleton. Please use PetDB.get() instead.")
+		self.__class__.__instance = self
 		if root is None:
 			root = os.getcwd()
 		if not os.path.exists(root):
 			raise Exception("Root directory does not exist")
 		self.__root = os.path.join(root, "petstorage")
 		if not os.path.exists(self.__root):
 			os.mkdir(self.__root)
-		self.__collections: dict[str, PetCollection] = {}
 		self.__load_collections()
 
+	def __getpath(self, name: str):
+		return os.path.join(self.__root, f"{name}.json")
+
 	def collection(self, name: str) -> PetCollection:
 		"""
 		Get access to the specific collection with the given name.
 
 		If the collection hasn't been accessed yet, a new collection instance will be
 		created. Otherwise, the previously created collection instance will be returned.
 
 		:param name: The name of the collection.
 		:return: :py:class:`PetCollection`
 		"""
-		if name not in self.__collections:
-			return self.__create_collection(name)
-		return self.__collections[name]
+		return PetCollection.get_instance(self.__getpath(name))
 
 	def collections(self) -> list[str]:
 		"""
 		Get the names of all collections in the database.
 
 		:returns: a list of collections names
 		"""
-		return list(self.__collections.keys())
+		return [os.path.basename(path).rsplit(".", 1)[0] for path in PetCollection.instances().keys()]
 
 	def drop_collection(self, name: str):
 		"""
 		Deletes the collection with the given name
 
 		:param name: The name of the collection to delete
 		"""
-		if name in self.__collections:
-			self.__collections[name].clear()
-			self.__collections.pop(name)
-			os.remove(os.path.join(self.__root, f"{name}.json"))
+		if self.__getpath(name) in PetCollection.instances():
+			col = PetCollection.get_instance(self.__getpath(name))
+			col.clear()
+			os.remove(self.__getpath(name))
+			PetCollection.instances().pop(self.__getpath(name))
 
 	def drop(self) -> None:
 		"""
 		Drop all collections from the database. **CANNOT BE REVERSED!**
 		"""
-		for name in self.__collections:
-			self.drop_collection(name)
+		for col in self:
+			col.clear()
+			os.remove(self.__getpath(col.name))
+		PetCollection.instances().clear()
 
 	def __getattr__(self, name: str) -> PetCollection:
 		"""
 		Alias for :py:meth:`PetDB.collection`
 
 		:return: :py:class:`PetCollection`
 		"""
@@ -85,18 +99,17 @@
 			raise TypeError("Name must be a string")
 		return self.collection(name)
 
 	def __load_collections(self):
 		for file in os.listdir(self.__root):
 			if not file.endswith(".json"):
 				continue
-			self.__collections[file.rsplit(".", 1)[0]] = PetCollection(os.path.join(self.__root, file))
+			PetCollection.get_instance(os.path.join(self.__root, file))
 
 	def __create_collection(self, name: str):
-		self.__collections[name] = PetCollection(os.path.join(self.__root, f"{name}.json"))
-		return self.__collections[name]
+		return PetCollection.get_instance(self.__getpath(name))
 
 	def __len__(self):
-		return len(self.__collections)
+		return len(PetCollection.instances())
 
 	def __iter__(self) -> Iterator[PetCollection]:
-		return iter(self.__collections.values())
+		return iter(PetCollection.instances().values())
```

### Comparing `petdb-0.5.0/petdb/putils.py` & `petdb-0.6.0/petdb/putils.py`

 * *Files identical despite different names*

### Comparing `petdb-0.5.0/petdb.egg-info/PKG-INFO` & `petdb-0.6.0/petdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: Light weight local document-oriented database
 Author-email: Maks Vinnytskyi <ownerofforest@gmail.com>
 Project-URL: Homepage, https://gitlab.com/Tullp/petdb
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
@@ -40,22 +40,22 @@
 
 ## Dependencies
 
 PetDB was created as a lightweight package, so there are no dependencies.
 
 ## Usage
 
-To use this database you should only import PetDB and create an instance.
+To use this database you should only import PetDB and get an instance.
 By default, it will create folder for storing collections in the current directory,
 but you can provide any path:
 
 ```python
 from petdb import PetDB
 
-db = PetDB(os.path.join(os.getcwd(), "persistent", "storage"))
+db = PetDB.get(os.path.join(os.getcwd(), "persistent", "storage"))
 ```
 
 Next you should select the collection, if it doesn't exist, it will created automatically.
 You can do it just by attribute access, by index key or use a method (it will create a new one if it doesn't exist):
 
 ```python
 users = db.users
@@ -63,15 +63,15 @@
 payments = db.collection("payments")
 ```
 
 ## Examples
 
 ```pycon
 >>> from petdb import PetDB
->>> db = PetDB()
+>>> db = PetDB.get()
 >>> users = db["users"]
 >>> users.insert_many([
 ...     {"name": "John", "age": 28, "subscriptions": ["tv", "cloud"]},
 ...     {"name": "Michael", "age": 32, "subscriptions": ["tv"]},
 ...     {"name": "Sam", "age": 18, "subscriptions": ["music", "cloud"]},
 ...     {"name": "Alex", "age": 24, "subscriptions": ["tv", "music"]},
 ...     {"name": "Bob", "age": 18, "subscriptions": ["music"]},
```

### Comparing `petdb-0.5.0/pyproject.toml` & `petdb-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "petdb"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
     { name = "Maks Vinnytskyi", email = "ownerofforest@gmail.com" },
 ]
 description = "Light weight local document-oriented database"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

