# Comparing `tmp/Nuitka-winsvc-2.1.4.tar.gz` & `tmp/Nuitka-winsvc-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-2.1.4.tar", last modified: Mon Apr  1 07:38:34 2024, max compression
+gzip compressed data, was "Nuitka-winsvc-2.1.5.tar", last modified: Sun Apr  7 02:16:35 2024, max compression
```

## Comparing `Nuitka-winsvc-2.1.4.tar` & `Nuitka-winsvc-2.1.5.tar`

### file list

```diff
@@ -1,1833 +1,1833 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:34.227652 Nuitka-winsvc-2.1.4/
--rw-rw-rw-   0        0        0      228 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/Changelog.rst
--rw-rw-rw-   0        0        0   152282 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1717 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:34.225700 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4853 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    77833 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-05 02:20:24.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 07:38:25.000000 Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4853 2024-04-01 07:38:34.226675 Nuitka-winsvc-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/README.md
--rw-rw-rw-   0        0        0    80812 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.761422 Nuitka-winsvc-2.1.4/bin/
--rw-rw-rw-   0        0        0     1166 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1165 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3105 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1194 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/nuitka
--rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.779972 Nuitka-winsvc-2.1.4/doc/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.807329 Nuitka-winsvc-2.1.4/doc/Logo/
--rw-rw-rw-   0        0        0     1797 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     1553 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0     1793 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.852234 Nuitka-winsvc-2.1.4/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Vertical.png
--rw-rw-rw-   0        0        0    33808 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/doc/nuitka-run.1
--rw-rw-rw-   0        0        0    33832 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/doc/nuitka.1
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.878352 Nuitka-winsvc-2.1.4/lib/
--rw-rw-rw-   0        0        0     4640 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/lib/hints.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.889145 Nuitka-winsvc-2.1.4/misc/
--rwxrwxrwx   0        0        0      924 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1061 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.919987 Nuitka-winsvc-2.1.4/nuitka/
--rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     5787 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3800 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1855 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Errors.py
--rw-rw-rw-   0        0        0    10335 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/HardImportRegistry.py
--rw-rw-rw-   0        0        0    38348 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8616 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    64040 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    75581 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/Options.py
--rw-rw-rw-   0        0        0     5276 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    14940 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     6797 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Progress.py
--rw-rw-rw-   0        0        0     9654 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4093 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    14557 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     8989 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Serialization.py
--rw-rw-rw-   0        0        0     4703 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    13335 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3513 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15470 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2466 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/Version.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5604 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.987753 Nuitka-winsvc-2.1.4/nuitka/build/
--rw-rw-rw-   0        0        0    36393 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8583 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    17770 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    14643 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    35449 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5592 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    15933 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2704 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    13210 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    26957 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.562483 Nuitka-winsvc-2.1.4/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.336546 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     8001 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3499 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     5196 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     2006 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9333 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2195 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9233 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    17661 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     7267 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9189 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1866 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7620 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1345 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0     1187 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/environment_variables.h
--rw-rw-rw-   0        0        0     1872 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/environment_variables_system.h
--rw-rw-rw-   0        0        0     5302 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/exception_groups.h
--rw-rw-rw-   0        0        0    34114 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3792 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6474 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.743388 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3698 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1233 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1164 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0    11894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10644 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13168 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1834 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13551 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1235 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     4291 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1827 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     2970 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9599 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3601 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1386 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4671 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12714 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5451 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5489 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2828 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15807 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13239 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5820 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4743 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5853 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5467 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    20173 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8699 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3782 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2756 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10655 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9230 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5176 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4378 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     5004 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4855 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     3381 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2367 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1175 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1141 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8750 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1363 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17975 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5749 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    16626 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     6150 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0    15484 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     2899 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1811 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2343 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3809 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3447 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     3135 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.608773 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.767538 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.769453 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.770432 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1695 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.563459 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.774336 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.775312 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.780196 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.780196 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.783138 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.793917 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.808560 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.815400 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.833954 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.584647 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.578786 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.847479 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.850410 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.853367 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.859198 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    15042 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.862707 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.865730 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.909962 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.915411 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.916371 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.919301 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4380 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.924190 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.581715 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.938502 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.940487 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.948329 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    17055 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.951250 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:26.961573 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.031989 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.056630 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.057605 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.062086 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.067315 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4435 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.069259 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.584647 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.090377 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.092333 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.110866 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.125506 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.135432 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.251827 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.256710 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.256710 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.258663 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.262607 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.265501 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4648 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.267501 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.268430 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.288045 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.606818 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.289990 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107452 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.606818 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.298312 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1595 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      307 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0    10790 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9726 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0      167 2024-01-29 03:26:21.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.299297 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.340820 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.341795 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.370195 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.371172 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:27.418312 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:28.041938 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/
--rw-rw-rw-   0        0        0     1002 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/LICENSE
--rw-rw-rw-   0        0        0    31605 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/crc32.c
--rw-rw-rw-   0        0        0   591749 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/crc32.h
--rw-rw-rw-   0        0        0    16682 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zconf.h
--rw-rw-rw-   0        0        0    96778 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zlib.h
--rw-rw-rw-   0        0        0     7247 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zutil.h
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:28.263252 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:29.691350 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:29.737690 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:30.947437 Nuitka-winsvc-2.1.4/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    84761 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     9142 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    58739 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    73577 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    40760 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0   109285 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    63983 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    56631 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    22473 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    19054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    38264 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    23678 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   114017 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3062 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13376 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   481627 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     2065 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     3051 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   318307 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4762 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   313126 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   312537 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   316340 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   315751 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   315055 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36776 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    20361 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    39584 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    26620 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     2066 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDumpBacktraces.c
--rw-rw-rw-   0        0        0     2194 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersEnvironmentVariables.c
--rw-rw-rw-   0        0        0     2979 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
--rw-rw-rw-   0        0        0     7145 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     8018 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    28806 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2455 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1803 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    16080 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    16403 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0    19996 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13944 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1669 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3587 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   181603 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    16729 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77811 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    68218 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1265 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    69479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6300 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83954 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13805 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183867 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188543 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3433 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    67184 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    79484 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1052 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77854 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70494 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68736 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   150679 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4240 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53151 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    77119 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47857 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17771 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136385 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142240 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74749 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    83262 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45341 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    82871 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76950 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3394 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    15663 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0     3868 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3759 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1975 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    27056 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     5628 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    12136 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    53985 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    63759 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     4827 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6651 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    21896 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    37113 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     8050 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:30.989953 Nuitka-winsvc-2.1.4/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6491 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10821 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2371 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    17005 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    36111 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4958 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    52589 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2408 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14272 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     5083 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    17645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7368 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     6661 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    33901 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8589 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1607 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28934 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2158 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9415 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12951 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     9011 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7383 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2126 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17804 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    28337 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7828 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     6384 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6985 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1870 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    14684 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1429 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1574 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1066 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3567 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12211 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     2055 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    16152 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6658 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0    10016 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3174 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1638 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6455 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8225 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0    12685 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    30146 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13251 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5267 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6591 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    14005 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0    10087 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8302 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0    11208 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0    14747 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9154 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8129 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:30.995817 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6102 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3432 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1837 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1411 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3642 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5161 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5244 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     3988 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19696 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2885 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.003132 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2948 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     8928 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2358 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6483 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3460 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3390 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2409 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4535 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    22938 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6800 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2508 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.071002 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11318 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5829 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23986 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5438 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1755 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1693 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2706 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    13624 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     1894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2618 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1394 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7047 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12700 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     1968 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     4081 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7257 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4142 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3710 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4379 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11758 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19167 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2693 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11336 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15540 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2829 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10271 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2407 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     2870 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2834 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3128 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.073931 Nuitka-winsvc-2.1.4/nuitka/containers/
--rw-rw-rw-   0        0        0     1468 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4430 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.075884 Nuitka-winsvc-2.1.4/nuitka/distutils/
--rw-rw-rw-   0        0        0     2308 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    15025 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.076861 Nuitka-winsvc-2.1.4/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1257 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6059 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.083696 Nuitka-winsvc-2.1.4/nuitka/freezer/
--rw-rw-rw-   0        0        0     7778 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2616 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    12609 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7469 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6633 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    11979 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/ImportDetection.py
--rw-rw-rw-   0        0        0    17908 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0    11415 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0    10516 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    11988 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.087602 Nuitka-winsvc-2.1.4/nuitka/importing/
--rw-rw-rw-   0        0        0    11040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    31922 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4869 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    18804 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    12784 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.146774 Nuitka-winsvc-2.1.4/nuitka/nodes/
--rw-rw-rw-   0        0        0     3670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4115 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    13255 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   378777 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4131 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2529 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1731 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2760 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4727 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4981 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2275 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     1457 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinInputNodes.py
--rw-rw-rw-   0        0        0     5367 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12756 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     2029 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3639 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3787 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   245569 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18648 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9100 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3353 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13576 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1606 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26146 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6511 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1583 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   623739 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8480 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6618 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30300 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    46568 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12246 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2867 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4614 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1747 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    51054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     7889 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     7408 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    44902 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    55109 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12024 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3577 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    39667 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5409 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6288 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6883 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    92183 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5378 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    47515 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2766 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1534 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11519 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11035 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16821 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23177 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    15007 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15995 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1745 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6567 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    32713 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0    24461 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15147 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5580 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31948 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     8975 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     5229 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12468 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    34736 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0    12241 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3440 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6805 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4748 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12547 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    97361 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9336 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28691 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3537 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8329 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0    17886 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2438 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0    11094 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    42396 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10779 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4607 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    31228 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4781 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3937 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.150676 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   157197 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4420 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     5076 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42509 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.155623 Nuitka-winsvc-2.1.4/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3358 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2177 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10866 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52487 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2288 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    45089 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    24504 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.156592 Nuitka-winsvc-2.1.4/nuitka/pgo/
--rw-rw-rw-   0        0        0     4932 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.158544 Nuitka-winsvc-2.1.4/nuitka/plugins/
--rw-rw-rw-   0        0        0    56921 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    59723 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.235718 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    30408 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3510 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0    10754 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     5080 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DelvewheelPlugin.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.257343 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin/
--rw-rw-rw-   0        0        0     1646 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin/DillPlugin.c
--rw-rw-rw-   0        0        0     9826 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
--rw-rw-rw-   0        0        0     2679 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    16277 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1913 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     4017 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     4854 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    32261 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     5024 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     8823 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     7080 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1220 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     7433 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1940 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     7042 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    53098 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1193 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    13878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1173 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0    10289 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TransformersPlugin.py
--rw-rw-rw-   0        0        0     1106 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5668 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   230668 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2352 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0    12392 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.268115 Nuitka-winsvc-2.1.4/nuitka/reports/
--rw-rw-rw-   0        0        0     2287 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/reports/CompilationReportReader.py
--rw-rw-rw-   0        0        0     2089 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    27497 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.274022 Nuitka-winsvc-2.1.4/nuitka/specs/
--rw-rw-rw-   0        0        0     5943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2818 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2573 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    26786 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6097 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4834 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     6244 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18739 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.274998 Nuitka-winsvc-2.1.4/nuitka/tools/
--rw-rw-rw-   0        0        0     1631 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.274998 Nuitka-winsvc-2.1.4/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      847 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.276951 Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    15004 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1338 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.277927 Nuitka-winsvc-2.1.4/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2481 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     4199 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.278904 Nuitka-winsvc-2.1.4/nuitka/tools/general/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.280859 Nuitka-winsvc-2.1.4/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2352 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.282812 Nuitka-winsvc-2.1.4/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/general/find_module/FindModuleCode.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/general/find_module/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.283787 Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0    12545 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.285740 Nuitka-winsvc-2.1.4/nuitka/tools/podman/
--rw-rw-rw-   0        0        0     1905 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/podman/Podman.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/podman/__init__.py
--rw-rw-rw-   0        0        0    11623 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/podman/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.286716 Nuitka-winsvc-2.1.4/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2561 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.288669 Nuitka-winsvc-2.1.4/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     3590 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2314 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.291599 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51531 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7717 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39659 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    35715 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.296533 Nuitka-winsvc-2.1.4/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    55682 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1516 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0    10024 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1311 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     8061 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5413 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3408 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.297511 Nuitka-winsvc-2.1.4/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.299463 Nuitka-winsvc-2.1.4/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29877 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.300438 Nuitka-winsvc-2.1.4/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1980 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.301414 Nuitka-winsvc-2.1.4/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8758 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.302390 Nuitka-winsvc-2.1.4/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    35342 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.303886 Nuitka-winsvc-2.1.4/nuitka/tools/watch/
--rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/watch/GitHub.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/watch/__init__.py
--rw-rw-rw-   0        0        0    20868 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tools/watch/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.324456 Nuitka-winsvc-2.1.4/nuitka/tree/
--rw-rw-rw-   0        0        0    50370 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    75150 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1733 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2604 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1544 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    43101 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2981 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11746 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15446 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    38235 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6523 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22175 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11196 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14757 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    30821 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    14095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6630 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2442 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     7608 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4711 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15606 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4857 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14948 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5707 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14439 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3852 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0    13212 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3790 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    23005 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20465 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.342381 Nuitka-winsvc-2.1.4/nuitka/utils/
--rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     4148 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     6395 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0    14981 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     6413 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    13185 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    41401 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.4/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     3753 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2395 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0    10121 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     7884 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2257 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4586 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1271 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4477 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5092 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9951 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4588 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     1889 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    23857 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3697 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     3687 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     2084 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/SlotMetaClasses.py
--rw-rw-rw-   0        0        0     6603 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2634 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2798 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    11527 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10606 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 07:38:34.227652 Nuitka-winsvc-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0    16350 2024-04-01 07:35:16.000000 Nuitka-winsvc-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.343357 Nuitka-winsvc-2.1.4/tests/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.906329 Nuitka-winsvc-2.1.4/tests/basics/
--rw-rw-rw-   0        0        0     1798 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5966 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5910 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4086 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1136 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3781 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17112 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      898 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4796 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3446 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1438 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4729 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4672 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1661 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2349 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1159 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      838 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14418 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      993 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1490 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6779 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1449 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1690 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12367 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3635 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2659 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      922 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1318 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2501 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4259 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1536 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1650 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1703 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2763 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2955 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3361 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1568 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1957 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     2008 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14935 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1859 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1484 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5885 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1931 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      895 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1444 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      910 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    24719 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2109 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7850 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     5041 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5478 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22998 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1573 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1820 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2118 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2244 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2307 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2336 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2360 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1125 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1909 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2143 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4913 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3103 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3851 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2302 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:31.930688 Nuitka-winsvc-2.1.4/tests/onefile/
--rw-rw-rw-   0        0        0     1341 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1339 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5846 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.055411 Nuitka-winsvc-2.1.4/tests/optimizations/
--rw-rw-rw-   0        0        0      991 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1087 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Attributes.py
--rw-rw-rw-   0        0        0     1053 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Calls.py
--rw-rw-rw-   0        0        0      953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Conditions.py
--rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/DecodingOperations.py
--rw-rw-rw-   0        0        0     1246 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/FormatStrings36.py
--rw-rw-rw-   0        0        0     1183 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/HardImports.py
--rw-rw-rw-   0        0        0     1007 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/HardImports_2.py
--rw-rw-rw-   0        0        0      950 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1292 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Len.py
--rw-rw-rw-   0        0        0     1133 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Matching310.py
--rw-rw-rw-   0        0        0     2295 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Operations.py
--rw-rw-rw-   0        0        0     1365 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/Subscripts.py
--rw-rw-rw-   0        0        0     8827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.064994 Nuitka-winsvc-2.1.4/tests/packages/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.089343 Nuitka-winsvc-2.1.4/tests/packages/package_data_files_embedding/
--rw-rw-rw-   0        0        0     1576 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/package_data_files_embedding/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.097156 Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2414 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.113755 Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      975 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.618454 Nuitka-winsvc-2.1.4/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.162968 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1262 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      940 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      942 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.196748 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      961 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      999 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0     1001 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.618454 Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.213402 Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2368 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.221201 Nuitka-winsvc-2.1.4/tests/plugins/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.229664 Nuitka-winsvc-2.1.4/tests/plugins/code_signing/
--rw-rw-rw-   0        0        0     1202 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/code_signing/CodeSigningMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.242455 Nuitka-winsvc-2.1.4/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1474 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.253083 Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.253083 Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      309 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.4/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.257581 Nuitka-winsvc-2.1.4/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1051 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2218 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3892 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.268229 Nuitka-winsvc-2.1.4/tests/programs/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.277824 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.309490 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      828 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1076 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      893 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.316258 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.328606 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.337556 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.346343 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.353179 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.357083 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.366483 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.370385 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.375271 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.383799 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.393564 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1107 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.399950 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.414164 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.417094 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.433695 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.446388 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.474708 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.542299 Nuitka-winsvc-2.1.4/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.549711 Nuitka-winsvc-2.1.4/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.555566 Nuitka-winsvc-2.1.4/tests/programs/deep/
--rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.575067 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0     1012 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.587310 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      984 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.590235 Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      826 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.603875 Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      829 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      889 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.613212 Nuitka-winsvc-2.1.4/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1037 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.631598 Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      978 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1130 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      854 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0     1026 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.638430 Nuitka-winsvc-2.1.4/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.670514 Nuitka-winsvc-2.1.4/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1112 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.683249 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1561 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.692155 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.710149 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.720472 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.728934 Nuitka-winsvc-2.1.4/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.743749 Nuitka-winsvc-2.1.4/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1110 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1391 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.754504 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.786035 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      868 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1791 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.787384 Nuitka-winsvc-2.1.4/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.792262 Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      856 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.797154 Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.806531 Nuitka-winsvc-2.1.4/tests/programs/package_code/
--rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.818026 Nuitka-winsvc-2.1.4/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.829182 Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.852151 Nuitka-winsvc-2.1.4/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      855 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.863957 Nuitka-winsvc-2.1.4/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1040 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.866687 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.875687 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.879392 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.885868 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      958 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.895467 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      997 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.901326 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0     1009 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.922063 Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      933 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.926616 Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.937359 Nuitka-winsvc-2.1.4/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      884 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.961785 Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.968293 Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     3004 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.980373 Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:25.633020 Nuitka-winsvc-2.1.4/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:32.989517 Nuitka-winsvc-2.1.4/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.000254 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1760 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.007638 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.019358 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.039672 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.042593 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.047475 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1585 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.051381 Nuitka-winsvc-2.1.4/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      891 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.063258 Nuitka-winsvc-2.1.4/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      803 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.068488 Nuitka-winsvc-2.1.4/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.073373 Nuitka-winsvc-2.1.4/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.083139 Nuitka-winsvc-2.1.4/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.087917 Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.096706 Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6646 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.111354 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.127509 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1268 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.139215 Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      822 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.141171 Nuitka-winsvc-2.1.4/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      995 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.142146 Nuitka-winsvc-2.1.4/tests/programs/with space/
--rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.143120 Nuitka-winsvc-2.1.4/tests/reflected/
--rw-rw-rw-   0        0        0    14194 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/run-tests
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.251453 Nuitka-winsvc-2.1.4/tests/standalone/
--rw-rw-rw-   0        0        0     1090 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2586 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1950 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/DateutilsUsing.py
--rw-rw-rw-   0        0        0     1168 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/GiUsing.py
--rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1216 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1057 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1118 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1215 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1598 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2570 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1759 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      979 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1479 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1098 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1248 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2106 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1099 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1369 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2198 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PyQt6Plugins.py
--rw-rw-rw-   0        0        0     2168 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PySide2Using.py
--rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PySide6Plugins.py
--rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1371 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0     1227 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.4/tests/standalone/SetuptoolsUsing.py
--rw-rw-rw-   0        0        0     1005 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1569 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1973 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3260 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1232 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9912 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:33.258287 Nuitka-winsvc-2.1.4/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1296 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:34.218461 Nuitka-winsvc-2.1.4/tests/syntax/
--rw-rw-rw-   0        0        0      844 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      818 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/AwaitInModule36.py
--rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0     1002 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      882 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1142 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      947 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      915 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      808 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2234 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.4/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:35.044941 Nuitka-winsvc-2.1.5/
+-rw-rw-rw-   0        0        0      228 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/Changelog.rst
+-rw-rw-rw-   0        0        0   152282 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1717 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:35.043941 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4853 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    77833 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-02-05 02:20:24.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-07 02:16:29.000000 Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4853 2024-04-07 02:16:35.043941 Nuitka-winsvc-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/README.md
+-rw-rw-rw-   0        0        0    80812 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.557336 Nuitka-winsvc-2.1.5/bin/
+-rw-rw-rw-   0        0        0     1166 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1165 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3105 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1194 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/nuitka
+-rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.582325 Nuitka-winsvc-2.1.5/doc/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.610616 Nuitka-winsvc-2.1.5/doc/Logo/
+-rw-rw-rw-   0        0        0     1797 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     1553 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0     1793 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.629212 Nuitka-winsvc-2.1.5/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Vertical.png
+-rw-rw-rw-   0        0        0    33808 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/doc/nuitka-run.1
+-rw-rw-rw-   0        0        0    33832 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/doc/nuitka.1
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.647259 Nuitka-winsvc-2.1.5/lib/
+-rw-rw-rw-   0        0        0     4640 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/lib/hints.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.657584 Nuitka-winsvc-2.1.5/misc/
+-rwxrwxrwx   0        0        0      924 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1061 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.677658 Nuitka-winsvc-2.1.5/nuitka/
+-rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5787 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3800 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1855 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    10335 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/HardImportRegistry.py
+-rw-rw-rw-   0        0        0    38348 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8616 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    64040 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    75773 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5276 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    14940 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     6797 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     9654 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4093 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    14557 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     8989 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Serialization.py
+-rw-rw-rw-   0        0        0     4703 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    13335 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3513 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15470 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2466 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/Version.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5604 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.708418 Nuitka-winsvc-2.1.5/nuitka/build/
+-rw-rw-rw-   0        0        0    36393 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8583 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    17770 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    14643 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    35449 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5592 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    15933 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2704 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    13210 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    26957 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.402326 Nuitka-winsvc-2.1.5/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.975375 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     8001 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3499 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     5196 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     2006 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9333 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2195 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9233 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    17661 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     7267 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9189 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1866 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7620 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1345 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0     1187 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/environment_variables.h
+-rw-rw-rw-   0        0        0     1872 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/environment_variables_system.h
+-rw-rw-rw-   0        0        0     5302 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/exception_groups.h
+-rw-rw-rw-   0        0        0    34114 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3792 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6474 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.380673 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3698 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1233 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1164 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0    11894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10644 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13168 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1834 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13551 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1235 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     4291 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1827 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     2970 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9599 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3601 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1386 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4671 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12714 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5451 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5489 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2828 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15807 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13239 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5820 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4743 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5853 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5467 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    20173 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8699 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3782 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2756 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10655 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9230 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5176 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4378 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     5004 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4855 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     3381 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2367 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1175 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1141 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8750 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1363 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17975 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5749 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    16626 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     6150 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0    15484 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     2899 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1811 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2343 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3809 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3447 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     3135 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.415313 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.411772 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.413771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.414771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1695 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.404319 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.418771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.419771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.422771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.423771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.433771 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.445772 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.458799 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.466786 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.482745 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.410321 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.406318 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.495746 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.497748 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.501747 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.507745 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    15042 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.509745 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.512745 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.549313 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.553312 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.554316 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.557317 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4380 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.561316 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.408317 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.571316 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.573315 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.579315 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    17055 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.581314 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.583317 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.620314 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.624314 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.624314 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.625332 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.627330 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4435 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.628323 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.411318 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.641922 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.643922 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.648923 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.652923 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.656474 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.692447 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.696454 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.696454 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.698454 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.699445 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.702446 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4648 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.704445 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.704445 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.711447 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.413318 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.713453 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107452 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.414329 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.720446 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1595 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      307 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0    10790 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9726 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0      167 2024-01-29 03:26:21.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.721445 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.738006 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.739002 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.748848 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.749847 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.760845 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.821431 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/
+-rw-rw-rw-   0        0        0     1002 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/LICENSE
+-rw-rw-rw-   0        0        0    31605 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/crc32.c
+-rw-rw-rw-   0        0        0   591749 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/crc32.h
+-rw-rw-rw-   0        0        0    16682 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zconf.h
+-rw-rw-rw-   0        0        0    96778 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zlib.h
+-rw-rw-rw-   0        0        0     7247 2023-12-06 01:19:25.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zutil.h
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.857431 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.943760 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:30.963758 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.748708 Nuitka-winsvc-2.1.5/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    84761 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     9142 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    58739 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    73577 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    40760 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0   109285 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    63983 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    56631 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    22473 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    19054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    38264 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    23678 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   114017 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3062 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13376 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   481627 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     2065 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     3051 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   318307 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4762 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   313126 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   312537 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   316340 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   315751 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   315055 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36776 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    20361 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    39584 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    26620 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     2066 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDumpBacktraces.c
+-rw-rw-rw-   0        0        0     2194 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariables.c
+-rw-rw-rw-   0        0        0     2979 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
+-rw-rw-rw-   0        0        0     7145 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     8018 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    28806 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2455 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1803 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    16080 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    16403 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0    19996 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13944 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1669 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3587 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   181603 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    16729 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77811 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    68218 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1265 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    69479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6300 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83954 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13805 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183867 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188543 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3433 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    67184 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    79484 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1052 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77854 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70494 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68736 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   150679 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4240 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53151 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    77119 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47857 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17771 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136385 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142240 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74749 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    83262 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45341 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    82871 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76950 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3394 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    15663 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0     3868 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3759 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1975 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    27056 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4181 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     5628 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    12136 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    54017 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    63759 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     4827 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6651 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    21896 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    37113 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     8050 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.789283 Nuitka-winsvc-2.1.5/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6491 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10821 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2371 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    17005 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    36111 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4958 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    52589 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2408 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14272 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     5083 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    17645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4479 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7368 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     6661 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    33901 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8589 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1607 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28934 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2158 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9415 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12951 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     9011 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7383 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2126 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17804 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    28337 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7828 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     6384 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6985 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1870 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    14684 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1429 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1574 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1066 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3567 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12211 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     2055 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2645 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    16152 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6658 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0    10016 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3174 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1638 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6455 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8225 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0    12685 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    30146 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13251 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5267 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6591 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    14005 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0    10087 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8302 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0    11208 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0    14747 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9154 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     8129 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.794284 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6102 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3432 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1837 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1411 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3642 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5161 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5244 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3988 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19696 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2885 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.801250 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2948 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     8928 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2358 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6483 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3460 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3390 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2409 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4535 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    22938 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6800 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2508 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.869775 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11318 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5829 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23986 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5438 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1755 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1693 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2706 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    13624 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     1894 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2618 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1394 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7047 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12700 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     1968 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     4081 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7257 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4142 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3710 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4379 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11758 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19167 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2693 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11336 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15540 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2829 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10271 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2407 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     2870 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2834 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3128 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.871774 Nuitka-winsvc-2.1.5/nuitka/containers/
+-rw-rw-rw-   0        0        0     1468 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4430 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.873786 Nuitka-winsvc-2.1.5/nuitka/distutils/
+-rw-rw-rw-   0        0        0     2308 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    15025 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.875776 Nuitka-winsvc-2.1.5/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1257 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6059 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.880775 Nuitka-winsvc-2.1.5/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7778 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2616 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    12609 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7469 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6633 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    11979 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/ImportDetection.py
+-rw-rw-rw-   0        0        0    17908 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0    11415 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0    10516 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    11988 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.884775 Nuitka-winsvc-2.1.5/nuitka/importing/
+-rw-rw-rw-   0        0        0    11040 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    31922 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4869 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    18804 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    12787 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.944774 Nuitka-winsvc-2.1.5/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3670 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4115 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    13255 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   378777 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4131 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2529 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1731 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2760 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4727 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4981 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2275 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     1457 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinInputNodes.py
+-rw-rw-rw-   0        0        0     5367 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12756 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     2029 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3639 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3787 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   245569 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18648 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9100 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3353 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13576 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1606 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26146 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6511 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1583 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   623739 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8480 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6618 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21716 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30300 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    46568 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12246 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2867 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4614 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1747 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51054 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     7889 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     7408 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    44902 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    55109 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12024 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3577 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    39667 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5409 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6288 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6961 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    92183 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5378 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    47515 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2766 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1534 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11519 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11035 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16821 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23177 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    15007 2024-03-06 05:39:35.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15995 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1745 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6567 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    32713 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0    24461 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15147 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5580 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31948 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     8975 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     5229 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12468 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    34736 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0    12241 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3440 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6805 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4748 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12547 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    97361 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9336 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28691 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3537 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8329 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0    17886 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2438 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0    11094 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    42396 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10779 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4607 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    31228 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4781 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3937 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.946773 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   157197 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4420 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     5076 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42509 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.951773 Nuitka-winsvc-2.1.5/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3358 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2177 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10866 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52487 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2288 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    45089 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    24504 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.952773 Nuitka-winsvc-2.1.5/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4932 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.953774 Nuitka-winsvc-2.1.5/nuitka/plugins/
+-rw-rw-rw-   0        0        0    56921 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    59723 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.979319 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    30408 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3510 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0    10754 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     5080 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DelvewheelPlugin.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:31.995319 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin/
+-rw-rw-rw-   0        0        0     1646 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin/DillPlugin.c
+-rw-rw-rw-   0        0        0     9826 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
+-rw-rw-rw-   0        0        0     2679 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    16277 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1913 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     4017 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     4854 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    32261 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     5024 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     8823 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     7080 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1220 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     7433 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1940 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     7042 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    53098 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1193 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    13878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1173 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0    12838 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TransformersPlugin.py
+-rw-rw-rw-   0        0        0     1106 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5668 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   231363 2024-04-07 02:15:13.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2352 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0    12392 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.009328 Nuitka-winsvc-2.1.5/nuitka/reports/
+-rw-rw-rw-   0        0        0     2287 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/reports/CompilationReportReader.py
+-rw-rw-rw-   0        0        0     2089 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    27497 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.016322 Nuitka-winsvc-2.1.5/nuitka/specs/
+-rw-rw-rw-   0        0        0     5943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2818 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2573 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    26786 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6097 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4834 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     6244 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18739 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.017322 Nuitka-winsvc-2.1.5/nuitka/tools/
+-rw-rw-rw-   0        0        0     1631 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.017322 Nuitka-winsvc-2.1.5/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      847 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.019319 Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    15004 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.021322 Nuitka-winsvc-2.1.5/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2481 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     4199 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.021322 Nuitka-winsvc-2.1.5/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.022322 Nuitka-winsvc-2.1.5/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2352 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.023326 Nuitka-winsvc-2.1.5/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/general/find_module/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.025322 Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0    12545 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.027322 Nuitka-winsvc-2.1.5/nuitka/tools/podman/
+-rw-rw-rw-   0        0        0     1905 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/podman/Podman.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/podman/__init__.py
+-rw-rw-rw-   0        0        0    11623 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/podman/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.028322 Nuitka-winsvc-2.1.5/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2561 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.029322 Nuitka-winsvc-2.1.5/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     3590 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2314 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.032322 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51531 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7717 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39659 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    35715 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.036322 Nuitka-winsvc-2.1.5/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    55682 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1516 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0    10024 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1311 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     8061 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5413 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3408 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.037322 Nuitka-winsvc-2.1.5/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.038320 Nuitka-winsvc-2.1.5/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29877 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.039322 Nuitka-winsvc-2.1.5/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1980 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.040322 Nuitka-winsvc-2.1.5/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8758 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.041322 Nuitka-winsvc-2.1.5/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    35342 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.042322 Nuitka-winsvc-2.1.5/nuitka/tools/watch/
+-rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/watch/GitHub.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/watch/__init__.py
+-rw-rw-rw-   0        0        0    20868 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tools/watch/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.060233 Nuitka-winsvc-2.1.5/nuitka/tree/
+-rw-rw-rw-   0        0        0    50370 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    75150 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1733 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2604 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1544 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    43101 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2981 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11746 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15446 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    38235 2024-03-20 02:57:24.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6523 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    22175 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11196 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14757 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    30821 2024-03-14 05:29:37.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    14095 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6630 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2442 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     7608 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4711 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15606 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4857 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14948 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5707 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14439 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3852 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0    13212 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3790 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    23005 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20465 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.075822 Nuitka-winsvc-2.1.5/nuitka/utils/
+-rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     4148 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     6395 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0    14981 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     6413 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    13185 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    41401 2024-04-01 07:34:44.000000 Nuitka-winsvc-2.1.5/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     3753 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2395 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0    10121 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     7884 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2257 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4586 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1271 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4477 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5092 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9951 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4588 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     1889 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    23857 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3697 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     3687 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     2084 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/SlotMetaClasses.py
+-rw-rw-rw-   0        0        0     6603 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2634 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2798 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    11527 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10606 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:16:35.044941 Nuitka-winsvc-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0    16350 2024-04-07 02:15:34.000000 Nuitka-winsvc-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:32.076822 Nuitka-winsvc-2.1.5/tests/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.366504 Nuitka-winsvc-2.1.5/tests/basics/
+-rw-rw-rw-   0        0        0     1798 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5966 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5910 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4086 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1136 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3781 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17112 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      898 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4796 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3446 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1438 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4729 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4672 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1661 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2349 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1159 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      838 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14418 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      993 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1490 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6779 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1449 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1690 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12367 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3635 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2659 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      922 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1318 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2501 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4259 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1536 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1650 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1703 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2763 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2955 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3361 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1568 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1957 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     2008 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14935 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1859 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1484 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5885 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1931 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      895 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1444 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      910 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    24719 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2109 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7850 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     5041 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5478 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22998 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1573 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1820 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2118 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2244 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2307 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2336 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2360 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1125 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1909 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2143 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4913 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3103 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3851 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2302 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.383539 Nuitka-winsvc-2.1.5/tests/onefile/
+-rw-rw-rw-   0        0        0     1341 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1339 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5846 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.409699 Nuitka-winsvc-2.1.5/tests/optimizations/
+-rw-rw-rw-   0        0        0      991 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1087 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Attributes.py
+-rw-rw-rw-   0        0        0     1053 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Calls.py
+-rw-rw-rw-   0        0        0      953 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Conditions.py
+-rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/DecodingOperations.py
+-rw-rw-rw-   0        0        0     1246 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/FormatStrings36.py
+-rw-rw-rw-   0        0        0     1183 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/HardImports.py
+-rw-rw-rw-   0        0        0     1007 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/HardImports_2.py
+-rw-rw-rw-   0        0        0      950 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1292 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Len.py
+-rw-rw-rw-   0        0        0     1133 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Matching310.py
+-rw-rw-rw-   0        0        0     2295 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Operations.py
+-rw-rw-rw-   0        0        0     1365 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/Subscripts.py
+-rw-rw-rw-   0        0        0     8827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.416699 Nuitka-winsvc-2.1.5/tests/packages/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.418699 Nuitka-winsvc-2.1.5/tests/packages/package_data_files_embedding/
+-rw-rw-rw-   0        0        0     1576 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/package_data_files_embedding/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.420711 Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2414 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.423699 Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      975 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.428353 Nuitka-winsvc-2.1.5/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.425699 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1262 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      940 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      942 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.427699 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      961 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      999 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0     1001 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.428353 Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.429699 Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2368 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.430699 Nuitka-winsvc-2.1.5/tests/plugins/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.439699 Nuitka-winsvc-2.1.5/tests/plugins/code_signing/
+-rw-rw-rw-   0        0        0     1202 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/code_signing/CodeSigningMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.453889 Nuitka-winsvc-2.1.5/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1474 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.463580 Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.463580 Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      309 2024-01-29 03:39:42.000000 Nuitka-winsvc-2.1.5/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.467579 Nuitka-winsvc-2.1.5/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1051 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2218 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3892 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.478582 Nuitka-winsvc-2.1.5/tests/programs/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.488583 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.520590 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      828 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      893 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.525583 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.531582 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.539584 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.548583 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.555607 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.559583 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.567600 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.573584 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.576584 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.586594 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.595583 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1107 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.597128 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.607137 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.611137 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.618464 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.623466 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.629465 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.653473 Nuitka-winsvc-2.1.5/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.659466 Nuitka-winsvc-2.1.5/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.665467 Nuitka-winsvc-2.1.5/tests/programs/deep/
+-rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.685467 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0     1012 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.770501 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      984 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.775482 Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      826 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.898098 Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      829 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      889 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.977581 Nuitka-winsvc-2.1.5/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1037 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:33.999444 Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      978 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1130 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      854 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0     1026 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.099084 Nuitka-winsvc-2.1.5/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.105118 Nuitka-winsvc-2.1.5/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1112 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.119090 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1561 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.128084 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.137090 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.147096 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1776 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.156086 Nuitka-winsvc-2.1.5/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.171087 Nuitka-winsvc-2.1.5/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1110 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1391 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.181707 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.213349 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      868 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1791 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.217350 Nuitka-winsvc-2.1.5/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.227350 Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      856 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.232349 Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.241350 Nuitka-winsvc-2.1.5/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.253361 Nuitka-winsvc-2.1.5/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.273349 Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.278356 Nuitka-winsvc-2.1.5/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      855 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.290347 Nuitka-winsvc-2.1.5/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1040 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.294351 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.302234 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.315219 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.316218 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      958 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.323484 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      997 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.328502 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0     1009 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.348502 Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      933 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.354515 Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.364502 Nuitka-winsvc-2.1.5/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      884 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.389501 Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.395502 Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     3004 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.416112 Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:29.439375 Nuitka-winsvc-2.1.5/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.434112 Nuitka-winsvc-2.1.5/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.444113 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1760 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.452112 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.473111 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.500112 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.503112 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.509114 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1585 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.521123 Nuitka-winsvc-2.1.5/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      891 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.531730 Nuitka-winsvc-2.1.5/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      803 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.538061 Nuitka-winsvc-2.1.5/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.543042 Nuitka-winsvc-2.1.5/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.551041 Nuitka-winsvc-2.1.5/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.557045 Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.566281 Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6646 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.580149 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.596138 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1268 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.609329 Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      822 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.619621 Nuitka-winsvc-2.1.5/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      995 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.622394 Nuitka-winsvc-2.1.5/tests/programs/with space/
+-rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.626199 Nuitka-winsvc-2.1.5/tests/reflected/
+-rw-rw-rw-   0        0        0    14194 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/run-tests
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.761699 Nuitka-winsvc-2.1.5/tests/standalone/
+-rw-rw-rw-   0        0        0     1090 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2586 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1950 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/DateutilsUsing.py
+-rw-rw-rw-   0        0        0     1168 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/GiUsing.py
+-rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1216 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1057 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1118 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1215 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1598 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2570 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1759 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      979 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1479 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1098 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1248 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2106 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1099 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1369 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2198 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PyQt6Plugins.py
+-rw-rw-rw-   0        0        0     2168 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PySide2Using.py
+-rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PySide6Plugins.py
+-rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1371 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0     1227 2024-03-25 02:50:30.000000 Nuitka-winsvc-2.1.5/tests/standalone/SetuptoolsUsing.py
+-rw-rw-rw-   0        0        0     1005 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1569 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1973 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3260 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1232 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9912 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:34.776707 Nuitka-winsvc-2.1.5/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1296 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:16:35.035941 Nuitka-winsvc-2.1.5/tests/syntax/
+-rw-rw-rw-   0        0        0      844 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      818 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/AwaitInModule36.py
+-rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0     1002 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      882 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1142 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      947 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      915 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      808 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2234 2024-03-06 05:39:36.000000 Nuitka-winsvc-2.1.5/tests/syntax/run_all.py
```

### Comparing `Nuitka-winsvc-2.1.4/Developer_Manual.rst` & `Nuitka-winsvc-2.1.5/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/LICENSE.txt` & `Nuitka-winsvc-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/MANIFEST.in` & `Nuitka-winsvc-2.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/PKG-INFO` & `Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 2.1.4
+Version: 2.1.5
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-2.1.4/Nuitka_winsvc.egg-info/SOURCES.txt` & `Nuitka-winsvc-2.1.5/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/PKG-INFO` & `Nuitka-winsvc-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 2.1.4
+Version: 2.1.5
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-2.1.4/README.md` & `Nuitka-winsvc-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/README.rst` & `Nuitka-winsvc-2.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/autoformat-nuitka-source` & `Nuitka-winsvc-2.1.5/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/check-nuitka-with-pylint` & `Nuitka-winsvc-2.1.5/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/compare_with_cpython` & `Nuitka-winsvc-2.1.5/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/compare_with_xml` & `Nuitka-winsvc-2.1.5/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/measure-construct-performance` & `Nuitka-winsvc-2.1.5/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/nuitka` & `Nuitka-winsvc-2.1.5/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/bin/nuitka-run` & `Nuitka-winsvc-2.1.5/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-winsvc-2.1.5/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-winsvc-2.1.5/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/nuitka-run.1` & `Nuitka-winsvc-2.1.5/doc/nuitka-run.1`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/doc/nuitka.1` & `Nuitka-winsvc-2.1.5/doc/nuitka.1`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/lib/hints.py` & `Nuitka-winsvc-2.1.5/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/misc/nuitka-run.bat` & `Nuitka-winsvc-2.1.5/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/misc/nuitka.bat` & `Nuitka-winsvc-2.1.5/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Builtins.py` & `Nuitka-winsvc-2.1.5/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/BytecodeCaching.py` & `Nuitka-winsvc-2.1.5/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Bytecodes.py` & `Nuitka-winsvc-2.1.5/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/CacheCleanup.py` & `Nuitka-winsvc-2.1.5/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Constants.py` & `Nuitka-winsvc-2.1.5/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Errors.py` & `Nuitka-winsvc-2.1.5/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/HardImportRegistry.py` & `Nuitka-winsvc-2.1.5/nuitka/HardImportRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/MainControl.py` & `Nuitka-winsvc-2.1.5/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/ModuleRegistry.py` & `Nuitka-winsvc-2.1.5/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/OptionParsing.py` & `Nuitka-winsvc-2.1.5/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Options.py` & `Nuitka-winsvc-2.1.5/nuitka/Options.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,20 @@
     value = _convertOldStylePathSpecQuotes(value)
     if old != value:
         Tracing.options_logger.warning(
             "Adapted '%s' option value from legacy quoting style to '%s' -> '%s'"
             % (arg_name, old, value)
         )
 
