# Comparing `tmp/alchemyrohan-0.4.0.tar.gz` & `tmp/alchemyrohan-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemyrohan-0.4.0.tar", last modified: Sun Mar 17 14:21:09 2024, max compression
+gzip compressed data, was "alchemyrohan-0.4.1.tar", last modified: Sat Apr  6 23:43:49 2024, max compression
```

## Comparing `alchemyrohan-0.4.0.tar` & `alchemyrohan-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxrwxr-x   0 ansgar    (1000) ansgar    (1000)        0 2024-03-17 14:21:09.460939 alchemyrohan-0.4.0/
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     1070 2023-12-10 23:28:42.000000 alchemyrohan-0.4.0/LICENSE
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)       71 2023-12-11 21:27:42.000000 alchemyrohan-0.4.0/MANIFEST.in
--rw-rw-r--   0 ansgar    (1000) ansgar    (1000)     8032 2024-03-17 14:21:09.456939 alchemyrohan-0.4.0/PKG-INFO
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     7248 2024-03-17 13:02:41.000000 alchemyrohan-0.4.0/README.md
--rw-rw-r--   0 ansgar    (1000) ansgar    (1000)    13793 2023-12-10 23:50:22.000000 alchemyrohan-0.4.0/THIRD_PARTY_LICENSES
-drwxrwxr-x   0 ansgar    (1000) ansgar    (1000)        0 2024-03-17 14:21:09.456939 alchemyrohan-0.4.0/alchemyrohan/
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)      520 2024-03-17 12:36:49.000000 alchemyrohan-0.4.0/alchemyrohan/__init__.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     2056 2024-03-17 12:40:58.000000 alchemyrohan-0.4.0/alchemyrohan/assemble.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     2161 2023-11-12 15:01:20.000000 alchemyrohan-0.4.0/alchemyrohan/meta_data.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)    12010 2023-12-05 12:07:46.000000 alchemyrohan-0.4.0/alchemyrohan/oracle.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     6102 2023-12-03 12:44:16.000000 alchemyrohan-0.4.0/alchemyrohan/sqlite.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     1984 2024-03-17 12:07:09.000000 alchemyrohan-0.4.0/alchemyrohan/utils.py
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     3594 2024-03-17 13:05:04.000000 alchemyrohan-0.4.0/alchemyrohan/wizard.py
-drwxrwxr-x   0 ansgar    (1000) ansgar    (1000)        0 2024-03-17 14:21:09.456939 alchemyrohan-0.4.0/alchemyrohan.egg-info/
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     8032 2024-03-17 14:21:09.000000 alchemyrohan-0.4.0/alchemyrohan.egg-info/PKG-INFO
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)      422 2024-03-17 14:21:09.000000 alchemyrohan-0.4.0/alchemyrohan.egg-info/SOURCES.txt
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)        1 2024-03-17 14:21:09.000000 alchemyrohan-0.4.0/alchemyrohan.egg-info/dependency_links.txt
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)       20 2024-03-17 14:21:09.000000 alchemyrohan-0.4.0/alchemyrohan.egg-info/requires.txt
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)       13 2024-03-17 14:21:09.000000 alchemyrohan-0.4.0/alchemyrohan.egg-info/top_level.txt
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)       43 2023-12-10 11:27:43.000000 alchemyrohan-0.4.0/requirements.txt
--rw-rw-r--   0 ansgar    (1000) ansgar    (1000)       38 2024-03-17 14:21:09.460939 alchemyrohan-0.4.0/setup.cfg
--rw-r--r--   0 ansgar    (1000) ansgar    (1000)     1246 2024-03-17 14:20:46.000000 alchemyrohan-0.4.0/setup.py
+-rw-r--r--   0        0        0     1072 2024-04-06 22:32:25.970943 alchemyrohan-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8162 2024-04-06 22:50:20.304616 alchemyrohan-0.4.1/README.md
+-rw-r--r--   0        0        0      544 2024-04-06 19:42:52.600887 alchemyrohan-0.4.1/alchemyrohan/__init__.py
+-rw-r--r--   0        0        0     3657 2024-04-06 21:41:58.511304 alchemyrohan-0.4.1/alchemyrohan/assemble.py
+-rw-r--r--   0        0        0     1827 2024-04-06 17:10:13.922941 alchemyrohan-0.4.1/alchemyrohan/meta_data.py
+-rw-r--r--   0        0        0    11892 2024-04-06 18:11:50.397318 alchemyrohan-0.4.1/alchemyrohan/oracle.py
+-rw-r--r--   0        0        0     6363 2024-04-06 21:03:25.098470 alchemyrohan-0.4.1/alchemyrohan/sqlite.py
+-rw-r--r--   0        0        0     1347 2024-04-06 19:57:00.571350 alchemyrohan-0.4.1/alchemyrohan/utils.py
+-rw-r--r--   0        0        0     3121 2024-04-06 21:03:25.106470 alchemyrohan-0.4.1/alchemyrohan/wizard.py
+-rw-r--r--   0        0        0     1207 2024-04-06 23:43:49.538745 alchemyrohan-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      851 2024-04-06 19:40:24.036004 alchemyrohan-0.4.1/tests/test_assemble.py
+-rw-r--r--   0        0        0      849 2024-04-06 19:30:43.716526 alchemyrohan-0.4.1/tests/test_assemble_error.py
+-rw-r--r--   0        0        0      799 2024-04-06 21:07:54.138880 alchemyrohan-0.4.1/tests/test_model.py
+-rw-r--r--   0        0        0     1762 2024-04-06 22:39:59.764928 alchemyrohan-0.4.1/tests/test_models/Child.py
+-rw-r--r--   0        0        0     1996 2024-04-06 22:39:59.764928 alchemyrohan-0.4.1/tests/test_models/Parent.py
+-rw-r--r--   0        0        0      159 2024-04-06 22:40:08.868807 alchemyrohan-0.4.1/tests/test_models/__init__.py
+-rw-r--r--   0        0        0      578 2024-04-05 22:58:43.923181 alchemyrohan-0.4.1/tests/test_sqlite/crt_test_db.py
+-rwxr-xr-x   0        0        0  3694080 2023-11-07 20:23:52.000000 alchemyrohan-0.4.1/tests/test_sqlite/sqlite3.exe
+-rw-r--r--   0        0        0    12288 2023-11-12 01:49:40.000000 alchemyrohan-0.4.1/tests/test_sqlite/test.db
+-rw-r--r--   0        0        0    10415 1970-01-01 00:00:00.000000 alchemyrohan-0.4.1/PKG-INFO
```

### Comparing `alchemyrohan-0.4.0/LICENSE` & `alchemyrohan-0.4.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 MIT License
 
 Copyright (c) 2023 Alan Wamberger
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `alchemyrohan-0.4.0/PKG-INFO` & `alchemyrohan-0.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,31 @@
-Metadata-Version: 2.1
-Name: alchemyrohan
-Version: 0.4.0
-Summary: An extension package for SqlAlchemy which automatically creates the database models
-Home-page: https://github.com/wamberger/alchemyrohan
-Author: Alan Wamberger
-Author-email: awamberger@proton.me
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 
 # Alchemyrohan
 
- ![pypi v22.0.3](https://img.shields.io/badge/pypi-v22.0.3-yellow) ![Python 3.9 | 3.10 | 3.11](https://img.shields.io/badge/python-3.9_|_3.10_|_3.11-blue) ![SqlAlchemy](https://img.shields.io/badge/SqlAlchemy-2.0-red)
+ ![pypi v23.x](https://img.shields.io/badge/pypi-v23.x-yellow) ![Python 3.12](https://img.shields.io/badge/python-3.12-blue) ![SqlAlchemy](https://img.shields.io/badge/SqlAlchemy-2.0-red)
 
 
-Alchemyrohan is a tool for **[SqlAlchemy](https://www.sqlalchemy.org/)** that helps to create database models based on the database schema.
+Alchemyrohan is a helpful tool for creating **[SqlAlchemy](https://www.sqlalchemy.org/)** models 
+based on the database schema.
 
 ---
 
 ## 📖 Content
 
 - [How to Install](#-How-to-Install)
 - [Database Support](#-Database-Support)
 - [How to use](#-How-to-use)
-  - [Functions](#-Functions)
-    - [Main Function](#-Main-Function)
-    - [Optional Functions](#-Optional-Functions)
-  - [Models](#-Models)
-- [Example](#-Example)
+  - [In Command-Line](#-In-Command-Line)
+  - [As Script](#-As-Script)
+    - [Functions](#-Functions)
+      - [Main Function](#-Main-Function)
+      - [Optional Function](#-Optional-Function)
+- [Models](#-Models)
 - [Dependencies](#-Dependencies)
 - [Important Note](#Important-Note)
 - [Release Notes](#-Release-Notes)
 - [License](#-License-and-Third-Party-Licenses)
 
 ---
 
@@ -56,211 +37,243 @@
 ```
 pip install alchemyrohan
 ```
 
 or from source:
 
 ```
