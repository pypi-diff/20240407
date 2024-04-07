# Comparing `tmp/blint-2.0.6.tar.gz` & `tmp/blint-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.0.6.tar", max compression
+gzip compressed data, was "blint-2.0.7.tar", max compression
```

## Comparing `blint-2.0.6.tar` & `blint-2.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-03-19 11:25:09.065692 blint-2.0.6/LICENSE
--rw-r--r--   0        0        0     6147 2024-03-19 11:25:09.065692 blint-2.0.6/README.md
--rw-r--r--   0        0        0        0 2024-03-19 11:25:09.065692 blint-2.0.6/blint/__init__.py
--rw-r--r--   0        0        0    24122 2024-03-19 11:25:09.065692 blint-2.0.6/blint/analysis.py
--rw-r--r--   0        0        0    13955 2024-03-19 11:25:09.065692 blint-2.0.6/blint/android.py
--rw-r--r--   0        0        0    56201 2024-03-19 11:25:09.065692 blint-2.0.6/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-03-19 11:25:09.065692 blint-2.0.6/blint/checks.py
--rw-r--r--   0        0        0     5804 2024-03-19 11:25:09.065692 blint-2.0.6/blint/cli.py
--rw-r--r--   0        0        0    20365 2024-03-19 11:25:09.065692 blint-2.0.6/blint/config.py
--rw-r--r--   0        0        0      324 2024-03-19 11:25:09.065692 blint-2.0.6/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-03-19 11:25:09.065692 blint-2.0.6/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-03-19 11:25:09.065692 blint-2.0.6/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-03-19 11:25:09.065692 blint-2.0.6/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-03-19 11:25:09.065692 blint-2.0.6/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 11:25:09.065692 blint-2.0.6/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-03-19 11:25:09.065692 blint-2.0.6/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-03-19 11:25:09.065692 blint-2.0.6/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-03-19 11:25:09.069692 blint-2.0.6/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-03-19 11:25:09.069692 blint-2.0.6/blint/logger.py
--rw-r--r--   0        0        0    22901 2024-03-19 11:25:09.069692 blint-2.0.6/blint/sbom.py
--rw-r--r--   0        0        0    14323 2024-03-19 11:25:09.069692 blint-2.0.6/blint/utils.py
--rw-r--r--   0        0        0     1812 2024-03-19 11:25:09.073692 blint-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     7333 1970-01-01 00:00:00.000000 blint-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-07 21:55:22.516859 blint-2.0.7/LICENSE
+-rw-r--r--   0        0        0     6215 2024-04-07 21:55:22.516859 blint-2.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 21:55:22.516859 blint-2.0.7/blint/__init__.py
+-rw-r--r--   0        0        0    24122 2024-04-07 21:55:22.516859 blint-2.0.7/blint/analysis.py
+-rw-r--r--   0        0        0    13955 2024-04-07 21:55:22.516859 blint-2.0.7/blint/android.py
+-rw-r--r--   0        0        0    56201 2024-04-07 21:55:22.516859 blint-2.0.7/blint/binary.py
+-rw-r--r--   0        0        0     2794 2024-04-07 21:55:22.516859 blint-2.0.7/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cli.py
+-rw-r--r--   0        0        0    20365 2024-04-07 21:55:22.520859 blint-2.0.7/blint/config.py
+-rw-r--r--   0        0        0      324 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-04-07 21:55:22.520859 blint-2.0.7/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-04-07 21:55:22.520859 blint-2.0.7/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-04-07 21:55:22.520859 blint-2.0.7/blint/logger.py
+-rw-r--r--   0        0        0    23205 2024-04-07 21:55:22.520859 blint-2.0.7/blint/sbom.py
+-rw-r--r--   0        0        0    14323 2024-04-07 21:55:22.520859 blint-2.0.7/blint/utils.py
+-rw-r--r--   0        0        0     1812 2024-04-07 21:55:22.524859 blint-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7401 1970-01-01 00:00:00.000000 blint-2.0.7/PKG-INFO
```

### Comparing `blint-2.0.6/LICENSE` & `blint-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/README.md` & `blint-2.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,15 @@
   -h, --help            show this help message and exit
   -i SRC_DIR_IMAGE [SRC_DIR_IMAGE ...], --src SRC_DIR_IMAGE [SRC_DIR_IMAGE ...]
                         Source directories, container images or binary files. Defaults to current directory.
   -o SBOM_OUTPUT, --output-file SBOM_OUTPUT
                         SBOM output file. Defaults to bom.json in current directory.
   --deep                Enable deep mode to collect more used symbols and modules aggressively. Slow
                         operation.
