# Comparing `tmp/morm-2.4.0.tar.gz` & `tmp/morm-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morm-2.4.0.tar", last modified: Sat Mar 30 09:04:34 2024, max compression
+gzip compressed data, was "morm-2.4.1.tar", last modified: Sun Apr  7 10:05:54 2024, max compression
```

## Comparing `morm-2.4.0.tar` & `morm-2.4.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-30 09:04:34.943597 morm-2.4.0/
--rw-rw-r--   0 jahid     (1000) jahid     (1001)     1703 2018-09-27 12:35:40.000000 morm-2.4.0/LICENSE
--rw-r--r--   0 jahid     (1000) jahid     (1001)    16655 2024-03-30 09:04:34.940264 morm-2.4.0/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)    15898 2024-03-08 06:33:45.000000 morm-2.4.0/README.md
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-30 09:04:34.936930 morm-2.4.0/morm/
--rw-r--r--   0 jahid     (1000) jahid     (1001)       50 2021-04-08 08:46:50.000000 morm-2.4.0/morm/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3243 2023-09-06 05:38:51.000000 morm-2.4.0/morm/admin.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    38327 2024-03-17 13:56:43.000000 morm-2.4.0/morm/db.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      636 2024-03-01 06:38:43.000000 morm-2.4.0/morm/dt.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      470 2021-04-08 08:46:50.000000 morm-2.4.0/morm/exceptions.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-30 09:04:34.936930 morm-2.4.0/morm/fields/
--rw-r--r--   0 jahid     (1000) jahid     (1001)       26 2021-04-08 08:46:50.000000 morm-2.4.0/morm/fields/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2047 2024-03-17 13:56:43.000000 morm-2.4.0/morm/fields/common.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    19186 2024-03-30 09:04:18.000000 morm-2.4.0/morm/fields/field.py
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)    24357 2024-03-01 06:38:43.000000 morm-2.4.0/morm/init_fap
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2915 2021-04-08 08:46:50.000000 morm-2.4.0/morm/meta.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    22305 2024-03-01 06:38:43.000000 morm-2.4.0/morm/migration.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    23329 2024-03-30 09:04:18.000000 morm-2.4.0/morm/model.py
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)       87 2021-03-16 13:12:06.000000 morm-2.4.0/morm/morm_admin
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1162 2024-03-01 06:38:43.000000 morm-2.4.0/morm/pg_models.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      541 2024-03-01 06:38:43.000000 morm-2.4.0/morm/q.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3533 2023-09-06 06:09:00.000000 morm-2.4.0/morm/utils.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-03-30 09:04:18.000000 morm-2.4.0/morm/version.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     2140 2024-03-01 06:38:43.000000 morm-2.4.0/morm/void.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-30 09:04:34.940264 morm-2.4.0/morm.egg-info/
--rw-r--r--   0 jahid     (1000) jahid     (1001)    16655 2024-03-30 09:04:34.000000 morm-2.4.0/morm.egg-info/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)      666 2024-03-30 09:04:34.000000 morm-2.4.0/morm.egg-info/SOURCES.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-03-30 09:04:34.000000 morm-2.4.0/morm.egg-info/dependency_links.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)       21 2024-03-30 09:04:34.000000 morm-2.4.0/morm.egg-info/requires.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        5 2024-03-30 09:04:34.000000 morm-2.4.0/morm.egg-info/top_level.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-03-30 09:04:34.943597 morm-2.4.0/setup.cfg
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1585 2024-03-07 08:55:57.000000 morm-2.4.0/setup.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-03-30 09:04:34.940264 morm-2.4.0/tests/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9442 2021-07-21 14:32:19.000000 morm-2.4.0/tests/test_Migration.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      929 2021-07-21 15:06:51.000000 morm-2.4.0/tests/test_admin.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      375 2021-07-21 15:06:51.000000 morm-2.4.0/tests/test_datetime.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    15408 2024-03-07 08:51:29.000000 morm-2.4.0/tests/test_db.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4648 2021-04-08 08:54:08.000000 morm-2.4.0/tests/test_field.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      335 2020-08-23 09:25:08.000000 morm-2.4.0/tests/test_meta.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)    17616 2021-03-15 07:33:40.000000 morm-2.4.0/tests/test_model.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      293 2020-08-23 09:44:54.000000 morm-2.4.0/tests/test_package.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      295 2021-03-10 12:56:49.000000 morm-2.4.0/tests/test_q.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      749 2020-08-23 09:53:12.000000 morm-2.4.0/tests/test_types.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      962 2020-08-04 06:22:01.000000 morm-2.4.0/tests/testd.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/
+-rw-rw-r--   0 jahid     (1000) jahid     (1001)     1703 2018-09-27 12:35:40.000000 morm-2.4.1/LICENSE
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    19914 2024-04-07 10:05:54.789579 morm-2.4.1/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    19104 2024-04-06 16:41:31.000000 morm-2.4.1/README.md
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.786246 morm-2.4.1/morm/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       50 2021-04-08 08:46:50.000000 morm-2.4.1/morm/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3243 2023-09-06 05:38:51.000000 morm-2.4.1/morm/admin.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2043 2024-04-06 16:27:25.000000 morm-2.4.1/morm/ctx.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    38299 2024-04-06 16:27:25.000000 morm-2.4.1/morm/db.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      636 2024-03-01 06:38:43.000000 morm-2.4.1/morm/dt.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      470 2021-04-08 08:46:50.000000 morm-2.4.1/morm/exceptions.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.786246 morm-2.4.1/morm/fields/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       26 2021-04-08 08:46:50.000000 morm-2.4.1/morm/fields/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2047 2024-03-17 13:56:43.000000 morm-2.4.1/morm/fields/common.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    25094 2024-04-06 17:48:27.000000 morm-2.4.1/morm/fields/field.py
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)    24349 2024-04-06 16:48:50.000000 morm-2.4.1/morm/init_fap
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2915 2021-04-08 08:46:50.000000 morm-2.4.1/morm/meta.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    22305 2024-03-01 06:38:43.000000 morm-2.4.1/morm/migration.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    24397 2024-04-06 16:48:50.000000 morm-2.4.1/morm/model.py
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)       87 2021-03-16 13:12:06.000000 morm-2.4.1/morm/morm_admin
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1162 2024-03-01 06:38:43.000000 morm-2.4.1/morm/pg_models.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      541 2024-03-01 06:38:43.000000 morm-2.4.1/morm/q.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3533 2023-09-06 06:09:00.000000 morm-2.4.1/morm/utils.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-06 16:27:25.000000 morm-2.4.1/morm/version.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     2140 2024-03-01 06:38:43.000000 morm-2.4.1/morm/void.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/morm.egg-info/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    19914 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      678 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/SOURCES.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/dependency_links.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       44 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/requires.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        5 2024-04-07 10:05:54.000000 morm-2.4.1/morm.egg-info/top_level.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-07 10:05:54.789579 morm-2.4.1/setup.cfg
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1614 2024-04-06 16:48:50.000000 morm-2.4.1/setup.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 10:05:54.789579 morm-2.4.1/tests/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9442 2021-07-21 14:32:19.000000 morm-2.4.1/tests/test_Migration.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      929 2021-07-21 15:06:51.000000 morm-2.4.1/tests/test_admin.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      357 2024-04-05 13:26:01.000000 morm-2.4.1/tests/test_datetime.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    15408 2024-03-07 08:51:29.000000 morm-2.4.1/tests/test_db.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4648 2021-04-08 08:54:08.000000 morm-2.4.1/tests/test_field.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      335 2020-08-23 09:25:08.000000 morm-2.4.1/tests/test_meta.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)    17616 2021-03-15 07:33:40.000000 morm-2.4.1/tests/test_model.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      293 2020-08-23 09:44:54.000000 morm-2.4.1/tests/test_package.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      295 2021-03-10 12:56:49.000000 morm-2.4.1/tests/test_q.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      749 2020-08-23 09:53:12.000000 morm-2.4.1/tests/test_types.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      962 2020-08-04 06:22:01.000000 morm-2.4.1/tests/testd.py
```

### Comparing `morm-2.4.0/LICENSE` & `morm-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/PKG-INFO` & `morm-2.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: morm
-Version: 2.4.0
-Summary: A minimal asynchronous database object relational mapper
-Home-page: https://github.com/neurobin/python-morm
-Author: Md. Jahidul Hamid
-Author-email: jahidulhamid@yahoo.com
-License: BSD
-Keywords: async,orm,postgresql
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: asyncpg
-Requires-Dist: nest_asyncio
-
 [![Build status image](https://travis-ci.org/neurobin/python-morm.svg?branch=release)](https://travis-ci.com/github/neurobin/python-morm) [![Coverage Status](https://coveralls.io/repos/github/neurobin/python-morm/badge.svg?branch=release)](https://coveralls.io/github/neurobin/python-morm?branch=release)
 
 A minimal asynchronous database object relational mapper that supports transaction, connection pool and migration.
 
 Currently supports *PostgreSQL* with `asyncpg`.
 
 # Install
@@ -79,15 +57,15 @@
 
 class User(Base):
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
 ```
 
-An advanced model could look like this:
+Advanced models could look like this:
 
 ```python
 import random
 
 def get_rand():
     return random.randint(1, 9)
 
@@ -100,17 +78,24 @@
         # see morm.meta.Meta for supported meta attributes.
 
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
     profession = Field('varchar(255)', default='Unknown')
     random = Field('integer', default=get_rand) # function can be default
+
+class UserProfile(User):
+    class Meta:
+        proxy = True
+        exclude_fields_down = ('password',) # exclude sensitive fields in retrieval
+        # this will also exclude this field from swagger docs if you are
+        # using our fastAPI framework
 ```
 
-**Rules for field names**
+## Rules for field names
 
 1. Must not start with an underscore (`_`). You can set arbitrary variables to the model instance with names starting with underscores; normally you can not set any variable to a model instance. Names not starting with an underscore are all expected to be field names, variables or methods that are defined during class definition.
 2. `_<name>_` such constructions are reserved for pre-defined overridable methods such as `_pre_save_`, `_post_save_`, etc..
 3. Name `Meta` is reserved to be a class that contains configuration of the model for both model and model instance.
 
 
 ## Initialize a model instance
@@ -475,7 +460,58 @@
 
 To run the production app as a service with `systemctl start app`, copy the **app.service** to `/etc/systemd/system`
 
 **Notes:**
 
 * You can setup your venv path in the `vact` file. To activate the venv with all the environment vars, just run `. vact`.
 * An environment file `.env_APP` is created in your home directory containing dev and production environments.
+
+
+# Pydantic support
+
+You can get pydantic model from any morm model using the `_pydantic_` method, e.g `User._pydantic_()` would give you the pydantic version of your `User` model. The `_pydantic_()` method supports a few parameters to customize the generated pydantic model:
+
+* `up=False`: Defines if the model should be for up (update into database) or down (retrieval from database).
+* `suffix=None`: You can add a suffix to the name of the generated pydantic model.
+* `include_validators=None`: Whether the validators defined in each field (with validator parameter) should be added as pydantic validators. When `None` (which is default) validators will be included for data update into database (i.e for `up=True`). Note that, the model field validators return True or False, while pydantic validators return the value, this conversion is automatically added internally while generating the pydantic model.
+
+If you are using our FastAPI framework, generating good docs for user data retrieval using the User model would be as simple as:
+
+```python
+@router.get('/crud/{model}', responses=Res.schema_all(User._pydantic_())
+async def get(request: Request, model: str, vals = '', col: str='', comp: str='=$1'):
+     if some_authentication_error:
+        raise Res(status=Res.Status.unauthorized, errors=['Invalid Credentials!']) # throws a correct HTTP error with additional error message
+    ...
+    return Res(user)
+```
+
+The above will define all common response types: 200, 401, 403, etc.. and the 200 success response will show an example with correct data types from your User model and will show only the fields that are allowed to be shown (controlled with `exclude_fields_down` or `fields_down` in the `User.Meta`).
+
+
+# JSON handling
+
+It may seem tempting to add json and jsonb support with `asyncpg.Connection.set_type_codec()` method, but we have not provided any option to use this method easily in `morm`, as it turned out to be making the queries very very slow. If you want to handle json, better add a `_clean_{field}` method in your model and  do the conversion there:
+
+```python
+class User(Base):
+    settings = Field('jsonb')
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
+
+If you want to have it converted to json during data retrieval from database as well, pass a validator which should return False if it is not json, and then pass a modifier in the field to do the conversion. Do note that modifier only runs if validator fails. Thus you will set and get the value as json (list or dict) and the `_clean_settings` will covert it back to text during database insert or update.
+
+```python
+class User(Base):
+    settings = Field('jsonb', validator=lambda x: isinstance(x, list|dict), modifier=lambda x: json.loads(x))
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
```

### Comparing `morm-2.4.0/README.md` & `morm-2.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: morm
+Version: 2.4.1
+Summary: A minimal asynchronous database object relational mapper
+Home-page: https://github.com/neurobin/python-morm
+Author: Md. Jahidul Hamid
+Author-email: jahidulhamid@yahoo.com
+License: BSD
+Keywords: async,orm,postgresql
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: asyncpg
+Requires-Dist: nest_asyncio
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: orjson
+
 [![Build status image](https://travis-ci.org/neurobin/python-morm.svg?branch=release)](https://travis-ci.com/github/neurobin/python-morm) [![Coverage Status](https://coveralls.io/repos/github/neurobin/python-morm/badge.svg?branch=release)](https://coveralls.io/github/neurobin/python-morm?branch=release)
 
 A minimal asynchronous database object relational mapper that supports transaction, connection pool and migration.
 
 Currently supports *PostgreSQL* with `asyncpg`.
 
 # Install
@@ -57,15 +81,15 @@
 
 class User(Base):
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
 ```
 
-An advanced model could look like this:
+Advanced models could look like this:
 
 ```python
 import random
 
 def get_rand():
     return random.randint(1, 9)
 
@@ -78,17 +102,24 @@
         # see morm.meta.Meta for supported meta attributes.
 
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
     profession = Field('varchar(255)', default='Unknown')
     random = Field('integer', default=get_rand) # function can be default
+
+class UserProfile(User):
+    class Meta:
+        proxy = True
+        exclude_fields_down = ('password',) # exclude sensitive fields in retrieval
+        # this will also exclude this field from swagger docs if you are
+        # using our fastAPI framework
 ```
 
-**Rules for field names**
+## Rules for field names
 
 1. Must not start with an underscore (`_`). You can set arbitrary variables to the model instance with names starting with underscores; normally you can not set any variable to a model instance. Names not starting with an underscore are all expected to be field names, variables or methods that are defined during class definition.
 2. `_<name>_` such constructions are reserved for pre-defined overridable methods such as `_pre_save_`, `_post_save_`, etc..
 3. Name `Meta` is reserved to be a class that contains configuration of the model for both model and model instance.
 
 
 ## Initialize a model instance
@@ -453,7 +484,58 @@
 
 To run the production app as a service with `systemctl start app`, copy the **app.service** to `/etc/systemd/system`
 
 **Notes:**
 
 * You can setup your venv path in the `vact` file. To activate the venv with all the environment vars, just run `. vact`.
 * An environment file `.env_APP` is created in your home directory containing dev and production environments.
+
+
+# Pydantic support
+
+You can get pydantic model from any morm model using the `_pydantic_` method, e.g `User._pydantic_()` would give you the pydantic version of your `User` model. The `_pydantic_()` method supports a few parameters to customize the generated pydantic model:
+
+* `up=False`: Defines if the model should be for up (update into database) or down (retrieval from database).
+* `suffix=None`: You can add a suffix to the name of the generated pydantic model.
+* `include_validators=None`: Whether the validators defined in each field (with validator parameter) should be added as pydantic validators. When `None` (which is default) validators will be included for data update into database (i.e for `up=True`). Note that, the model field validators return True or False, while pydantic validators return the value, this conversion is automatically added internally while generating the pydantic model.
+
+If you are using our FastAPI framework, generating good docs for user data retrieval using the User model would be as simple as:
+
+```python
+@router.get('/crud/{model}', responses=Res.schema_all(User._pydantic_())
+async def get(request: Request, model: str, vals = '', col: str='', comp: str='=$1'):
+     if some_authentication_error:
+        raise Res(status=Res.Status.unauthorized, errors=['Invalid Credentials!']) # throws a correct HTTP error with additional error message
+    ...
+    return Res(user)
+```
+
+The above will define all common response types: 200, 401, 403, etc.. and the 200 success response will show an example with correct data types from your User model and will show only the fields that are allowed to be shown (controlled with `exclude_fields_down` or `fields_down` in the `User.Meta`).
+
+
+# JSON handling
+
+It may seem tempting to add json and jsonb support with `asyncpg.Connection.set_type_codec()` method, but we have not provided any option to use this method easily in `morm`, as it turned out to be making the queries very very slow. If you want to handle json, better add a `_clean_{field}` method in your model and  do the conversion there:
+
+```python
+class User(Base):
+    settings = Field('jsonb')
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
+
+If you want to have it converted to json during data retrieval from database as well, pass a validator which should return False if it is not json, and then pass a modifier in the field to do the conversion. Do note that modifier only runs if validator fails. Thus you will set and get the value as json (list or dict) and the `_clean_settings` will covert it back to text during database insert or update.
+
+```python
+class User(Base):
+    settings = Field('jsonb', validator=lambda x: isinstance(x, list|dict), modifier=lambda x: json.loads(x))
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
```

### Comparing `morm-2.4.0/morm/admin.py` & `morm-2.4.1/morm/admin.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/db.py` & `morm-2.4.1/morm/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     Args:
         record (Record): Record object.
         model_class (ModelType): Model class
 
     Returns:
         Model: Model instance.
     """
-    new_record = model_class()
+    mob = model_class()
     for k,v in record.items():
-        new_record.Meta._fromdb_.append(k)
-        setattr(new_record, k, v)
-    return new_record
+        mob.Meta._fromdb_.append(k)
+        setattr(mob, k, v)
+    return mob
 
 
 class Pool(object):
     """Open database connection pool.
 
     ```python
     from morm.db import Pool
```

### Comparing `morm-2.4.0/morm/dt.py` & `morm-2.4.1/morm/dt.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/fields/common.py` & `morm-2.4.1/morm/fields/common.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/fields/field.py` & `morm-2.4.1/morm/fields/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 __author__ = 'Md Jahidul Hamid <jahidulhamid@yahoo.com>'
 __copyright__ = 'Copyright © Md Jahidul Hamid <https://github.com/neurobin/>'
 __license__ = '[BSD](http://www.opensource.org/licenses/bsd-license.php)'
 __version__ = '0.0.1'
 
 import copy, inspect
 from typing import Any, Optional, Callable, Tuple, Dict, List, Union
+from decimal import Decimal
+from typing_extensions import Annotated
+from pydantic import Field as pdField, AfterValidator, ValidationError
 from morm.void import Void
 import morm.exceptions as ex
 
 
 def always_valid(value: Any)-> bool:
     """Always return True regradless of the value.
 
@@ -30,14 +33,25 @@
         value (Any): Any value.
 
     Returns:
         Any: The save value that is passed.
     """
     return value
 
+def wrap_validator(func, help=''):
+    def wrapped(v):
+        if func(v):
+            return v
+        msg = f"Validation failed for {v}"
+        if help == 'auto':
+            msg += ". Reason: " + inspect.getsource(func).split('\n')[0].strip()
+        elif help:
+            msg += f". Reason: {help}"
+        raise ValidationError(msg)
+    return wrapped
 
 class ColumnConfig():
     """Config container for each column/feild.
 
     This class is easily derivable from a json config.
     """
     def __init__(self, **kwargs):
@@ -130,15 +144,15 @@
         Returns:
             Tuple[str, str]: sql query, message
         """
         # TODO: handle alter settings.
         queries = []
         msgs = []
         if self.conf['sql_type'] != prev.conf['sql_type']:
-            q = f'ALTER TABLE "{table_name}" ALTER COLUMN "{self.conf["column_name"]}" SET DATA TYPE {self.conf["sql_type"]};'
+            q = f'ALTER TABLE "{table_name}" ALTER COLUMN "{self.conf["column_name"]}" SET DATA TYPE {self.conf["sql_type"]} USING "{self.conf["column_name"]}"::{self.conf["sql_type"]};'
             queries.append(q)
             msg = f"\n* > MODIFY: {prev.conf['column_name']}: {prev.conf['sql_type']} --> {self.conf['sql_type']}"
             msgs.append(msg)
 
         settings_query, msg = self.get_query_column_alter(prev.conf['sql_alter'], table_name) # type: ignore
         if settings_query:
             queries.append(settings_query)
@@ -219,14 +233,42 @@
     if value.lower() in ['null','none']: return 'null'
     try:
         if '.' in value: return float(value)
         return int(value)
     except:
         return f"'{value}'"
 
+def sqlTypeToNative(sql_type: str, optional=False, containerType=None) -> Any:
+    '''Convert sql type to python native type.
+
+    Returns:
+        Tuple[Any, Any]: (native_type, raw_type)
+    '''
+    dtype = str
+    if 'interval' in sql_type:
+        dtype = str
+    if 'int' in sql_type or 'serial' in sql_type:
+        dtype = int
+    elif 'float' in sql_type or 'double' in sql_type or 'real' in sql_type:
+        dtype = float
+    elif 'money' in sql_type or 'numeric' in sql_type or 'decimal' in sql_type:
+        dtype = Decimal
+    elif 'bool' in sql_type:
+        dtype = bool
+    elif 'json' in sql_type:
+        dtype = Union[Dict[str, Any], List]
+    elif 'bytea' in sql_type:
+        dtype = bytearray
+
+    if '[' in sql_type or 'array' in sql_type.lower():
+        containerType = List
+    if optional:
+        return Optional[dtype] if containerType is None else Optional[containerType[dtype]], dtype
+    return dtype if containerType is None else containerType[dtype], dtype
+
 
 class Field(object):
     """Initialize the Field object with data type (sql).
 
     Example sql_type: `'varchar(255)'`, `'integer'`, etc..
 
     Example sql_onadd: `'PRIMARY KEY'`, `'NOT NULL'`, `'UNIQUE'` etc..
@@ -249,68 +291,99 @@
 
     {table} and {column} will be replaced with table name,
     and column name respectively.
 
 
     Args:
         sql_type (str): Data type in SQL.
+        max_length (int, optional): Maximum length of the field. Defaults to None.
+        max_digits (int, optional): Maximum digits for numeric type. Defaults to None.
+        decimal_places (int, optional): Decimal places for numeric type. Defaults to None.
+        array_dimension (Tuple[int, ...], optional): Array dimension. Defaults to ().
         sql_onadd (str): sql to add in ADD clause after 'ADD COLUMN column_name data_type'
         sql_ondrop (str): Either 'RESTRICT' or 'CASCADE'.
         sql_alter (Tuple[str]): Alter column queries; Example: ('ALTER TABLE "{table}" ALTER COLUMN "{column}" DROP DEFAULT',).
         sql_engine (str): db engine, postgresql, mysql etc.. Defaults to 'postgresql'
         default (Any, optional): Pythonic default value (can be a callable). Defaults to Void. (Do not use mutable values, use function instead)
         value (Any, optional): Set a value that will prevail unless changed manually. Can be a function. Useful to make updated_at like fields.
+        unique (bool, optional): Whether the field is unique. Defaults to False.
+        index (str, optional): Index type. Defaults to None. 'btree', 'hash', 'gin', 'gist', prepend with - to remove the index.
         choices (Tuple[Tuple[str, Any], ...], optional): choices tuple: (('Name of choice', 'value'), ...)
         help_text (str, optional):  help text to describe this field.
         validator (callable, optional): A callable that accepts exactly one argument. Validates the value in `clean` method. Defaults to always_valid.
         modifier (callable, optional): A callable that accepts exactly one argument. Modifies the value if validation fails when the `clean` method is called.. Defaults to nomodify.
         fallback (bool, optional): Whether invalid value should fallback to default value suppressing exception. (May hide bugs in your program)
     """
     def __init__(self, sql_type: str,
+                max_length: Optional[int]=None, # added to sql_type e.g varchar(max_length)
+                max_digits: Optional[int]=None, # added to sql_type e.g numeric(max_digits, decimal_places)
+                decimal_places: Optional[int]=None, # added to sql_type e.g numeric(max_digits, decimal_places)
+                array_dimension: Tuple[int, ...] = (),
                 sql_onadd='',
                 sql_ondrop='',
                 sql_alter: Tuple[str, ...] = (),
                 sql_engine='postgresql',
                 default: Any=Void,
                 value: Any=Void,
                 unique=False,
                 index=None, # 'btree', 'hash', 'gin', 'gist', prepend with - to remove the index.
                 choices: Tuple[Tuple[str, Any], ...] = (),
                 help_text: str = '',
                 validator: Callable=always_valid,
+                validator_text: str = '',
                 modifier: Callable=nomodify,
                 fallback=False,): # if you add new param here, update __repr__ method
         # Rules for using a variable name here as local variables go into the self._json_:
         # 1. Must precede with underscore if not in the parameter list
         # 2. Make sure to exclude unnecessary variables in the self._json_ like 'self' etc..
         _init_args = list(locals().keys())[1:] # this must be the first line here in __init__
+        self.max_length = max_length
+        self.max_digits = max_digits
+        self.decimal_places = decimal_places
+        self.validator_text = validator_text
+        self.native_type, self.native_type_raw = sqlTypeToNative(sql_type, optional=default is not Void, containerType=None if not array_dimension else List)
+        if max_length and self.native_type_raw is not str:
+            raise ValueError(f"max_length is only valid for types that are string like, {sql_type} given.")
+        if max_length or max_digits:
+            if '(' in sql_type:
+                raise ValueError(f"Please remove (max_length) or (max_digits) from sql_type: {sql_type} as you are using max_length or max_digits explicitly.")
+        if max_length:
+            sql_type = f'{sql_type}({max_length})'
+        elif max_digits and decimal_places:
+            sql_type = f'{sql_type}({max_digits}, {decimal_places})'
+        elif max_digits:
+            sql_type = f'{sql_type}({max_digits})'
+        if array_dimension:
+            if '[' in sql_type or 'array' in sql_type.lower():
+                raise ValueError(f"Please remove array indicator from sql_type: {sql_type} as you are using array_dimension.")
+            sql_type = f'{sql_type}'+ ''.join([f'[{x}]' for x in array_dimension])
 
         self.sql_type = sql_type
         _unique_constraint = '__UNQ_{table}_{column}__'
         if unique:
             _sql_unique = 'ALTER TABLE "{table}" ADD CONSTRAINT "%s" UNIQUE ("{column}");' % (_unique_constraint,)
         else:
             _sql_unique = 'ALTER TABLE "{table}" DROP CONSTRAINT IF EXISTS "%s";' % (_unique_constraint,)
         if index:
-            idx_remove = True if index[0] == '-' else False
-            if idx_remove:
+            _idx_remove = True if index[0] == '-' else False
+            if _idx_remove:
                 index = index[1:]
             if index not in ['btree', 'hash', 'gin', 'gist', 'spgist', 'brin']:
                 raise ValueError(f"Invalid index type: {index}")
             _index_name = '__IDX_{table}_{column}_'+index+'__'
-            if not idx_remove:
+            if not _idx_remove:
                 _sql_index = 'CREATE INDEX IF NOT EXISTS "%s" ON "{table}" USING %s ("{column}")' % (_index_name, index)
             else:
                 _sql_index = 'DROP INDEX IF EXISTS "%s"' % (_index_name,)
         sql_alter = (_sql_unique, *sql_alter)
         if index:
             sql_alter = (*sql_alter, _sql_index)
         # handle default
         if isinstance(default, (int, float, str, bool)) or is_sql_array(default):
-            sql_alter = (*sql_alter, "ALTER TABLE \"{table}\" ALTER COLUMN \"{column}\" SET DEFAULT "+f"{sql_val(default, sql_type)};")
+            sql_alter = (*sql_alter, "ALTER TABLE \"{table}\" ALTER COLUMN \"{column}\" SET DEFAULT "+f"{sql_val(default, sql_type)}::{sql_type};")
         self.sql_conf = ColumnConfig(sql_type=sql_type, sql_onadd=sql_onadd, sql_ondrop=sql_ondrop, sql_alter=sql_alter, sql_engine=sql_engine)
         self.validator = validator
         self.modifier = modifier
         self._name = ''
         self.fallback = fallback
         self._is_perpetual_default = False
         if value is not Void:
@@ -326,15 +399,15 @@
         # make a json
         self._json_ = {
             '_name': self.name,
             '_init_args': _init_args,
         }
         args = locals()
         for k,v in args.items():
-            if k in ['self', '_init_args']: continue
+            if k in ['self', '_init_args'] or k.startswith('_'): continue
             if callable(v):
                 v_src = inspect.getsource(v)
                 v_src = v_src.split('\n')[0].strip()+' ...'
                 self._json_[k] = v_src
             else:
                 self._json_[k] = 'Void' if v == Void else v
 
@@ -363,28 +436,80 @@
     def to_json(self):
         res = self._json_.copy()
         res['_name'] = self.name
         res['_repr'] = self.__repr__()
         del res['_init_args']
         return res
 
+    def to_pydantic_override(self, dType) -> Tuple[Any, Dict[str, Any]]:
+        '''Override this method to return the type and a dict of pydantic field overrides.
+
+        you can return a different dType to change the type of the field in pydantic model.
+
+        Parameters:
+            dType: The type that is returned by the default to_pydantic method.
+
+        '''
+        return dType, {}
+
+    def to_pydantic(self, include_validator=True) -> Tuple[Any, pdField]:
+        """Get the pydantic field with type
+
+        Returns:
+            (dataType, pydantic.Field)
+        """
+        opts = {
+            'description': self.help_text,
+            'title': self.name.replace('_', ' ').title(),
+        }
+        if self.default is not Void:
+            k = 'default_factory' if callable(self.default) else 'default'
+            opts[k] = self.default
+        if self.max_length: opts['max_length'] = self.max_length
+        if self.max_digits: opts['max_digits'] = self.max_digits
+        if self.decimal_places: opts['decimal_places'] = self.decimal_places
+
+        # Final processing: overrides
+        dType, _opts = self.to_pydantic_override(self.native_type)
+        if include_validator:
+            dType = Annotated[dType, AfterValidator(wrap_validator(self.validator, help=self.validator_text))]
+        opts.update(_opts)
+        return dType, pdField(**opts)
+
     def __invert__(self):
         return self.name
 
     @property
     def name(self) -> str:
         """Get the name of the field"""
         return self._name
 
     @name.setter
     def name(self, v: str):
         """Set the name of the field"""
         self._name = v
         self.sql_conf.conf['column_name'] = v
 
+    def field_validator_error(self, value: Any, e=None) -> str:
+        """Get the error message for the validator
+
+        Args:
+            value (Any): value
+            e (Exception, optional): Exception. Defaults to None.
+
+        Returns:
+            str: error message
+        """
+        emsg = f"Value of type '{type(value).__name__}' did not pass validation check for field '{self.name}'"
+        if self.validator_text:
+            emsg += f". {self.validator_text}"
+        if e:
+            emsg += f". Reason: {str(e)}"
+        return emsg
+
     def clean(self, value: Any, fallback: bool=False):
         """Clean the value by calling validator -> modifier -> validator
 
         If fallback is set to True, value that does not pass the
         validator will not raise any exception and will return the
         default value.
 
@@ -395,24 +520,29 @@
 
         Raises:
             ValueError: If validation fails
 
         Returns:
             Any: value
         """
-        if not self.validator(value):
-            value = self.modifier(value)
-        else:
+        try:
+            if not self.validator(value):
+                value = self.modifier(value)
+            else:
+                return value
+            # the value may have been changed, try to validate again
+            if not self.validator(value):
+                if fallback:
+                    return self.get_default()
+                raise ValueError(self.field_validator_error(value))
             return value
-        # the value may have been changed, try to validate again
-        if not self.validator(value):
-            if fallback:
-                return self.get_default()
-            raise ValueError("Value (%s) (type: %s) did not pass validation check for '%s'" % (str(value), type(value), self.name,))
-        return value
+        except ValidationError:
+            raise
+        except Exception as e:
+            raise ValueError(self.field_validator_error(value,e=e)) from e
 
     def get_default(self):
         """Get the default value.
 
         The default given is treated as a callable first, if it fails
         then it is returned as a value.
```

### Comparing `morm-2.4.0/morm/init_fap` & `morm-2.4.1/morm/init_fap`

 * *Files 0% similar despite different names*

```diff
@@ -324,22 +324,22 @@
 
 "
 
     ["$root/core/schemas/res.py"]="'''Response schemas'''
 import typing, re
 from starlette.datastructures import MutableHeaders
 from starlette.exceptions import HTTPException
-from fastapi.responses import JSONResponse, ORJSONResponse
+from fastapi.responses import ORJSONResponse
 from starlette.background import BackgroundTask
 from pydantic import Field, create_model
 from $app_py_path.core.schemas.internal import _global_Res_, DataType, _Res
 from $app_py_path.core.schemas.status import Status, Map
 
 
-class Res(HTTPException, JSONResponse, typing.Generic[DataType]):
+class Res(HTTPException, ORJSONResponse, typing.Generic[DataType]):
     '''Response schema, can be raised as exception or returned as response
 
     #### Res.schema
     New response schema can be created using the Res.schema() class method.
     This methods creates a new response schema with custom default status code and message if not exists already.
 
     #### Res.schema_all
@@ -359,15 +359,15 @@
         media_type: typing.Optional[str] = None,
         background: typing.Optional[BackgroundTask] = None
     ) -> None:
         '''Response schema class, can be raised as Exception or returned as a response directly'''
         HTTPException.__init__(self, status.status, detail=status.msg, headers=headers)
         errors = [status.msg] if status != Status.success and not errors else errors
         ResClass = self.__class__.schema(DataType, status)
-        JSONResponse.__init__(self, content=ResClass(data=data,status=status.status, msg=status.msg, errors=errors, warnings=warnings).model_dump(), status_code=status.status, headers=headers, media_type=media_type, background=background)
+        ORJSONResponse.__init__(self, content=ResClass(data=data,status=status.status, msg=status.msg, errors=errors, warnings=warnings).model_dump(), status_code=status.status, headers=headers, media_type=media_type, background=background)
 
     @classmethod
     def schema(cls, dType: DataType, status: Map):
         '''Create and return response schema with custom default status code and message if not exists already'''
         dataTypeName = dType.__name__ if hasattr(dType, '__name__') else str(dType)
         dataTypeName = re.sub(r'[^\w]', '_', dataTypeName)
         name = f'Res{dataTypeName}{status.status}{status.msg}'
@@ -389,15 +389,15 @@
             if isinstance(v, Map):
                 dtype = dType if v.status == 200 else None
                 res_all[v.status] = {'description': v.msg, 'model': Res.schema(dtype, v)}
         return res_all
 
     @property
     def headers(self) -> MutableHeaders:
-        return super(JSONResponse, self).headers
+        return super(ORJSONResponse, self).headers
 
     @headers.setter
     def headers(self, v: dict|None) -> MutableHeaders:
         self.init_headers(v)
 
 "
```

### Comparing `morm-2.4.0/morm/meta.py` & `morm-2.4.1/morm/meta.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/migration.py` & `morm-2.4.1/morm/migration.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/model.py` & `morm-2.4.1/morm/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Model.
 """
 
 __author__ = 'Md Jahidul Hamid <jahidulhamid@yahoo.com>'
 __copyright__ = 'Copyright © Md Jahidul Hamid <https://github.com/neurobin/>'
 __license__ = '[BSD](http://www.opensource.org/licenses/bsd-license.php)'
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 import inspect, re
 from typing import Dict, List, Tuple, Any, Iterator, ClassVar
 import copy
+import pydantic
 from morm.fields.field import Field, FieldValue
 from morm.void import Void
 import morm.meta as mt      # for internal use
 
 # morm.db must not be imported here.
 
 Meta = mt.Meta  # For client use
@@ -256,20 +257,49 @@
         res = {}
         fields = self._get_fields_(up)
         all_fields = self._get_all_fields_()
         for k in fields:
             res[k] = all_fields[k].to_json()
         return res
 
+    def _pydantic_(self, up=False, suffix=None, include_validators=None):
+        '''Create a pydantic model from the model
+
+        ### Parameters:
+
+        up: bool
+            Whether it's for up (data update) or down (data retrieval)
+        suffix: str
+            Suffix to append to the model name, default: _UP or _DOWN
+        include_validators: bool
+            Include validators for each fields, default: None. When None
+            It will include validators when up=True.
+
+        ### Returns:
+            pydantic model
+        '''
+        include_validators = up if include_validators is None else include_validators
+        name = self.__name__
+        u = '_UP' if up else '_DOWN'
+        if suffix: u = suffix
+        name = name + u
+        res = {}
+        fields = self._get_fields_(up)
+        all_fields = self._get_all_fields_()
+        for k in fields:
+            res[k] = all_fields[k].to_pydantic(include_validator=include_validators)
+        return pydantic.create_model(name, **res)
+
     def _run_validations_(self, k: str, v: FieldValue, mob=None) -> FieldValue:
         try:
             validator = getattr(mob, '_clean_' + k)
-            v.value = validator(v.value)
+            v._value = validator(v.value) # do not trigger the field validator
+            # and do not increase the change count
         except AttributeError:
-            v.value = v.value # at least trigger the value validation
+            pass
         return v
 
 
     def _get_FieldValue_data_valid_(self, data: dict, up=False, validate_all=False, mob=None) -> Iterator[Tuple[str, Any]]:
         """Yields valid key,value pairs from data.
 
         Validity is checked against include/exclude key/value criteria.
```

### Comparing `morm-2.4.0/morm/pg_models.py` & `morm-2.4.1/morm/pg_models.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/q.py` & `morm-2.4.1/morm/q.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/utils.py` & `morm-2.4.1/morm/utils.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm/void.py` & `morm-2.4.1/morm/void.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/morm.egg-info/PKG-INFO` & `morm-2.4.1/morm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morm
-Version: 2.4.0
+Version: 2.4.1
 Summary: A minimal asynchronous database object relational mapper
 Home-page: https://github.com/neurobin/python-morm
 Author: Md. Jahidul Hamid
 Author-email: jahidulhamid@yahoo.com
 License: BSD
 Keywords: async,orm,postgresql
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncpg
 Requires-Dist: nest_asyncio
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: orjson
 
 [![Build status image](https://travis-ci.org/neurobin/python-morm.svg?branch=release)](https://travis-ci.com/github/neurobin/python-morm) [![Coverage Status](https://coveralls.io/repos/github/neurobin/python-morm/badge.svg?branch=release)](https://coveralls.io/github/neurobin/python-morm?branch=release)
 
 A minimal asynchronous database object relational mapper that supports transaction, connection pool and migration.
 
 Currently supports *PostgreSQL* with `asyncpg`.
 
@@ -79,15 +81,15 @@
 
 class User(Base):
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
 ```
 
-An advanced model could look like this:
+Advanced models could look like this:
 
 ```python
 import random
 
 def get_rand():
     return random.randint(1, 9)
 
@@ -100,17 +102,24 @@
         # see morm.meta.Meta for supported meta attributes.
 
     name = Field('varchar(65)')
     email = Field('varchar(255)')
     password = Field('varchar(255)')
     profession = Field('varchar(255)', default='Unknown')
     random = Field('integer', default=get_rand) # function can be default
+
+class UserProfile(User):
+    class Meta:
+        proxy = True
+        exclude_fields_down = ('password',) # exclude sensitive fields in retrieval
+        # this will also exclude this field from swagger docs if you are
+        # using our fastAPI framework
 ```
 
-**Rules for field names**
+## Rules for field names
 
 1. Must not start with an underscore (`_`). You can set arbitrary variables to the model instance with names starting with underscores; normally you can not set any variable to a model instance. Names not starting with an underscore are all expected to be field names, variables or methods that are defined during class definition.
 2. `_<name>_` such constructions are reserved for pre-defined overridable methods such as `_pre_save_`, `_post_save_`, etc..
 3. Name `Meta` is reserved to be a class that contains configuration of the model for both model and model instance.
 
 
 ## Initialize a model instance
@@ -475,7 +484,58 @@
 
 To run the production app as a service with `systemctl start app`, copy the **app.service** to `/etc/systemd/system`
 
 **Notes:**
 
 * You can setup your venv path in the `vact` file. To activate the venv with all the environment vars, just run `. vact`.
 * An environment file `.env_APP` is created in your home directory containing dev and production environments.
+
+
+# Pydantic support
+
+You can get pydantic model from any morm model using the `_pydantic_` method, e.g `User._pydantic_()` would give you the pydantic version of your `User` model. The `_pydantic_()` method supports a few parameters to customize the generated pydantic model:
+
+* `up=False`: Defines if the model should be for up (update into database) or down (retrieval from database).
+* `suffix=None`: You can add a suffix to the name of the generated pydantic model.
+* `include_validators=None`: Whether the validators defined in each field (with validator parameter) should be added as pydantic validators. When `None` (which is default) validators will be included for data update into database (i.e for `up=True`). Note that, the model field validators return True or False, while pydantic validators return the value, this conversion is automatically added internally while generating the pydantic model.
+
+If you are using our FastAPI framework, generating good docs for user data retrieval using the User model would be as simple as:
+
+```python
+@router.get('/crud/{model}', responses=Res.schema_all(User._pydantic_())
+async def get(request: Request, model: str, vals = '', col: str='', comp: str='=$1'):
+     if some_authentication_error:
+        raise Res(status=Res.Status.unauthorized, errors=['Invalid Credentials!']) # throws a correct HTTP error with additional error message
+    ...
+    return Res(user)
+```
+
+The above will define all common response types: 200, 401, 403, etc.. and the 200 success response will show an example with correct data types from your User model and will show only the fields that are allowed to be shown (controlled with `exclude_fields_down` or `fields_down` in the `User.Meta`).
+
+
+# JSON handling
+
+It may seem tempting to add json and jsonb support with `asyncpg.Connection.set_type_codec()` method, but we have not provided any option to use this method easily in `morm`, as it turned out to be making the queries very very slow. If you want to handle json, better add a `_clean_{field}` method in your model and  do the conversion there:
+
+```python
+class User(Base):
+    settings = Field('jsonb')
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
+
+If you want to have it converted to json during data retrieval from database as well, pass a validator which should return False if it is not json, and then pass a modifier in the field to do the conversion. Do note that modifier only runs if validator fails. Thus you will set and get the value as json (list or dict) and the `_clean_settings` will covert it back to text during database insert or update.
+
+```python
+class User(Base):
+    settings = Field('jsonb', validator=lambda x: isinstance(x, list|dict), modifier=lambda x: json.loads(x))
+    ...
+
+    def _clean_settings(self, v):
+        if not isinstance(v, str):
+            v = json.dumps(v)
+        return v
+```
```

### Comparing `morm-2.4.0/morm.egg-info/SOURCES.txt` & `morm-2.4.1/morm.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 morm/__init__.py
 morm/admin.py
+morm/ctx.py
 morm/db.py
 morm/dt.py
 morm/exceptions.py
 morm/init_fap
 morm/meta.py
 morm/migration.py
 morm/model.py
```

### Comparing `morm-2.4.0/setup.py` & `morm-2.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,10 +37,10 @@
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
       ],
       python_requires='>=3.10.0',
-      install_requires=['asyncpg','nest_asyncio'],
+      install_requires=['asyncpg','nest_asyncio', 'pydantic>=2.6.4', 'orjson'],
       scripts=['morm/morm_admin', 'morm/init_fap',],
 test_suite="morm.tests.test")
```

### Comparing `morm-2.4.0/tests/test_Migration.py` & `morm-2.4.1/tests/test_Migration.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/test_admin.py` & `morm-2.4.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/test_db.py` & `morm-2.4.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/test_field.py` & `morm-2.4.1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/test_model.py` & `morm-2.4.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/test_types.py` & `morm-2.4.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `morm-2.4.0/tests/testd.py` & `morm-2.4.1/tests/testd.py`

 * *Files identical despite different names*