-git clone --recursive https://github.com/wamberger/alchemyrohan.git
-cd alchemyrohan
-python3 setup.py install
+pip install pdm
+git clone https://github.com/wamberger/alchemyrohan.git
+pdm install
 ```
 
 
 ## 🗄 Database Support
 
 This project is currently designed to work with the following databases:
 
 - **SqLite**
 - **Oracle**
 
 
 ## 🔨 How to use
 
-Import in your code:
+### ⌨️ In Command-Line
 
-`import alchemyrohan` 
+You can execute the tool by entering the following command along with its arguments:
 
-or 
+> arohan -c sqlite:///path/to/database/test.db -y tests.test_models -p /path/to/save/models/ -m table1 table2 table3
 
-`import alchemyrohan as ar`
+Arguments:
 
+        -c, --conn_str:
+            Connection string to connect with the database.
+            Required argument. Accepts a string.
 
-### 🪄 Functions
+        -p, --path:
+            Path where to save the models.
+            Optional argument. Defaults to the current working directory.
+            Accepts a string.
 
-#### 🔮 Main Function
+        -y, --py_path:
+            Pythonic path to models in the project.
+            Optional argument. Defaults to 'py_path'.
+            Accepts a string.
 
-- **assemble_models()** is the main function. This function is used to create a SqlAlchemy database model and is accepting the following arguments:
-    | argument | description |
-    | --------- | --------- |
-    | *db_creds* | Credential string to connect to the database |
-    | *table_names* | Names of the tables |
-    | *abs_path_to_models* | Absolute path to the location where the created models will be saved |
-    | *py_path_to_model* | pythonic path to the models |
+        -m, --models:
+            Names of the database tables.
+            Required argument. Accepts one or more strings.
 
+        --verbose:
+            Enables verbose mode.
+            Optional argument. Activates verbose mode if provided.
+            Does not require any additional argument value.
 
-#### 💉 Optional Functions
 
-- **is_model():** This function is used to check if the model exists. You need to pass the *table_name* and *abs_path_to_model* arguments.
+### 💻 As Script 
 
-- **get_model():** It retrieves the desired database object of the SqlAlchemy model. It requires the *table_name* and *py_path_to_model* arguments.
+You can find an example script in the directory *help_file/*.
 
-- **is_module():** This function is used to check the Pythonic path. It requires the *py_path_to_model* argument.
+#### 🪄 Functions
 
-- **reload_module():** If you have a specific reason for using the code in production or creating models in a running script, you may need to compile the newly created code. In such cases, you will need to use this function. Here's how you do it:
+##### 🔮 Main Function
 
-    ~~~python
-    import tests.test_models
+**assemble_models()** is the main function. This function is used to create a 
+SqlAlchemy database model and is accepting the following arguments:
+ 
+| argument      | description |
+|---------------| --------- |
+| *conn_str*    | Credential string to connect to the database |
+| *table_names* | Names of the tables |
+| *path*        | Absolute path to the location where the created models will be saved |
+| *py_path*     | pythonic path to the models |
 
-    ...some code...
+**Simple example how to use the function *assemble_models()*:**
 
-    reload_module(tests.test_models)
-    ~~~
+~~~python
 
-### 🗂 Models
 
-Created SqlAlchemy models have some additional features:
+import os
 
-- Default values.
-- Parent-child relationships.
-- The *_post_init_* method is used for validation.
-- When 'printing', the string will contain the model/object name and attribute names with their values.
+from sqlalchemy.exc import SQLAlchemyError
+from alchemyrohan import assemble_models
 
-All models are named with the same convention as they are in the database, with one difference: they are capitalized according to Python class naming conventions.
 
+def main():
 
-## 📝 Example
+    path = os.path.dirname(__file__)
 
-**Simple example how to use the code:**
+    # Sqlite example
+    conn_str = f"sqlite:///{path}{os.sep}test_sqlite{os.sep}test.db"
+    # Oracle-Database example
+    # db_creds = f'oracle+oracledb://{username}:{password}@{hostname}:{port}/{service_name}'
 
-~~~python
+    path = os.path.join(path, 'test_models') # path to save models
+    py_path = 'tests.test_models' # pythonic path to models
 
-import os
+    table_names = ['parent', 'child'] # all names will be capitilized
+
+    try:
+        assemble_models(conn_str, table_names, path,py_path)
+    except SQLAlchemyError as e:
+        raise SQLAlchemyError(e) from e
 
-from alchemyrohan.assemble import assemble_models
 
-dir = os.path.dirname(__file__)
+if __name__ == '__main__':
+    main()
 
-# Sqlite example
-db_creds = f"sqlite:///{dir}{os.sep}test_sqlite{os.sep}test.db"
-# Oracle-Database example
-#db_creds = f'oracle+cx_oracle://{username}:{password}@{hostname}:{port}/{service_name}'
-
-abs_os_path_to_model = os.path.join(dir, 'test_models') # path to save models
-py_path_to_model = 'tests.test_models' # pythonic path to models
-table_names = ['parent', 'child'] # all names will be capitilized
-
-try:
-    assemble_models(
-        db_creds, 
-        table_names, 
-        abs_path_to_models,
-        py_path_to_model
-        )
-    exit(0)
-except Exception as e:
-    print(e)
-    exit(1)
 
 ~~~
 
+##### 💉 Optional Function
+
+**get_model():** It retrieves the desired database object of the SqlAlchemy model. It requires the *table_name* and *py_path_to_model* arguments.
+
+~~~python
+
+from alchemyrohan import get_model
+
+~~~
+
+## 🗂 Models
+
+Created SqlAlchemy models have some additional features:
+
+- Default values.
+- Parent-child relationships.
+- The *validate* method is used for validation.
+- When 'printing', the string will contain the model/object name and attribute names with their values.
+
+All models are named with the same convention as they are in the database, with one difference: they are capitalized according to Python class naming conventions.
+
+
 **Example of one created model**:
 
 ~~~python
 
+
 from sqlalchemy import Column
 from tests.test_models import Base
+from sqlalchemy import ForeignKey
 from sqlalchemy.dialects.sqlite import INTEGER
 from sqlalchemy.dialects.sqlite import TEXT
 from sqlalchemy.orm import relationship
 
 
 class Child(Base):
     __tablename__ = 'child'
 
 
     id = Column(INTEGER, primary_key=True)
-    parent_id = Column(INTEGER, nullable=True, default=None)
+    parent_id = Column(INTEGER, ForeignKey('parent.id'), nullable=True, default=None)
     name = Column(TEXT, nullable=True, default=None)
     grade = Column(INTEGER, nullable=True, default=None)
 
 
     parent_Parent = relationship("Parent", back_populates="children_Child", lazy="joined")
 
-    def __post_init__(self):
+    def validate(self):
 
-        if not isinstance(self.id, int):
+        if self.id and not isinstance(self.id, int):
             try:
                 self.id = int(self.id)
             except:
                 raise SyntaxError(f'< {self.id} > is not integer')
         
-        if not isinstance(self.parent_id, int):
+        if self.parent_id and not isinstance(self.parent_id, int):
             try:
                 self.parent_id = int(self.parent_id)
             except:
                 raise SyntaxError(f'< {self.parent_id} > is not integer')
         
-        if not isinstance(self.name, str):
+        if self.name and not isinstance(self.name, str):
             try:
                 self.name = str(self.name)
             except:
                 raise SyntaxError(f'< {self.name} > is not string')
         
-        if not isinstance(self.grade, int):
+        if self.grade and not isinstance(self.grade, int):
             try:
                 self.grade = int(self.grade)
             except:
                 raise SyntaxError(f'< {self.grade} > is not integer')
         
     
     def __str__(self):
 
         return f'User(id={self.id},'\
 			f'parent_id={self.parent_id},'\
 			f'name={self.name},'\
 			f'grade={self.grade})'
 
+
 ~~~ 
 
 
 ## 📚 Dependencies
 
-- **sqlalchemy** (version 2.0.x) is an ORM and provides code for its models.
-- **oracledb** (version 1.4.x) is used to shape a database table model with an Oracle table schema.
+- **sqlalchemy** (version 2.x.x) is an ORM and provides code for its models.
+- **oracledb** (version 2.x.x) is used to shape a database table model with an Oracle table schema.
 
 
 ## ❗Important Note
 
-In most cases, you will need to correct the code manually. 
-This will be the case when:
+You should always check the code and correct it manually if necessary. 
+This may be necessary in cases when:
 
-- You are not adding a Pythonic path.
+- You add the wrong path.
 
-- You are creating only one model which has relationships to other tables, thus you will need to create those models or delete the relevant part of the code.
+- You are creating only one model which has relationships to other tables, 
+ thus you will need to create those models or delete the relevant part of the code.
 
 - Your tables have no primary keys. SQLAlchemy requires at least one primary key.
 
-- Your database may have some data types or features which have not yet been tested.
+- Your database may have some data types or features which have not yet been tested - Please report!
 
 
 ## 📋 Release Notes
 
+- ***v0.4.1*** - Some vital changes! Please look at CHANGELOG.md. In short:
+  - New command-line: *arohan*.
+  - Removed functions: *is_model()*, *reload_module()*, *is_module()*.
+  - Changing parameter names in the function *assemble_models()*.
+  - Bug fixing (*relationship*).
+  - In models, method *validate*.
 
-- ***v0.1.0*** - creation of the initial code and tested with SqLite database
-- ***v0.2.0*** - tested with Oracle database
-- ***v0.3.0*** - added additional functions
-- ***v0.3.1*** - bug fixing
-- ***v0.3.2*** - text fixing and adding third party licenses
 - ***v0.4.0*** - Main update! Not compatible with previous versions. Changes:
-    - Changed function name from *assemble_model()* to *assemble_models()*.
-    - Updated parameters of the *assemble_models()* function.
-    - Revised code structure of the *assemble_models()* function.
-    - Adjusted naming or added text in *utils.py*, *wizard.py* and *__init__py*.
-    - Updated README.md file.
+  - Changed function name from *assemble_model()* to *assemble_models()*.
+  - Updated parameters of the *assemble_models()* function.
+  - Revised code structure of the *assemble_models()* function.
+  - Adjusted naming or added text in *utils.py*, *wizard.py* and *__init__py*.
+  - Updated README.md file.
+- ***v0.3.2*** - text fixing and adding third party licenses
+- ***v0.3.1*** - bug fixing
+- ***v0.3.0*** - added additional functions
+- ***v0.2.0*** - tested with Oracle database
+- ***v0.1.0*** - creation of the initial code and tested with SqLite database
 
 
 ## 📄 License and Third-Party Licenses
 
 Alchemyrohan is MIT licensed, as stated in the [LICENSE][1] file.
 
 The following software components are included in this project:
@@ -268,9 +281,8 @@
 * SqlAlchemy (MIT License)
 * python-oracledb (Apache License 2.0) 
 
 [THIRD PARTY LICENSES][2]
 
 
 [1]: https://github.com/wamberger/alchemyrohan/blob/master/LICENSE
-[2]: https://github.com/wamberger/alchemyrohan/blob/master/THIRD_PARTY_LICENSES
-
+[2]: https://github.com/wamberger/alchemyrohan/blob/master/THIRD_PARTY_LICENSES
```

### Comparing `alchemyrohan-0.4.0/alchemyrohan/__init__.py` & `alchemyrohan-0.4.1/alchemyrohan/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 __author__ = 'Alan Wamberger'
 __email__ = 'awamberger@proton.me'
 
 __license__ = 'MIT'
 __copyright__ = '2023 %s' % __author__
 
 
-from alchemyrohan.assemble import *
-from alchemyrohan.utils import *
+from alchemyrohan.assemble import assemble_models
+from alchemyrohan.utils import get_model
```

### Comparing `alchemyrohan-0.4.0/alchemyrohan/meta_data.py` & `alchemyrohan-0.4.1/alchemyrohan/meta_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,57 @@
 
 
-from sqlalchemy import Connection
-from sqlalchemy import inspect
-from sqlalchemy.engine import Engine
-
+__all__ = ['MetaDataHolder']
 
-__all__ = [
-    'MetaDataHolder',
-    'AlchemyRohanDatabaseError'
-]
 
-
-class AlchemyRohanDatabaseError(Exception): ...
+from sqlalchemy import inspect
+from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.engine import Engine
 
 
 class MetaDataHolder:
-    def __init__(
-        self,
-        engine: Engine,
-        table: str
-        ):
-        
-        self._chk_conn(engine)
-        
+    def __init__(self, engine: Engine, table: str) -> None:
         self.name = table
         self.rdbms = engine.name
 
         inspector = inspect(engine)
         self.schema = inspector.default_schema_name
         self.columns = self._get_columns(inspector, table)
         self.primary_key = self._get_primary_key(inspector, table)
         self.foreign_keys = self._get_foreign_keys(inspector, table)
         self.multi_foreign_keys = self._get_multi_foreign_keys(inspector)
         self.unique_keys = self._get_unique_cons(inspector, table)
 
     @staticmethod
-    def _chk_conn(engine) -> None:
-        try:
-            Connection(engine)
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
-
-    @staticmethod
     def _get_columns(inspector, table):
         try:
             return inspector.get_columns(table)
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
+        except SQLAlchemyError as e:
+            raise SQLAlchemyError(e) from e
 
     @staticmethod
     def _get_primary_key(inspector, table):
         try:
             return inspector.get_pk_constraint(table)
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
+        except SQLAlchemyError as e:
+            raise SQLAlchemyError(e) from e
     
     @staticmethod
     def _get_foreign_keys(inspector, table):
         try:
             return inspector.get_foreign_keys(table)
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
+        except SQLAlchemyError as e:
+            raise SQLAlchemyError(e) from e
     
     @staticmethod
     def _get_multi_foreign_keys(inspector):
         try:
             return inspector.get_multi_foreign_keys()
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
+        except SQLAlchemyError as e:
+            raise SQLAlchemyError(e) from e
 
     @staticmethod
     def _get_unique_cons(inspector, table):
         try:
             return inspector.get_unique_constraints(table)
-        except Exception as e:
-            raise AlchemyRohanDatabaseError(e)
+        except SQLAlchemyError as e:
+            raise SQLAlchemyError(e) from e
```

### Comparing `alchemyrohan-0.4.0/alchemyrohan/oracle.py` & `alchemyrohan-0.4.1/alchemyrohan/oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 
 
+__all__ = ['read_oracle_and_build_code']
+
+
 from typing import Any
 from datetime import datetime
 from datetime import timedelta
 from sqlalchemy.dialects.oracle import BINARY_DOUBLE
 from sqlalchemy.dialects.oracle import BINARY_FLOAT
 from sqlalchemy.dialects.oracle import BLOB
 from sqlalchemy.dialects.oracle import CHAR
@@ -25,18 +28,15 @@
 from sqlalchemy.dialects.oracle import VARCHAR
 from sqlalchemy.dialects.oracle import VARCHAR2
 
 from alchemyrohan.meta_data import MetaDataHolder
 from alchemyrohan.utils import str_print
 
 
-__all__ = ['read_oracle_and_build_code']
-
-
-_dialect_imports = []
+dialect_imports = []
 
 
 def _get_default(typ: str) -> Any:
     if typ == 'BINARY_DOUBLE':
         return 0.0
     if typ == 'BINARY_FLOAT':
         return 0.0
@@ -192,26 +192,24 @@
         if self.{col} and not isinstance(self.{col}, int):
             try:
                 self.{col} = int(self.{col})
             except:
                 raise SyntaxError(f'< {{self.{col}}} > is not integer')
         """
     
-    elif typ == 'BLOB'\
-    or typ == 'RAW':
+    elif typ == 'BLOB' or typ == 'RAW':
         tmp = f"""
         if self.{col} and not isinstance(self.{col}, bytes):
             try:
                 self.{col} = int(self.{col})
             except:
                 raise SyntaxError(f'< {{self.{col}}} > is not bytes type')
         """
     
-    elif typ == 'DATE'\
-    or typ == 'TIMESTAMP':
+    elif typ == 'DATE' or typ == 'TIMESTAMP':
         tmp = f"""
         if self.{col} and not isinstance(self.{col}, datetime):
             try:
                 self.{col} = int(self.{col})
             except:
                 raise SyntaxError(f'< {{self.{col}}} > is not datetime type')
         """
@@ -242,45 +240,36 @@
             except:
                 raise SyntaxError(f'< {{self.{col}}} > is not string')
         """
 
     return tmp
 
 
