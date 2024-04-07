# Comparing `tmp/firebirdsql_run-1.1.2a1.tar.gz` & `tmp/firebirdsql_run-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.1.2a1.tar", max compression
+gzip compressed data, was "firebirdsql_run-2.0.0a0.tar", max compression
```

## Comparing `firebirdsql_run-1.1.2a1.tar` & `firebirdsql_run-2.0.0a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:34:38.251083 firebirdsql_run-1.1.2a1/LICENSE
--rw-r--r--   0        0        0     3347 2024-04-07 15:34:38.251083 firebirdsql_run-1.1.2a1/README.md
--rw-r--r--   0        0        0     2797 2024-04-07 15:34:49.399071 firebirdsql_run-1.1.2a1/pyproject.toml
--rw-r--r--   0        0        0      241 2024-04-07 15:34:38.251083 firebirdsql_run-1.1.2a1/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     5312 2024-04-07 15:34:38.255083 firebirdsql_run-1.1.2a1/src/firebirdsql_run/main.py
--rw-r--r--   0        0        0     1859 2024-04-07 15:34:38.255083 firebirdsql_run-1.1.2a1/src/firebirdsql_run/type.py
--rw-r--r--   0        0        0     1264 2024-04-07 15:34:38.255083 firebirdsql_run-1.1.2a1/src/firebirdsql_run/util.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 firebirdsql_run-1.1.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     2284 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/README.md
+-rw-r--r--   0        0        0     2525 2024-02-21 12:22:38.486592 firebirdsql_run-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     5174 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/src/firebirdsql_run/main.py
+-rw-r--r--   0        0        0     1476 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/src/firebirdsql_run/type.py
+-rw-r--r--   0        0        0      632 2024-02-21 12:22:28.950417 firebirdsql_run-2.0.0a0/src/firebirdsql_run/util.py
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 firebirdsql_run-2.0.0a0/PKG-INFO
```

### Comparing `firebirdsql_run-1.1.2a1/LICENSE` & `firebirdsql_run-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.1.2a1/README.md` & `firebirdsql_run-2.0.0a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,106 @@
+Metadata-Version: 2.1
+Name: firebirdsql-run
+Version: 2.0.0a0
+Summary: Firebirdsql wrapper inspired by subprocess.run
+Home-page: https://github.com/DeadNews/firebirdsql-run
+License: MIT
+Keywords: firebird,sql,api
+Author: DeadNews
+Author-email: aurczpbgr@mozmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Database
+Requires-Dist: firebirdsql (>=1.2.3,<2.0.0)
+Project-URL: Repository, https://github.com/DeadNews/firebirdsql-run
+Description-Content-Type: text/markdown
+
 # firebirdsql-run
 
 > [Firebirdsql](https://github.com/nakagami/pyfirebirdsql/) wrapper inspired by [subprocess.run](https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
-[![PyPI: Version](https://img.shields.io/pypi/v/firebirdsql-run?logo=pypi&logoColor=white)](https://pypi.org/project/firebirdsql-run)
-[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/firebirdsql-run?logo=github&logoColor=white)](https://github.com/deadnews/firebirdsql-run/releases/latest)
-[![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/firebirdsql-run)
-[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/firebirdsql-run/main)
-[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/firebirdsql-run/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/firebirdsql-run/actions/workflows/main.yml)
-[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/firebirdsql-run?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/firebirdsql-run)
-
-**[Installation](#installation)** • **[Examples](#examples)** • **[Env Variables](#env-variables)**
+[![PyPI version](https://img.shields.io/pypi/v/firebirdsql-run)](https://pypi.org/project/firebirdsql-run)
+[![Main](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml)
+[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/firebirdsql-run/main)
+[![codecov](https://codecov.io/gh/DeadNews/firebirdsql-run/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/firebirdsql-run)
 
 ## Installation
 
 ```sh
 pip install firebirdsql-run
-# or
-poetry add firebirdsql-run
 ```
 
 ## Examples
 
-Execute a query with read-only access:
+- Execute a transaction
 
 ```py
-from firebirdsql_run import DBAccess, execute
-
-# Execute a query with read-only access.
-result = execute(query="SELECT * FROM table", db="database", access=DBAccess.READ_ONLY)
-
-# Output: List of dictionaries containing the query results.
-print(result.data)
+result = execute(query="SELECT * FROM table", db="database")
+print(result.data)  # Output: List of dictionaries containing the query results
 ```
 
-Execute a query with parameters and log the result:
+- Execute a transaction with custom parameters and an existing connection
 
 ```py
-# Execute a query with parameters.
-result = execute(query="INSERT INTO customers (name, age) VALUES (?, ?)", params=("John", 25))
-
-# Log the result.
-if result.returncode != 0:
-    logger.error(result)
-else:
-    logger.info(result)
+conn = connection(db="/path/to/database.fdb")
+result = execute("INSERT INTO customers (name, age) VALUES (?, ?)", params=("John", 25), use_conn=conn)
+print(result.returncode)  # Output: 0 (success)
+conn.close()
 ```
 
-Execute a query using the existing connection:
+## Representation of a completed transaction
 
-```py
-# Create a connection object.
-conn = connection(db="database", access=DBAccess.READ_ONLY)
-# Execute a query using the existing connection.
-result = execute(query="SELECT * FROM table", use_conn=conn)
-# Close the connection.
-conn.close()
+- Table
 
-# Output: Named tuple representing the completed transaction.
-print(result)
-```
+| maker | model | type |
+| ----- | ----- | ---- |
+| B     | 1121  | PC   |
+| A     | 1232  | PC   |
 
-An example of a successful transaction:
+- Success example
 
 ```py
->>> print(result)
 CompletedTransaction(
     host="127.0.0.1",
     db="database",
     user="TWUSER",
     access="READ_ONLY",
     returncode=0,
     exception="",
     query="SELECT * FROM table",
     params=(),
-    time=0.001,
     data=[
-        {'id': 1, 'name': 'John Doe', 'department': 'Sales'},
-        {'id': 2, 'name': 'Jane Smith', 'department': 'Sales'},
+        {"maker": "B", "model": 1121, "type": "PC"},
+        {"maker": "A", "model": 1232, "type": "PC"},
     ],
 )
 ```
 
-An example of a failed transaction:
+- Error example
 
 ```py
->>> print(result)
 CompletedTransaction(
     host="127.0.0.1",
     db="database",
     user="TWUSER",
     access="READ_ONLY",
     returncode=1,
     exception="Dynamic SQL Error\nSQL error code = -204\nTable unknown\ntable\nAt line 1, column 15\n",
     query="SELECT * FROM table",
     params=(),
-    time=0.001,
     data=[],
 )
 ```
 
-## Env Variables
+## Env variables
 
 ```ini
 FIREBIRD_KEY=
 ```
 
-The `FIREBIRD_KEY` environment variable can be overridden with the functions argument `passwd`.
+The `FIREBIRD_KEY` environment variable can be overridden with the function argument `passwd`.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `firebirdsql_run-1.1.2a1/pyproject.toml` & `firebirdsql_run-2.0.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.1.2-alpha.1"
+version = "2.0.0-alpha.0"
 description = "Firebirdsql wrapper inspired by subprocess.run"
-authors = ["DeadNews <deadnewsgit@gmail.com>"]
+authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/deadnews/firebirdsql-run"
-repository = "https://github.com/deadnews/firebirdsql-run"
-documentation = "https://deadnews.github.io/firebirdsql-run"
+homepage = "https://github.com/DeadNews/firebirdsql-run"
+repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
 classifiers = ["Operating System :: OS Independent", "Topic :: Database"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-firebirdsql = "^1.2.5"
+firebirdsql = "^1.2.3"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "^1.9.0"
-poethepoet = "^0.25.0"
-pyright = "^1.1.353"
-ruff = "^0.3.2"
+mypy = "^1.8.0"
+poethepoet = "^0.24.4"
+pyright = "^1.1.351"
+ruff = "^0.2.1"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.1.1"
+pytest = "^8.0.1"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.12.0"
 
-[tool.poetry.group.docs.dependencies]
-mkdocs = "^1.5.3"
-mkdocs-gen-files = "^0.5.0"
-mkdocs-literate-nav = "^0.6.1"
-mkdocs-material = "^9.5.13"
-mkdocstrings = "^0.24.1"
-mkdocstrings-python = "^1.9.0"
-
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
 mypy = "mypy ."
 pyright = "pyright ."
 ruff = "ruff check ."
 ruff-fmt = "ruff format ."
-lint.sequence = ["ruff", "ruff-fmt", "mypy", "pyright"]
+lint.sequence = ["ruff", "ruff-fmt", "mypy"]
 
 [tool.poe.tasks.test]
 cmd = "pytest --cov-report=xml"
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src --cov-report=term"
 testpaths = ["tests"]
```

### Comparing `firebirdsql_run-1.1.2a1/src/firebirdsql_run/main.py` & `firebirdsql_run-2.0.0a0/src/firebirdsql_run/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from firebirdsql import (
     Connection,
     connect,
 )
 
 from firebirdsql_run.type import CompletedTransaction, DBAccess
-from firebirdsql_run.util import Timer, get_env
+from firebirdsql_run.util import get_env
 
 
 def connection(
     db: Path | str,
     host: str = "127.0.0.1",
     port: int = 3050,
     user: str = "TWUSER",
@@ -27,15 +27,15 @@
         host: The host address of the server.
         port: The port number of the server.
         user: The username for authentication.
         passwd: The password. If omitted, it is taken from `FIREBIRD_KEY` environment variable.
         access: The access mode for the connection.
 
     Returns:
-        conn: The connection object.
+        Connection: The connection object.
     """
     return connect(
         host=getfqdn(host),
         database=f"{db}",
         port=port,
         user=user,
         password=passwd or get_env("FIREBIRD_KEY"),
@@ -64,29 +64,27 @@
         port: The port number of the server.
         user: The username for authentication.
         passwd: The password. If omitted, it is taken from `FIREBIRD_KEY` environment variable.
         access: The access mode for the connection.
         use_conn: An existing connection to use. Takes precedence over the default connection settings.
 
     Returns:
-        result: An named tuple containing the transaction details, including the query result.
+        CompletedTransaction: An named tuple containing the transaction details, including the query result.
     """
     conn: Connection | None = None
-    timer: Timer | None = None
-
     try:
         conn = use_conn or connection(
             host=host,
             db=db,
             port=port,
             user=user,
             passwd=passwd,
             access=access,
         )
-        with conn.cursor() as cur, Timer() as timer:
+        with conn.cursor() as cur:
             cur.execute(query=query, params=params)
             lines = cur.fetchall()
             descr = cur.description
 
     except Exception as e:  # noqa: BLE001
         data = []
         returncode = 1
@@ -100,36 +98,34 @@
         if conn is not None:
             conn.commit()
             if use_conn is None:
                 conn.close()
 
     return CompletedTransaction(
         host=host if conn is None else conn.hostname,
-        port=port if conn is None else conn.port,
         db=f"{db}" if conn is None else f"{conn.filename}",
         user=user if conn is None else f"{conn.user}",
         access=access.name if conn is None else DBAccess(conn.isolation_level).name,
         returncode=returncode,
         exception=exception,
         query=query,
         params=params,
-        time=0 if timer is None else round(timer.interval, 5),
         data=data,
     )
 
 
 def make_query(procname: str, params: tuple) -> str:
     """Create a query for a stored procedure in a Firebird database.
 
     Args:
         procname: The name of the stored procedure to execute.
         params: The parameters to pass to the stored procedure.
 
     Returns:
-        query: The query for the stored procedure.
+        str: The query for the stored procedure.
     """
     return f"EXECUTE PROCEDURE {procname} " + ",".join("?" * len(params))
 
 
 def callproc(
     procname: str,
     params: tuple = (),
@@ -151,15 +147,15 @@
         port: The port number of the server.
         user: The username for authentication.
         passwd: The password. If omitted, it is taken from `FIREBIRD_KEY` environment variable.
         access: The access mode for the connection.
         use_conn: An existing connection to use. Takes precedence over the default connection settings.
 
     Returns:
-        result: An named tuple containing the transaction details, including the query result.
+        CompletedTransaction: An named tuple containing the transaction details, including the query result.
     """
     return execute(
         query=make_query(procname, params),
         params=params,
         host=host,
         port=port,
         db=db,
```

### Comparing `firebirdsql_run-1.1.2a1/src/firebirdsql_run/type.py` & `firebirdsql_run-2.0.0a0/src/firebirdsql_run/type.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,57 +3,45 @@
 from datetime import datetime
 from enum import IntEnum
 from typing import NamedTuple
 
 from firebirdsql import consts
 
 FBTypes = str | float | datetime | None
-"""Type alias for the possible types of data returned by a FirebirdSQL query."""
-
 Dataset = list[dict[str, FBTypes]]
-"""Type alias for a list of dictionaries representing a dataset."""
 
 
 class DBAccess(IntEnum):
-    """Enumeration of access modes for FirebirdSQL connections.
-
-    Attributes:
-        READ_ONLY: Read-only access mode.
-        READ_WRITE: Read-write access mode.
-    """
+    """Enumeration of access modes for FirebirdSQL connections."""
 
     READ_ONLY = consts.ISOLATION_LEVEL_READ_COMMITED_RO
     READ_WRITE = consts.ISOLATION_LEVEL_READ_COMMITED
 
 
 class CompletedTransaction(NamedTuple):
     """Represents a completed transaction in a database.
 
     Attributes:
-        host (str): The host address of the server.
-        port (int): The port number of the server.
+        host (str): The host where the transaction was executed.
         db (str): The database where the transaction was executed.
         user (str): The user who executed the transaction.
         access (str): The access mode used for the transaction.
         returncode (int): The return code of the transaction execution.
-        exception (str): The exception message if the transaction failed.
+        exception (str): The error message, if any encountered during the transaction execution.
         query (str): The SQL query executed in the transaction.
         params (tuple): The parameters used in the SQL query.
-        time (float): The number of seconds it took to execute the transaction.
         data (Dataset): The data returned by the transaction, represented as a list of dictionaries.
     """
 
     host: str
     db: str
-    port: int
     user: str
     access: str
     returncode: int
     exception: str
     query: str
     params: tuple
-    time: float
     data: Dataset
 
 
 class ExecuteError(Exception):
     """Exception raised when an error occurs during the transaction execution."""
```