+    if "\n" in value or "\r" in value:
+        Tracing.options_logger.sysexit(
+            "Using a new line in value '%s=%r' value is not allowed."
+            % (arg_name, value)
+        )
+
     if "{NONE}" in value:
         if not allow_disable:
             Tracing.options_logger.sysexit(
                 "Using value '{NONE}' in '%s=%s' value is not allowed."
                 % (arg_name, value)
             )
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/OutputDirectories.py` & `Nuitka-winsvc-2.1.5/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/PostProcessing.py` & `Nuitka-winsvc-2.1.5/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Progress.py` & `Nuitka-winsvc-2.1.5/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/PythonFlavors.py` & `Nuitka-winsvc-2.1.5/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/PythonOperators.py` & `Nuitka-winsvc-2.1.5/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/PythonVersions.py` & `Nuitka-winsvc-2.1.5/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Serialization.py` & `Nuitka-winsvc-2.1.5/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/SourceCodeReferences.py` & `Nuitka-winsvc-2.1.5/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Tracing.py` & `Nuitka-winsvc-2.1.5/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/TreeXML.py` & `Nuitka-winsvc-2.1.5/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Variables.py` & `Nuitka-winsvc-2.1.5/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/Version.py` & `Nuitka-winsvc-2.1.5/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V2.1.4
+Nuitka V2.1.5
 Copyright (C) 2024 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/__past__.py` & `Nuitka-winsvc-2.1.5/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/Backend.scons` & `Nuitka-winsvc-2.1.5/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/CCompilerVersion.scons` & `Nuitka-winsvc-2.1.5/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/DataComposerInterface.py` & `Nuitka-winsvc-2.1.5/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/Onefile.scons` & `Nuitka-winsvc-2.1.5/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsCaching.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsCompilerSettings.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsHacks.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsInterface.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsProgress.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsSpawn.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/SconsUtils.py` & `Nuitka-winsvc-2.1.5/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/allocator.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/builtins.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/calling.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/checkers.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/constants.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/environment_variables.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/environment_variables.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/environment_variables_system.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/environment_variables_system.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/exception_groups.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/exception_groups.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/freelists.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/hedley.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/helpers.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/importing.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/incbin.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/prelude.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/printing.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/threading.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/tracing.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-winsvc-2.1.5/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/LICENSE` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/crc32.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/crc32.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zconf.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zlib.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zlib/zutil.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-winsvc-2.1.5/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersDumpBacktraces.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersDumpBacktraces.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersEnvironmentVariables.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariables.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersImport.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersLists.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/MainProgram.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/MainProgram.c`

 * *Files 1% similar despite different names*

