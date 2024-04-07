# Comparing `tmp/dmtgen-0.5.0.dev2.tar.gz` & `tmp/dmtgen-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtgen-0.5.0.dev2.tar", last modified: Sun Apr  7 08:17:43 2024, max compression
+gzip compressed data, was "dmtgen-1.0.0.dev0.tar", last modified: Wed Oct 19 05:29:46 2022, max compression
```

## Comparing `dmtgen-0.5.0.dev2.tar` & `dmtgen-1.0.0.dev0.tar`

### file list

```diff
@@ -1,36 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.266838 dmtgen-0.5.0.dev2/
--rw-rw-rw-   0        0        0     1093 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/LICENSE
--rw-rw-rw-   0        0        0      499 2024-04-07 08:17:43.252259 dmtgen-0.5.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0      105 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 08:17:43.266838 dmtgen-0.5.0.dev2/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-04-07 08:17:34.000000 dmtgen-0.5.0.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.089836 dmtgen-0.5.0.dev2/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.147410 dmtgen-0.5.0.dev2/src/dmtgen/
--rw-rw-rw-   0        0        0      330 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/__init__.py
--rw-rw-rw-   0        0        0     3694 2024-04-07 07:59:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/base_generator.py
--rw-rw-rw-   0        0        0     1689 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/src/dmtgen/basic_template_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.209420 dmtgen-0.5.0.dev2/src/dmtgen/common/
--rw-rw-rw-   0        0        0        0 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/__init__.py
--rw-rw-rw-   0        0        0     2657 2024-04-07 08:13:22.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/blueprint.py
--rw-rw-rw-   0        0        0     3587 2024-04-07 07:59:00.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/blueprint_attribute.py
--rw-rw-rw-   0        0        0     1128 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/enum_description.py
--rw-rw-rw-   0        0        0     7759 2024-04-07 08:08:34.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/package.py
--rw-rw-rw-   0        0        0      254 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/common/system_package.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.089836 dmtgen-0.5.0.dev2/src/dmtgen/data/
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.089836 dmtgen-0.5.0.dev2/src/dmtgen/data/system/
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.228044 dmtgen-0.5.0.dev2/src/dmtgen/data/system/SIMOS/
--rw-rw-rw-   0        0        0      454 2024-04-07 08:04:42.000000 dmtgen-0.5.0.dev2/src/dmtgen/data/system/SIMOS/entity.json
--rw-rw-rw-   0        0        0      536 2024-04-07 08:04:46.000000 dmtgen-0.5.0.dev2/src/dmtgen/data/system/SIMOS/named_enity.json
--rw-rw-rw-   0        0        0      533 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/none_generator.py
--rw-rw-rw-   0        0        0      445 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/src/dmtgen/package_generator.py
--rw-rw-rw-   0        0        0      214 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/dmtgen/template.py
--rw-rw-rw-   0        0        0      722 2024-03-15 06:34:17.000000 dmtgen-0.5.0.dev2/src/dmtgen/template_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.245287 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/
--rw-rw-rw-   0        0        0      499 2024-04-07 08:17:42.000000 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-07 08:17:43.000000 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 08:17:42.000000 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 08:17:42.000000 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 08:17:43.000000 dmtgen-0.5.0.dev2/src/dmtgen.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 08:17:43.238726 dmtgen-0.5.0.dev2/src/tests/
--rw-rw-rw-   0        0        0        0 2024-03-15 06:07:02.000000 dmtgen-0.5.0.dev2/src/tests/__init__.py
--rw-rw-rw-   0        0        0      732 2024-03-15 06:54:16.000000 dmtgen-0.5.0.dev2/src/tests/test_relative_paths.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.124677 dmtgen-1.0.0.dev0/
+-rw-rw-rw-   0        0        0     1093 2022-03-22 09:41:00.000000 dmtgen-1.0.0.dev0/LICENSE
+-rw-rw-rw-   0        0        0      540 2022-10-19 05:29:46.123677 dmtgen-1.0.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-09-10 11:08:42.000000 dmtgen-1.0.0.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-19 05:29:46.124677 dmtgen-1.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2022-10-19 05:06:42.000000 dmtgen-1.0.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:45.999678 dmtgen-1.0.0.dev0/src/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.050679 dmtgen-1.0.0.dev0/src/dmtgen/
+-rw-rw-rw-   0        0        0      208 2022-10-19 05:20:30.000000 dmtgen-1.0.0.dev0/src/dmtgen/__init__.py
+-rw-rw-rw-   0        0        0     3725 2022-10-19 05:15:02.000000 dmtgen-1.0.0.dev0/src/dmtgen/base_generator.py
+-rw-rw-rw-   0        0        0     1689 2022-10-19 05:18:49.000000 dmtgen-1.0.0.dev0/src/dmtgen/basic_template_generator.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.110677 dmtgen-1.0.0.dev0/src/dmtgen/common/
+-rw-rw-rw-   0        0        0        0 2021-09-10 09:22:37.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/__init__.py
+-rw-rw-rw-   0        0        0     2873 2022-10-19 05:21:50.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint.py
+-rw-rw-rw-   0        0        0     2213 2022-10-19 05:27:29.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint_attribute.py
+-rw-rw-rw-   0        0        0     1528 2022-05-30 12:16:28.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/enum_description.py
+-rw-rw-rw-   0        0        0     4639 2021-09-10 09:22:37.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/package.py
+-rw-rw-rw-   0        0        0      187 2021-09-10 10:54:56.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/system_package.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.001678 dmtgen-1.0.0.dev0/src/dmtgen/data/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.001678 dmtgen-1.0.0.dev0/src/dmtgen/data/system/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.122677 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/
+-rw-rw-rw-   0        0        0      503 2022-09-29 12:07:04.000000 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/entity.json
+-rw-rw-rw-   0        0        0      585 2022-09-29 12:07:11.000000 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/named_enity.json
+-rw-rw-rw-   0        0        0      445 2022-10-19 05:13:00.000000 dmtgen-1.0.0.dev0/src/dmtgen/package_generator.py
+-rw-rw-rw-   0        0        0      186 2021-09-10 09:22:09.000000 dmtgen-1.0.0.dev0/src/dmtgen/template.py
+-rw-rw-rw-   0        0        0      722 2022-08-15 06:50:41.000000 dmtgen-1.0.0.dev0/src/dmtgen/template_generator.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.074677 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/
+-rw-rw-rw-   0        0        0      540 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/top_level.txt
```

### Comparing `dmtgen-0.5.0.dev2/LICENSE` & `dmtgen-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtgen-0.5.0.dev2/setup.py` & `dmtgen-1.0.0.dev0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt',encoding='utf8') as f:
     required = f.read().splitlines()
 
 setup(
     name='dmtgen',
-    version='0.5.0.dev2',
+    version='1.0.0.dev0',
     author="SINTEF Ocean",
     description="Python generator utilities for DMT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages= find_packages(where="src"),
     package_data={'dmtgen': ['data/system/SIMOS/*.json']},
```

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen/base_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/base_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,19 @@
     def __init__(self, root_dir: Path, package_name: str,
                  output_dir: Path, root_package: Package) -> None:
         self.package_name = package_name
         self.template_root = root_dir /"templates"
         self.output_dir = output_dir
         self.source_only = False
         self.root_package = root_package
+        self.generators = self.get_template_generators()
 
-    # pylint: disable=unused-argument
-    def get_template_generator(self, template: Path, config: Dict) -> TemplateBasedGenerator:
-        """ Override in subclasses to control which template generator to use"""
-        return BasicTemplateGenerator()
-
+    def get_template_generators(self) -> Dict[str,TemplateBasedGenerator]:
+        """ Override in subclasses """
+        return {}
 
     def generate_package(self, config: Dict):
         """ Generate package """
         self.source_only = config.get("source",self.source_only)
         self.__generate_from_templates(self.template_root, self.output_dir,config)
 
 
@@ -52,34 +51,37 @@
 
         self.post_generate(output_dir)
 
     def copy_templates(self, template_root: Path, output_dir: Path):
         """Copy template folder to output folder"""
         # First we copy the entire tree structure
         # Then we have the sceleton to convert the files afterwards
-        shutil.copytree(str(template_root), str(output_dir),  dirs_exist_ok=True)
+        shutil.copytree(str(template_root), str(output_dir))
 
     def pre_generate(self,output_dir: Path):
         """ override in subclass """
 
     def post_generate(self,output_dir: Path):
         """ override in subclass """
 
     def __find_templates_and_generate(self, output_dir: Path, config: Dict):
         for path in sorted(output_dir.rglob('*.jinja')):
-            generator = self.get_template_generator(path, config)
+            generator = self.generators.get(path.name,self.get_basic_generator())
             self.__generate_template(path, generator, config)
 
+    def get_basic_generator(self) -> TemplateBasedGenerator:
+        return BasicTemplateGenerator()
+
     @staticmethod
     def __read_template(templatefile: Path):
         loader = jinja2.FileSystemLoader(templatefile.parents[0])
-        env_parameters = {
-            "loader": loader,
-            "undefined":jinja2.StrictUndefined
-        }
+        env_parameters = dict(
+            loader=loader,
+            undefined=jinja2.StrictUndefined
+        )
         environment = jinja2.Environment(**env_parameters)
         environment.filters["escape_string"] = escape_string
         return environment.get_template(templatefile.name)
 
     def __generate_template(self, template_file: Path, template_generator: TemplateBasedGenerator, config: Dict):
         template = self.__read_template(template_file)
         file_name = self.__remove_suffix(template_file)
```

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen/basic_template_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/basic_template_generator.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen/common/blueprint_attribute.py` & `dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint_attribute.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,77 @@
 """ " A basic SIMOS Attribute"""
-from __future__ import annotations
+
+
 from typing import Dict
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from .blueprint import Blueprint
+
 
 class BlueprintAttribute:
     """ " A basic SIMOS Attribute"""
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, content: Dict, parent: Blueprint) -> None:
+    def __init__(self, content: Dict) -> None:
         self.content = content