-def _validations(
-    code_holder: dict, 
-    table_meta_data: MetaDataHolder
-    ) -> None:
+def _validations(code_holder: dict, table_meta_data: MetaDataHolder) -> None:
 
     col = []
     for c in table_meta_data.columns:
-        col.append(_get_validation(
-            _get_type_name(c['type']), 
-            c['name']
-            )
-        )
+        col.append(
+            _get_validation(_get_type_name(c['type']), c['name']))
 
     code_holder.update({'validations': col})
 
 
-def _columns(
-    code_holder: dict, 
-    table_meta_data: MetaDataHolder
-    ) -> None:
+def _columns(code_holder: dict, table_meta_data: MetaDataHolder) -> None:
     
     col = []
     for c in table_meta_data.columns:
         
         tmp = f"{c['name']} = Column("
         tmp = ''.join([tmp, _get_type_prop(c['type'])])
 
         imp = f"from sqlalchemy.dialects.oracle import"\
             f" {_get_type_name(c['type'])}"
-        if imp not in _dialect_imports:
-            _dialect_imports.append(imp)
+        if imp not in dialect_imports:
+            dialect_imports.append(imp)
 
         pk = False
         for k, v in table_meta_data.primary_key.items():
             if k == 'constrained_columns':
                 for e in v:
                     if c['name'] == e:
                         tmp = ', '.join([tmp, 'primary_key=True'])
@@ -294,16 +283,16 @@
                     if fk == c['name']:
                         ref_table = f['referred_table']
                         tmp = ', '.join(
                             [tmp, 
                             f"ForeignKey('{ref_table}.{fk}')"]
                             )
                         imp = 'from sqlalchemy import ForeignKey'