```diff
@@ -1324,17 +1324,17 @@
 #else
     {
         environment_char_t const *python_path_cstr = getEnvironmentVariable("NUITKA_PYTHONPATH");
 
         if (python_path_cstr != NULL) {
             PyObject *python_path_str = Nuitka_String_FromFilename(python_path_cstr);
 #ifdef _WIN32
-            PyObject *python_path_list = PyObject_CallMethod(python_path_str, "split", "s", ";");
+            PyObject *python_path_list = PyObject_CallMethod(python_path_str, (char *)"split", (char *)"s", ";");
 #else
-            PyObject *python_path_list = PyObject_CallMethod(python_path_str, "split", "s", ":");
+            PyObject *python_path_list = PyObject_CallMethod(python_path_str, (char *)"split", (char *)"s", ":");
 #endif
             Py_DECREF(python_path_str);
 
             PySys_SetObject("path", python_path_list);
 
             unsetEnvironmentVariable("NUITKA_PYTHONPATH");
         }
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-winsvc-2.1.5/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/AttributeCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/BranchCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CallCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ClassCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeGeneration.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeHelpers.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ConstantCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/Contexts.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/CtypesCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/DictCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/Emission.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ErrorCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/EvalCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/FrameCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/FunctionCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/GlobalConstants.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/IdCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ImportCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/Indentation.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/IndexCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/InjectCCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/IntegerCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/IteratorCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/LabelCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ListCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/LoaderCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/LoopCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/MatchCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ModuleCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/Namify.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/OperationCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/PrintCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/RaisingCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/Reports.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/ReturnCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/SetCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/SliceCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/StringCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/TryCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/TupleCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/VariableCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/YieldCodes.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/c_types/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-winsvc-2.1.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/containers/Namedtuples.py` & `Nuitka-winsvc-2.1.5/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/containers/OrderedDicts.py` & `Nuitka-winsvc-2.1.5/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/containers/OrderedSets.py` & `Nuitka-winsvc-2.1.5/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-winsvc-2.1.5/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/containers/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/distutils/Build.py` & `Nuitka-winsvc-2.1.5/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/distutils/DistutilCommands.py` & `Nuitka-winsvc-2.1.5/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/distutils/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/finalizations/Finalization.py` & `Nuitka-winsvc-2.1.5/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-winsvc-2.1.5/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/finalizations/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/DependsExe.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/ImportDetection.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/ImportDetection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/Onefile.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/Standalone.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/freezer/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/IgnoreListing.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/ImportCache.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/ImportResolving.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/Importing.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/PreloadedPackages.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/Recursion.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/StandardLibrary.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/StandardLibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                     yield ModuleName(import_path + "." + module_name)
 
         if python_version >= 0x300:
             if "__pycache__" in dirs:
                 dirs.remove("__pycache__")
 
         # Ignore ".idea", ".git" and similar folders, they are not modules
-        dirs = [dirname for dirname in dirs if not dirname.startswith(".")]
+        dirs[:] = [dirname for dirname in dirs if not dirname.startswith(".")]
 
         for dirname in dirs:
             if import_path == "":
                 yield ModuleName(dirname)
             else:
                 yield ModuleName(import_path + "." + dirname)
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/importing/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinInputNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinInputNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/BytesNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/CallNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/Checkers.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ClassNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ComparisonNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ConditionalNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/CoroutineNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/CtypesNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/DictionaryNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ExceptionNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionBases.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/FrameNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/FunctionNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/FutureSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/GeneratorNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     kind = "EXPRESSION_BUILTIN_LOCALS_REF"
 
     def __init__(self, locals_scope, source_ref):
         ExpressionBuiltinLocalsBase.__init__(
             self, locals_scope=locals_scope, source_ref=source_ref
         )
 
+    def getDetails(self):
+        return {"locals_scope": self.locals_scope}
+
     def getLocalsScope(self):
         return self.locals_scope
 
     # For overload.
     def isFinalUseOfLocals(self):
         return self.parent.isStatementReturn()
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ImportHardNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ImportNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/IndicatorMixins.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/InjectCNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/IterationHandles.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ListOperationNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/LocalsScopes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/LoopNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/MatchNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ModuleNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/NodeBases.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/OperatorNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/OsSysNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/OutlineNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/PrintNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/ReturnNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/SideEffectNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/SliceNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/StatementNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/StrNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/SubscriptNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/TryNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/TypeNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/VariableDelNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/VariableNameNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/VariableRefNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/YieldNodes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/nodes/shapes/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/FunctionInlining.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/Graphs.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/Optimization.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/Tags.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/TraceCollections.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/ValueTraces.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/optimizations/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/pgo/PGO.py` & `Nuitka-winsvc-2.1.5/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/pgo/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/PluginBase.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/Plugins.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin/DillPlugin.c` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin/DillPlugin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin/dill-postLoad.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin/dill-postLoad.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #     Copyright 2024, Kay Hayen, mailto:kay.hayen@gmail.com find license text at end of file
 
 
 """ Plugin to provide transformers implicit dependencies.
 
 """
 