+  --stdout              Print the SBOM to stdout instead of a file.
 ```
 
 To test any binary, including default commands
 
 ```bash
 blint -i /bin/netstat -o /tmp/blint
 ```
```

### Comparing `blint-2.0.6/blint/analysis.py` & `blint-2.0.7/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/android.py` & `blint-2.0.7/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/binary.py` & `blint-2.0.7/blint/binary.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/checks.py` & `blint-2.0.7/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/cli.py` & `blint-2.0.7/blint/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
+import logging
 import os
 import sys
 
 from blint.analysis import AnalysisRunner, report
 from blint.logger import LOG
 from blint.sbom import generate
 from blint.utils import gen_file_list
@@ -100,14 +101,21 @@
         "--deep",
         action="store_true",
         default=False,
         dest="deep_mode",
         help="Enable deep mode to collect more used symbols and modules "
              "aggressively. Slow operation.",
     )
+    sbom_parser.add_argument(
+        "--stdout",
+        action="store_true",
+        default=False,
+        dest="stdout_mode",
+        help="Print the SBOM to stdout instead of a file.",
+    )
     return parser.parse_args()
 
 
 def parse_input(src):
     """Parses the input source.
 
     This function takes the input source as a list and parses it to extract the
@@ -134,15 +142,15 @@
     arguments, reports directory, and source directory.
 
     Returns:
         tuple: A tuple containing the parsed arguments, reports directory, and
                source directory.
     """
     args = build_args()
-    if not args.no_banner:
+    if not args.no_banner and args.subcommand_name != "sbom":
         print(BLINT_LOGO)
     if not args.src_dir_image:
         args.src_dir_image = [os.getcwd()]
     if not os.getenv("CI"):
         src_dirs = args.src_dir_image
     else:
         src_dirs = parse_input(args.src_dir_image)
@@ -159,21 +167,25 @@
 
 def main():
     """Main function of the blint tool"""
     args, reports_dir, src_dirs = handle_args()
 
     # SBOM command
     if args.subcommand_name == "sbom":
-        if args.sbom_output:
-            sbom_output = args.sbom_output
+        if args.stdout_mode:
+            sbom_output = sys.stdout
+            LOG.setLevel(logging.ERROR)
         else:
-            sbom_output = os.path.join(os.getcwd(), "bom.json")
-        sbom_output_dir = os.path.dirname(sbom_output)
-        if sbom_output_dir and not os.path.exists(sbom_output_dir):
-            os.makedirs(sbom_output_dir)
+            if args.sbom_output:
+                sbom_output = args.sbom_output
+            else:
+                sbom_output = os.path.join(os.getcwd(), "bom.json")
+            sbom_output_dir = os.path.dirname(sbom_output)
+            if sbom_output_dir and not os.path.exists(sbom_output_dir):
+                os.makedirs(sbom_output_dir)
         generate(src_dirs, sbom_output, args.deep_mode)
     # Default case
     else:
         if reports_dir and not os.path.exists(reports_dir):
             os.makedirs(reports_dir)
         files = gen_file_list(src_dirs)
         analyzer = AnalysisRunner()
