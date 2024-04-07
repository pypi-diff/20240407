# Comparing `tmp/pyhocon-dantic-0.0.3.tar.gz` & `tmp/pyhocon-dantic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhocon-dantic-0.0.3.tar", last modified: Wed Mar  6 04:34:27 2024, max compression
+gzip compressed data, was "pyhocon-dantic-0.0.4.tar", last modified: Sun Apr  7 10:02:06 2024, max compression
```

## Comparing `pyhocon-dantic-0.0.3.tar` & `pyhocon-dantic-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-03-06 04:34:27.016148 pyhocon-dantic-0.0.3/
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)     1065 2024-03-05 12:27:53.000000 pyhocon-dantic-0.0.3/LICENSE
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      954 2024-03-06 04:34:27.015949 pyhocon-dantic-0.0.3/PKG-INFO
-drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-03-06 04:34:27.014373 pyhocon-dantic-0.0.3/pyhocon_dantic/
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)     2817 2024-03-05 12:44:02.000000 pyhocon-dantic-0.0.3/pyhocon_dantic/__init__.py
-drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-03-06 04:34:27.015378 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      954 2024-03-06 04:34:27.000000 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/PKG-INFO
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      238 2024-03-06 04:34:27.000000 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/SOURCES.txt
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)        1 2024-03-06 04:34:27.000000 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/dependency_links.txt
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      153 2024-03-06 04:34:27.000000 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/requires.txt
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)       15 2024-03-06 04:34:27.000000 pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/top_level.txt
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      854 2024-03-06 04:34:06.000000 pyhocon-dantic-0.0.3/pyproject.toml
--rw-r--r--   0 yuhan-kunlun   (501) staff       (20)       38 2024-03-06 04:34:27.016180 pyhocon-dantic-0.0.3/setup.cfg
+drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-04-07 10:02:06.421677 pyhocon-dantic-0.0.4/
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)     1065 2024-03-05 12:27:53.000000 pyhocon-dantic-0.0.4/LICENSE
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      954 2024-04-07 10:02:06.421452 pyhocon-dantic-0.0.4/PKG-INFO
+drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-04-07 10:02:06.420182 pyhocon-dantic-0.0.4/pyhocon_dantic/
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)     2817 2024-04-07 10:01:37.000000 pyhocon-dantic-0.0.4/pyhocon_dantic/__init__.py
+drwxr-xr-x   0 yuhan-kunlun   (501) staff       (20)        0 2024-04-07 10:02:06.420888 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      954 2024-04-07 10:02:06.000000 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/PKG-INFO
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      238 2024-04-07 10:02:06.000000 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/SOURCES.txt
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)        1 2024-04-07 10:02:06.000000 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/dependency_links.txt
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      153 2024-04-07 10:02:06.000000 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/requires.txt
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)       15 2024-04-07 10:02:06.000000 pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/top_level.txt
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)      854 2024-04-07 10:01:56.000000 pyhocon-dantic-0.0.4/pyproject.toml
+-rw-r--r--   0 yuhan-kunlun   (501) staff       (20)       38 2024-04-07 10:02:06.421708 pyhocon-dantic-0.0.4/setup.cfg
```

### Comparing `pyhocon-dantic-0.0.3/LICENSE` & `pyhocon-dantic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhocon-dantic-0.0.3/PKG-INFO` & `pyhocon-dantic-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhocon-dantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic settings source for hocon file
 Author-email: Yuhan Wei <weiyuhan@pku.edu.cn>
 Project-URL: Homepage, https://github.com/weiyuhan/fastapi-easy-crud
 Project-URL: Issues, https://github.com/weiyuhan/fastapi-easy-crud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyhocon-dantic-0.0.3/pyhocon_dantic/__init__.py` & `pyhocon-dantic-0.0.4/pyhocon_dantic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 import pyhocon
 from pydantic.fields import FieldInfo
 from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
 
 
 class HoconConfigSettingsSource(PydanticBaseSettingsSource):
-    def __init__(self, settings_cls: type[BaseSettings], config_path: str):
+    def __init__(self, settings_cls: Type[BaseSettings], config_path: str):
         self.hocon_config = pyhocon.ConfigFactory.parse_file(config_path)
         super().__init__(settings_cls)
 
     def get_field_value(
         self, field: FieldInfo, field_name: str
-    ) -> tuple[Any, str, bool]:
+    ) -> Tuple[Any, str, bool]:
         if field.alias or field.validation_alias:
             field_name = str(field.alias) or str(field.validation_alias)
             value = self.hocon_config.get(field.alias)
         else:
             value = self.hocon_config.get(field_name)
 
         return value, field_name, type(value) in (dict, list, pyhocon.ConfigTree)
@@ -30,15 +30,15 @@
             return dict(value)
         if isinstance(value, list):
             return list(value)
         if isinstance(value, pyhocon.ConfigList):
             return list(value)
         return json.loads(value)
 
-    def __call__(self) -> dict[str, Any]:
+    def __call__(self) -> Dict[str, Any]:
         d: Dict[str, Any] = {}
         for field_name, field in self.settings_cls.model_fields.items():
             field_value, field_key, value_is_complex = self.get_field_value(
                 field, field_name
             )
             field_value = self.prepare_field_value(
                 field_name, field, field_value, value_is_complex
```

### Comparing `pyhocon-dantic-0.0.3/pyhocon_dantic.egg-info/PKG-INFO` & `pyhocon-dantic-0.0.4/pyhocon_dantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhocon-dantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic settings source for hocon file
 Author-email: Yuhan Wei <weiyuhan@pku.edu.cn>
 Project-URL: Homepage, https://github.com/weiyuhan/fastapi-easy-crud
 Project-URL: Issues, https://github.com/weiyuhan/fastapi-easy-crud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyhocon-dantic-0.0.3/pyproject.toml` & `pyhocon-dantic-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyhocon-dantic"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Yuhan Wei", email="weiyuhan@pku.edu.cn" },
 ]
 description = "Pydantic settings source for hocon file"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