-
 from nuitka.plugins.PluginBase import NuitkaPluginBase
 
 
 class NuitkaPluginTransformers(NuitkaPluginBase):
     plugin_name = "transformers"
 
     plugin_desc = "Provide implicit imports for transformers package."
@@ -17,213 +16,275 @@
     @staticmethod
     def isAlwaysEnabled():
         return True
 
     # Found via grep -re "_import_structure = {"
     _import_structure_modules = (
         "transformers",
-        "transformers.integrations",
         "transformers.generation",
+        "transformers.integrations",
         "transformers.models.albert",
         "transformers.models.align",
         "transformers.models.altclip",
         "transformers.models.audio_spectrogram_transformer",
         "transformers.models.auto",
+        "transformers.models.autoformer",
+        "transformers.models.bark",
         "transformers.models.bart",
         "transformers.models.barthez",
         "transformers.models.bartpho",
         "transformers.models.beit",
         "transformers.models.bert",
-        "transformers.models.bertweet",
         "transformers.models.bert_generation",
         "transformers.models.bert_japanese",
-        "transformers.models.bigbird_pegasus",
+        "transformers.models.bertweet",
         "transformers.models.big_bird",
+        "transformers.models.bigbird_pegasus",
         "transformers.models.biogpt",
         "transformers.models.bit",
         "transformers.models.blenderbot",
         "transformers.models.blenderbot_small",
         "transformers.models.blip",
         "transformers.models.blip_2",
         "transformers.models.bloom",
         "transformers.models.bridgetower",
+        "transformers.models.bros",
         "transformers.models.byt5",
         "transformers.models.camembert",
         "transformers.models.canine",
         "transformers.models.chinese_clip",
         "transformers.models.clap",
         "transformers.models.clip",
         "transformers.models.clipseg",
+        "transformers.models.clvp",
+        "transformers.models.code_llama",
         "transformers.models.codegen",
+        "transformers.models.cohere",
         "transformers.models.conditional_detr",
         "transformers.models.convbert",
         "transformers.models.convnext",
         "transformers.models.convnextv2",
         "transformers.models.cpm",
         "transformers.models.cpmant",
         "transformers.models.ctrl",
         "transformers.models.cvt",
         "transformers.models.data2vec",
         "transformers.models.deberta",
         "transformers.models.deberta_v2",
         "transformers.models.decision_transformer",
         "transformers.models.deformable_detr",
         "transformers.models.deit",
+        "transformers.models.depth_anything",
         "transformers.models.deta",
         "transformers.models.detr",
         "transformers.models.dinat",
+        "transformers.models.dinov2",
         "transformers.models.distilbert",
         "transformers.models.donut",
         "transformers.models.dpr",
         "transformers.models.dpt",
         "transformers.models.efficientformer",
         "transformers.models.efficientnet",
         "transformers.models.electra",
+        "transformers.models.encodec",
         "transformers.models.encoder_decoder",
         "transformers.models.ernie",
         "transformers.models.ernie_m",
         "transformers.models.esm",
+        "transformers.models.falcon",
+        "transformers.models.fastspeech2_conformer",
         "transformers.models.flaubert",
         "transformers.models.flava",
         "transformers.models.fnet",
         "transformers.models.focalnet",
         "transformers.models.fsmt",
         "transformers.models.funnel",
+        "transformers.models.fuyu",
+        "transformers.models.gemma",
         "transformers.models.git",
         "transformers.models.glpn",
         "transformers.models.gpt2",
-        "transformers.models.gptj",
-        "transformers.models.gptsan_japanese",
         "transformers.models.gpt_bigcode",
         "transformers.models.gpt_neo",
         "transformers.models.gpt_neox",
         "transformers.models.gpt_neox_japanese",
         "transformers.models.gpt_sw3",
+        "transformers.models.gptj",
+        "transformers.models.gptsan_japanese",
         "transformers.models.graphormer",
         "transformers.models.groupvit",
         "transformers.models.herbert",
         "transformers.models.hubert",
         "transformers.models.ibert",
+        "transformers.models.idefics",
         "transformers.models.imagegpt",
         "transformers.models.informer",
+        "transformers.models.instructblip",
         "transformers.models.jukebox",
+        "transformers.models.kosmos2",
         "transformers.models.layoutlm",
         "transformers.models.layoutlmv2",
         "transformers.models.layoutlmv3",
         "transformers.models.layoutxlm",
         "transformers.models.led",
         "transformers.models.levit",
         "transformers.models.lilt",
         "transformers.models.llama",
+        "transformers.models.llava",
+        "transformers.models.llava_next",
         "transformers.models.longformer",
         "transformers.models.longt5",
         "transformers.models.luke",
         "transformers.models.lxmert",
         "transformers.models.m2m_100",
+        "transformers.models.mamba",
         "transformers.models.marian",
         "transformers.models.markuplm",
         "transformers.models.mask2former",
         "transformers.models.maskformer",
         "transformers.models.mbart",
         "transformers.models.mbart50",
         "transformers.models.mctct",
         "transformers.models.mega",
         "transformers.models.megatron_bert",
         "transformers.models.mgp_str",
+        "transformers.models.mistral",
+        "transformers.models.mixtral",
         "transformers.models.mluke",
         "transformers.models.mmbt",
         "transformers.models.mobilebert",
         "transformers.models.mobilenet_v1",
         "transformers.models.mobilenet_v2",
         "transformers.models.mobilevit",
+        "transformers.models.mobilevitv2",
         "transformers.models.mpnet",
+        "transformers.models.mpt",
+        "transformers.models.mra",
         "transformers.models.mt5",
+        "transformers.models.musicgen",
+        "transformers.models.musicgen_melody",
         "transformers.models.mvp",
         "transformers.models.nat",
         "transformers.models.nezha",
         "transformers.models.nllb",
         "transformers.models.nllb_moe",
+        "transformers.models.nougat",
         "transformers.models.nystromformer",
         "transformers.models.oneformer",
-        "transformers.models.openai",
         "transformers.models.open_llama",
+        "transformers.models.openai",
         "transformers.models.opt",
+        "transformers.models.owlv2",
         "transformers.models.owlvit",
+        "transformers.models.patchtsmixer",
+        "transformers.models.patchtst",
         "transformers.models.pegasus",
         "transformers.models.pegasus_x",
         "transformers.models.perceiver",
+        "transformers.models.persimmon",
+        "transformers.models.phi",
         "transformers.models.phobert",
         "transformers.models.pix2struct",
         "transformers.models.plbart",
         "transformers.models.poolformer",
+        "transformers.models.pop2piano",
         "transformers.models.prophetnet",
+        "transformers.models.pvt",
+        "transformers.models.pvt_v2",
         "transformers.models.qdqbert",
+        "transformers.models.qwen2",
         "transformers.models.rag",
         "transformers.models.realm",
         "transformers.models.reformer",
         "transformers.models.regnet",
         "transformers.models.rembert",
         "transformers.models.resnet",
         "transformers.models.retribert",
         "transformers.models.roberta",
         "transformers.models.roberta_prelayernorm",
         "transformers.models.roc_bert",
         "transformers.models.roformer",
         "transformers.models.rwkv",
         "transformers.models.sam",
+        "transformers.models.seamless_m4t",
+        "transformers.models.seamless_m4t_v2",
         "transformers.models.segformer",
+        "transformers.models.seggpt",
         "transformers.models.sew",
         "transformers.models.sew_d",
-        "transformers.models.speecht5",
+        "transformers.models.siglip",
         "transformers.models.speech_encoder_decoder",
         "transformers.models.speech_to_text",
         "transformers.models.speech_to_text_2",
+        "transformers.models.speecht5",
         "transformers.models.splinter",
         "transformers.models.squeezebert",
+        "transformers.models.stablelm",
+        "transformers.models.starcoder2",
+        "transformers.models.superpoint",
+        "transformers.models.swiftformer",
         "transformers.models.swin",
         "transformers.models.swin2sr",
         "transformers.models.swinv2",
         "transformers.models.switch_transformers",
         "transformers.models.t5",
         "transformers.models.table_transformer",
         "transformers.models.tapas",
         "transformers.models.tapex",
-        "transformers.models.timesformer",
         "transformers.models.time_series_transformer",
+        "transformers.models.timesformer",
+        "transformers.models.timm_backbone",
         "transformers.models.trajectory_transformer",
-        "transformers.models.transfo_xl",
+        "transformers.models.deprecated.mctct",
+        "transformers.models.deprecated.mmbt",
+        "transformers.models.deprecated.open_llama",
+        "transformers.models.deprecated.retribert",
+        "transformers.models.deprecated.tapex",
+        "transformers.models.deprecated.trajectory_transformer",
+        "transformers.models.deprecated.transfo_xl",
+        "transformers.models.deprecated.van",
         "transformers.models.trocr",
         "transformers.models.tvlt",
+        "transformers.models.tvp",
+        "transformers.models.udop",
+        "transformers.models.umt5",
         "transformers.models.unispeech",
         "transformers.models.unispeech_sat",
+        "transformers.models.univnet",
         "transformers.models.upernet",
         "transformers.models.van",
         "transformers.models.videomae",
         "transformers.models.vilt",
+        "transformers.models.vipllava",
         "transformers.models.vision_encoder_decoder",
         "transformers.models.vision_text_dual_encoder",
         "transformers.models.visual_bert",
         "transformers.models.vit",
         "transformers.models.vit_hybrid",
         "transformers.models.vit_mae",
         "transformers.models.vit_msn",
+        "transformers.models.vitdet",
+        "transformers.models.vitmatte",
+        "transformers.models.vits",
+        "transformers.models.vivit",
         "transformers.models.wav2vec2",
+        "transformers.models.wav2vec2_bert",
         "transformers.models.wav2vec2_conformer",
         "transformers.models.wav2vec2_phoneme",
         "transformers.models.wav2vec2_with_lm",
         "transformers.models.wavlm",
         "transformers.models.whisper",
+        "transformers.models.x_clip",
         "transformers.models.xglm",
         "transformers.models.xlm",
         "transformers.models.xlm_prophetnet",
         "transformers.models.xlm_roberta",
         "transformers.models.xlm_roberta_xl",
         "transformers.models.xlnet",
         "transformers.models.xmod",
-        "transformers.models.x_clip",
         "transformers.models.yolos",
         "transformers.models.yoso",
         "transformers.onnx",
         "transformers.tools",
     )
 
     def getImplicitImports(self, module):
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -386,22 +386,27 @@
 
 - module-name: 'bitarray' # checksum: b157a72f
   anti-bloat:
     - description: 'remove unittest reference'
       change_function:
         'test': 'un-callable'
 