-        name = content["name"]
-        if len(name)==0:
-            raise ValueError("Attribute has no name")
-        self.name = name
         if "description" not in content:
             content["description"] = ""
+        name = content["name"]
+        if not name:
+            raise Exception("Attribute has no name")
+        self.name = name
         self.description = content["description"].replace('"',"'")
-        dims=content.get("dimensions")
-        if dims:
-            self.dimensions = dims.split(",")
-        else:
-            self.dimensions = []
-
+        self.__is_many= "dimensions" in content
+        self.__contained = content.get("contained",True)
         atype = content["attributeType"]
-        self.__parent = parent
-        package = parent.parent
-        self.__type = package.resolve_type(atype)
-        self.__optional = self.content.get("optional",True)
-        self.__is_primitive = atype in ['boolean', 'number', 'string', 'integer']
-        self.__is_enum = self.content.get("enumType",None) is not None
-        self.__is_blueprint = not (self.is_primitive or self.is_enum)
-        self.__is_array = len(self.dimensions)>0
-        self.__is_string = self.type == "string"
-        self.__is_boolean = self.type == "boolean"
-        self.__is_integer = self.type == "integer"
-        self.__is_number = self.type == "number"
-        self.is_contained = content.get("contained",True)
-
-    @property
-    def parent(self) -> Blueprint:
-        """The parent blueprint"""
-        return self.__parent
+        self.__type = atype
+        primitive_types =  ['boolean', 'number', 'string', 'integer']
+        self.__is_primitive = atype in primitive_types
+        self.is_enum = self.content.get("enumType",None) is not None
+
+    @property
+    def name(self) -> str:
+        """Entity id"""
+        return self.__name
+
+    @name.setter
+    def name(self, value: str):
+        """Set name"""
+        self.__name = str(value)
 
     @property
     def type(self) -> str:
-        """The type of the attribute"""
+        """Attribute type"""
         return self.__type
 
     @property
-    def optional(self) -> bool:
-        """Is this an optional attribute"""
-        return self.__optional
+    def description(self) -> str:
+        """Entity id"""
+        return self.__description
+
+    @property
+    def contained(self) -> bool:
+        """Is contained"""
+        return self.__contained
 
+    @property
     def is_primitive(self) -> bool:
-        """Is this a primitive type"""
+        """Is this a primitive attribute"""
         return self.__is_primitive
 
-    def is_enum(self) -> bool:
-        """Is this an enum type"""
-        return self.__is_enum
-
-    def is_blueprint(self) -> bool:
-        """Is this a blueprint type"""
-        return self.__is_blueprint
-
-    def is_string(self) -> bool:
-        """Is this a string"""
-        return self.__is_string
-
-    def is_boolean(self) -> bool:
-        """Is this a boolean"""
-        return self.__is_boolean
-
-    def is_integer(self) -> bool:
-        """Is this an integer"""
-        return self.__is_integer
-
-    def is_number(self) -> bool:
-        """Is this a number"""
-        return self.__is_number
-
-    def is_optional(self) -> bool:
-        """Is an optional relation"""
-        return self.__optional
-
-    def is_required(self) -> bool:
-        """Is a required relation"""
-        return not self.__optional
-
-    def is_array(self) -> bool:
-        """Is this an array"""
-        return self.__is_array
-
-    def is_fixed_array(self) -> bool:
-        """Is this a fixed array"""
-        return self.__is_array and "*" not in self.dimensions
-
-    def is_variable_array(self) -> bool:
-        """Is this a variable array"""
-        return self.__is_array and "*" in self.dimensions
+    @property
+    def is_many(self) -> bool:
+        """Is this a many relation"""
+        return self.__is_many
+
+    @property
+    def optional(self) -> bool:
+        """Is this a many relation"""
+        return self.content.get("optional",True)
+
+    @description.setter
+    def description(self, value: str):
+        """Set description"""
+        self.__description = str(value)
 
     def get(self, key, default=None):
         """Return the content value or an optional default"""
         return self.content.get(key,default)
 
     def as_dict(self) -> Dict:
         """Return the attribute as a dictionary"""