```

### Comparing `blint-2.0.6/blint/config.py` & `blint-2.0.7/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/cyclonedx/spdx.py` & `blint-2.0.7/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/cyclonedx/spec.py` & `blint-2.0.7/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_entries_generic.yml` & `blint-2.0.7/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_entries_pe.yml` & `blint-2.0.7/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_exe_go.yml` & `blint-2.0.7/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_imports_pe.yml` & `blint-2.0.7/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_methods_generic.yml` & `blint-2.0.7/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_methods_mips.yml` & `blint-2.0.7/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_monero_generic.yml` & `blint-2.0.7/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_monero_go.yml` & `blint-2.0.7/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_monero_rust` & `blint-2.0.7/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_monero_rust.yml` & `blint-2.0.7/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_rootkits_win.yml` & `blint-2.0.7/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.0.7/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_symbols_generic.yml` & `blint-2.0.7/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.0.7/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_symbols_macho.yml` & `blint-2.0.7/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/annotations/review_symbols_rust.yml` & `blint-2.0.7/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/data/rules.yml` & `blint-2.0.7/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/logger.py` & `blint-2.0.7/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/blint/sbom.py` & `blint-2.0.7/blint/sbom.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,28 +171,37 @@
                 {
                     "ref": sbom.metadata.component.bom_ref.model_dump(mode="python"),
                     "dependsOn": root_depends_on,
                 }
             )
     # Populate the dependencies
     sbom.dependencies = dependencies
-    LOG.debug(
-        f"SBOM includes {len(components)} components and {len(dependencies)} dependencies",
-    )
-    with open(output_file, mode="w", encoding="utf-8") as fp:
-        fp.write(
-            sbom.model_dump_json(
-                indent=None if deep_mode else 2,
-                exclude_none=True,
-                exclude_defaults=True,
-                warnings=False,
-                by_alias=True
-            )
+    if isinstance(output_file, str):
+        LOG.debug(
+            f"SBOM includes {len(components)} components and {len(dependencies)} dependencies",
         )
-        LOG.debug(f"SBOM file generated successfully at {output_file}")
+        with open(output_file, mode="w", encoding="utf-8") as fp:
+            fp.write(
+                sbom.model_dump_json(
+                    indent=None if deep_mode else 2,
+                    exclude_none=True,
+                    exclude_defaults=True,
+                    warnings=False,
+                    by_alias=True
+                )
+            )
+            LOG.debug(f"SBOM file generated successfully at {output_file}")
+    else:
+        output_file.write(sbom.model_dump_json(
+            indent=2,
+            exclude_none=True,
+            exclude_defaults=True,
+            warnings=False,
+            by_alias=True
+        ))
     return True
 
 
 def components_from_symbols_version(symbols_version: list[dict]) -> list[Component]:
     """
     Creates a list of Component objects from symbols version.
     This style of detection is quite imprecise since the version is just a min specifier.
```

### Comparing `blint-2.0.6/blint/utils.py` & `blint-2.0.7/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.0.6/pyproject.toml` & `blint-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.0.6"
+version = "2.0.7"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
```

### Comparing `blint-2.0.6/PKG-INFO` & `blint-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.0.6
+Version: 2.0.7
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -104,14 +104,15 @@
   -h, --help            show this help message and exit
   -i SRC_DIR_IMAGE [SRC_DIR_IMAGE ...], --src SRC_DIR_IMAGE [SRC_DIR_IMAGE ...]
                         Source directories, container images or binary files. Defaults to current directory.
   -o SBOM_OUTPUT, --output-file SBOM_OUTPUT
                         SBOM output file. Defaults to bom.json in current directory.
   --deep                Enable deep mode to collect more used symbols and modules aggressively. Slow
                         operation.
+  --stdout              Print the SBOM to stdout instead of a file.
 ```
 
 To test any binary, including default commands
 
 ```bash
 blint -i /bin/netstat -o /tmp/blint
 ```
```

