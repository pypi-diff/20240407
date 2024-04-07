# Comparing `tmp/dmtgenfor-0.2.0.tar.gz` & `tmp/dmtgenfor-0.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtgenfor-0.2.0.tar", last modified: Tue Nov 29 09:05:18 2022, max compression
+gzip compressed data, was "dmtgenfor-0.3.0.dev3.tar", last modified: Sun Apr  7 09:14:21 2024, max compression
```

## Comparing `dmtgenfor-0.2.0.tar` & `dmtgenfor-0.3.0.dev3.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.469473 dmtgenfor-0.2.0/
--rw-rw-rw-   0        0        0     1093 2022-08-12 07:07:36.000000 dmtgenfor-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      884 2022-11-29 09:05:18.468473 dmtgenfor-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      415 2022-11-29 09:04:04.000000 dmtgenfor-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2022-11-29 09:05:18.469473 dmtgenfor-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1145 2022-11-29 09:05:07.000000 dmtgenfor-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.372473 dmtgenfor-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.391473 dmtgenfor-0.2.0/src/dmtgenfor/
--rw-rw-rw-   0        0        0        0 2022-08-12 07:07:36.000000 dmtgenfor-0.2.0/src/dmtgenfor/__init__.py
--rw-rw-rw-   0        0        0      748 2022-11-29 09:04:04.000000 dmtgenfor-0.2.0/src/dmtgenfor/generator.py
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.437473 dmtgenfor-0.2.0/src/dmtgenfor/generators/
--rw-rw-rw-   0        0        0        0 2022-08-16 12:42:49.000000 dmtgenfor-0.2.0/src/dmtgenfor/generators/__init__.py
--rw-rw-rw-   0        0        0     5908 2022-11-29 09:04:04.000000 dmtgenfor-0.2.0/src/dmtgenfor/generators/basic_template_generator.py
--rw-rw-rw-   0        0        0     1934 2022-10-04 06:00:10.000000 dmtgenfor-0.2.0/src/dmtgenfor/generators/graph.py
--rw-rw-rw-   0        0        0     1247 2022-11-29 09:04:04.000000 dmtgenfor-0.2.0/src/dmtgenfor/generators/runtime_generator.py
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.452473 dmtgenfor-0.2.0/src/dmtgenfor/templates/
--rw-rw-rw-   0        0        0      496 2022-08-15 06:39:19.000000 dmtgenfor-0.2.0/src/dmtgenfor/templates/cmake-project.jsonc.jinja
--rw-rw-rw-   0        0        0      441 2022-11-29 09:04:04.000000 dmtgenfor-0.2.0/src/dmtgenfor/templates/fpm.toml.jinja
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.466473 dmtgenfor-0.2.0/src/dmtgenfor/templates/src/
--rw-rw-rw-   0        0        0     7594 2022-10-07 06:44:57.000000 dmtgenfor-0.2.0/src/dmtgenfor/templates/src/json_io.f90.jinja
--rw-rw-rw-   0        0        0      419 2022-10-05 11:25:05.000000 dmtgenfor-0.2.0/src/dmtgenfor/templates/src/types_mod.f90.jinja
-drwxrwxrwx   0        0        0        0 2022-11-29 09:05:18.413474 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/
--rw-rw-rw-   0        0        0      884 2022-11-29 09:05:18.000000 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2022-11-29 09:05:18.000000 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-29 09:05:18.000000 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-11-29 09:05:18.000000 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-29 09:05:18.000000 dmtgenfor-0.2.0/src/dmtgenfor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.348649 dmtgenfor-0.3.0.dev3/
+-rw-rw-rw-   0        0        0     1093 2024-03-15 09:22:57.000000 dmtgenfor-0.3.0.dev3/LICENSE
+-rw-rw-rw-   0        0        0      833 2024-04-07 09:14:21.335845 dmtgenfor-0.3.0.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-04-05 08:00:51.000000 dmtgenfor-0.3.0.dev3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 09:14:21.349656 dmtgenfor-0.3.0.dev3/setup.cfg
+-rw-rw-rw-   0        0        0     1150 2024-04-06 05:59:07.000000 dmtgenfor-0.3.0.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.090680 dmtgenfor-0.3.0.dev3/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.111097 dmtgenfor-0.3.0.dev3/src/dmtgenfor/
+-rw-rw-rw-   0        0        0        0 2024-03-15 09:22:57.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/__init__.py
+-rw-rw-rw-   0        0        0      689 2024-04-05 07:05:12.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.217517 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/
+-rw-rw-rw-   0        0        0        0 2024-03-15 09:22:57.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/__init__.py
+-rw-rw-rw-   0        0        0     7822 2024-04-07 08:47:54.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/basic_template_generator.py
+-rw-rw-rw-   0        0        0     1934 2024-03-15 09:22:57.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/graph.py
+-rw-rw-rw-   0        0        0     1234 2024-04-07 08:31:09.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/runtime_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.280459 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/
+-rw-rw-rw-   0        0        0        0 2024-03-15 09:22:57.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-07 08:49:15.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/common.py
+-rw-rw-rw-   0        0        0     7960 2024-04-07 09:04:23.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/entity_model.py
+-rw-rw-rw-   0        0        0    30540 2024-04-07 08:53:08.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/hdf5_model.py
+-rw-rw-rw-   0        0        0     2738 2024-04-07 08:53:29.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/resize_model.py
+-rw-rw-rw-   0        0        0     2361 2024-04-07 08:45:08.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/simos.py
+-rw-rw-rw-   0        0        0     3418 2024-04-07 08:26:07.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/simos/simos_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.321658 dmtgenfor-0.3.0.dev3/src/dmtgenfor/templates/
+-rw-rw-rw-   0        0        0    10082 2024-04-05 11:18:08.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/templates/json_io_mod.f90.jinja
+-rw-rw-rw-   0        0        0    20565 2024-04-05 07:52:56.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/templates/simos.F90.jinja
+-rw-rw-rw-   0        0        0      602 2024-04-05 08:05:23.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor/templates/types_mod.f90.jinja
+drwxrwxrwx   0        0        0        0 2024-04-07 09:14:21.198965 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/
+-rw-rw-rw-   0        0        0      833 2024-04-07 09:14:20.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2024-04-07 09:14:21.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 09:14:20.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-07 09:14:20.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-07 09:14:20.000000 dmtgenfor-0.3.0.dev3/src/dmtgenfor.egg-info/top_level.txt
```

### Comparing `dmtgenfor-0.2.0/LICENSE` & `dmtgenfor-0.3.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtgenfor-0.2.0/setup.py` & `dmtgenfor-0.3.0.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt',encoding='utf8') as f:
     required = f.read().splitlines()
 
 setup(
     name='dmtgenfor',
-    version='0.2.0',
+    version='0.3.0.dev3',
     author="SINTEF Ocean",
     description="Fortran generator for DMT based models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages= find_packages(where="src"),
     package_data={'dmtgenfor':  ['templates/*','templates/src/*','templates/tests/*']},
```

### Comparing `dmtgenfor-0.2.0/src/dmtgenfor/generators/basic_template_generator.py` & `dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/basic_template_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,35 +15,29 @@
     types = {"number": "real(dp)", "double": "real(dp)", "string": "character(:)", "char": "character",
             "integer": "integer", "short": "short", "boolean": "logical"}
 
     default_values = {"number": "0.0", "boolean": ".false.", "integer": "0"}
 
     def generate(self, package_generator: PackageGenerator, template, outputfile: Path, config: Dict):
         """Basic generator, one template, one output file"""
+
         model = {}
-        package_name = package_generator.package_name
-        model["package_name"] = package_name
-        model["package_class"] = self.first_to_upper(package_name) + "PackageDescription"
-        model["lib_name"] = config.get("lib_name",f'{package_name}-for')
-        model["description"] = package_name + " - Generated types"
-        model["version"] = config["version"]
         etypes = {}
-
         pkg: Package = package_generator.root_package
-
         dependencies = {}
-
         for blueprint in pkg.blueprints:
             etype = {}
             name = blueprint.name
             ftype = underscore(name)+"_t"
             etype["name"] = name
             etype["type"] = ftype
             etype["path"] = blueprint.get_path()
             etype["description"] = blueprint.description
+            etype["formatted_description"] = self.__format_description(blueprint.description)
+            etype["has_description"] = len(blueprint.description) > 0
             etype["file_basename"] = name.lower()
             attributes = []
             etype["attributes"]=attributes
             attribute_deps = set()
             for attribute in blueprint.all_attributes.values():
                 attributes.append(self.__to_attribute_dict(attribute, pkg, attribute_deps))
             dependencies[name]=attribute_deps
@@ -52,52 +46,90 @@
         model["types"] = self.__sort(etypes, dependencies)
 
         with codecs.open(outputfile, "w", "utf-8") as file:
             file.write(template.render(model))
 
     def __to_attribute_dict(self,attribute: BlueprintAttribute, pkg: Package, attribute_deps):
         fieldname =underscore(attribute.name)
+        fieldname_temp = fieldname + "_temp" # We need a temp variable (allocatable) to assign to static arrays (non-allocatable)
+
+        if attribute.is_array():
+            dimensions = attribute.dimensions
+            array_rank = len(dimensions)
+            shape = ",".join(attribute.dimensions).replace("*", ":")
+            shape_temp = ','.join(array_rank*[':'])
+        else:
+            dimensions = None
+            array_rank = 0
+            shape = ''
+            shape_temp = ''
 
-        if attribute.is_primitive:
+        if attribute.is_primitive():
             atype = self.__map(attribute.type, self.types)
             # integer :: index
             # character(:), allocatable :: name
-            allocatable = attribute.is_many or attribute.type == "string"
+            allocatable = attribute.is_variable_array() or attribute.is_string()
             if allocatable:
                 type_init = atype + ", allocatable :: " + fieldname
+                type_init_allocatable_temp = atype + ", allocatable :: " + fieldname_temp
             else:
                 type_init = atype + " :: " + fieldname
+                type_init_allocatable_temp = atype + ", allocatable :: " + fieldname_temp # We need an allocatable temp variable to assign to static arrays
+
+            if attribute.is_array():
+                type_init += '(' + shape + ')'
+                type_init_allocatable_temp += '(' + shape_temp + ')'
+
+            if not allocatable:
                 default = self.__find_default_value(attribute)
-                if default:
-                    type_init += " = " + str(default)
-            if attribute.is_many:
-                type_init += "(:)"
+                if default is not None:
+                    type_init += " = " + default
+
         else:
+
+            if array_rank > 1:
+                raise ValueError("Only one-dimensional derived type arrays are supported")
+
             bp=pkg.get_blueprint(attribute.type)
             attribute_deps.add(bp.name)
             atype = underscore(bp.name)+"_t"
-            if attribute.is_many:
-                type_init = "type(" + atype + "), allocatable :: " + fieldname + "(:)"
-            elif attribute.optional:
+
+            allocatable = attribute.is_variable_array() or attribute.optional
+
+            if allocatable:
                 type_init = "type(" + atype + "), allocatable :: " + fieldname
+                type_init_allocatable_temp = "type(" + atype + "), allocatable :: " + fieldname_temp # We need an allocatable temp variable to assign to static arrays
             else:
                 type_init = "type(" + atype + ") :: " + fieldname
+                type_init_allocatable_temp = "type(" + atype + "), allocatable :: " + fieldname_temp # We need an allocatable temp variable to assign to static arrays
 
-            if len(attribute.description)>0:
-                type_init += " ! " + attribute.description
+            if attribute.is_array():
+                type_init += '(' + shape + ')'
+                type_init_allocatable_temp += '(' + shape_temp + ')'
+
+        if len(attribute.description) > 0:
+            has_description = True
+        else:
+            has_description = False
 
         return {
             "name": attribute.name,
             "fieldname": fieldname,
-            "is_required": not attribute.optional,
+            "fieldname_temp": fieldname_temp,
+            "is_required": attribute.is_required(),
             "type" : atype,
-            "is_primitive" : attribute.is_primitive,
-            "is_many" : attribute.is_many,
+            "is_primitive" : attribute.is_primitive(),
+            "is_many" : attribute.is_array(),
+            "array_rank" : array_rank, # Number of dimensions in array
+            "has_dynamic_shape" : attribute.is_variable_array(), # True if at least one dimension is *
+            "shape" : shape, # Shape of array
             "type_init" : type_init,
-            "description" : attribute.description
+            "type_init_allocatable_temp" : type_init_allocatable_temp,
+            "description" : attribute.description,
+            "has_description" : has_description
         }
 
     def __sort(self, etypes, dependencies):
         vertices = [x["name"] for x in etypes.values()]
         graph = Graph(vertices)
         for etype in etypes.values():
             name = etype["name"]
@@ -108,38 +140,47 @@
         for name in sorted_names:
             sorted_types.append(etypes[name])
         return sorted_types
 
     def __map(self, key, values):
         converted = values[key]
         if not converted:
-            raise Exception("Unkown type " + key)
+            raise ValueError("Unkown type " + key)
         return converted
 
     def __find_default_value(self, attribute: BlueprintAttribute):
         default_value = attribute.get("default")
         if default_value is not None:
             return self.__convert_default(attribute,default_value)
         return default_value
 
     def __convert_default(self,attribute: BlueprintAttribute, default_value):
         # converts json value to fortran value
         if isinstance(default_value,str):
             if default_value == '' or default_value == '""':
                 return '""'
             elif attribute.type == 'integer':
-                return int(default_value)
+                return default_value
             elif attribute.type == 'number':
-                return float(default_value)
+                return default_value + "_dp"
             elif attribute.type == 'boolean':
                 conversion = {
                     "false": ".false.",
                     "true": ".true.",
                 }
                 return conversion.get(default_value, default_value)
             else:
                 return "'" + default_value + "'"
 
     @staticmethod
-    def first_to_upper(string):
+    def first_to_upper(string: str):
         """ Make sure the first letter is uppercase """
         return string[:1].upper() + string[1:]
+
+    @staticmethod
+    def __format_description(desc: str):
+        if len(desc) > 0:
+            lst = desc.splitlines()
+            flst = ['!! ' + s for s in lst]
+            return flst
+        else:
+            return [desc]
```

### Comparing `dmtgenfor-0.2.0/src/dmtgenfor/generators/graph.py` & `dmtgenfor-0.3.0.dev3/src/dmtgenfor/generators/graph.py`

 * *Files identical despite different names*