-- module-name: 'bitsandbytes.cextension' # checksum: 70a78a03
+- module-name: 'bitsandbytes' # checksum: 14f2c5d0
   dlls:
     - from_filenames:
         prefixes:
           - 'libbitsandbytes_'
         suffixes:
-          # Applies currently to all OSes in bitsandbytes wheels.
+          # Applied to all OSes in bitsandbytes wheels.
           - 'so'
+      when: 'version("bitsandbytes") < (0,43)'
+    - from_filenames:
+        prefixes:
+          - 'libbitsandbytes_'
+      when: 'version("bitsandbytes") >= (0,43)'
 
 - module-name: 'bitsandbytes.triton.dequantize_rowwise' # checksum: 291bbd89
   anti-bloat:
     - description: 'remove setuptools usage via triton'
       replacements_plain:
         'is_triton_available()': 'False'
       when: 'not use_setuptools'
@@ -2231,14 +2236,19 @@
       when: 'not use_unittest'
 
 - module-name: 'nacl._sodium' # checksum: ff2e6560
   implicit-imports:
     - depends:
         - '_cffi_backend'
 
+- module-name: 'names' # checksum: 4d754910
+  data-files:
+    patterns:
+      - 'dist.*'
+
 - module-name: 'networkx' # checksum: 6f2aa88a
   anti-bloat:
     - description: 'remove networkx.testing usage and pytest reference (via nose)'
       replacements_plain:
         'from networkx.testing.test import run as test': 'test = None'
         'from networkx.tests.test import run as test': 'test = None'
       no-auto-follow:
@@ -4110,14 +4120,19 @@
       - '*.ttf'
 
 - module-name: 'qtawesome' # checksum: 2c2a9970
   data-files:
     dirs:
       - 'fonts'
 
+- module-name: 'randomname' # checksum: 8d6f0c80
+  data-files:
+    dirs:
+      - 'wordlists'
+
 - module-name: 'rapidfuzz' # checksum: 2248cb4c
   implicit-imports:
     - depends:
         - '.utils_py'
         - '.utils_cpp'
         - '.fuzz_py'
         - '.fuzz_cpp'
@@ -4260,15 +4275,15 @@
       when: 'not win32'
 
 - module-name: 'scapy.all' # checksum: 8a9944ce
   implicit-imports:
     - depends:
         - 'scapy.layers.*'
 
-- module-name: 'scipy' # checksum: 2e8d63ef
+- module-name: 'scipy' # checksum: 30cb05e1
   data-files:
     patterns:
       - 'stats/_sobol_direction_numbers.npz' # for scipy.stats._sobol._initialize_direction_numbers
 
   dlls:
     - from_filenames:
         relative_path: '.libs'
@@ -4276,14 +4291,20 @@
           - ''
     - from_filenames:
         relative_path: 'extra_dll'
         prefixes:
           - ''
       when: 'win32'
 