-                        if imp not in _dialect_imports:
-                            _dialect_imports.append(imp)
+                        if imp not in dialect_imports:
+                            dialect_imports.append(imp)
                         break
 
             if c['nullable']:
                 tmp = ', '.join([tmp, 'nullable=True', 'default=None'])
             else:
                 if c['default']:
                     tmp = ', '.join([
@@ -329,18 +318,15 @@
     {tmp}"""
         
         col.append(tmp)
        
     code_holder.update({'columns': col})
 
 
-def _relations(
-    code_holder: dict, 
-    table_meta_data: MetaDataHolder
-    ) -> None:
+def _relations(code_holder: dict, table_meta_data: MetaDataHolder) -> None:
 
     rel = []
     for f in table_meta_data.foreign_keys:
         referred_table = f['referred_table']
 
         tmp = f'parent_{referred_table.capitalize()}'\
             f' = relationship("{referred_table.capitalize()}",'\
@@ -369,25 +355,23 @@
 
                             rel.append(tmp)
 
             break
                     
     if rel:
         imp = 'from sqlalchemy.orm import relationship'
-        if imp not in _dialect_imports:
-            _dialect_imports.append(imp)
+        if imp not in dialect_imports:
+            dialect_imports.append(imp)
 
     code_holder.update(
-        {'imports': code_holder['imports'] + _dialect_imports}
+        {'imports': code_holder['imports'] + dialect_imports}
         )
     code_holder.update({'relations': rel})
 
 
 def read_oracle_and_build_code(
-    code_holder: dict, 
-    table_meta_data: MetaDataHolder
-    ) -> None:
+        code_holder: dict, table_meta_data: MetaDataHolder) -> None:
 
     _columns(code_holder, table_meta_data)
     _relations(code_holder, table_meta_data)
     _validations(code_holder, table_meta_data)
-    str_print(code_holder, table_meta_data)
+    str_print(code_holder, table_meta_data)
```

### Comparing `alchemyrohan-0.4.0/alchemyrohan/sqlite.py` & `alchemyrohan-0.4.1/alchemyrohan/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,382 +1,398 @@
-00000000: 0d0a 0d0a 6672 6f6d 2074 7970 696e 6720  ....from typing 
-00000010: 696d 706f 7274 2041 6e79 0d0a 6672 6f6d  import Any..from
-00000020: 2073 716c 616c 6368 656d 792e 6469 616c   sqlalchemy.dial
-00000030: 6563 7473 2e73 716c 6974 6520 696d 706f  ects.sqlite impo
-00000040: 7274 2054 4558 540d 0a66 726f 6d20 7371  rt TEXT..from sq
-00000050: 6c61 6c63 6865 6d79 2e64 6961 6c65 6374  lalchemy.dialect
-00000060: 732e 7371 6c69 7465 2069 6d70 6f72 7420  s.sqlite import 
-00000070: 494e 5445 4745 520d 0a66 726f 6d20 7371  INTEGER..from sq
-00000080: 6c61 6c63 6865 6d79 2e64 6961 6c65 6374  lalchemy.dialect
-00000090: 732e 7371 6c69 7465 2069 6d70 6f72 7420  s.sqlite import 
-000000a0: 5245 414c 0d0a 6672 6f6d 2073 716c 616c  REAL..from sqlal
-000000b0: 6368 656d 792e 6469 616c 6563 7473 2e73  chemy.dialects.s
-000000c0: 716c 6974 6520 696d 706f 7274 2042 4c4f  qlite import BLO
-000000d0: 420d 0a0d 0a66 726f 6d20 616c 6368 656d  B....from alchem
-000000e0: 7972 6f68 616e 2e6d 6574 615f 6461 7461  yrohan.meta_data
-000000f0: 2069 6d70 6f72 7420 4d65 7461 4461 7461   import MetaData
-00000100: 486f 6c64 6572 0d0a 6672 6f6d 2061 6c63  Holder..from alc
-00000110: 6865 6d79 726f 6861 6e2e 7574 696c 7320  hemyrohan.utils 
-00000120: 696d 706f 7274 2073 7472 5f70 7269 6e74  import str_print
-00000130: 0d0a 0d0a 0d0a 5f5f 616c 6c5f 5f20 3d20  ......__all__ = 
-00000140: 5b27 7265 6164 5f73 716c 6974 655f 616e  ['read_sqlite_an
-00000150: 645f 6275 696c 645f 636f 6465 275d 0d0a  d_build_code']..
-00000160: 0d0a 0d0a 5f64 6961 6c65 6374 5f69 6d70  ...._dialect_imp
-00000170: 6f72 7473 203d 205b 5d0d 0a0d 0a0d 0a64  orts = []......d
-00000180: 6566 205f 6765 745f 6465 6661 756c 7428  ef _get_default(
-00000190: 7479 703a 2073 7472 2920 2d3e 2041 6e79  typ: str) -> Any
-000001a0: 3a0d 0a20 2020 2069 6620 7479 7020 3d3d  :..    if typ ==
-000001b0: 2027 5445 5854 273a 0d0a 2020 2020 2020   'TEXT':..      
-000001c0: 2020 7265 7475 726e 2022 2720 2722 0d0a    return "' '"..
-000001d0: 2020 2020 656c 6966 2074 7970 203d 3d20      elif typ == 
-000001e0: 2749 4e54 4547 4552 273a 0d0a 2020 2020  'INTEGER':..    
-000001f0: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
-00000200: 2020 656c 6966 2074 7970 203d 3d20 2752    elif typ == 'R
-00000210: 4541 4c27 3a0d 0a20 2020 2020 2020 2072  EAL':..        r
-00000220: 6574 7572 6e20 302e 300d 0a20 2020 2065  eturn 0.0..    e
-00000230: 6c69 6620 7479 7020 3d3d 2027 424c 4f42  lif typ == 'BLOB
-00000240: 273a 0d0a 2020 2020 2020 2020 7265 7475  ':..        retu
-00000250: 726e 2062 2227 2027 220d 0a0d 0a0d 0a64  rn b"' '"......d
-00000260: 6566 205f 6765 745f 7479 7065 2874 7970  ef _get_type(typ
-00000270: 3a20 416e 7929 202d 3e20 7374 723a 0d0a  : Any) -> str:..
-00000280: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00000290: 6528 7479 702c 2054 4558 5429 3a0d 0a20  e(typ, TEXT):.. 
-000002a0: 2020 2020 2020 2072 6574 7572 6e20 2754         return 'T
-000002b0: 4558 5427 0d0a 2020 2020 656c 6966 2069  EXT'..    elif i
-000002c0: 7369 6e73 7461 6e63 6528 7479 702c 2049  sinstance(typ, I
-000002d0: 4e54 4547 4552 293a 0d0a 2020 2020 2020  NTEGER):..      
-000002e0: 2020 7265 7475 726e 2027 494e 5445 4745    return 'INTEGE
-000002f0: 5227 0d0a 2020 2020 656c 6966 2069 7369  R'..    elif isi
-00000300: 6e73 7461 6e63 6528 7479 702c 2052 4541  nstance(typ, REA
-00000310: 4c29 3a0d 0a20 2020 2020 2020 2072 6574  L):..        ret
-00000320: 7572 6e20 2752 4541 4c27 0d0a 2020 2020  urn 'REAL'..    
-00000330: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00000340: 7479 702c 2042 4c4f 4229 3a0d 0a20 2020  typ, BLOB):..   
-00000350: 2020 2020 2072 6574 7572 6e20 2742 4c4f       return 'BLO
-00000360: 4227 0d0a 2020 2020 0d0a 0d0a 6465 6620  B'..    ....def 
-00000370: 5f67 6574 5f76 616c 6964 6174 696f 6e28  _get_validation(
-00000380: 7479 703a 2073 7472 2c20 636f 6c3a 2073  typ: str, col: s
-00000390: 7472 2920 2d3e 2073 7472 3a0d 0a20 2020  tr) -> str:..   
-000003a0: 200d 0a20 2020 2074 6d70 3a20 7374 7220   ..    tmp: str 
-000003b0: 3d20 2727 0d0a 2020 2020 6966 2074 7970  = ''..    if typ
-000003c0: 203d 3d20 2754 4558 5427 5c0d 0a20 2020   == 'TEXT'\..   
-000003d0: 206f 7220 7479 7020 3d3d 2027 424c 4f42   or typ == 'BLOB
-000003e0: 273a 0d0a 2020 2020 2020 2020 746d 7020  ':..        tmp 
-000003f0: 3d20 6622 2222 0d0a 2020 2020 2020 2020  = f"""..        
-00000400: 6966 2073 656c 662e 7b63 6f6c 7d20 616e  if self.{col} an
-00000410: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
-00000420: 2873 656c 662e 7b63 6f6c 7d2c 2073 7472  (self.{col}, str
-00000430: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000440: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00000450: 2020 2020 2020 7365 6c66 2e7b 636f 6c7d        self.{col}
-00000460: 203d 2073 7472 2873 656c 662e 7b63 6f6c   = str(self.{col
-00000470: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00000480: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
-00000490: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-000004a0: 796e 7461 7845 7272 6f72 2866 273c 207b  yntaxError(f'< {
-000004b0: 7b73 656c 662e 7b63 6f6c 7d7d 7d20 3e20  {self.{col}}} > 
-000004c0: 6973 206e 6f74 2073 7472 696e 6727 290d  is not string').
-000004d0: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
-000004e0: 2020 2020 656c 6966 2074 7970 203d 3d20      elif typ == 
-000004f0: 2749 4e54 4547 4552 273a 0d0a 2020 2020  'INTEGER':..    
-00000500: 2020 2020 746d 7020 3d20 6622 2222 0d0a      tmp = f"""..
-00000510: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000520: 7b63 6f6c 7d20 616e 6420 6e6f 7420 6973  {col} and not is
-00000530: 696e 7374 616e 6365 2873 656c 662e 7b63  instance(self.{c
-00000540: 6f6c 7d2c 2069 6e74 293a 0d0a 2020 2020  ol}, int):..    
-00000550: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00000560: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000570: 6c66 2e7b 636f 6c7d 203d 2069 6e74 2873  lf.{col} = int(s
-00000580: 656c 662e 7b63 6f6c 7d29 0d0a 2020 2020  elf.{col})..    
-00000590: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
-000005a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000005b0: 2072 6169 7365 2053 796e 7461 7845 7272   raise SyntaxErr
-000005c0: 6f72 2866 273c 207b 7b73 656c 662e 7b63  or(f'< {{self.{c
-000005d0: 6f6c 7d7d 7d20 3e20 6973 206e 6f74 2069  ol}}} > is not i
-000005e0: 6e74 6567 6572 2729 0d0a 2020 2020 2020  nteger')..      
-000005f0: 2020 2222 220d 0a0d 0a20 2020 2065 6c69    """....    eli
-00000600: 6620 7479 7020 3d3d 2027 5245 414c 273a  f typ == 'REAL':
-00000610: 0d0a 2020 2020 2020 2020 746d 7020 3d20  ..        tmp = 
-00000620: 6622 2222 0d0a 2020 2020 2020 2020 6966  f"""..        if
-00000630: 2073 656c 662e 7b63 6f6c 7d20 616e 6420   self.{col} and 
-00000640: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
-00000650: 656c 662e 7b63 6f6c 7d2c 2066 6c6f 6174  elf.{col}, float
-00000660: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000670: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00000680: 2020 2020 2020 7365 6c66 2e7b 636f 6c7d        self.{col}
-00000690: 203d 2066 6c6f 6174 2873 656c 662e 7b63   = float(self.{c
-000006a0: 6f6c 7d29 0d0a 2020 2020 2020 2020 2020  ol})..          
-000006b0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-000006c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000006d0: 2053 796e 7461 7845 7272 6f72 2866 273c   SyntaxError(f'<
-000006e0: 207b 7b73 656c 662e 7b63 6f6c 7d7d 7d20   {{self.{col}}} 
-000006f0: 3e20 6973 206e 6f74 2066 6c6f 6174 2729  > is not float')
-00000700: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-00000710: 0a20 2020 2072 6574 7572 6e20 746d 700d  .    return tmp.
-00000720: 0a0d 0a0d 0a64 6566 205f 7661 6c69 6461  .....def _valida
-00000730: 7469 6f6e 7328 0d0a 2020 2020 636f 6465  tions(..    code
-00000740: 5f68 6f6c 6465 723a 2064 6963 742c 200d  _holder: dict, .
-00000750: 0a20 2020 2074 6162 6c65 5f6d 6574 615f  .    table_meta_
-00000760: 6461 7461 3a20 4d65 7461 4461 7461 486f  data: MetaDataHo
-00000770: 6c64 6572 0d0a 2020 2020 2920 2d3e 204e  lder..    ) -> N
-00000780: 6f6e 653a 0d0a 0d0a 2020 2020 636f 6c20  one:....    col 
-00000790: 3d20 5b5d 0d0a 2020 2020 666f 7220 6320  = []..    for c 
-000007a0: 696e 2074 6162 6c65 5f6d 6574 615f 6461  in table_meta_da
-000007b0: 7461 2e63 6f6c 756d 6e73 3a0d 0a20 2020  ta.columns:..   
-000007c0: 2020 2020 2063 6f6c 2e61 7070 656e 6428       col.append(
-000007d0: 5f67 6574 5f76 616c 6964 6174 696f 6e28  _get_validation(
-000007e0: 0d0a 2020 2020 2020 2020 2020 2020 5f67  ..            _g
-000007f0: 6574 5f74 7970 6528 635b 2774 7970 6527  et_type(c['type'
-00000800: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
-00000810: 2020 635b 276e 616d 6527 5d0d 0a20 2020    c['name']..   
-00000820: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00000830: 2020 2020 290d 0a0d 0a20 2020 2063 6f64      )....    cod
-00000840: 655f 686f 6c64 6572 2e75 7064 6174 6528  e_holder.update(
-00000850: 7b27 7661 6c69 6461 7469 6f6e 7327 3a20  {'validations': 
-00000860: 636f 6c7d 290d 0a0d 0a0d 0a64 6566 205f  col})......def _
-00000870: 636f 6c75 6d6e 7328 0d0a 2020 2020 636f  columns(..    co
-00000880: 6465 5f68 6f6c 6465 723a 2064 6963 742c  de_holder: dict,
-00000890: 200d 0a20 2020 2074 6162 6c65 5f6d 6574   ..    table_met
-000008a0: 615f 6461 7461 3a20 4d65 7461 4461 7461  a_data: MetaData
-000008b0: 486f 6c64 6572 0d0a 2020 2020 2920 2d3e  Holder..    ) ->
-000008c0: 204e 6f6e 653a 0d0a 2020 2020 0d0a 2020   None:..    ..  
-000008d0: 2020 636f 6c20 3d20 5b5d 0d0a 2020 2020    col = []..    
-000008e0: 666f 7220 6320 696e 2074 6162 6c65 5f6d  for c in table_m
-000008f0: 6574 615f 6461 7461 2e63 6f6c 756d 6e73  eta_data.columns
-00000900: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00000910: 2020 2020 2074 6d70 203d 2066 227b 635b       tmp = f"{c[
-00000920: 276e 616d 6527 5d7d 203d 2043 6f6c 756d  'name']} = Colum
-00000930: 6e28 220d 0a20 2020 2020 2020 2074 6d70  n("..        tmp
-00000940: 203d 2027 272e 6a6f 696e 285b 746d 702c   = ''.join([tmp,
-00000950: 205f 6765 745f 7479 7065 2863 5b27 7479   _get_type(c['ty
-00000960: 7065 275d 295d 290d 0a20 2020 2020 2020  pe'])])..       
-00000970: 2069 6d70 203d 2066 2266 726f 6d20 7371   imp = f"from sq
-00000980: 6c61 6c63 6865 6d79 2e64 6961 6c65 6374  lalchemy.dialect
-00000990: 732e 7371 6c69 7465 2069 6d70 6f72 7420  s.sqlite import 
-000009a0: 7b5f 6765 745f 7479 7065 2863 5b27 7479  {_get_type(c['ty
-000009b0: 7065 275d 297d 220d 0a20 2020 2020 2020  pe'])}"..       
-000009c0: 2069 6620 696d 7020 6e6f 7420 696e 205f   if imp not in _
-000009d0: 6469 616c 6563 745f 696d 706f 7274 733a  dialect_imports:
-000009e0: 0d0a 2020 2020 2020 2020 2020 2020 5f64  ..            _d
-000009f0: 6961 6c65 6374 5f69 6d70 6f72 7473 2e61  ialect_imports.a
-00000a00: 7070 656e 6428 696d 7029 0d0a 0d0a 2020  ppend(imp)....  
-00000a10: 2020 2020 2020 6966 2063 5b27 7072 696d        if c['prim
-00000a20: 6172 795f 6b65 7927 5d20 3d3d 2031 3a0d  ary_key'] == 1:.
-00000a30: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-00000a40: 203d 2027 2c20 272e 6a6f 696e 285b 746d   = ', '.join([tm
-00000a50: 702c 2027 7072 696d 6172 795f 6b65 793d  p, 'primary_key=
-00000a60: 5472 7565 275d 290d 0a20 2020 2020 2020  True'])..       
-00000a70: 2065 6c73 653a 0d0a 0d0a 2020 2020 2020   else:....      
-00000a80: 2020 2020 2020 666f 7220 6620 696e 2074        for f in t
-00000a90: 6162 6c65 5f6d 6574 615f 6461 7461 2e66  able_meta_data.f
-00000aa0: 6f72 6569 676e 5f6b 6579 733a 0d0a 2020  oreign_keys:..  
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00000ac0: 7220 666b 2069 6e20 665b 2772 6566 6572  r fk in f['refer
-00000ad0: 7265 645f 636f 6c75 6d6e 7327 5d3a 0d0a  red_columns']:..
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2020 6966 2066 6b20 3d3d 2063 5b27      if fk == c['
-00000b00: 6e61 6d65 275d 3a0d 0a20 2020 2020 2020  name']:..       
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2072 6566 5f74 6162 6c65 203d 2066 5b27   ref_table = f['
-00000b30: 7265 6665 7272 6564 5f74 6162 6c65 275d  referred_table']
-00000b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b50: 2020 2020 2020 2020 2020 746d 7020 3d20            tmp = 
-00000b60: 272c 2027 2e6a 6f69 6e28 0d0a 2020 2020  ', '.join(..    
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 2020 2020 2020 2020 5b74 6d70 2c20 0d0a          [tmp, ..
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 2020 2020 2020 2020 2020 2020 6622 466f              f"Fo
-00000bb0: 7265 6967 6e4b 6579 2827 7b72 6566 5f74  reignKey('{ref_t
-00000bc0: 6162 6c65 7d2e 7b66 6b7d 2729 225d 0d0a  able}.{fk}')"]..
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 2020 2020 2020 2063 6f64 655f 686f 6c64         code_hold
-00000c10: 6572 5b27 696d 706f 7274 7327 5d2e 6170  er['imports'].ap
-00000c20: 7065 6e64 280d 0a20 2020 2020 2020 2020  pend(..         
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c40: 2020 2027 6672 6f6d 2073 716c 616c 6368     'from sqlalch
-00000c50: 656d 7920 696d 706f 7274 2046 6f72 6569  emy import Forei
-00000c60: 676e 4b65 7927 0d0a 2020 2020 2020 2020  gnKey'..        
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00000ca0: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
-00000cb0: 2020 2020 6966 2063 5b27 6e75 6c6c 6162      if c['nullab
-00000cc0: 6c65 275d 3a0d 0a20 2020 2020 2020 2020  le']:..         
-00000cd0: 2020 2020 2020 2074 6d70 203d 2027 2c20         tmp = ', 
-00000ce0: 272e 6a6f 696e 285b 746d 702c 2027 6e75  '.join([tmp, 'nu
-00000cf0: 6c6c 6162 6c65 3d54 7275 6527 2c20 2764  llable=True', 'd
-00000d00: 6566 6175 6c74 3d4e 6f6e 6527 5d29 0d0a  efault=None'])..
-00000d10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000d20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000d30: 2020 2069 6620 635b 2764 6566 6175 6c74     if c['default
-00000d40: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
-00000d50: 2020 2020 2020 2020 2074 6d70 203d 2027           tmp = '
-00000d60: 2c20 272e 6a6f 696e 285b 0d0a 2020 2020  , '.join([..    
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 746d 702c 2027 6e75 6c6c 6162      tmp, 'nullab
-00000d90: 6c65 3d46 616c 7365 272c 2066 2264 6566  le=False', f"def
-00000da0: 6175 6c74 3d7b 635b 2764 6566 6175 6c74  ault={c['default
-00000db0: 275d 7d22 5d0d 0a20 2020 2020 2020 2020  ']}"]..         
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00000dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000de0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000df0: 2020 2020 2020 2020 2020 2020 2074 6d70               tmp
-00000e00: 203d 2027 2c20 272e 6a6f 696e 285b 0d0a   = ', '.join([..
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2020 2020 746d 702c 200d 0a20          tmp, .. 
+00000000: 0d0a 0d0a 5f5f 616c 6c5f 5f20 3d20 5b27  ....__all__ = ['
+00000010: 7265 6164 5f73 716c 6974 655f 616e 645f  read_sqlite_and_
+00000020: 6275 696c 645f 636f 6465 275d 0d0a 0d0a  build_code']....
+00000030: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+00000040: 706f 7274 2041 6e79 0d0a 6672 6f6d 2073  port Any..from s
+00000050: 716c 616c 6368 656d 792e 6469 616c 6563  qlalchemy.dialec
+00000060: 7473 2e73 716c 6974 6520 696d 706f 7274  ts.sqlite import
+00000070: 2054 4558 540d 0a66 726f 6d20 7371 6c61   TEXT..from sqla
+00000080: 6c63 6865 6d79 2e64 6961 6c65 6374 732e  lchemy.dialects.
+00000090: 7371 6c69 7465 2069 6d70 6f72 7420 494e  sqlite import IN
+000000a0: 5445 4745 520d 0a66 726f 6d20 7371 6c61  TEGER..from sqla
+000000b0: 6c63 6865 6d79 2e64 6961 6c65 6374 732e  lchemy.dialects.
+000000c0: 7371 6c69 7465 2069 6d70 6f72 7420 5245  sqlite import RE
+000000d0: 414c 0d0a 6672 6f6d 2073 716c 616c 6368  AL..from sqlalch
+000000e0: 656d 792e 6469 616c 6563 7473 2e73 716c  emy.dialects.sql
+000000f0: 6974 6520 696d 706f 7274 2042 4c4f 420d  ite import BLOB.
+00000100: 0a0d 0a66 726f 6d20 616c 6368 656d 7972  ...from alchemyr
+00000110: 6f68 616e 2e6d 6574 615f 6461 7461 2069  ohan.meta_data i
+00000120: 6d70 6f72 7420 4d65 7461 4461 7461 486f  mport MetaDataHo
+00000130: 6c64 6572 0d0a 6672 6f6d 2061 6c63 6865  lder..from alche
+00000140: 6d79 726f 6861 6e2e 7574 696c 7320 696d  myrohan.utils im
+00000150: 706f 7274 2073 7472 5f70 7269 6e74 0d0a  port str_print..
+00000160: 0d0a 0d0a 6469 616c 6563 745f 696d 706f  ....dialect_impo
+00000170: 7274 7320 3d20 5b5d 0d0a 0d0a 0d0a 6465  rts = []......de
+00000180: 6620 5f67 6574 5f64 6566 6175 6c74 2874  f _get_default(t
+00000190: 7970 3a20 7374 7229 202d 3e20 416e 793a  yp: str) -> Any:
+000001a0: 0d0a 2020 2020 6966 2074 7970 203d 3d20  ..    if typ == 
+000001b0: 2754 4558 5427 3a0d 0a20 2020 2020 2020  'TEXT':..       
+000001c0: 2072 6574 7572 6e20 2227 2027 220d 0a20   return "' '".. 
+000001d0: 2020 2065 6c69 6620 7479 7020 3d3d 2027     elif typ == '
+000001e0: 494e 5445 4745 5227 3a0d 0a20 2020 2020  INTEGER':..     
+000001f0: 2020 2072 6574 7572 6e20 300d 0a20 2020     return 0..   
+00000200: 2065 6c69 6620 7479 7020 3d3d 2027 5245   elif typ == 'RE
+00000210: 414c 273a 0d0a 2020 2020 2020 2020 7265  AL':..        re
+00000220: 7475 726e 2030 2e30 0d0a 2020 2020 656c  turn 0.0..    el
+00000230: 6966 2074 7970 203d 3d20 2742 4c4f 4227  if typ == 'BLOB'
+00000240: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00000250: 6e20 6222 2720 2722 0d0a 0d0a 0d0a 6465  n b"' '"......de
+00000260: 6620 5f67 6574 5f74 7970 6528 7479 703a  f _get_type(typ:
+00000270: 2041 6e79 2920 2d3e 2073 7472 3a0d 0a20   Any) -> str:.. 
+00000280: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00000290: 2874 7970 2c20 5445 5854 293a 0d0a 2020  (typ, TEXT):..  
+000002a0: 2020 2020 2020 7265 7475 726e 2027 5445        return 'TE
+000002b0: 5854 270d 0a20 2020 2065 6c69 6620 6973  XT'..    elif is
+000002c0: 696e 7374 616e 6365 2874 7970 2c20 494e  instance(typ, IN
+000002d0: 5445 4745 5229 3a0d 0a20 2020 2020 2020  TEGER):..       
+000002e0: 2072 6574 7572 6e20 2749 4e54 4547 4552   return 'INTEGER
+000002f0: 270d 0a20 2020 2065 6c69 6620 6973 696e  '..    elif isin
+00000300: 7374 616e 6365 2874 7970 2c20 5245 414c  stance(typ, REAL
+00000310: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00000320: 726e 2027 5245 414c 270d 0a20 2020 2065  rn 'REAL'..    e
+00000330: 6c69 6620 6973 696e 7374 616e 6365 2874  lif isinstance(t
+00000340: 7970 2c20 424c 4f42 293a 0d0a 2020 2020  yp, BLOB):..    
+00000350: 2020 2020 7265 7475 726e 2027 424c 4f42      return 'BLOB
+00000360: 270d 0a20 2020 200d 0a0d 0a64 6566 205f  '..    ....def _
+00000370: 6765 745f 7661 6c69 6461 7469 6f6e 2874  get_validation(t
+00000380: 7970 3a20 7374 722c 2063 6f6c 3a20 7374  yp: str, col: st
+00000390: 7229 202d 3e20 7374 723a 0d0a 2020 2020  r) -> str:..    
+000003a0: 0d0a 2020 2020 746d 703a 2073 7472 203d  ..    tmp: str =
+000003b0: 2027 270d 0a20 2020 2069 6620 7479 7020   ''..    if typ 
+000003c0: 3d3d 2027 5445 5854 273a 0d0a 2020 2020  == 'TEXT':..    
+000003d0: 2020 2020 746d 7020 3d20 6622 2222 0d0a      tmp = f"""..
+000003e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000003f0: 7b63 6f6c 7d20 616e 6420 6e6f 7420 6973  {col} and not is
+00000400: 696e 7374 616e 6365 2873 656c 662e 7b63  instance(self.{c
+00000410: 6f6c 7d2c 2073 7472 293a 0d0a 2020 2020  ol}, str):..    
+00000420: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00000430: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000440: 6c66 2e7b 636f 6c7d 203d 2073 7472 2873  lf.{col} = str(s
+00000450: 656c 662e 7b63 6f6c 7d29 0d0a 2020 2020  elf.{col})..    
+00000460: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
+00000470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000480: 2072 6169 7365 2053 796e 7461 7845 7272   raise SyntaxErr
+00000490: 6f72 2866 273c 207b 7b73 656c 662e 7b63  or(f'< {{self.{c
+000004a0: 6f6c 7d7d 7d20 3e20 6973 206e 6f74 2073  ol}}} > is not s
+000004b0: 7472 696e 6727 290d 0a20 2020 2020 2020  tring')..       
+000004c0: 2022 2222 0d0a 0d0a 2020 2020 656c 6966   """....    elif
+000004d0: 2074 7970 203d 3d20 2749 4e54 4547 4552   typ == 'INTEGER
+000004e0: 273a 0d0a 2020 2020 2020 2020 746d 7020  ':..        tmp 
+000004f0: 3d20 6622 2222 0d0a 2020 2020 2020 2020  = f"""..        
+00000500: 6966 2073 656c 662e 7b63 6f6c 7d20 616e  if self.{col} an
+00000510: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+00000520: 2873 656c 662e 7b63 6f6c 7d2c 2069 6e74  (self.{col}, int
+00000530: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000540: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00000550: 2020 2020 2020 7365 6c66 2e7b 636f 6c7d        self.{col}
+00000560: 203d 2069 6e74 2873 656c 662e 7b63 6f6c   = int(self.{col
+00000570: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00000580: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
+00000590: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+000005a0: 796e 7461 7845 7272 6f72 2866 273c 207b  yntaxError(f'< {
+000005b0: 7b73 656c 662e 7b63 6f6c 7d7d 7d20 3e20  {self.{col}}} > 
+000005c0: 6973 206e 6f74 2069 6e74 6567 6572 2729  is not integer')
+000005d0: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+000005e0: 0a20 2020 2065 6c69 6620 7479 7020 3d3d  .    elif typ ==
+000005f0: 2027 5245 414c 273a 0d0a 2020 2020 2020   'REAL':..      
+00000600: 2020 746d 7020 3d20 6622 2222 0d0a 2020    tmp = f"""..  
+00000610: 2020 2020 2020 6966 2073 656c 662e 7b63        if self.{c
+00000620: 6f6c 7d20 616e 6420 6e6f 7420 6973 696e  ol} and not isin
+00000630: 7374 616e 6365 2873 656c 662e 7b63 6f6c  stance(self.{col
+00000640: 7d2c 2066 6c6f 6174 293a 0d0a 2020 2020  }, float):..    
+00000650: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00000660: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000670: 6c66 2e7b 636f 6c7d 203d 2066 6c6f 6174  lf.{col} = float
+00000680: 2873 656c 662e 7b63 6f6c 7d29 0d0a 2020  (self.{col})..  
+00000690: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000006a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000006b0: 2020 2072 6169 7365 2053 796e 7461 7845     raise SyntaxE
+000006c0: 7272 6f72 2866 273c 207b 7b73 656c 662e  rror(f'< {{self.
+000006d0: 7b63 6f6c 7d7d 7d20 3e20 6973 206e 6f74  {col}}} > is not
+000006e0: 2066 6c6f 6174 2729 0d0a 2020 2020 2020   float')..      
+000006f0: 2020 2222 220d 0a0d 0a20 2020 2065 6c69    """....    eli
+00000700: 6620 7479 7020 3d3d 2027 424c 4f42 273a  f typ == 'BLOB':
+00000710: 0d0a 2020 2020 2020 2020 746d 7020 3d20  ..        tmp = 
+00000720: 6622 2222 0d0a 2020 2020 2020 2020 6966  f"""..        if
+00000730: 2073 656c 662e 7b63 6f6c 7d20 616e 6420   self.{col} and 
+00000740: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
+00000750: 656c 662e 7b63 6f6c 7d2c 2062 7974 6573  elf.{col}, bytes
+00000760: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000770: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00000780: 2020 2020 2020 7365 6c66 2e7b 636f 6c7d        self.{col}
+00000790: 203d 2069 6e74 2873 656c 662e 7b63 6f6c   = int(self.{col
+000007a0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000007b0: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
+000007c0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+000007d0: 796e 7461 7845 7272 6f72 2866 273c 207b  yntaxError(f'< {
+000007e0: 7b73 656c 662e 7b63 6f6c 7d7d 7d20 3e20  {self.{col}}} > 
+000007f0: 6973 206e 6f74 2062 7974 6573 2729 0d0a  is not bytes')..
+00000800: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
+00000810: 2020 2072 6574 7572 6e20 746d 700d 0a0d     return tmp...
+00000820: 0a0d 0a64 6566 205f 7661 6c69 6461 7469  ...def _validati
+00000830: 6f6e 7328 636f 6465 5f68 6f6c 6465 723a  ons(code_holder:
+00000840: 2064 6963 742c 2074 6162 6c65 5f6d 6574   dict, table_met
+00000850: 615f 6461 7461 3a20 4d65 7461 4461 7461  a_data: MetaData
+00000860: 486f 6c64 6572 2920 2d3e 204e 6f6e 653a  Holder) -> None:
+00000870: 0d0a 0d0a 2020 2020 636f 6c20 3d20 5b5d  ....    col = []
+00000880: 0d0a 2020 2020 666f 7220 6320 696e 2074  ..    for c in t
+00000890: 6162 6c65 5f6d 6574 615f 6461 7461 2e63  able_meta_data.c
+000008a0: 6f6c 756d 6e73 3a0d 0a20 2020 2020 2020  olumns:..       
+000008b0: 2063 6f6c 2e61 7070 656e 6428 0d0a 2020   col.append(..  
+000008c0: 2020 2020 2020 2020 2020 5f67 6574 5f76            _get_v
+000008d0: 616c 6964 6174 696f 6e28 5f67 6574 5f74  alidation(_get_t
+000008e0: 7970 6528 635b 2774 7970 6527 5d29 2c20  ype(c['type']), 
+000008f0: 635b 276e 616d 6527 5d29 290d 0a0d 0a20  c['name'])).... 
+00000900: 2020 2063 6f64 655f 686f 6c64 6572 2e75     code_holder.u
+00000910: 7064 6174 6528 7b27 7661 6c69 6461 7469  pdate({'validati
+00000920: 6f6e 7327 3a20 636f 6c7d 290d 0a0d 0a0d  ons': col}).....
+00000930: 0a64 6566 205f 636f 6c75 6d6e 7328 636f  .def _columns(co
+00000940: 6465 5f68 6f6c 6465 723a 2064 6963 742c  de_holder: dict,
+00000950: 2074 6162 6c65 5f6d 6574 615f 6461 7461   table_meta_data
+00000960: 3a20 4d65 7461 4461 7461 486f 6c64 6572  : MetaDataHolder
+00000970: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00000980: 0d0a 2020 2020 636f 6c20 3d20 5b5d 0d0a  ..    col = []..
+00000990: 2020 2020 666f 7220 6320 696e 2074 6162      for c in tab
+000009a0: 6c65 5f6d 6574 615f 6461 7461 2e63 6f6c  le_meta_data.col
+000009b0: 756d 6e73 3a0d 0a20 2020 2020 2020 200d  umns:..        .
+000009c0: 0a20 2020 2020 2020 2074 6d70 203d 2066  .        tmp = f
+000009d0: 227b 635b 276e 616d 6527 5d7d 203d 2043  "{c['name']} = C
+000009e0: 6f6c 756d 6e28 220d 0a20 2020 2020 2020  olumn("..       
+000009f0: 2074 6d70 203d 2027 272e 6a6f 696e 285b   tmp = ''.join([
+00000a00: 746d 702c 205f 6765 745f 7479 7065 2863  tmp, _get_type(c
+00000a10: 5b27 7479 7065 275d 295d 290d 0a20 2020  ['type'])])..   
+00000a20: 2020 2020 2069 6d70 203d 2066 2266 726f       imp = f"fro
+00000a30: 6d20 7371 6c61 6c63 6865 6d79 2e64 6961  m sqlalchemy.dia
+00000a40: 6c65 6374 732e 7371 6c69 7465 2069 6d70  lects.sqlite imp
+00000a50: 6f72 7420 7b5f 6765 745f 7479 7065 2863  ort {_get_type(c
+00000a60: 5b27 7479 7065 275d 297d 220d 0a20 2020  ['type'])}"..   
+00000a70: 2020 2020 2069 6620 696d 7020 6e6f 7420       if imp not 
+00000a80: 696e 2064 6961 6c65 6374 5f69 6d70 6f72  in dialect_impor
+00000a90: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00000aa0: 2064 6961 6c65 6374 5f69 6d70 6f72 7473   dialect_imports
+00000ab0: 2e61 7070 656e 6428 696d 7029 0d0a 0d0a  .append(imp)....
+00000ac0: 2020 2020 2020 2020 6966 2063 5b27 7072          if c['pr
+00000ad0: 696d 6172 795f 6b65 7927 5d20 3d3d 2031  imary_key'] == 1
+00000ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00000af0: 6d70 203d 2027 2c20 272e 6a6f 696e 285b  mp = ', '.join([
+00000b00: 746d 702c 2027 7072 696d 6172 795f 6b65  tmp, 'primary_ke
+00000b10: 793d 5472 7565 275d 290d 0a20 2020 2020  y=True'])..     
+00000b20: 2020 2065 6c73 653a 0d0a 0d0a 2020 2020     else:....    
+00000b30: 2020 2020 2020 2020 666f 7220 6620 696e          for f in
+00000b40: 2074 6162 6c65 5f6d 6574 615f 6461 7461   table_meta_data
+00000b50: 2e66 6f72 6569 676e 5f6b 6579 733a 0d0a  .foreign_keys:..
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 666f 7220 666b 2069 6e20 665b 2763 6f6e  for fk in f['con
+00000b80: 7374 7261 696e 6564 5f63 6f6c 756d 6e73  strained_columns
+00000b90: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+00000ba0: 2020 2020 2020 2020 2069 6620 666b 203d           if fk =
+00000bb0: 3d20 635b 276e 616d 6527 5d20 616e 6420  = c['name'] and 
+00000bc0: 665b 2772 6566 6572 7265 645f 636f 6c75  f['referred_colu
+00000bd0: 6d6e 7327 5d3a 0d0a 2020 2020 2020 2020  mns']:..        
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bf0: 7265 665f 636f 6c20 3d20 665b 2772 6566  ref_col = f['ref
+00000c00: 6572 7265 645f 636f 6c75 6d6e 7327 5d5b  erred_columns'][
+00000c10: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00000c20: 2020 2020 2020 2020 2020 2020 7265 665f              ref_
+00000c30: 7461 626c 6520 3d20 665b 2772 6566 6572  table = f['refer
+00000c40: 7265 645f 7461 626c 6527 5d2e 6c6f 7765  red_table'].lowe
+00000c50: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+00000c60: 2020 2020 2020 2020 2020 2020 2074 6d70               tmp
+00000c70: 203d 2027 2c20 272e 6a6f 696e 280d 0a20   = ', '.join(.. 
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 2020 205b 746d 702c             [tmp,
+00000ca0: 2066 2246 6f72 6569 676e 4b65 7928 277b   f"ForeignKey('{
+00000cb0: 7265 665f 7461 626c 657d 2e7b 7265 665f  ref_table}.{ref_
+00000cc0: 636f 6c7d 2729 225d 290d 0a20 2020 2020  col}')"])..     
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2063 6f64 655f 686f 6c64 6572 5b27     code_holder['
+00000cf0: 696d 706f 7274 7327 5d2e 6170 7065 6e64  imports'].append
+00000d00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000d20: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00000d30: 696d 706f 7274 2046 6f72 6569 676e 4b65  import ForeignKe
+00000d40: 7927 290d 0a20 2020 2020 2020 2020 2020  y')..           
+00000d50: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00000d60: 616b 0d0a 0d0a 2020 2020 2020 2020 2020  ak....          
+00000d70: 2020 6966 2063 5b27 6e75 6c6c 6162 6c65    if c['nullable
+00000d80: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+00000d90: 2020 2020 2074 6d70 203d 2027 2c20 272e       tmp = ', '.
+00000da0: 6a6f 696e 285b 746d 702c 2027 6e75 6c6c  join([tmp, 'null
+00000db0: 6162 6c65 3d54 7275 6527 2c20 2764 6566  able=True', 'def
+00000dc0: 6175 6c74 3d4e 6f6e 6527 5d29 0d0a 2020  ault=None'])..  
+00000dd0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00000de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000df0: 2069 6620 635b 2764 6566 6175 6c74 275d   if c['default']
+00000e00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000e10: 2020 2020 2020 2074 6d70 203d 2027 2c20         tmp = ', 
+00000e20: 272e 6a6f 696e 285b 0d0a 2020 2020 2020  '.join([..      
 00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 2020 2020 2020 2027 6e75 6c6c 6162 6c65         'nullable
-00000e50: 3d46 616c 7365 272c 200d 0a20 2020 2020  =False', ..     
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 2066 2264 6566 6175 6c74 3d7b 5f67     f"default={_g
-00000e80: 6574 5f64 6566 6175 6c74 285f 6765 745f  et_default(_get_
-00000e90: 7479 7065 2863 5b27 7479 7065 275d 2929  type(c['type']))
-00000ea0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-00000eb0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 2020 2029 2020 2020 2020 2020         )        
-00000ee0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00000ef0: 2066 6f72 2075 2069 6e20 7461 626c 655f   for u in table_
-00000f00: 6d65 7461 5f64 6174 612e 756e 6971 7565  meta_data.unique
-00000f10: 5f6b 6579 733a 0d0a 2020 2020 2020 2020  _keys:..        
-00000f20: 2020 2020 2020 2020 666f 7220 6520 696e          for e in
-00000f30: 2075 5b27 636f 6c75 6d6e 5f6e 616d 6573   u['column_names
-00000f40: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
-00000f50: 2020 2020 2020 2020 2069 6620 635b 276e           if c['n
-00000f60: 616d 6527 5d20 3d3d 2065 3a0d 0a20 2020  ame'] == e:..   
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2074 6d70 203d 2027 2c20 272e       tmp = ', '.
-00000f90: 6a6f 696e 285b 746d 702c 2027 756e 6971  join([tmp, 'uniq
-00000fa0: 7565 3d54 7275 6527 5d29 0d0a 2020 2020  ue=True'])..    
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
-00000fd0: 2020 2020 2074 6d70 203d 2027 272e 6a6f       tmp = ''.jo
-00000fe0: 696e 285b 746d 702c 2027 2927 5d29 0d0a  in([tmp, ')'])..
-00000ff0: 0d0a 2020 2020 2020 2020 746d 7020 3d20  ..        tmp = 
-00001000: 6622 2222 0d0a 2020 2020 7b74 6d70 7d22  f"""..    {tmp}"
-00001010: 2222 0d0a 2020 2020 2020 2020 0d0a 2020  ""..        ..  
-00001020: 2020 2020 2020 636f 6c2e 6170 7065 6e64        col.append
-00001030: 2874 6d70 290d 0a20 2020 2020 2020 0d0a  (tmp)..       ..
-00001040: 2020 2020 636f 6465 5f68 6f6c 6465 722e      code_holder.
-00001050: 7570 6461 7465 287b 2763 6f6c 756d 6e73  update({'columns
-00001060: 273a 2063 6f6c 7d29 0d0a 0d0a 0d0a 6465  ': col})......de
-00001070: 6620 5f72 656c 6174 696f 6e73 280d 0a20  f _relations(.. 
-00001080: 2020 2063 6f64 655f 686f 6c64 6572 3a20     code_holder: 
-00001090: 6469 6374 2c20 0d0a 2020 2020 7461 626c  dict, ..    tabl
-000010a0: 655f 6d65 7461 5f64 6174 613a 204d 6574  e_meta_data: Met
-000010b0: 6144 6174 6148 6f6c 6465 720d 0a20 2020  aDataHolder..   
-000010c0: 2029 202d 3e20 4e6f 6e65 3a0d 0a0d 0a20   ) -> None:.... 
-000010d0: 2020 2072 656c 203d 205b 5d0d 0a20 2020     rel = []..   
-000010e0: 2066 6f72 2066 2069 6e20 7461 626c 655f   for f in table_
-000010f0: 6d65 7461 5f64 6174 612e 666f 7265 6967  meta_data.foreig
-00001100: 6e5f 6b65 7973 3a0d 0a20 2020 2020 2020  n_keys:..       
-00001110: 2072 6566 6572 7265 645f 7461 626c 6520   referred_table 
-00001120: 3d20 665b 2772 6566 6572 7265 645f 7461  = f['referred_ta
-00001130: 626c 6527 5d0d 0a0d 0a20 2020 2020 2020  ble']....       
-00001140: 2074 6d70 203d 2066 2770 6172 656e 745f   tmp = f'parent_
-00001150: 7b72 6566 6572 7265 645f 7461 626c 652e  {referred_table.
-00001160: 6361 7069 7461 6c69 7a65 2829 7d27 5c0d  capitalize()}'\.
-00001170: 0a20 2020 2020 2020 2020 2020 2066 2720  .            f' 
-00001180: 3d20 7265 6c61 7469 6f6e 7368 6970 2822  = relationship("
-00001190: 7b72 6566 6572 7265 645f 7461 626c 652e  {referred_table.
-000011a0: 6361 7069 7461 6c69 7a65 2829 7d22 2c27  capitalize()}",'
-000011b0: 5c0d 0a20 2020 2020 2020 2020 2020 2066  \..            f
-000011c0: 2720 6261 636b 5f70 6f70 756c 6174 6573  ' back_populates
-000011d0: 3d22 6368 696c 6472 656e 5f7b 7461 626c  ="children_{tabl
-000011e0: 655f 6d65 7461 5f64 6174 612e 6e61 6d65  e_meta_data.name
-000011f0: 2e63 6170 6974 616c 697a 6528 297d 222c  .capitalize()}",
-00001200: 275c 0d0a 2020 2020 2020 2020 2020 2020  '\..            
-00001210: 2720 6c61 7a79 3d22 6a6f 696e 6564 2229  ' lazy="joined")
-00001220: 270d 0a20 2020 2020 2020 200d 0a20 2020  '..        ..   
-00001230: 2020 2020 2074 6d70 203d 2066 2222 220d       tmp = f""".
-00001240: 0a20 2020 207b 746d 707d 2222 2220 0d0a  .    {tmp}""" ..
-00001250: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001260: 2020 7265 6c2e 6170 7065 6e64 2874 6d70    rel.append(tmp
-00001270: 290d 0a0d 0a20 2020 2066 6f72 206b 2c20  )....    for k, 
-00001280: 7620 696e 2074 6162 6c65 5f6d 6574 615f  v in table_meta_
-00001290: 6461 7461 2e6d 756c 7469 5f66 6f72 6569  data.multi_forei
-000012a0: 676e 5f6b 6579 732e 6974 656d 7328 293a  gn_keys.items():
-000012b0: 0d0a 2020 2020 2020 2020 6966 206b 5b31  ..        if k[1
-000012c0: 5d20 3d3d 2074 6162 6c65 5f6d 6574 615f  ] == table_meta_
-000012d0: 6461 7461 2e6e 616d 6520 616e 6420 6e6f  data.name and no
-000012e0: 7420 763a 0d0a 2020 2020 2020 2020 2020  t v:..          
-000012f0: 2020 666f 7220 6368 696c 645f 7461 626c    for child_tabl
-00001300: 652c 2072 2069 6e20 7461 626c 655f 6d65  e, r in table_me
-00001310: 7461 5f64 6174 612e 6d75 6c74 695f 666f  ta_data.multi_fo
-00001320: 7265 6967 6e5f 6b65 7973 2e69 7465 6d73  reign_keys.items
-00001330: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00001340: 2020 2020 2069 6620 723a 0d0a 2020 2020       if r:..    
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 666f 7220 7274 2069 6e20 723a 0d0a 2020  for rt in r:..  
-00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001380: 2020 2020 2020 6966 2072 745b 2772 6566        if rt['ref
-00001390: 6572 7265 645f 7461 626c 6527 5d20 3d3d  erred_table'] ==
-000013a0: 2074 6162 6c65 5f6d 6574 615f 6461 7461   table_meta_data
-000013b0: 2e6e 616d 653a 0d0a 2020 2020 2020 2020  .name:..        
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013d0: 2020 2020 746d 7020 3d20 6627 6368 696c      tmp = f'chil
-000013e0: 6472 656e 5f7b 6368 696c 645f 7461 626c  dren_{child_tabl
-000013f0: 655b 315d 2e63 6170 6974 616c 697a 6528  e[1].capitalize(
-00001400: 297d 275c 0d0a 2020 2020 2020 2020 2020  )}'\..          
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2020 6627 203d 2072 656c 6174 696f 6e73    f' = relations
-00001430: 6869 7028 227b 6368 696c 645f 7461 626c  hip("{child_tabl
-00001440: 655b 315d 2e63 6170 6974 616c 697a 6528  e[1].capitalize(
-00001450: 297d 222c 275c 0d0a 2020 2020 2020 2020  )}",'\..        
-00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001470: 2020 2020 6627 2062 6163 6b5f 706f 7075      f' back_popu
-00001480: 6c61 7465 733d 2270 6172 656e 745f 7b74  lates="parent_{t
-00001490: 6162 6c65 5f6d 6574 615f 6461 7461 2e6e  able_meta_data.n
-000014a0: 616d 652e 6361 7069 7461 6c69 7a65 2829  ame.capitalize()
-000014b0: 7d22 2c27 5c0d 0a20 2020 2020 2020 2020  }",'\..         
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2020 2027 206c 617a 793d 226a 6f69 6e65     ' lazy="joine
-000014e0: 6422 2927 0d0a 2020 2020 2020 2020 0d0a  d")'..        ..
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 2020 2020 2020 2020 746d 7020              tmp 
-00001510: 3d20 6622 2222 0d0a 2020 2020 7b74 6d70  = f"""..    {tmp
-00001520: 7d22 2222 200d 0a0d 0a20 2020 2020 2020  }""" ....       
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 2072 656c 2e61 7070 656e 6428       rel.append(
-00001550: 746d 7029 0d0a 0d0a 2020 2020 2020 2020  tmp)....        
-00001560: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-00001570: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00001580: 0a20 2020 2069 6620 7265 6c3a 0d0a 2020  .    if rel:..  
-00001590: 2020 2020 2020 696d 7020 3d20 2766 726f        imp = 'fro
-000015a0: 6d20 7371 6c61 6c63 6865 6d79 2e6f 726d  m sqlalchemy.orm
-000015b0: 2069 6d70 6f72 7420 7265 6c61 7469 6f6e   import relation
-000015c0: 7368 6970 270d 0a20 2020 2020 2020 2069  ship'..        i
-000015d0: 6620 696d 7020 6e6f 7420 696e 205f 6469  f imp not in _di
-000015e0: 616c 6563 745f 696d 706f 7274 733a 0d0a  alect_imports:..
-000015f0: 2020 2020 2020 2020 2020 2020 5f64 6961              _dia
-00001600: 6c65 6374 5f69 6d70 6f72 7473 2e61 7070  lect_imports.app
-00001610: 656e 6428 696d 7029 0d0a 0d0a 2020 2020  end(imp)....    
-00001620: 636f 6465 5f68 6f6c 6465 722e 7570 6461  code_holder.upda
-00001630: 7465 280d 0a20 2020 2020 2020 207b 2769  te(..        {'i
-00001640: 6d70 6f72 7473 273a 2063 6f64 655f 686f  mports': code_ho
-00001650: 6c64 6572 5b27 696d 706f 7274 7327 5d20  lder['imports'] 
-00001660: 2b20 5f64 6961 6c65 6374 5f69 6d70 6f72  + _dialect_impor
-00001670: 7473 7d0d 0a20 2020 2020 2020 2029 0d0a  ts}..        )..
-00001680: 2020 2020 636f 6465 5f68 6f6c 6465 722e      code_holder.
-00001690: 7570 6461 7465 287b 2772 656c 6174 696f  update({'relatio
-000016a0: 6e73 273a 2072 656c 7d29 0d0a 0d0a 0d0a  ns': rel})......
-000016b0: 6465 6620 7265 6164 5f73 716c 6974 655f  def read_sqlite_
-000016c0: 616e 645f 6275 696c 645f 636f 6465 280d  and_build_code(.
-000016d0: 0a20 2020 2063 6f64 655f 686f 6c64 6572  .    code_holder
-000016e0: 3a20 6469 6374 2c20 0d0a 2020 2020 7461  : dict, ..    ta
-000016f0: 626c 655f 6d65 7461 5f64 6174 613a 204d  ble_meta_data: M
-00001700: 6574 6144 6174 6148 6f6c 6465 720d 0a20  etaDataHolder.. 
-00001710: 2020 2029 202d 3e20 4e6f 6e65 3a0d 0a0d     ) -> None:...
-00001720: 0a20 2020 205f 636f 6c75 6d6e 7328 636f  .    _columns(co
-00001730: 6465 5f68 6f6c 6465 722c 2074 6162 6c65  de_holder, table
-00001740: 5f6d 6574 615f 6461 7461 290d 0a20 2020  _meta_data)..   
-00001750: 205f 7265 6c61 7469 6f6e 7328 636f 6465   _relations(code
-00001760: 5f68 6f6c 6465 722c 2074 6162 6c65 5f6d  _holder, table_m
-00001770: 6574 615f 6461 7461 290d 0a20 2020 205f  eta_data)..    _
-00001780: 7661 6c69 6461 7469 6f6e 7328 636f 6465  validations(code
-00001790: 5f68 6f6c 6465 722c 2074 6162 6c65 5f6d  _holder, table_m
-000017a0: 6574 615f 6461 7461 290d 0a20 2020 2073  eta_data)..    s
-000017b0: 7472 5f70 7269 6e74 2863 6f64 655f 686f  tr_print(code_ho
-000017c0: 6c64 6572 2c20 7461 626c 655f 6d65 7461  lder, table_meta
-000017d0: 5f64 6174 6129                           _data)
+00000e40: 2020 746d 702c 2027 6e75 6c6c 6162 6c65    tmp, 'nullable
+00000e50: 3d46 616c 7365 272c 2066 2264 6566 6175  =False', f"defau
+00000e60: 6c74 3d7b 635b 2764 6566 6175 6c74 275d  lt={c['default']
+00000e70: 7d22 5d0d 0a20 2020 2020 2020 2020 2020  }"]..           
+00000e80: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ea0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000eb0: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
+00000ec0: 2027 2c20 272e 6a6f 696e 285b 0d0a 2020   ', '.join([..  
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ee0: 2020 2020 2020 746d 702c 200d 0a20 2020        tmp, ..   
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 2020 2020 2027 6e75 6c6c 6162 6c65 3d46       'nullable=F
+00000f10: 616c 7365 272c 200d 0a20 2020 2020 2020  alse', ..       
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f30: 2066 2264 6566 6175 6c74 3d7b 5f67 6574   f"default={_get
+00000f40: 5f64 6566 6175 6c74 285f 6765 745f 7479  _default(_get_ty
+00000f50: 7065 2863 5b27 7479 7065 275d 2929 7d22  pe(c['type']))}"
+00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000f70: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2020 2020 2029 2020 2020 2020 2020 200d       )         .
+00000fa0: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00000fb0: 6f72 2075 2069 6e20 7461 626c 655f 6d65  or u in table_me
+00000fc0: 7461 5f64 6174 612e 756e 6971 7565 5f6b  ta_data.unique_k
+00000fd0: 6579 733a 0d0a 2020 2020 2020 2020 2020  eys:..          
+00000fe0: 2020 2020 2020 666f 7220 6520 696e 2075        for e in u
+00000ff0: 5b27 636f 6c75 6d6e 5f6e 616d 6573 275d  ['column_names']
+00001000: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001010: 2020 2020 2020 2069 6620 635b 276e 616d         if c['nam
+00001020: 6527 5d20 3d3d 2065 3a0d 0a20 2020 2020  e'] == e:..     
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2074 6d70 203d 2027 2c20 272e 6a6f     tmp = ', '.jo
+00001050: 696e 285b 746d 702c 2027 756e 6971 7565  in([tmp, 'unique
+00001060: 3d54 7275 6527 5d29 0d0a 2020 2020 2020  =True'])..      
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 6272 6561 6b0d 0a0d 0a20 2020 2020    break....     
+00001090: 2020 2074 6d70 203d 2027 272e 6a6f 696e     tmp = ''.join
+000010a0: 285b 746d 702c 2027 2927 5d29 0d0a 0d0a  ([tmp, ')'])....
+000010b0: 2020 2020 2020 2020 746d 7020 3d20 6622          tmp = f"
+000010c0: 2222 0d0a 2020 2020 7b74 6d70 7d22 2222  ""..    {tmp}"""
+000010d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000010e0: 2020 2020 636f 6c2e 6170 7065 6e64 2874      col.append(t
+000010f0: 6d70 290d 0a20 2020 2020 2020 0d0a 2020  mp)..       ..  
+00001100: 2020 636f 6465 5f68 6f6c 6465 722e 7570    code_holder.up
+00001110: 6461 7465 287b 2763 6f6c 756d 6e73 273a  date({'columns':
+00001120: 2063 6f6c 7d29 0d0a 0d0a 0d0a 6465 6620   col})......def 
+00001130: 5f72 656c 6174 696f 6e73 280d 0a20 2020  _relations(..   
+00001140: 2020 2020 2063 6f64 655f 686f 6c64 6572       code_holder
+00001150: 3a20 6469 6374 2c20 7461 626c 655f 6d65  : dict, table_me
+00001160: 7461 5f64 6174 613a 204d 6574 6144 6174  ta_data: MetaDat
+00001170: 6148 6f6c 6465 7229 202d 3e20 4e6f 6e65  aHolder) -> None
+00001180: 3a0d 0a0d 0a20 2020 2072 656c 203d 205b  :....    rel = [
+00001190: 5d0d 0a20 2020 2066 6f72 2066 2069 6e20  ]..    for f in 
+000011a0: 7461 626c 655f 6d65 7461 5f64 6174 612e  table_meta_data.
+000011b0: 666f 7265 6967 6e5f 6b65 7973 3a0d 0a20  foreign_keys:.. 
+000011c0: 2020 2020 2020 2072 6566 6572 7265 645f         referred_
+000011d0: 7461 626c 6520 3d20 665b 2772 6566 6572  table = f['refer
+000011e0: 7265 645f 7461 626c 6527 5d0d 0a0d 0a20  red_table'].... 
+000011f0: 2020 2020 2020 2074 6d70 203d 2066 2770         tmp = f'p
+00001200: 6172 656e 745f 7b72 6566 6572 7265 645f  arent_{referred_
+00001210: 7461 626c 652e 6361 7069 7461 6c69 7a65  table.capitalize
+00001220: 2829 7d27 5c0d 0a20 2020 2020 2020 2020  ()}'\..         
+00001230: 2020 2066 2720 3d20 7265 6c61 7469 6f6e     f' = relation
+00001240: 7368 6970 2822 7b72 6566 6572 7265 645f  ship("{referred_
+00001250: 7461 626c 652e 6361 7069 7461 6c69 7a65  table.capitalize
+00001260: 2829 7d22 2c27 5c0d 0a20 2020 2020 2020  ()}",'\..       
+00001270: 2020 2020 2066 2720 6261 636b 5f70 6f70       f' back_pop
+00001280: 756c 6174 6573 3d22 6368 696c 6472 656e  ulates="children
+00001290: 5f7b 7461 626c 655f 6d65 7461 5f64 6174  _{table_meta_dat
+000012a0: 612e 6e61 6d65 2e63 6170 6974 616c 697a  a.name.capitaliz
+000012b0: 6528 297d 222c 275c 0d0a 2020 2020 2020  e()}",'\..      
+000012c0: 2020 2020 2020 2720 6c61 7a79 3d22 6a6f        ' lazy="jo
+000012d0: 696e 6564 2229 270d 0a20 2020 2020 2020  ined")'..       
+000012e0: 200d 0a20 2020 2020 2020 2074 6d70 203d   ..        tmp =
+000012f0: 2066 2222 220d 0a20 2020 207b 746d 707d   f"""..    {tmp}
+00001300: 2222 2220 0d0a 2020 2020 2020 2020 0d0a  """ ..        ..
+00001310: 2020 2020 2020 2020 7265 6c2e 6170 7065          rel.appe
+00001320: 6e64 2874 6d70 290d 0a0d 0a20 2020 2066  nd(tmp)....    f
+00001330: 6f72 206b 2c20 7620 696e 2074 6162 6c65  or k, v in table
+00001340: 5f6d 6574 615f 6461 7461 2e6d 756c 7469  _meta_data.multi
+00001350: 5f66 6f72 6569 676e 5f6b 6579 732e 6974  _foreign_keys.it
+00001360: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+00001370: 6966 206b 5b31 5d20 3d3d 2074 6162 6c65  if k[1] == table
+00001380: 5f6d 6574 615f 6461 7461 2e6e 616d 6520  _meta_data.name 
+00001390: 616e 6420 6e6f 7420 763a 0d0a 2020 2020  and not v:..    
+000013a0: 2020 2020 2020 2020 666f 7220 6368 696c          for chil
+000013b0: 645f 7461 626c 652c 2072 2069 6e20 7461  d_table, r in ta
+000013c0: 626c 655f 6d65 7461 5f64 6174 612e 6d75  ble_meta_data.mu
+000013d0: 6c74 695f 666f 7265 6967 6e5f 6b65 7973  lti_foreign_keys
+000013e0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+000013f0: 2020 2020 2020 2020 2020 2069 6620 723a             if r:
+00001400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001410: 2020 2020 2020 666f 7220 7274 2069 6e20        for rt in 
+00001420: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00001430: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00001440: 745b 2772 6566 6572 7265 645f 7461 626c  t['referred_tabl
+00001450: 6527 5d20 3d3d 2074 6162 6c65 5f6d 6574  e'] == table_met
+00001460: 615f 6461 7461 2e6e 616d 6520 5c0d 0a20  a_data.name \.. 
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 2020 206f 7220 7274 5b27 7265         or rt['re
+00001490: 6665 7272 6564 5f74 6162 6c65 275d 203d  ferred_table'] =
+000014a0: 3d20 7461 626c 655f 6d65 7461 5f64 6174  = table_meta_dat
+000014b0: 612e 6e61 6d65 2e63 6170 6974 616c 697a  a.name.capitaliz
+000014c0: 6528 293a 0d0a 2020 2020 2020 2020 2020  e():..          
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 746d 7020 3d20 6627 6368 696c 6472    tmp = f'childr
+000014f0: 656e 5f7b 6368 696c 645f 7461 626c 655b  en_{child_table[
+00001500: 315d 2e63 6170 6974 616c 697a 6528 297d  1].capitalize()}
+00001510: 275c 0d0a 2020 2020 2020 2020 2020 2020  '\..            
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 6627 203d 2072 656c 6174 696f 6e73 6869  f' = relationshi
+00001540: 7028 227b 6368 696c 645f 7461 626c 655b  p("{child_table[
+00001550: 315d 2e63 6170 6974 616c 697a 6528 297d  1].capitalize()}
+00001560: 222c 275c 0d0a 2020 2020 2020 2020 2020  ",'\..          
+00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001580: 2020 6627 2062 6163 6b5f 706f 7075 6c61    f' back_popula
+00001590: 7465 733d 2270 6172 656e 745f 7b74 6162  tes="parent_{tab
+000015a0: 6c65 5f6d 6574 615f 6461 7461 2e6e 616d  le_meta_data.nam
+000015b0: 652e 6361 7069 7461 6c69 7a65 2829 7d22  e.capitalize()}"
+000015c0: 2c27 5c0d 0a20 2020 2020 2020 2020 2020  ,'\..           
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2027 206c 617a 793d 226a 6f69 6e65 6422   ' lazy="joined"
+000015f0: 2927 0d0a 2020 2020 2020 2020 0d0a 2020  )'..        ..  
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 2020 746d 7020 3d20            tmp = 
+00001620: 6622 2222 0d0a 2020 2020 7b74 6d70 7d22  f"""..    {tmp}"
+00001630: 2222 200d 0a0d 0a20 2020 2020 2020 2020  "" ....         
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2072 656c 2e61 7070 656e 6428 746d     rel.append(tm
+00001660: 7029 0d0a 0d0a 2020 2020 2020 2020 2020  p)....          
+00001670: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00001680: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00001690: 2020 2069 6620 7265 6c3a 0d0a 2020 2020     if rel:..    
+000016a0: 2020 2020 696d 7020 3d20 2766 726f 6d20      imp = 'from 
+000016b0: 7371 6c61 6c63 6865 6d79 2e6f 726d 2069  sqlalchemy.orm i
+000016c0: 6d70 6f72 7420 7265 6c61 7469 6f6e 7368  mport relationsh
+000016d0: 6970 270d 0a20 2020 2020 2020 2069 6620  ip'..        if 
+000016e0: 696d 7020 6e6f 7420 696e 2064 6961 6c65  imp not in diale
+000016f0: 6374 5f69 6d70 6f72 7473 3a0d 0a20 2020  ct_imports:..   
+00001700: 2020 2020 2020 2020 2064 6961 6c65 6374           dialect
+00001710: 5f69 6d70 6f72 7473 2e61 7070 656e 6428  _imports.append(
+00001720: 696d 7029 0d0a 0d0a 2020 2020 636f 6465  imp)....    code
+00001730: 5f68 6f6c 6465 722e 7570 6461 7465 280d  _holder.update(.
+00001740: 0a20 2020 2020 2020 207b 2769 6d70 6f72  .        {'impor
+00001750: 7473 273a 2063 6f64 655f 686f 6c64 6572  ts': code_holder
+00001760: 5b27 696d 706f 7274 7327 5d20 2b20 6469  ['imports'] + di
+00001770: 616c 6563 745f 696d 706f 7274 737d 0d0a  alect_imports}..
+00001780: 2020 2020 2020 2020 290d 0a20 2020 2063          )..    c
+00001790: 6f64 655f 686f 6c64 6572 2e75 7064 6174  ode_holder.updat
+000017a0: 6528 7b27 7265 6c61 7469 6f6e 7327 3a20  e({'relations': 
+000017b0: 7265 6c7d 290d 0a0d 0a0d 0a64 6566 2072  rel})......def r
+000017c0: 6561 645f 7371 6c69 7465 5f61 6e64 5f62  ead_sqlite_and_b
+000017d0: 7569 6c64 5f63 6f64 6528 0d0a 2020 2020  uild_code(..    
+000017e0: 2020 2020 636f 6465 5f68 6f6c 6465 723a      code_holder:
+000017f0: 2064 6963 742c 2074 6162 6c65 5f6d 6574   dict, table_met
+00001800: 615f 6461 7461 3a20 4d65 7461 4461 7461  a_data: MetaData
+00001810: 486f 6c64 6572 2920 2d3e 204e 6f6e 653a  Holder) -> None:
+00001820: 0d0a 0d0a 2020 2020 5f63 6f6c 756d 6e73  ....    _columns
+00001830: 2863 6f64 655f 686f 6c64 6572 2c20 7461  (code_holder, ta
+00001840: 626c 655f 6d65 7461 5f64 6174 6129 0d0a  ble_meta_data)..
+00001850: 2020 2020 5f72 656c 6174 696f 6e73 2863      _relations(c
+00001860: 6f64 655f 686f 6c64 6572 2c20 7461 626c  ode_holder, tabl
+00001870: 655f 6d65 7461 5f64 6174 6129 0d0a 2020  e_meta_data)..  
+00001880: 2020 5f76 616c 6964 6174 696f 6e73 2863    _validations(c
+00001890: 6f64 655f 686f 6c64 6572 2c20 7461 626c  ode_holder, tabl
+000018a0: 655f 6d65 7461 5f64 6174 6129 0d0a 2020  e_meta_data)..  
+000018b0: 2020 7374 725f 7072 696e 7428 636f 6465    str_print(code
+000018c0: 5f68 6f6c 6465 722c 2074 6162 6c65 5f6d  _holder, table_m
+000018d0: 6574 615f 6461 7461 290d 0a              eta_data)..
```

### Comparing `alchemyrohan-0.4.0/alchemyrohan/wizard.py` & `alchemyrohan-0.4.1/alchemyrohan/wizard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,45 @@
 
 
-import os
-
-from alchemyrohan.meta_data import *
-
-
 __all__ = [
     'generate_model',
     'generate_code',
     'generate_init_file',
-    'construct_model',
-    'AlchemyRohanPathError'
-]   
-
-
-std_imports = [
-    'from sqlalchemy import Column'
-]
+    'construct_model'
+    ]
 
+import os
 
-class AlchemyRohanPathError(Exception): ...
+from sqlalchemy.exc import SQLAlchemyError
+from alchemyrohan.meta_data import MetaDataHolder
 
-class AlchemyRohanGenerateModelError(Exception): ...
+std_imports = ['from sqlalchemy import Column']
 
 
-def _write_template(
-        file: str, 
-        mode: str,
-        template: str
-        ) -> None:
-    
+def _write_template(file: str, mode: str, template: str) -> None:
     with open(file, mode) as f:
         f.write(template)
         f.close()
 
 
 def generate_model(
-    filename: str,
-    model_template: str,
-    abs_os_path_to_model: str
-    ) -> None:
-
-    if os.path.isdir(abs_os_path_to_model):
-        file = os.path.join(
-            abs_os_path_to_model, 
-            filename.capitalize() + '.py'
-            )
+        filename: str, model_template: str, path: str) -> None:
+    if os.path.isdir(path):
+        file = os.path.join(path, filename.capitalize() + '.py')
     else:
-        raise AlchemyRohanPathError(
-            f'No path: {abs_os_path_to_model}'
-            )
+        raise SQLAlchemyError(f'No path: {path}')
     
     try:
-        
         _write_template(file, 'w', model_template)
-
-    except Exception as e:
-        raise AlchemyRohanGenerateModelError(e)
+    except SQLAlchemyError as e:
+        raise SQLAlchemyError(e) from e
 
 
 def generate_code(
-    table_meta_data: MetaDataHolder,
-    py_path_to_model: str
-    ) -> dict:
+        table_meta_data: MetaDataHolder, py_path_to_model: str) -> dict:
 
     imp = f'from {py_path_to_model} import Base'
     if imp not in std_imports:
         std_imports.append(f'from {py_path_to_model} import Base')
 
     code_holder = {
         'name': table_meta_data.name,
@@ -79,88 +52,74 @@
     if table_meta_data.rdbms == 'sqlite':
         
         from alchemyrohan.sqlite import read_sqlite_and_build_code
 
         read_sqlite_and_build_code(code_holder, table_meta_data)
 
     elif table_meta_data.rdbms == 'mysql':  
-        
-        None
+        ...
         # TODO
 
     elif table_meta_data.rdbms == 'oracle':  
         
         from alchemyrohan.oracle import read_oracle_and_build_code
 
         read_oracle_and_build_code(code_holder, table_meta_data)
     
     else:
-        raise AlchemyRohanDatabaseError(
-            f'No supported dialect: {table_meta_data.rdbms}'
-            )
+        raise SQLAlchemyError(
+            f'No supported dialect: {table_meta_data.rdbms}')
 
     return code_holder
 
 
-def construct_model(
-    code_holder: dict
-    ) -> str:
+def construct_model(code_holder: dict) -> str:
 
-    def _add(tmp_list):
+    def _add(tmp_list: list) -> str:
         for e in tmp_list:
             yield e
 
-    BACKSLASH = '\n'
+    backslash = '\n'
 
     template = f"""
 
-{f'{BACKSLASH}'.join(_add(code_holder['imports']))}
+{f'{backslash}'.join(_add(code_holder['imports']))}
 
 
 {code_holder['class_name']}
     {code_holder['table_name']}
 
 {''.join(_add(code_holder['columns']))}
 
 {''.join(_add(code_holder['relations']))}
 
-    def __post_init__(self):
+    def validate(self):
 {''.join(code_holder['validations'])}
     
     def __str__(self):
 {code_holder['str_print']}
 """
     
     return template
 
 
-def generate_init_file(
-    table_name: str,
-    abs_os_path_to_model: str,
-    py_path_to_model: str
-    ) -> None:
-
-    file = os.path.join(
-        abs_os_path_to_model, 
-        '__init__.py'
-        )
+def generate_init_file(table_name: str, path: str, py_path: str) -> None:
+
+    file = os.path.join(path, '__init__.py')
 
     if os.path.isfile(file):
-        
         model_name = table_name.capitalize()
-        template = f'\nfrom {py_path_to_model}.{model_name} import {model_name}'
+        template = f'\nfrom {py_path}.{model_name} import {model_name}'
 
         _write_template(file, 'a', template)
-
     else:
-
         model_name = table_name.capitalize()
 
         template = f"""
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 
-from {py_path_to_model}.{model_name} import {model_name}
+from {py_path}.{model_name} import {model_name}
 """
         
         _write_template(file, 'w', template)
```