```

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen/data/system/SIMOS/named_enity.json` & `dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/named_enity.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'storageRecipes'": '[]', "'uiRecipes'": '[]'}*

```diff
@@ -10,9 +10,11 @@
         }
     ],
     "description": "Describes the required attributes (name, type, description). All other blueprints should extend this one, or implement the attributes itself",
     "extends": [
         "system/SIMOS/Entity"
     ],
     "name": "NamedEntity",
-    "type": "system/SIMOS/Blueprint"
+    "storageRecipes": [],
+    "type": "system/SIMOS/Blueprint",
+    "uiRecipes": []
 }
```

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen/template_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/template_generator.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.5.0.dev2/src/dmtgen.egg-info/SOURCES.txt` & `dmtgen-1.0.0.dev0/src/dmtgen.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 src/dmtgen/__init__.py
 src/dmtgen/base_generator.py
 src/dmtgen/basic_template_generator.py
-src/dmtgen/none_generator.py
 src/dmtgen/package_generator.py
 src/dmtgen/template.py
 src/dmtgen/template_generator.py
 src/dmtgen.egg-info/PKG-INFO
 src/dmtgen.egg-info/SOURCES.txt
 src/dmtgen.egg-info/dependency_links.txt
 src/dmtgen.egg-info/requires.txt
@@ -16,10 +15,8 @@
 src/dmtgen/common/__init__.py
 src/dmtgen/common/blueprint.py
 src/dmtgen/common/blueprint_attribute.py
 src/dmtgen/common/enum_description.py
 src/dmtgen/common/package.py
 src/dmtgen/common/system_package.py
 src/dmtgen/data/system/SIMOS/entity.json
-src/dmtgen/data/system/SIMOS/named_enity.json
-src/tests/__init__.py
-src/tests/test_relative_paths.py
+src/dmtgen/data/system/SIMOS/named_enity.json
```