+  anti-bloat:
+    - description: 'torch and cupy checks should not cause usage'
+      no-auto-follow:
+        'cupy': 'ignore'
+        'torch': 'ignore'
+
 - module-name: 'scipy._distributor_init' # checksum: 3316da5c
   anti-bloat:
     - description: 'workaround for scipy DLL loading'
       append_plain: |
         if os.name == "nt":
           libs_dir = os.path.join(os.path.dirname(__file__), '..', 'scipy.libs')
           for filename in glob.glob(os.path.join(libs_dir, '*openblas*dll')):
@@ -4407,14 +4428,19 @@
         - 'scipy.spatial.transform._rotation_groups'
 
 - module-name: 'scipy.special' # checksum: 93a78ec1
   implicit-imports:
     - depends:
         - 'scipy.special._ufuncs_cxx'
 
+- module-name: 'scipy.special._ufuncs' # checksum: 4ded0e67
+  implicit-imports:
+    - depends:
+        - 'scipy.special._cdflib'
+
 - module-name: 'scipy.stats._fit' # checksum: 7547ad25
   anti-bloat:
     - no-auto-follow:
         'matplotlib': 'plotting will lack matplotlib'
 
 - module-name: 'scipy.stats._stats' # checksum: 41c1ec8f
   implicit-imports:
@@ -6674,17 +6700,19 @@
 - module-name: 'transformers.models.deta.modeling_deta' # checksum: baab8e6b
   anti-bloat:
     - description: 'remove setuptools usage'
       change_function:
         'load_cuda_kernels': 'un-callable'
       when: 'not use_setuptools'
 
-- module-name: 'transformers.models.mra.modeling_mra' # checksum: baab8e6b
+- module-name: 'transformers.models.mra.modeling_mra' # checksum: a554c6d
   anti-bloat:
     - description: 'remove setuptools usage'
+      replacements_plain:
+        'from torch.utils.cpp_extension import load': ''
       change_function:
         'load_cuda_kernels': 'un-callable'
       when: 'not use_setuptools'
 
 - module-name: 'transformers.models.rwkv.modeling_rwkv' # checksum: f186b69e
   anti-bloat:
     - description: 'remove setuptools usage'
