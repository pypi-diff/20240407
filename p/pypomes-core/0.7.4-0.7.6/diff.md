# Comparing `tmp/pypomes_core-0.7.4.tar.gz` & `tmp/pypomes_core-0.7.6.tar.gz`

## Comparing `pypomes_core-0.7.4.tar` & `pypomes_core-0.7.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    20247 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    20247 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.6/PKG-INFO
```

### Comparing `pypomes_core-0.7.4/src/pypomes_core/.ruff.toml` & `pypomes_core-0.7.6/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/__init__.py` & `pypomes_core-0.7.6/src/pypomes_core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+import os
+
 from .datetime_pomes import (
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
     TIMEZONE_LOCAL, TIMEZONE_UTC,
     date_reformat, date_parse, datetime_parse,
 )
 from .dict_pomes import (
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_clone,
     dict_get_key, dict_get_keys, dict_from_object, dict_from_list, dict_replace_value, dict_pop_value,
 )
 from .email_pomes import (
-    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send,
+    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER,
+    email_send,
 )
 from .encoding_pomes import (
     encode_ascii_hex, decode_ascii_hex,
 )
 from .env_pomes import (
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float, env_get_path,
+    env_get_str, env_get_int, env_get_bool, env_get_float, env_get_path,
 )
 from .exception_pomes import (
     exc_format,
 )
 from .file_pomes import (
     TEMP_DIR,
     file_from_request, file_get_data
@@ -48,34 +51,37 @@
 from .validation_pomes import (
     VALIDATE_MSG_LANGUAGE, VALIDATE_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
     validate_date, validate_datetime, validate_ints, validate_strs,
     validate_format_error, validate_format_errors, validate_unformat_errors,
 )
 from .xml_pomes import (
-    XML_FILE_HEADER, xml_to_dict, xml_normalize_keys,
+    XML_FILE_HEADER,
+    xml_to_dict, xml_normalize_keys,
 )
 
 __all__ = [
     # datetime_pomes
     "DATE_FORMAT_STD", "DATE_FORMAT_COMPACT", "DATE_FORMAT_INV",
     "DATETIME_FORMAT_STD", "DATETIME_FORMAT_COMPACT", "DATETIME_FORMAT_INV",
     "TIMEZONE_LOCAL", "TIMEZONE_UTC",
     "date_reformat", "date_parse", "datetime_parse",
     # dict_pomes
     "dict_has_key_chain", "dict_get_value", "dict_set_value", "dict_reduce",
     "dict_listify", "dict_transform", "dict_merge", "dict_coalesce", "dict_clone",
     "dict_get_key", "dict_get_keys", "dict_from_object", "dict_from_list",
     "dict_replace_value", "dict_pop_value",
     # email_pomes
-    "EMAIL_ACCOUNT", "EMAIL_PWD", "EMAIL_PORT", "EMAIL_SERVER", "email_send",
+    "EMAIL_ACCOUNT", "EMAIL_PWD", "EMAIL_PORT", "EMAIL_SERVER",
+    "email_send",
     # encoding_pomes
     "encode_ascii_hex", "decode_ascii_hex",
     # env_pomes
-    "APP_PREFIX", "env_get_str", "env_get_int", "env_get_bool", "env_get_float", "env_get_path",
+    "APP_PREFIX",
+    "env_get_str", "env_get_int", "env_get_bool", "env_get_float", "env_get_path",
     # exception_pomes
     "exc_format",
     # file_pomes
     "TEMP_DIR",
     "file_from_request", "file_get_data",
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
@@ -94,13 +100,18 @@
     "validate_add_msgs", "validate_set_msgs",
     # validation_pomes
     "VALIDATE_MSG_LANGUAGE", "VALIDATE_MSG_PREFIX",
     "validate_value", "validate_bool", "validate_int", "validate_float", "validate_str",
     "validate_date", "validate_datetime", "validate_ints", "validate_strs",
     "validate_format_error", "validate_format_errors", "validate_unformat_errors",
     # xml_pomes
-    "XML_FILE_HEADER", "xml_to_dict", "xml_normalize_keys",
+    "XML_FILE_HEADER",
+    "xml_to_dict", "xml_normalize_keys",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_core")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
+
+# the prefix for the names of the environment variables
+from typing import Final
+APP_PREFIX: Final[str] = os.environ["PYPOMES_APP_PREFIX"]
```

### Comparing `pypomes_core-0.7.4/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/email_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/env_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/env_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,11 +81,7 @@
     result: Path
     try:
         result = Path(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
-
-
-# the prefix to the names of the environment variables
-APP_PREFIX = env_get_str("PYPOMES_APP_PREFIX", "PYPOMES")
```

### Comparing `pypomes_core-0.7.4/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/file_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/json_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/list_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/str_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.7.6/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.7.6/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/LICENSE` & `pypomes_core-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.4/pyproject.toml` & `pypomes_core-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.7.4"
+version = "0.7.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.7.4/PKG-INFO` & `pypomes_core-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.7.4
+Version: 0.7.6
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

