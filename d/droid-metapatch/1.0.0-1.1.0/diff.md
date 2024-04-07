# Comparing `tmp/droid_metapatch-1.0.0.tar.gz` & `tmp/droid_metapatch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid_metapatch-1.0.0.tar", max compression
+gzip compressed data, was "droid_metapatch-1.1.0.tar", max compression
```

## Comparing `droid_metapatch-1.0.0.tar` & `droid_metapatch-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     8632 2024-04-04 19:33:48.334657 droid_metapatch-1.0.0/README.md
--rw-r--r--   0        0        0      155 2024-04-04 07:42:22.856150 droid_metapatch-1.0.0/metapatch/__init__.py
--rw-r--r--   0        0        0     2431 2024-04-04 19:16:50.476894 droid_metapatch-1.0.0/metapatch/base.py
--rw-r--r--   0        0        0    11020 2024-04-04 19:25:23.451626 droid_metapatch-1.0.0/metapatch/metapatch.py
--rw-r--r--   0        0        0     6928 2024-04-04 09:31:45.638933 droid_metapatch-1.0.0/metapatch/options.py
--rw-r--r--   0        0        0      697 2024-04-04 09:40:34.183085 droid_metapatch-1.0.0/metapatch/utils.py
--rw-r--r--   0        0        0      425 2024-04-04 19:30:50.468212 droid_metapatch-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9243 1970-01-01 00:00:00.000000 droid_metapatch-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    12277 2024-04-07 14:09:48.013767 droid_metapatch-1.1.0/README.md
+-rw-r--r--   0        0        0      155 2024-04-04 07:42:22.856150 droid_metapatch-1.1.0/metapatch/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-07 09:24:15.339115 droid_metapatch-1.1.0/metapatch/base.py
+-rwxr-xr-x   0        0        0     9650 2024-04-07 14:06:52.964592 droid_metapatch-1.1.0/metapatch/cli_util.py
+-rw-r--r--   0        0        0    11477 2024-04-07 08:42:30.705814 droid_metapatch-1.1.0/metapatch/metapatch.py
+-rw-r--r--   0        0        0     6928 2024-04-04 09:31:45.638933 droid_metapatch-1.1.0/metapatch/options.py
+-rw-r--r--   0        0        0      697 2024-04-04 09:40:34.183085 droid_metapatch-1.1.0/metapatch/utils.py
+-rw-r--r--   0        0        0      493 2024-04-07 13:25:26.220124 droid_metapatch-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12888 1970-01-01 00:00:00.000000 droid_metapatch-1.1.0/PKG-INFO
```

### Comparing `droid_metapatch-1.0.0/README.md` & `droid_metapatch-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,159 @@
+Metadata-Version: 2.1
+Name: droid-metapatch
+Version: 1.1.0
+Summary: DROID patch generator
+License: GPL-3.0-only
+Author: Allan Eising
+Author-email: allan@eising.dk
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # Introduction
 
 The DROID metapatch library aims to create an easier and more pythonic way of creating DROID patch generators. DROID patch generators are a recent feature added to the the DROID Forge application that allows you to define python scripts that generate full-fledges patches.
 
 DROID is a series of eurorack controllers and CV processors made by [Der Mann mit der Maschine](https://shop.dermannmitdermaschine.de/).
 
 
-# Getting started
+# Installation
 
-A few examples have been distributed with the source code of this library that you may look at to see full implementations.
+
+## Installing the library
 
 Before you can write a patch generator, please install this library to your system python environment. Forge does not support virtual environments, so you must install this library somewhere where your default python library can find it.
 
 This library is available from pypi, use `pip install droid-metapatch` to install it.
 
 
+## Installation on MacOS
+
+DROID Forge uses the version of python that is bundled with MacOS. If you have installed python via homebrew or any other way, you may have multiple different python versions available.
+
+There are several ways to solve this:
+
+
+### Install the library with the system Python
+
+To ensure install this library to the one bundled with MacOS, run the following command:
+
+```
+$ /usr/bin/python3 -m pip install droid-metapatch
+```
+
+Note that this may result in a situation where the Forge has this library available, but your editor or shell does not. In that case, you can run the `pip install droid-metapatch` also. You will then have two copies installed, one for each environment.
+
+
+### Installing the metapatch library by hand
+
+You could also clone or download this repository, and place the `metapatch` folder into your Generators folder (located in your home directory under the `DROID Patches` folder.)
+
+This should work, but note that the `droid-metapatch` CLI utility will not be available then.
+
+
+# Getting started
+
+A few examples have been distributed with the source code of this library that you may look at to see full implementations.
+
+
+## Using droid-metapatch to convert an existing patch to a patch generator
+
+To get started really quickly, there&rsquo;s a helpful CLI script bundled with this library.
+
+```
+$ droid-metapatch --help
+usage: droid-metapatch [-h] [--boilerplate] [infile] [outfile]
+
+Metapatch helper script.
+
+positional arguments:
+  infile         Input file. Defaults to stdin.
+  outfile        Output file. Defaults to stdout.
+
+options:
+  -h, --help     show this help message and exit
+  --boilerplate  Generate a full example patch generator.
+
+If called without any arguments, you may input one or more droid circuits, and get the corresponding
+python code back.
+```
+
+If you run it without any arguments, you can paste one or more circuits, and get just the python code back that you can use within an ongoing patchgenerator project.
+
+However, if you provide a full patch as input, and use the `--boilerplate` option, it will output a full patch generator you can continue.
+
+
+### Example
+
+Here I&rsquo;m using one of the bundled patches from the blue4 DROID release:
+
+```
+$ droid-metapatch ~/p/droid/releases/droid-blue-4/patches/motoquencer_minimal.ini --boilerplate
+
+import metapatch
+
+class PatchGenerator(metapatch.PatchGenerator):
+    """Patch Generator boilerplate.
+
+    Change this to something more meaningful.
+    Also remember to add parameters and presets.
+    """
+    title = "Title of your patch generator"  # CHANGEME
+    description = "Description of your patch generator"  # CHANGEME
+
+    def generate(self) -> None:
+        """Patch generator function.
+
+        Modify this function to create your patch generator.
+        """
+        self.add_controller("p2b8", 1)
+        self.add_controller("m4", 2)
+
+        self.add_section("LFO and Sequencer")
+
+        self.add_circuit(
+            "lfo",
+            {
+                "hz": "20 * P1.1",
+                "square": "_CLOCK",
+            },
+            "Master clock"
+        )
+
+        self.add_circuit(
+            "motoquencer",
+            {
+                "clock": "_CLOCK",
+                "cv": "O1",
+                "gate": "O5",
+            },
+            "This motoquencer has as many steps as you have M4 faders"
+        )
+if __name__ == "__main__":
+    PatchGenerator.run()
+
+```
+
+If you specify an additional filename, the output will be written to that file instead of your terminal.
+
+
+### Continuing
+
+After this, you need to continue on your own. You should add presets and input parameters, and make the patch generator do something with those input parameters.
+
+See the next section for more details.
+
+
 ## Defining your patch generator class
 
 To start, you must define a python `class` that is a subclass of `metapatch.PatchGenerator`.
 
 Inside this class, you must at least define a `title` and a `description`, as well as a method called `generate`.
 
 This method should contain all the logic needed to create your patch. To actually define the patch, the class instance provides functions that allow you to add circuits, controllers and even sections.
@@ -291,7 +427,8 @@
 # Getting help
 
 If you have any problems with the library, let me know on the DROID discord server. I&rsquo;m known as eising on that server.
 
 Please note that any support will be on a best effort basis, if I have the time an energy.
 
 If you have found a bug, please create an issue here on github.
+
```

### Comparing `droid_metapatch-1.0.0/metapatch/base.py` & `droid_metapatch-1.1.0/metapatch/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,12 +89,15 @@
             section = "inputs"
         elif item.startswith("O"):
             section = "outputs"
         elif res := re.match(r"([A-Z])(\d+)\.(\d+)", item):
             module_num = res.group(2)
             controller_type = res.group(1)
             if controller_type == "G":
-                section = f"gates on module {module_num}"
+                if "." in item:
+                    section = f"gates on module {module_num}"
+                else:
+                    section = "gates on x7"
             else:
                 section = f"controller {module_num}"
 
         return cls(section, item, short_label, long_label)
```

### Comparing `droid_metapatch-1.0.0/metapatch/metapatch.py` & `droid_metapatch-1.1.0/metapatch/metapatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Class based patch generator interface."""
 
 import argparse
 import json
 import textwrap
 
 from abc import abstractmethod
+from itertools import groupby
 from typing import (
     Any,
     Dict,
     List,
     Mapping,
     Optional,
 )
@@ -63,15 +64,15 @@
 
         synopsis = {
             "title": cls.title,
             "description": cls.description,
             "sections": section_list,
             "presets": presets,
         }
-        return {"synopsis": synopsis}
+        return synopsis
 
     @property
     def presets(cls) -> List[Dict[str, Any]]:
         """Fetch presets."""
         presets: List[Dict[str, Any]] = []
         for name, opt in cls.__dict__.items():
             if isinstance(opt, Preset):
@@ -160,31 +161,32 @@
         all_param_help = {}
         for key, value in cls.__dict__.items():
             if not hasattr(value, "_ispatchoption"):
                 continue
             if issubclass(value, (BoolOption, EnumOption, NumberOption)):
                 all_param_help[value.title] = value.help(key)
 
-        longest = max(
-            [
-                len(varname[0])
-                for param in list(all_param_help.values())
-                for varname in param
-            ]
-        )
-        for title, opthelp in all_param_help.items():
-            params += textwrap.indent(title, "  ") + "\n"
-            for opt, descr in opthelp:
-                params += textwrap.indent(f"{opt:<{longest}}  {descr}", "    ")
-                params += "\n"
+        if all_param_help:
+            longest = max(
+                [
+                    len(varname[0])
+                    for param in list(all_param_help.values())
+                    for varname in param
+                ]
+            )
+            for title, opthelp in all_param_help.items():
+                params += textwrap.indent(title, "  ") + "\n"
+                for opt, descr in opthelp:
+                    params += textwrap.indent(f"{opt:<{longest}}  {descr}", "    ")
+                    params += "\n"
 
-            params += "\n"
+                params += "\n"
 
-        epilog += params
-        parser.epilog = epilog
+            epilog += params
+            parser.epilog = epilog
 
         args = parser.parse_args()
 
         return args
 
     @classmethod
     def run(cls) -> None:
@@ -265,66 +267,75 @@
         return self._section
 
     @section.setter
     def section(self, name: str) -> None:
         """Set the section."""
         if not isinstance(name, str):
             raise ValueError("Section name must be a string.")
+        if name not in self.sections:
+            self.sections[name] = None
         self._section = name
 
     def add_section(self, name: str, comment: Optional[str] = None) -> None:
         """Add a section with an optional comment."""
-        if name in self.sections:
-            return
-        self.sections[name] = comment
         self._section = name
+        if name not in self.sections or self.sections.get(name) != comment:
+            self.sections[name] = comment
 
     @property
     def _has_sections(self) -> bool:
         """Check if sections are defined."""
         sections = [circuit.section for circuit in self.circuits]
         return any(sections)
 
     def _get_circuits_as_strings(self) -> str:
-        """Get circuits as a string."""
+        """Get circuits as a string.
+
+        This is for circuits when there are no sections at all.
+        """
+        circuits = [str(circuit) for circuit in self.circuits]
+        return "\n".join(circuits)
+
+    def _get_circuits_with_sections(self) -> str:
+        """Get circuits as a string with sections."""
         circuits = []
-        current_section: Optional[str] = None
 
-        if self._has_sections:
-            if not self.circuits[0].section:
-                # If circuits were added before a section was defined, then we
-                # use a default name for this section.
-                current_section = DEFAULT_SECTION_NAME
+        groups = {}
+        for section, grouped_circuits in groupby(self.circuits, lambda x: x.section):
+            if section is None:
+                section_name = DEFAULT_SECTION_NAME
             else:
-                current_section = self.circuits[0].section
-
-            comment = self.sections.get(current_section)
-            circuits.append(write_patch_section(current_section, comment))
+                section_name = section
+            if section_name not in groups:
+                groups[section_name] = []
+            groups[section_name].extend(grouped_circuits)
+
+        for section_name, grouped_circuits in groups.items():
+            if section_name == DEFAULT_SECTION_NAME:
+                circuits.append(write_patch_section(DEFAULT_SECTION_NAME))
+            else:
+                comment = self.sections.get(section_name)
+                circuits.append(write_patch_section(section_name, comment))
 
-        for circuit in self.circuits:
-            if (
-                current_section
-                and circuit.section is not None
-                and circuit.section != current_section
-            ):
-                comment = self.sections.get(circuit.section)
-                circuits.append(write_patch_section(circuit.section, comment))
-                current_section = circuit.section
-            circuits.append(str(circuit))
+            for circuit in grouped_circuits:
+                circuits.append(str(circuit))
 
         return "\n".join(circuits)
 
     def __str__(self) -> str:
         """Output patch as string."""
         self._generate()
 
         labels = self._generate_labels()
         sorted_controllers = sorted(self.controllers, key=lambda x: x.position)
         controllers = "\n".join([str(controller) for controller in sorted_controllers])
-        circuits = self._get_circuits_as_strings()
+        if self._has_sections:
+            circuits = self._get_circuits_with_sections()
+        else:
+            circuits = self._get_circuits_as_strings()
 
         return f"{labels}{controllers}\n\n{circuits}"
 
     def _generate(self) -> None:
         """Generate patch.
 
         This is an internal function that ensures that we reset the patch if needed.
```

### Comparing `droid_metapatch-1.0.0/metapatch/options.py` & `droid_metapatch-1.1.0/metapatch/options.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.0.0/metapatch/utils.py` & `droid_metapatch-1.1.0/metapatch/utils.py`

 * *Files identical despite different names*