```

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-winsvc-2.1.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/reports/CompilationReportReader.py` & `Nuitka-winsvc-2.1.5/nuitka/reports/CompilationReportReader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-winsvc-2.1.5/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/reports/Reports.py` & `Nuitka-winsvc-2.1.5/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/reports/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/HardImportSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/ParameterSpecs.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/specs/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/Basics.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/commercial/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/data_composer/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/environments/Virtualenv.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/environments/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/general/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/general/find_module/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/podman/Podman.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/podman/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/podman/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/profiler/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/profiler/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/scanning/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/specialize/Common.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/specialize/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/Common.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/Constructs.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/OutputComparison.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/Pythons.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/SearchModes.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/Valgrind.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/watch/GitHub.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/watch/GitHub.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/watch/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tools/watch/__main__.py` & `Nuitka-winsvc-2.1.5/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/Building.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/Extractions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/InternalModule.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/Operations.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationClasses.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationClasses3.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationMultidist.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/SourceHandling.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/SyntaxErrors.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/TreeHelpers.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/VariableClosure.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/tree/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/AppDirs.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/CStrings.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/CommandLineOptions.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Distributions.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Download.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Execution.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/FileOperations.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Hashing.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Images.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Importing.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/InstalledPythons.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/InstanceCounters.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Jinja2.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Json.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/MacOSApp.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/MemoryUsage.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/ModuleNames.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/ReExecute.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Rest.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/SharedLibraries.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Shebang.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Signing.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/SlotMetaClasses.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/SlotMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/StaticLibraries.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/ThreadedExecutor.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Timing.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Utils.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/WindowsFileUsage.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/WindowsResources.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/Yaml.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/nuitka/utils/__init__.py` & `Nuitka-winsvc-2.1.5/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/pyproject.toml` & `Nuitka-winsvc-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/setup.py` & `Nuitka-winsvc-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/AssertsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/AssignmentsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/AssignmentsTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/BranchingTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/BuiltinOverload.py` & `Nuitka-winsvc-2.1.5/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/BuiltinSuperTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/BuiltinsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ClassMinimalTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ClassesTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ClassesTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ClassesTest34.py` & `Nuitka-winsvc-2.1.5/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ComparisonChainsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ConstantsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ConstantsTest27.py` & `Nuitka-winsvc-2.1.5/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/DecoratorsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/DefaultParametersTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/DoubleDeletionsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/EmptyModuleTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-winsvc-2.1.5/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ExecEvalTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ExtremeClosureTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/FunctionObjectsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/FunctionsTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/FutureTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-winsvc-2.1.5/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/GlobalStatementTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/HelloWorldTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ImportingTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/InplaceOperationsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/InspectionTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/InspectionTest_35.py` & `Nuitka-winsvc-2.1.5/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/InspectionTest_36.py` & `Nuitka-winsvc-2.1.5/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/LambdasTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ListContractionsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/LoopingTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/MainProgramsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ModuleAttributesTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/OperatorsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/OrderChecksTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/OrderChecksTest27.py` & `Nuitka-winsvc-2.1.5/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ParameterErrorsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ParameterErrorsTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/PrintFutureTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/PrintingTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/RecursionTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest27.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest33.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest35.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest36.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ReferencingTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/SlotsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-winsvc-2.1.5/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryContinueFinallyTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryExceptContinueTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryExceptFinallyTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryExceptFramesTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryReturnFinallyTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/TryYieldFinallyTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/UnicodeTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/UnpackingTest35.py` & `Nuitka-winsvc-2.1.5/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/VarargsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/WithStatementsTest.py` & `Nuitka-winsvc-2.1.5/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/YieldFromTest33.py` & `Nuitka-winsvc-2.1.5/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/run_all.py` & `Nuitka-winsvc-2.1.5/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/basics/run_xml.py` & `Nuitka-winsvc-2.1.5/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/onefile/HelloWorldTest.py` & `Nuitka-winsvc-2.1.5/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-winsvc-2.1.5/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/onefile/run_all.py` & `Nuitka-winsvc-2.1.5/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/ArgumentTypes.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Attributes.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Calls.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Conditions.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/DecodingOperations.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/FormatStrings36.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/HardImports.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/HardImports_2.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Iterations.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Len.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Matching310.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Matching310.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Operations.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/Subscripts.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/optimizations/run_all.py` & `Nuitka-winsvc-2.1.5/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py` & `Nuitka-winsvc-2.1.5/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/package_data_files_embedding/__init__.py` & `Nuitka-winsvc-2.1.5/tests/packages/package_data_files_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/run_all.py` & `Nuitka-winsvc-2.1.5/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-winsvc-2.1.5/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-winsvc-2.1.5/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-winsvc-2.1.5/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-winsvc-2.1.5/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/parameters/ParametersMain.py` & `Nuitka-winsvc-2.1.5/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-winsvc-2.1.5/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/plugins/run_all.py` & `Nuitka-winsvc-2.1.5/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/local.py` & `Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/absolute_import/foobar/util.py` & `Nuitka-winsvc-2.1.5/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dash_import/DashImportMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dash_import/dash-module.py` & `Nuitka-winsvc-2.1.5/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dash_import/plus+module.py` & `Nuitka-winsvc-2.1.5/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dash_main/Dash-Main.py` & `Nuitka-winsvc-2.1.5/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/DeepProgramMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/main_raises/ErrorMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-winsvc-2.1.5/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-winsvc-2.1.5/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_exits/Main.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-winsvc-2.1.5/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_code/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_contains_main/local.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_module_collision/something.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_overload/Main.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/bar.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_overload/foo/bar2.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-winsvc-2.1.5/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-winsvc-2.1.5/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/relative_import/dircache.py` & `Nuitka-winsvc-2.1.5/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/run_all.py` & `Nuitka-winsvc-2.1.5/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-winsvc-2.1.5/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-winsvc-2.1.5/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-winsvc-2.1.5/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/programs/with space/Space Main.py` & `Nuitka-winsvc-2.1.5/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/reflected/compile_itself.py` & `Nuitka-winsvc-2.1.5/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/run-tests` & `Nuitka-winsvc-2.1.5/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/BrotliUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/CtypesUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/DateutilsUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/DateutilsUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/FlaskUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/GiUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/GiUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/GlfwUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/GtkUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/HexEncodingTest_2.py` & `Nuitka-winsvc-2.1.5/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/IdnaUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/LxmlUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/MatplotlibUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/NumpyUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/OpenGLUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PandasUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PasslibUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PendulumUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PmwUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PyQt5Plugins.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PyQt5Using.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PyQt6Plugins.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PyQt6Using.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PySide2Using.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PySide2Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PySide6Plugins.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/PySide6Using.py` & `Nuitka-winsvc-2.1.5/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/RsaUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/SetuptoolsUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/SetuptoolsUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/ShlibUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/SocketUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/TkInterUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/Urllib3Using.py` & `Nuitka-winsvc-2.1.5/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/Win32ComUsing.py` & `Nuitka-winsvc-2.1.5/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/run_all.py` & `Nuitka-winsvc-2.1.5/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-winsvc-2.1.5/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/AsyncgenReturn36.py` & `Nuitka-winsvc-2.1.5/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/AwaitInModule36.py` & `Nuitka-winsvc-2.1.5/tests/syntax/AwaitInModule36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/BreakWithoutLoop.py` & `Nuitka-winsvc-2.1.5/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/ClassReturn.py` & `Nuitka-winsvc-2.1.5/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/ClosureDel_2.py` & `Nuitka-winsvc-2.1.5/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-winsvc-2.1.5/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/DuplicateArgument.py` & `Nuitka-winsvc-2.1.5/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/ExecWithNesting_2.py` & `Nuitka-winsvc-2.1.5/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/FutureBraces.py` & `Nuitka-winsvc-2.1.5/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/FutureUnknown.py` & `Nuitka-winsvc-2.1.5/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/GeneratorExpressions38.py` & `Nuitka-winsvc-2.1.5/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/GeneratorReturn_2.py` & `Nuitka-winsvc-2.1.5/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/GlobalForParameter.py` & `Nuitka-winsvc-2.1.5/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/Importing32.py` & `Nuitka-winsvc-2.1.5/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/IndentationError.py` & `Nuitka-winsvc-2.1.5/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/LateFutureImport.py` & `Nuitka-winsvc-2.1.5/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/MisplacedFutureImport.py` & `Nuitka-winsvc-2.1.5/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/ModuleReturn.py` & `Nuitka-winsvc-2.1.5/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-winsvc-2.1.5/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/NonlocalForParameter32.py` & `Nuitka-winsvc-2.1.5/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/NonlocalNotFound32.py` & `Nuitka-winsvc-2.1.5/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/StarImportExtra.py` & `Nuitka-winsvc-2.1.5/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/SyntaxError.py` & `Nuitka-winsvc-2.1.5/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-winsvc-2.1.5/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-winsvc-2.1.5/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/UnpackNoTuple.py` & `Nuitka-winsvc-2.1.5/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/UnpackTwoStars32.py` & `Nuitka-winsvc-2.1.5/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/YieldFromInModule.py` & `Nuitka-winsvc-2.1.5/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/YieldInAsync35.py` & `Nuitka-winsvc-2.1.5/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/YieldInGenexp38.py` & `Nuitka-winsvc-2.1.5/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/YieldInModule.py` & `Nuitka-winsvc-2.1.5/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-2.1.4/tests/syntax/run_all.py` & `Nuitka-winsvc-2.1.5/tests/syntax/run_all.py`

 * *Files identical despite different names*

